# NBSAP-TEST
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Vanuatu NBSAP Target 3 Monitoring Platform - 30x30 Initiative</title>
    
    <script src="https://cdnjs.cloudflare.com/ajax/libs/shpjs/4.0.4/shp.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/chart.js@4.4.0/dist/chart.umd.min.js"></script>
    
    <style>
        /* Leaflet Core CSS */
        .leaflet-pane,.leaflet-tile,.leaflet-marker-icon,.leaflet-marker-shadow,.leaflet-tile-container,.leaflet-pane>svg,.leaflet-pane>canvas,.leaflet-zoom-box,.leaflet-image-layer,.leaflet-layer{position:absolute;left:0;top:0}.leaflet-container{overflow:hidden}.leaflet-tile,.leaflet-marker-icon,.leaflet-marker-shadow{-webkit-user-select:none;-moz-user-select:none;user-select:none;-webkit-user-drag:none}.leaflet-tile::selection{background:0 0}.leaflet-safari .leaflet-tile{image-rendering:-webkit-optimize-contrast}.leaflet-safari .leaflet-tile-container{width:1600px;height:1600px;-webkit-transform-origin:0 0}.leaflet-marker-icon,.leaflet-marker-shadow{display:block}.leaflet-container .leaflet-overlay-pane svg{max-width:none!important;max-height:none!important}.leaflet-container .leaflet-marker-pane img,.leaflet-container .leaflet-shadow-pane img,.leaflet-container .leaflet-tile-pane img,.leaflet-container img.leaflet-image-layer,.leaflet-container .leaflet-tile{max-width:none!important;max-height:none!important;width:auto;padding:0}.leaflet-container.leaflet-touch-zoom{-ms-touch-action:pan-x pan-y;touch-action:pan-x pan-y}.leaflet-container.leaflet-touch-drag{-ms-touch-action:pinch-zoom;touch-action:none;touch-action:pinch-zoom}.leaflet-container.leaflet-touch-drag.leaflet-touch-zoom{-ms-touch-action:none;touch-action:none}.leaflet-container{-webkit-tap-highlight-color:transparent}.leaflet-container a{-webkit-tap-highlight-color:rgba(51,181,229,.4)}.leaflet-tile{filter:inherit;visibility:hidden}.leaflet-tile-loaded{visibility:inherit}.leaflet-zoom-box{width:0;height:0;-moz-box-sizing:border-box;box-sizing:border-box;z-index:800}.leaflet-overlay-pane svg{-moz-user-select:none}.leaflet-pane{z-index:400}.leaflet-tile-pane{z-index:200}.leaflet-overlay-pane{z-index:400}.leaflet-shadow-pane{z-index:500}.leaflet-marker-pane{z-index:600}.leaflet-tooltip-pane{z-index:650}.leaflet-popup-pane{z-index:700}.leaflet-map-pane canvas{z-index:100}.leaflet-map-pane svg{z-index:200}.leaflet-vml-shape{width:1px;height:1px}.lvml{behavior:url(#default#VML);display:inline-block;position:absolute}.leaflet-control{position:relative;z-index:800;pointer-events:visiblePainted;pointer-events:auto}.leaflet-top,.leaflet-bottom{position:absolute;z-index:1000;pointer-events:none}.leaflet-top{top:0}.leaflet-right{right:0}.leaflet-bottom{bottom:0}.leaflet-left{left:0}.leaflet-control{float:left;clear:both}.leaflet-right .leaflet-control{float:right}.leaflet-top .leaflet-control{margin-top:10px}.leaflet-bottom .leaflet-control{margin-bottom:10px}.leaflet-left .leaflet-control{margin-left:10px}.leaflet-right .leaflet-control{margin-right:10px}.leaflet-fade-anim .leaflet-popup{opacity:0;-webkit-transition:opacity .2s linear;-moz-transition:opacity .2s linear;transition:opacity .2s linear}.leaflet-fade-anim .leaflet-map-pane .leaflet-popup{opacity:1}.leaflet-zoom-animated{-webkit-transform-origin:0 0;-ms-transform-origin:0 0;transform-origin:0 0}.leaflet-zoom-anim .leaflet-zoom-animated{will-change:transform}.leaflet-zoom-anim .leaflet-zoom-animated{-webkit-transition:-webkit-transform .25s cubic-bezier(0,0,.25,1);-moz-transition:-moz-transform .25s cubic-bezier(0,0,.25,1);transition:transform .25s cubic-bezier(0,0,.25,1)}.leaflet-pan-anim .leaflet-tile,.leaflet-touching .leaflet-zoom-animated{-webkit-transition:none;-moz-transition:none;transition:none}.leaflet-zoom-anim .leaflet-zoom-hide{visibility:hidden}.leaflet-interactive{cursor:pointer}.leaflet-grab{cursor:-webkit-grab;cursor:-moz-grab;cursor:grab}.leaflet-crosshair,.leaflet-crosshair .leaflet-interactive{cursor:crosshair}.leaflet-popup-pane,.leaflet-control{cursor:auto}.leaflet-dragging .leaflet-grab,.leaflet-dragging .leaflet-grab .leaflet-interactive,.leaflet-dragging .leaflet-marker-draggable{cursor:move;cursor:-webkit-grabbing;cursor:-moz-grabbing;cursor:grabbing}.leaflet-marker-icon,.leaflet-marker-shadow,.leaflet-image-layer,.leaflet-pane>svg path,.leaflet-tile-container{pointer-events:none}.leaflet-marker-icon.leaflet-interactive,.leaflet-image-layer.leaflet-interactive,.leaflet-pane>svg path.leaflet-interactive,svg.leaflet-image-layer.leaflet-interactive path{pointer-events:visiblePainted;pointer-events:auto}.leaflet-container{background:#ddd;outline-offset:1px}.leaflet-container a{color:#0078A8}.leaflet-zoom-box{border:2px dotted #38f;background:rgba(255,255,255,.5)}.leaflet-container{font-family:"Helvetica Neue",Arial,Helvetica,sans-serif;font-size:12px;font-size:.75rem;line-height:1.5}.leaflet-bar{box-shadow:0 1px 5px rgba(0,0,0,.65);border-radius:4px}.leaflet-bar a{background-color:#fff;border-bottom:1px solid #ccc;width:26px;height:26px;line-height:26px;display:block;text-align:center;text-decoration:none;color:#000}.leaflet-bar a,.leaflet-control-layers-toggle{background-position:50% 50%;background-repeat:no-repeat;display:block}.leaflet-bar a:hover,.leaflet-bar a:focus{background-color:#f4f4f4}.leaflet-bar a:first-child{border-top-left-radius:4px;border-top-right-radius:4px}.leaflet-bar a:last-child{border-bottom-left-radius:4px;border-bottom-right-radius:4px;border-bottom:none}.leaflet-bar a.leaflet-disabled{cursor:default;background-color:#f4f4f4;color:#bbb}.leaflet-touch .leaflet-bar a{width:30px;height:30px;line-height:30px}.leaflet-touch .leaflet-bar a:first-child{border-top-left-radius:2px;border-top-right-radius:2px}.leaflet-touch .leaflet-bar a:last-child{border-bottom-left-radius:2px;border-bottom-right-radius:2px}.leaflet-control-zoom-in,.leaflet-control-zoom-out{font:bold 18px 'Lucida Console',Monaco,monospace;text-indent:1px}.leaflet-touch .leaflet-control-zoom-in,.leaflet-touch .leaflet-control-zoom-out{font-size:22px}.leaflet-control-layers{box-shadow:0 1px 5px rgba(0,0,0,.4);background:#fff;border-radius:5px}.leaflet-control-layers-toggle{background-image:url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIzNiIgaGVpZ2h0PSIzNiI+PHBhdGggZD0iTTEgMTFoMzR2M0gxem0wIDEwaDE2djNIMXptMCAxMGgxOHYzSDF6IiBmaWxsPSIjMDAwIi8+PC9zdmc+);width:36px;height:36px}.leaflet-retina .leaflet-control-layers-toggle{background-size:26px 26px}.leaflet-touch .leaflet-control-layers-toggle{width:44px;height:44px}.leaflet-control-layers .leaflet-control-layers-list,.leaflet-control-layers-expanded .leaflet-control-layers-toggle{display:none}.leaflet-control-layers-expanded .leaflet-control-layers-list{display:block;position:relative}.leaflet-control-layers-expanded{padding:6px 10px 6px 6px;color:#333;background:#fff}.leaflet-control-layers-scrollbar{overflow-y:scroll;overflow-x:hidden;padding-right:5px}.leaflet-control-layers-selector{margin-top:2px;position:relative;top:1px}.leaflet-control-layers label{display:block;font-size:13px;font-size:1.08333em}.leaflet-control-layers-separator{height:0;border-top:1px solid #ddd;margin:5px -10px 5px -6px}.leaflet-default-icon-path{background-image:url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABkAAAApCAYAAADAk4LOAAAFgUlEQVR4Aa1XA5BjWRTN2oW17d3YaZtr2962HUzbDNpjszW24mRt28p47v7zq/bXZtrp/lWnXr337j3nPCe85NcypgSFdugCpW5YoDAMRaIMqRi6aKq5E3YqDQO3qAwjVWrD8Ncq/RBpykd8oZUb/kaJutow8r1aP9II0WmLKLIsJyv1w/kqw9Ch2MYdB++12Onxee/QMwvf4/Dk/Lfp/i4nxTXtOoQ4pW5Aj7wpici1A9erdAN2OH64x8OSP9j3Ft3b7aWkTg/Fm91siTra0f9on5sQr9INejH6CUUUpavjFNq1B+Oadhxmnfa8RrO+8zzNbVcftWNW0nKfc2N7HpmRmrJ0Z8S+0NLcq6NwYJ5I3hAAj6AXNeyvjmDYcxOBFj7PkZDu1QCWPh7o/vHqD7NuEKQ+4AkscXZOzdXFJrP75hHcT4MTkRlTIxHnYb2pWkcfpqNuP0AHYMQ4QpIBwK6tnKe6P8hFEYs2VXXpXLFKq4Nf8M+yvpPXCa/z7gHJM3PXmZQNTj8Y0W+6fKs+W4i0aXLnICvKKV5mvPW9m1rLX3Mx1yFvJF3d74g+D7K8SFT/TtFxKW5K4tFPtHj3y4TH7SvCQOSNn8JLn9M+9npLWLfKr2dGZ7eT6a7N3vhv1kXXnyfCc2ycRZTD5yk8+EZvp4mPlJqBqJxBjPY7mqMlYlQC3vO2FqD4kqXsGlJvBOqrX5HPqr2dGZ7eT6a7N3vhv1kXXnyfCc2ycRZTD5yk8+EZvp4mPlJqBqJxBjPY7mqMlYlQC3vO2FqD4kqXsGlJvBOqrX5HPqr2dGZ7eT6a7N3vhv1kXXnyfCc2ycRZTD5yk8+EZvp4mPlJqBqJxBjPY7mqMlYlQC3vO2FqD4kqXsGlJvBOqrX5HPqr2dGZ7eT6a7N3vhv1kXXnyfCc2ycRZTD5yk8+EZvp4mPlJqBqJxBjPY7mqMlYlQC3vO2FqD4kqXsGlJvBOqrX5HPqr2dGZ7eT6a7N3vhv1kXXnyfCc2ycRZTD5yk8+EZvp4mPlJqBqJxBjPY7mqMlYlQC3vO2FqD4kqXsGlJvBOqrX5HPqr2dGZ7eT6a7N3vhv1kXXnyfCc2ycRZTD5yk8+EZvp4mPlJqBqJxBjPY7mqMlYlQC3vO2FqD4kqXsGlJvBOqrX5HPqr2dGZ7eT6a7N3vhv1kXXnyfCc2ycRZTD5yk8+EZvp4mPlJqBqJxBjPY7mqMlYlQC3vO2FqD4kqXsGlJvBOqrX5HPqr2dGZ7eT6a7N3vhv1kXXnyfCc2ycRZTD5yk8+EZvp4mPlJqBqJxBjPY7mqMlYlQC3vO2FqD4kqXsGlJvBOqrX5HPqr2dGZ7eT6a7N3vhv1kXXnyfCc2ycRZTD5yk8+EZvp4mPlJqBqJxBjPY7mqMlYlQC3vO2FqD4kqXsGlJvBOqrX5HPqr2dGZ7eT6a7N3vhv1kXXnyfCc2ycRZTD5yk8+EZvp4mPlJqBqJxBjPY7mqMlYlQC3vO2FqD4kqXsGlJvBOqrX5HPqr2dGZ7eT6a7N3vhv1kXXnyfCc2ycRZTD5yk8+EZvp4mPlJqBqJxBjPY7mqMlYlQC3vO2FqD4kqXsGlJvBOqrX5HPqr2dGZ7eT6a7N3vhv1kXXnyfCc2ycRZTD5yk8+EZvp4mPlJqBqJxBjPY7mqMlYlQC3vO2FqD4kqXsGlJvBOqrX5HPqr2dGZ7eT6a7N3vhv1kXXnyfCc2ycRZTD5yk8+EZvp4mPlJqBqJxBjPY7mqMlYlQC3vO2FqD4kqXsGlJvBOqrX5HPqr2dGZ7eT6a7N3vhv1kXXnyfCc2ycRZTD5yk8+EZvp4mPlJqBqJxBjPY7mqMlYlQC3vO2FqD4kqXsGlJvBOqrX5HPqr2dGZ7eT6a7N3vhv1kXXnyfCc2ycRZTD5yk8+EZvp4mPlJqBqJxBjPY7mqMlYlQC3vO2FqD4kqXsGlJvBOqrX5HPqr2dGZ7eT6a7N3vhv1kXXnyfCc2ycRZTD5yk8+EZvp4mPlJqBqJxBjPY7mqMlYlQC3vO2FqD4kqXsGlJvBOqrX5HPqr2dGZ7eT6a7N3vhv1kXXnyfCc2ycRZTD5yk8+EZvp4mPlJqBqJxBjPY7mqMlYlQC3vO2FqD4kqXsGlJvBOqrX5HPqr2dGZ7eT6a7N3vhv1kXXnyfCc2ycRZTD5yk8+EZvp4mPlJqBqJxBjPY7mqMlYlQC3vO2FqD4kqXsGlJvBOqrX5HPqr2dGZ7eT6a7N3vhv1kXXnyfCc2ycRZTD5yk8+EZvp4mPlJqBqJxBjPY7mqMlYlQC3vO2FqD4kqXsGlJvBOqrX5HPqr2dGZ7eT6a7N3vhv1kXXnyfCc2ycRZTD5yk8+EZvp4mPlJqBqJxBjPY7mqMlYlQC3vO2FqD4kqXsGlJvBOqrX5HPqr2dGZ7eT6a7N3vhv1kXXnyfCc2ycRZTD5yk8+EZvp4mPlJqBqJxBjPY7mqMlYlQC3vO2FqD4kqXsGlJvBOqrX5HPqr2dGZ7eT6a7N3vhv1kXXnyfCc2ycRZTD5yk8+EZvp4mPlJqBqJxBjPY7mqMlYlQC3vO2FqD4kqXsGlJvBOqrX5HPqr2dGZ7eT6a7N3vhv1kXXnyfCc2ycRZTD5yk8+EZvp4mPlJqBqJxBjPY7mqMlYlQC3vO2FqD4kqXsGlJvBOqrX5HPqr2dGZ7eT6a7N3vhv1kXXnyfCc2ycRZTD5yk8+EZvp4mPlJqBqJxBjPY7mqMlYlQC3vO2FqD4kqXsGlJvBOqrX5HPqr2dGZ7eT6a7N3vhv1kXXnyfCc2ycRZTD5yk8+EZvp4mPlJqBqJxBjPY7mqMlYlQC3vO2FqD4kqXsGlJvBOqrX5HPqr2dGZ7eT6a7N3vhv1kXXnyfCc2ycRZTD5yk8+EZvp4mPlJqBqJxBjPY7mqMlYlQC3vO2FqD4kqXsGlJvBOqrX5HPqr2dGZ7eT6a7N3vhv1kXXnyfCc2ycRZTD5yk8+EZvp4mPlJqBqJxBjPY7mqMlYlQC3vO2FqD4kqXsGlJvBOqrX5HPqr2dGZ7eT6a7N3vhv1kXXnyfCc2ycRZTD5yk8+EZvp4mPlJqBqJxBjPY7mqMlYlQC3vO2FqD4kqXsGlJvBOqrX5HPqr2dGZ7eT6a7N3vhv1kXXnyfCc2ycRZTD5yk8+EZvp4mPlJqBqJxBjPY7mqMlYlQC3vO2FqD4kqXsGlJvBOqrX5HPqr2dGZ7eT6a7N3vhv1kXXnyfCc2ycRZTD5yk8+EZvp4mPlJqBqJxBjPY7mqMlYlQC3vO2FqD4kqXsGlJvBOqrX5HPqr2dGZ7eT6a7N3vhv1kXXnyfCc2ycRZTD5yk8+EZvp4mPlJqBqJxBjPY7mqMlYlQC3vO2FqD4kqXsGlJvBOqrX5HPqr2dGZ7eT6a7N3vhv1kXXnyfCc2ycRZTD5yk8+EZvp4mPlJqBqJxBjPY7mqMlYlQC3vO2FqD4kqXsGlJvBOqrX5HPqr2dGZ7eT6a7N3vhv1kXXnyfCc2ycRZTD5yk8+EZvp4mPlJqBqJxBjPY7mqMlYlQC3vO2FqD4kqXsGlJvBOqrX5HPqr2dGZ7eT6a7N3vhv1kXXnyfCc2ycRZTD5yk8+EZvp4mPlJqBqJxBjPY7mqMlYlQC3vO2FqD4kqXsGlJvBOqrX5HPqr2dGZ7eT6a7N3vhv1kXXnyfCc2ycRZTD5yk8+EZvp4mPlJqBqJxBjPY7mqMlYlQC3vO2FqD4kqXsGlJvBOqrX5HPqr2dGZ7eT6a7N3vhv1kXXnyfCc2ycRZTD5yk8+EZvp4mPlJqBqJxBjPY7mqMlYlQC3vO2FqD4kqXsGlJvBOqrX5HPqr2dGZ7eT6a7N3vhv1kXXnyfCc2ycRZTD5yk8+EZvp4mPlJqBqJxBjPY7mqMlYlQC3vO2FqD4kqXsGlJvBOqrX5HPqr2dGZ7eT6a7N3vhv1kXXnyfCc2ycRZTD5yk8+EZvp4mPlJqBqJxBjPY7mqMlYlQC3vO2FqD4kqXsGlJvBOqrX5HPqr2dGZ7eT6a7N3vhv1kXXnyfCc2ycRZTD5yk8+EZvp4mPlJqBqJxBjPY7mqMlYlQC3vO2FqD4kqXsGlJvBOqrX5HPqr2dGZ7eT6a7N3vhv1kXXnyfCc2ycRZTD5yk8+EZvp4mPlJqBqJxBjPY7mqMlYlQC3vO2FqD4kqXsGlJvBOqrX5HPqr2dGZ7eT6a7N3vhv1kXXnyfCc2ycRZTD5yk8+EZvp4mPlJqBqJxBjPY7mqMlYlQC3vO2FqD4kqXsGlJvBOqrX5HPqr2dGZ7eT6a7N3vhv1kXXnyfCc2ycRZTD5yk8+EZvp4mPlJqBqJxBjPY7mqMlYlQC3vO2FqD4kqXsGlJvBOqrX5HPqr2dGZ7eT6a7N3vhv1kXXnyfCc2ycRZTD5yk8+EZvp4mPlJqBqJxBjPY7mqMlYlQC3vO2FqD4kqXsGlJvBOqrX5HPqr2dGZ7eT6a7N3vhv1kXXnyfCc2ycRZTD5yk8+EZvp4mPlJqBqJxBjPY7mqMlYlQC3vO2FqD4kqXsGlJvBOqrX5HPqr2dGZ7eT6a7N3vhv1kXXnyfCc2ycRZTD5yk8+EZvp4mPlJqBqJxBjPY7mqMlYlQC3vO2FqD4kqXsGlJvBOqrX5HPqr2dGZ7eT6a7N3vhv1kXXnyfCc2ycRZTD5yk8+EZvp4mPlJqBqJxBjPY7mqMlYlQC3vO2FqD4kqXsGlJvBOqrX5HPqr2dGZ7eT6a7N3vhv1kXXnyfCc2ycRZTD5yk8+EZvp4mPlJqBqJxBjPY7mqMlYlQC3vO2FqD4kqXsGlJvBOqrX5HPqr2dGZ7eT6a7N3vhv1kXXnyfCc2ycRZTD5yk8+EZvp4mPlJqBqJxBjPY7mqMlYlQC3vO2FqD4kqXsGlJvBOqrX5HPqr2dGZ7eT6a7N3vhv1kXXnyfCc2ycRZTD5yk8+EZvp4mPlJqBqJxBjPY7mqMlYlQC3vO2FqD4kqXsGlJvBOqrX5HPqr2dGZ7eT6a7N3vhv1kXXnyfCc2ycRZTD5yk8+EZvp4mPlJqBqJxBjPY7mqMlYlQC3vO2FqD4kqXsGlJvBOqrX5HPqr2dGZ7eT6a7N3vhv1kXXnyfCc2ycRZTD5yk8+EZvp4mPlJqBqJxBjPY7mqMlYlQC3vO2FqD4kqXsGlJvBOqrX5HPqr2dGZ7eT6a7N3vhv1kXXnyfCc2ycRZTD5yk8+EZvp4mPlJqBqJxBjPY7mqMlYlQC3vO2FqD4kqXsGlJvBOqrX5HPqr2dGZ7eT6a7N3vhv1kXXnyfCc2ycRZTD5yk8+EZvp4mPlJqBqJxBjPY7mqMlYlQC3vO2FqD4kqXsGlJvBOqrX5HPqr2dGZ7eT6a7N3vhv1kXXnyfCc2ycRZTD5yk8+EZvp4mPlJqBqJxBjPY7mqMlYlQC3vO2FqD4kqXsGlJvBOqrX5HPqr2dGZ7eT6a7N3vhv1kXXnyfCc2ycRZTD5yk8+EZvp4mPlJqBqJxBjPY7mqMlYlQC3vO2FqD4kqXsGlJvBOqr
        /* Leaflet Draw CSS */
        .leaflet-draw-section{position:relative}.leaflet-draw-toolbar{margin-top:12px}.leaflet-draw-toolbar-top{margin-top:0}.leaflet-draw-toolbar-notop a:first-child{border-top-right-radius:0}.leaflet-draw-toolbar-nobottom a:last-child{border-bottom-right-radius:0}.leaflet-draw-toolbar a{background-image:url('data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIzMDAiIGhlaWdodD0iMzAwIj48cmVjdCB3aWR0aD0iMzAwIiBoZWlnaHQ9IjMwMCIgZmlsbD0ibm9uZSIvPjwvc3ZnPg==');background-repeat:no-repeat}.leaflet-draw a{display:block;text-align:center;text-decoration:none}.leaflet-draw a .sr-only{position:absolute;width:1px;height:1px;padding:0;margin:-1px;overflow:hidden;clip:rect(0,0,0,0);border:0}.leaflet-draw-actions{display:none;list-style:none;margin:0;padding:0;position:absolute;left:26px;top:0;white-space:nowrap}.leaflet-touch .leaflet-draw-actions{left:32px}.leaflet-right .leaflet-draw-actions{right:26px;left:auto}.leaflet-touch .leaflet-right .leaflet-draw-actions{right:32px;left:auto}.leaflet-draw-actions li{display:inline-block}.leaflet-draw-actions li:first-child a{border-left:none}.leaflet-draw-actions li:last-child a{-webkit-border-radius:0 4px 4px 0;border-radius:0 4px 4px 0}.leaflet-right .leaflet-draw-actions li:last-child a{-webkit-border-radius:0;border-radius:0}.leaflet-right .leaflet-draw-actions li:first-child a{-webkit-border-radius:4px 0 0 4px;border-radius:4px 0 0 4px}.leaflet-draw-actions a{background-color:#919187;border-left:1px solid #AAA;color:#FFF;font:11px/19px "Helvetica Neue",Arial,Helvetica,sans-serif;line-height:28px;text-decoration:none;padding-left:10px;padding-right:10px;height:28px}.leaflet-touch .leaflet-draw-actions a{font-size:12px;line-height:30px;height:30px}.leaflet-draw-actions-bottom{margin-top:0}.leaflet-draw-actions-top{margin-top:1px}.leaflet-draw-actions-top a,.leaflet-draw-actions-bottom a{height:27px;line-height:27px}.leaflet-draw-actions a:hover{background-color:#a0a098}.leaflet-draw-actions-top.leaflet-draw-actions-bottom a{height:26px;line-height:26px}.leaflet-draw-toolbar .leaflet-draw-draw-polyline{background-position:-2px -2px}.leaflet-touch .leaflet-draw-toolbar .leaflet-draw-draw-polyline{background-position:0 -1px}.leaflet-draw-toolbar .leaflet-draw-draw-polygon{background-position:-31px -2px}.leaflet-touch .leaflet-draw-toolbar .leaflet-draw-draw-polygon{background-position:-29px -1px}.leaflet-draw-toolbar .leaflet-draw-draw-rectangle{background-position:-62px -2px}.leaflet-touch .leaflet-draw-toolbar .leaflet-draw-draw-rectangle{background-position:-60px -1px}.leaflet-draw-toolbar .leaflet-draw-draw-circle{background-position:-92px -2px}.leaflet-touch .leaflet-draw-toolbar .leaflet-draw-draw-circle{background-position:-90px -1px}.leaflet-draw-toolbar .leaflet-draw-draw-marker{background-position:-122px -2px}.leaflet-touch .leaflet-draw-toolbar .leaflet-draw-draw-marker{background-position:-120px -1px}.leaflet-draw-toolbar .leaflet-draw-draw-circlemarker{background-position:-273px -2px}.leaflet-touch .leaflet-draw-toolbar .leaflet-draw-draw-circlemarker{background-position:-271px -1px}.leaflet-draw-toolbar .leaflet-draw-edit-edit{background-position:-152px -2px}.leaflet-touch .leaflet-draw-toolbar .leaflet-draw-edit-edit{background-position:-150px -1px}.leaflet-draw-toolbar .leaflet-draw-edit-remove{background-position:-182px -2px}.leaflet-touch .leaflet-draw-toolbar .leaflet-draw-edit-remove{background-position:-180px -1px}.leaflet-draw-toolbar .leaflet-draw-edit-edit.leaflet-disabled{background-position:-212px -2px}.leaflet-touch .leaflet-draw-toolbar .leaflet-draw-edit-edit.leaflet-disabled{background-position:-210px -1px}.leaflet-draw-toolbar .leaflet-draw-edit-remove.leaflet-disabled{background-position:-242px -2px}.leaflet-touch .leaflet-draw-toolbar .leaflet-draw-edit-remove.leaflet-disabled{background-position:-240px -2px}.leaflet-mouse-marker{background-color:#fff;cursor:crosshair}.leaflet-draw-tooltip{background:#363636;background:rgba(0,0,0,.5);border:1px solid transparent;-webkit-border-radius:4px;border-radius:4px;color:#fff;font:12px/18px "Helvetica Neue",Arial,Helvetica,sans-serif;margin-left:20px;margin-top:-21px;padding:4px 8px;position:absolute;visibility:hidden;white-space:nowrap;z-index:6}.leaflet-draw-tooltip:before{border-right:6px solid black;border-right-color:rgba(0,0,0,.5);border-top:6px solid transparent;border-bottom:6px solid transparent;content:"";position:absolute;top:7px;left:-7px}.leaflet-error-draw-tooltip{background-color:#f2dede;border:1px solid #e6b6bd;color:#b94a48}.leaflet-error-draw-tooltip:before{border-right-color:#e6b6bd}.leaflet-draw-tooltip-single{margin-top:-12px}.leaflet-draw-tooltip-subtext{color:#f8d5e4}.leaflet-draw-guide-dash{font-size:1%;opacity:.6;position:absolute;width:5px;height:5px}.leaflet-edit-marker-selected{background-color:rgba(254,87,161,.1);border:4px dashed rgba(254,87,161,.6);-webkit-border-radius:4px;border-radius:4px;box-sizing:content-box}.leaflet-edit-move{cursor:move}.leaflet-edit-resize{cursor:pointer}.leaflet-oldie .leaflet-draw-toolbar{border:1px solid #999}
        
        :root {
            --primary-blue: #009edb;
            --dark-blue: #1d5289;
            --success-green: #00a86b;
            --warning-orange: #ff8c42;
            --danger-red: #dc3545;
            --protected-green: #2d5016;
            --marine-blue: #006994;
            --forest-green: #228B22;
            --cca-purple: #9b59b6;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Segoe UI', 'Helvetica Neue', Arial, sans-serif;
            height: 100vh;
            display: flex;
            flex-direction: column;
            overflow: hidden;
            background: #f8f9fa;
        }
        
        .header {
            background: linear-gradient(135deg, var(--dark-blue) 0%, var(--primary-blue) 100%);
            color: white;
            padding: 15px 30px;
            box-shadow: 0 2px 8px rgba(0,0,0,0.15);
            z-index: 2000;
        }
        
        .header-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
            max-width: 1920px;
            margin: 0 auto;
        }
        
        .header-title {
            display: flex;
            align-items: center;
            gap: 15px;
        }
        
        .logo {
            font-size: 40px;
        }
        
        .title-text h1 {
            font-size: 20px;
            font-weight: 700;
            letter-spacing: 0.5px;
            margin-bottom: 2px;
        }
        
        .title-text h2 {
            font-size: 13px;
            opacity: 0.95;
            font-weight: 400;
        }
        
        .header-stats {
            display: flex;
            gap: 30px;
        }
        
        .header-stat {
            text-align: right;
        }
        
        .stat-label {
            font-size: 11px;
            opacity: 0.85;
            text-transform: uppercase;
            letter-spacing: 0.5px;
        }
        
        .stat-value {
            font-size: 24px;
            font-weight: 700;
            margin-top: 2px;
        }
        
        .stat-unit {
            font-size: 14px;
            opacity: 0.9;
        }
        
        .main-container {
            display: flex;
            flex: 1;
            overflow: hidden;
        }
        
        .sidebar {
            width: 420px;
            background: white;
            overflow-y: auto;
            box-shadow: 2px 0 15px rgba(0,0,0,0.1);
            z-index: 1000;
        }
        
        .panel-section {
            padding: 20px;
            border-bottom: 1px solid #e0e0e0;
        }
        
        .section-title {
            font-size: 14px;
            font-weight: 700;
            color: var(--dark-blue);
            text-transform: uppercase;
            letter-spacing: 0.5px;
            margin-bottom: 15px;
            display: flex;
            align-items: center;
            gap: 8px;
        }
        
        .section-title::before {
            content: '';
            width: 4px;
            height: 16px;
            background: var(--primary-blue);
            border-radius: 2px;
        }
        
        #map {
            flex: 1;
            height: 100%;
            background: #e8f4f8;
        }
        
        .progress-card {
            background: linear-gradient(135deg, #f8f9fa 0%, #e9ecef 100%);
            border-left: 5px solid var(--success-green);
            padding: 20px;
            border-radius: 8px;
            margin: 15px 0;
        }
        
        .progress-title {
            font-size: 13px;
            font-weight: 700;
            color: var(--dark-blue);
            margin-bottom: 10px;
            text-transform: uppercase;
        }
        
        .progress-bar-container {
            background: white;
            height: 40px;
            border-radius: 20px;
            overflow: hidden;
            position: relative;
            margin: 15px 0;
            box-shadow: inset 0 2px 4px rgba(0,0,0,0.1);
        }
        
        .progress-bar {
            height: 100%;
            background: linear-gradient(90deg, var(--success-green) 0%, #00d084 100%);
            transition: width 0.8s ease;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-weight: 700;
            font-size: 16px;
        }
        
        .progress-target {
            position: absolute;
            right: 0;
            top: 0;
            bottom: 0;
            width: 2px;
            background: var(--danger-red);
            box-shadow: 0 0 10px rgba(220, 53, 69, 0.5);
        }
        
        .progress-target::after {
            content: '30% Target';
            position: absolute;
            right: 5px;
            top: 50%;
            transform: translateY(-50%);
            font-size: 10px;
            color: var(--danger-red);
            font-weight: 700;
            white-space: nowrap;
        }
        
        .progress-details {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 15px;
            margin-top: 15px;
        }
        
        .detail-item {
            background: white;
            padding: 12px;
            border-radius: 6px;
            border: 1px solid #dee2e6;
        }
        
        .detail-label {
            font-size: 11px;
            color: #6c757d;
            text-transform: uppercase;
            letter-spacing: 0.5px;
            margin-bottom: 5px;
        }
        
        .detail-value {
            font-size: 18px;
            font-weight: 700;
            color: var(--dark-blue);
        }
        
        .layer-group {
            margin: 15px 0;
        }
        
        .layer-group-title {
            font-size: 12px;
            font-weight: 700;
            color: #495057;
            margin-bottom: 10px;
            text-transform: uppercase;
            letter-spacing: 0.3px;
        }
        
        .layer-item {
            display: flex;
            align-items: center;
            padding: 12px;
            background: #f8f9fa;
            border: 1px solid #dee2e6;
            border-radius: 6px;
            margin: 8px 0;
            cursor: pointer;
            transition: all 0.2s;
        }
        
        .layer-item:hover {
            background: #e7f3ff;
            border-color: var(--primary-blue);
        }
        
        .layer-checkbox {
            width: 20px;
            height: 20px;
            margin-right: 12px;
            cursor: pointer;
            accent-color: var(--primary-blue);
        }
        
        .layer-info {
            flex: 1;
        }
        
        .layer-name {
            font-size: 13px;
            font-weight: 600;
            color: #495057;
            margin-bottom: 2px;
        }
        
        .layer-meta {
            font-size: 11px;
            color: #6c757d;
        }
        
        .layer-color {
            width: 30px;
            height: 30px;
            border-radius: 4px;
            border: 2px solid white;
            box-shadow: 0 2px 4px rgba(0,0,0,0.2);
            margin-left: 10px;
        }
        
        .chart-container {
            background: white;
            padding: 20px;
            border-radius: 8px;
            margin: 15px 0;
            border: 1px solid #dee2e6;
        }
        
        .chart-title {
            font-size: 13px;
            font-weight: 700;
            color: var(--dark-blue);
            margin-bottom: 15px;
            text-align: center;
        }
        
        .upload-zone {
            border: 3px dashed #dee2e6;
            border-radius: 8px;
            padding: 25px 20px;
            text-align: center;
            background: #f8f9fa;
            cursor: pointer;
            transition: all 0.3s;
            margin: 15px 0;
            position: relative;
        }
        
        .upload-zone:hover {
            border-color: var(--primary-blue);
            background: #e7f3ff;
            transform: translateY(-2px);
        }
        
        .upload-zone:active {
            transform: translateY(0);
        }
        
        .upload-icon {
            font-size: 40px;
            margin-bottom: 10px;
        }
        
        .upload-text {
            font-size: 13px;
            font-weight: 600;
            color: #495057;
            margin-bottom: 5px;
        }
        
        .upload-subtext {
            font-size: 11px;
            color: #6c757d;
        }
        
        .file-input {
            position: absolute;
            opacity: 0;
            width: 0.1px;
            height: 0.1px;
            z-index: -1;
        }
        
        .uploaded-files {
            margin-top: 10px;
        }
        
        .file-item {
            display: flex;
            align-items: center;
            justify-content: space-between;
            padding: 10px 12px;
            background: white;
            border: 1px solid #dee2e6;
            border-radius: 6px;
            margin: 8px 0;
            font-size: 12px;
        }
        
        .file-info {
            display: flex;
            align-items: center;
            gap: 10px;
            flex: 1;
        }
        
        .file-actions {
            display: flex;
            gap: 5px;
        }
        
        .btn-icon {
            background: white;
            border: 1px solid #dee2e6;
            cursor: pointer;
            font-size: 16px;
            padding: 6px 10px;
            border-radius: 4px;
            transition: all 0.2s;
        }
        
        .btn-icon:hover {
            background: var(--primary-blue);
            color: white;
            border-color: var(--primary-blue);
        }
        
        .button-primary {
            width: 100%;
            padding: 14px;
            background: linear-gradient(135deg, var(--primary-blue) 0%, var(--dark-blue) 100%);
            color: white;
            border: none;
            border-radius: 6px;
            font-size: 13px;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s;
            text-transform: uppercase;
            letter-spacing: 0.5px;
            margin: 8px 0;
        }
        
        .button-primary:hover {
            transform: translateY(-2px);
            box-shadow: 0 6px 20px rgba(0, 158, 219, 0.4);
        }
        
        .stats-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 12px;
            margin: 15px 0;
        }
        
        .stat-card {
            background: white;
            padding: 15px;
            border-radius: 6px;
            border-left: 4px solid var(--primary-blue);
            box-shadow: 0 2px 4px rgba(0,0,0,0.05);
        }
        
        .stat-card-label {
            font-size: 11px;
            color: #6c757d;
            text-transform: uppercase;
            letter-spacing: 0.5px;
            margin-bottom: 6px;
        }
        
        .stat-card-value {
            font-size: 20px;
            font-weight: 700;
            color: var(--dark-blue);
        }
        
        .alert {
            padding: 12px 15px;
            border-radius: 6px;
            margin: 10px 0;
            font-size: 12px;
            display: none;
        }
        
        .alert-success {
            background: #d4edda;
            border: 1px solid #c3e6cb;
            color: #155724;
        }
        
        .alert-info {
            background: #d1ecf1;
            border: 1px solid #bee5eb;
            color: #0c5460;
        }
        
        .legend-box {
            background: white;
            padding: 15px;
            border-radius: 6px;
            border: 1px solid #dee2e6;
            margin: 15px 0;
        }
        
        .legend-title {
            font-size: 12px;
            font-weight: 700;
            color: var(--dark-blue);
            margin-bottom: 12px;
            text-transform: uppercase;
        }
        
        .legend-item {
            display: flex;
            align-items: center;
            margin: 8px 0;
        }
        
        .legend-color {
            width: 30px;
            height: 20px;
            border-radius: 3px;
            border: 1px solid #dee2e6;
            margin-right: 12px;
        }
        
        .legend-text {
            font-size: 12px;
            color: #495057;
            font-weight: 500;
        }
        
        .info-box {
            background: #e7f3ff;
            border-left: 4px solid var(--primary-blue);
            padding: 12px 15px;
            border-radius: 4px;
            font-size: 12px;
            line-height: 1.6;
            color: #495057;
            margin: 15px 0;
        }
        
        .info-box strong {
            color: var(--dark-blue);
            display: block;
            margin-bottom: 5px;
        }
        
        .category-container {
            background: #f8f9fa;
            border: 1px solid #dee2e6;
            border-radius: 6px;
            padding: 10px;
            margin: 10px 0;
        }
        
        .category-header {
            font-size: 12px;
            font-weight: 700;
            color: var(--dark-blue);
            padding: 8px 10px;
            background: white;
            border-radius: 4px;
            margin-bottom: 8px;
            cursor: move;
            display: flex;
            align-items: center;
            justify-content: space-between;
        }
        
        .category-header:hover {
            background: #e7f3ff;
        }
        
        .drag-handle {
            font-size: 16px;
            color: #6c757d;
            cursor: grab;
        }
        
        .drag-handle:active {
            cursor: grabbing;
        }
        
        .layer-controls {
            display: flex;
            gap: 5px;
            margin-top: 8px;
            padding: 8px;
            background: #f8f9fa;
            border-radius: 4px;
            border: 1px solid #dee2e6;
        }
        
        .control-group {
            flex: 1;
            display: flex;
            flex-direction: column;
            gap: 4px;
        }
        
        .control-label {
            font-size: 10px;
            font-weight: 600;
            color: #6c757d;
            text-transform: uppercase;
            letter-spacing: 0.5px;
        }
        
        .control-input {
            width: 100%;
            padding: 4px 6px;
            border: 1px solid #dee2e6;
            border-radius: 3px;
            font-size: 11px;
        }
        
        .color-input {
            width: 100%;
            height: 28px;
            border: 1px solid #dee2e6;
            border-radius: 3px;
            cursor: pointer;
        }
        
        .dragging {
            opacity: 0.5;
        }
        
        .drag-over {
            border: 2px dashed var(--primary-blue);
            background: #e7f3ff;
        }
        
        .form-label {
            font-size: 12px;
            font-weight: 600;
            color: #495057;
            text-transform: uppercase;
            letter-spacing: 0.3px;
        }
        
        .footer {
            background: #f8f9fa;
            padding: 12px 20px;
            text-align: center;
            font-size: 11px;
            color: #6c757d;
            border-top: 1px solid #dee2e6;
        }
        
        .loading {
            position: fixed;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            background: rgba(255, 255, 255, 0.98);
            padding: 40px 50px;
            border-radius: 12px;
            box-shadow: 0 10px 40px rgba(0,0,0,0.3);
            z-index: 3000;
            display: none;
            text-align: center;
        }
        
        .spinner {
            border: 4px solid #f3f3f3;
            border-top: 4px solid var(--primary-blue);
            border-radius: 50%;
            width: 50px;
            height: 50px;
            animation: spin 1s linear infinite;
            margin: 0 auto 20px;
        }
        
        @keyframes spin {
            0% { transform: rotate(0deg); }
            100% { transform: rotate(360deg); }
        }
        
        .measurement-controls {
            background: white;
            padding: 15px;
            border-radius: 6px;
            border: 1px solid #dee2e6;
            margin: 15px 0;
        }
        
        .measurement-title {
            font-size: 12px;
            font-weight: 700;
            color: var(--dark-blue);
            margin-bottom: 10px;
            text-transform: uppercase;
        }
        
        .measurement-result {
            background: #f8f9fa;
            padding: 12px;
            border-radius: 4px;
            margin-top: 10px;
            font-size: 13px;
            color: #495057;
            display: none;
        }
        
        @media (max-width: 1024px) {
            .sidebar {
                width: 350px;
            }
        }
    </style>
</head>
<body>
    <div class="header">
        <div class="header-content">
            <div class="header-title">
                <div class="logo">🌏</div>
                <div class="title-text">
                    <h1>Vanuatu National Biodiversity Strategy and Action Plan (NBSAP)</h1>
                    <h2>Target 3: 30x30 Protected Area Monitoring Platform | Department of Environmental Protection and Conservation</h2>
                </div>
            </div>
            <div class="header-stats">
                <div class="header-stat">
                    <div class="stat-label">Current Coverage</div>
                    <div class="stat-value"><span id="current-percentage">18.5</span><span class="stat-unit">%</span></div>
                </div>
                <div class="header-stat">
                    <div class="stat-label">2030 Target</div>
                    <div class="stat-value">30<span class="stat-unit">%</span></div>
                </div>
                <div class="header-stat">
                    <div class="stat-label">Gap to Target</div>
                    <div class="stat-value"><span id="gap-percentage">11.5</span><span class="stat-unit">%</span></div>
                </div>
            </div>
        </div>
    </div>
    
    <div class="main-container">
        <div class="sidebar">
            <div class="panel-section">
                <div class="section-title">📊 Progress to NBSAP Target 3</div>
                
                <div class="progress-card">
                    <div class="progress-title">Protected Area Coverage Progress</div>
                    <div class="progress-bar-container">
                        <div class="progress-bar" id="progress-bar" style="width: 61.7%;">
                            <span id="progress-text">18.5%</span>
                        </div>
                        <div class="progress-target" style="left: 30%;"></div>
                    </div>
                    
                    <div class="progress-details">
                        <div class="detail-item">
                            <div class="detail-label">Protected Area</div>
                            <div class="detail-value"><span id="protected-area">2,261</span> km²</div>
                        </div>
                        <div class="detail-item">
                            <div class="detail-label">Total Land & Sea</div>
                            <div class="detail-value"><span id="total-area">12,189</span> km²</div>
                        </div>
                        <div class="detail-item">
                            <div class="detail-label">Additional Needed</div>
                            <div class="detail-value"><span id="gap-area">1,396</span> km²</div>
                        </div>
                        <div class="detail-item">
                            <div class="detail-label">Time to 2030</div>
                            <div class="detail-value"><span id="years-left">4.9</span> years</div>
                        </div>
                    </div>
                </div>
                
                <div class="chart-container">
                    <div class="chart-title">Coverage Breakdown by Type</div>
                    <canvas id="coverage-chart" height="200"></canvas>
                </div>
            </div>
            
            <div class="panel-section">
                <div class="section-title">🗺️ Conservation Layers</div>
                
                <div class="layer-group">
                    <div class="layer-group-title">Protected Areas</div>
                    <div class="layer-item" id="layer-item-mpa">
                        <input type="checkbox" class="layer-checkbox" id="check-mpa" checked>
                        <div class="layer-info">
                            <div class="layer-name">Marine Protected Areas (MPAs)</div>
                            <div class="layer-meta">Coverage: <span id="mpa-coverage">1,850</span> km² | <span id="mpa-count">6</span> sites</div>
                        </div>
                        <div class="layer-color" style="background: var(--marine-blue);"></div>
                    </div>
                    
                    <div class="layer-item" id="layer-item-terrestrial">
                        <input type="checkbox" class="layer-checkbox" id="check-terrestrial" checked>
                        <div class="layer-info">
                            <div class="layer-name">Terrestrial Protected Areas</div>
                            <div class="layer-meta">Coverage: <span id="terrestrial-coverage">245</span> km² | <span id="terrestrial-count">4</span> sites</div>
                        </div>
                        <div class="layer-color" style="background: var(--protected-green);"></div>
                    </div>
                    
                    <div class="layer-item" id="layer-item-cca">
                        <input type="checkbox" class="layer-checkbox" id="check-cca" checked>
                        <div class="layer-info">
                            <div class="layer-name">Community Conservation Areas (CCAs)</div>
                            <div class="layer-meta">Coverage: <span id="cca-coverage">166</span> km² | <span id="cca-count">12</span> sites</div>
                        </div>
                        <div class="layer-color" style="background: var(--cca-purple);"></div>
                    </div>
                </div>
                
                <div class="layer-group">
                    <div class="layer-group-title">Biodiversity Features</div>
                    <div class="layer-item" id="layer-item-kba">
                        <input type="checkbox" class="layer-checkbox" id="check-kba">
                        <div class="layer-info">
                            <div class="layer-name">Key Biodiversity Areas (KBAs)</div>
                            <div class="layer-meta"><span id="kba-count">15</span> identified sites</div>
                        </div>
                        <div class="layer-color" style="background: #e74c3c;"></div>
                    </div>
                    
                    <div class="layer-item" id="layer-item-forest">
                        <input type="checkbox" class="layer-checkbox" id="check-forest">
                        <div class="layer-info">
                            <div class="layer-name">Forest Cover</div>
                            <div class="layer-meta">Dense & Open Forest</div>
                        </div>
                        <div class="layer-color" style="background: var(--forest-green);"></div>
                    </div>
                    
                    <div class="layer-item" id="layer-item-mangrove">
                        <input type="checkbox" class="layer-checkbox" id="check-mangrove">
                        <div class="layer-info">
                            <div class="layer-name">Mangrove Areas</div>
                            <div class="layer-meta">Coastal wetlands</div>
                        </div>
                        <div class="layer-color" style="background: #00CED1;"></div>
                    </div>
                </div>
                
                <div class="info-box">
                    <strong>Note on Coverage Calculation</strong>
                    Protected area percentage calculated as: (Total Protected Area / Total Land & Sea Area) × 100. Includes terrestrial, marine, and community-conserved areas.
                </div>
            </div>
            
            <div class="panel-section">
                <div class="section-title">📤 Upload Data by Category</div>
                
                <div style="margin-bottom: 15px;">
                    <label class="form-label" style="display: block; margin-bottom: 8px;">Select Category</label>
                    <select id="upload-category" style="width: 100%; padding: 10px; border: 2px solid #dee2e6; border-radius: 6px; font-size: 13px; font-weight: 600;">
                        <option value="mpa">🌊 Marine Protected Areas</option>
                        <option value="terrestrial">🌲 Terrestrial Protected Areas</option>
                        <option value="cca">🏘️ Community Conservation Areas</option>
                        <option value="kba">🦜 Key Biodiversity Areas</option>
                        <option value="proposed">📋 Proposed Protected Areas</option>
                        <option value="forest">🌳 Forest Cover</option>
                        <option value="mangrove">🌴 Mangrove Areas</option>
                        <option value="other">📍 Other Features</option>
                    </select>
                </div>
                
                <div class="upload-zone" id="upload-zone">
                    <div class="upload-icon">📁</div>
                    <div class="upload-text">Upload to <span id="category-display" style="font-weight: 700; color: var(--marine-blue);">Marine Protected Areas</span></div>
                    <div class="upload-subtext">Drag & drop or click (.shp, .zip, .geojson)</div>
                </div>
                <input type="file" id="file-input" class="file-input" accept=".shp,.zip,.geojson,.kml,.json" multiple>
                
                <div class="alert" id="upload-alert"></div>
                
                <div style="margin-top: 20px;">
                    <div class="layer-group-title">Uploaded Layers</div>
                    <div id="category-containers">
                        <div id="category-mpa" class="category-container" style="display: none;">
                            <div class="category-header">🌊 Marine Protected Areas</div>
                            <div class="uploaded-files" data-category="mpa"></div>
                        </div>
                        <div id="category-terrestrial" class="category-container" style="display: none;">
                            <div class="category-header">🌲 Terrestrial Protected Areas</div>
                            <div class="uploaded-files" data-category="terrestrial"></div>
                        </div>
                        <div id="category-cca" class="category-container" style="display: none;">
                            <div class="category-header">🏘️ Community Conservation Areas</div>
                            <div class="uploaded-files" data-category="cca"></div>
                        </div>
                        <div id="category-kba" class="category-container" style="display: none;">
                            <div class="category-header">🦜 Key Biodiversity Areas</div>
                            <div class="uploaded-files" data-category="kba"></div>
                        </div>
                        <div id="category-proposed" class="category-container" style="display: none;">
                            <div class="category-header">📋 Proposed Protected Areas</div>
                            <div class="uploaded-files" data-category="proposed"></div>
                        </div>
                        <div id="category-forest" class="category-container" style="display: none;">
                            <div class="category-header">🌳 Forest Cover</div>
                            <div class="uploaded-files" data-category="forest"></div>
                        </div>
                        <div id="category-mangrove" class="category-container" style="display: none;">
                            <div class="category-header">🌴 Mangrove Areas</div>
                            <div class="uploaded-files" data-category="mangrove"></div>
                        </div>
                        <div id="category-other" class="category-container" style="display: none;">
                            <div class="category-header">📍 Other Features</div>
                            <div class="uploaded-files" data-category="other"></div>
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="panel-section">
                <div class="section-title">📏 Spatial Analysis Tools</div>
                
                <div class="measurement-controls">
                    <div class="measurement-title">Calculate Area</div>
                    <button class="button-primary" id="btn-measure">🔧 Measure Polygon Area</button>
                    <div class="measurement-result" id="measurement-result"></div>
                </div>
                
                <button class="button-primary" id="btn-report">📄 Generate Progress Report</button>
                <button class="button-primary" id="btn-export-geojson">💾 Export All Data (GeoJSON)</button>
                <button class="button-primary" id="btn-export-csv">📊 Export Summary Statistics (CSV)</button>
            </div>
            
            <div class="panel-section">
                <div class="section-title">📖 Legend</div>
                
                <div class="legend-box">
                    <div class="legend-title">Conservation Categories</div>
                    <div class="legend-item">
                        <div class="legend-color" style="background: var(--marine-blue);"></div>
                        <div class="legend-text">Marine Protected Areas</div>
                    </div>
                    <div class="legend-item">
                        <div class="legend-color" style="background: var(--protected-green);"></div>
                        <div class="legend-text">Terrestrial Protected Areas</div>
                    </div>
                    <div class="legend-item">
                        <div class="legend-color" style="background: var(--cca-purple);"></div>
                        <div class="legend-text">Community Conservation Areas</div>
                    </div>
                    <div class="legend-item">
                        <div class="legend-color" style="background: #e74c3c;"></div>
                        <div class="legend-text">Key Biodiversity Areas</div>
                    </div>
                    <div class="legend-item">
                        <div class="legend-color" style="background: var(--forest-green);"></div>
                        <div class="legend-text">Forest Cover</div>
                    </div>
                    <div class="legend-item">
                        <div class="legend-color" style="background: #00CED1;"></div>
                        <div class="legend-text">Mangrove Areas</div>
                    </div>
                </div>
            </div>
        </div>
        
        <div id="map"></div>
    </div>
    
    <div class="footer">
        © 2025 Government of Vanuatu | Department of Environmental Protection and Conservation (DEPC)<br>
        NBSAP Target 3 Monitoring Platform | Data Sources: DEPC, IUCN, UNEP-WCMC | Last Updated: February 2026
    </div>
    
    <div class="loading" id="loading">
        <div class="spinner"></div>
        <div style="font-weight: 600; color: var(--dark-blue);">Loading spatial data...</div>
    </div>
    
    <script src="https://cdn.jsdelivr.net/npm/leaflet@1.9.4/dist/leaflet.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/leaflet-draw@1.0.4/dist/leaflet.draw.js"></script>
    
    <script>
        // Global variables
        let map;
        let layers = {
            mpa: null,
            terrestrial: null,
            cca: null,
            kba: null,
            forest: null,
            mangrove: null
        };
        let uploadedLayers = [];
        let layerCounter = 0;
        let drawControl;
        let drawnItems;
        
        // Dynamic layer categories
        let dynamicCategories = {
            mpa: { area: 0, count: 0, layers: [] },
            terrestrial: { area: 0, count: 0, layers: [] },
            cca: { area: 0, count: 0, layers: [] },
            kba: { area: 0, count: 0, layers: [] },
            proposed: { area: 0, count: 0, layers: [] },
            other: { area: 0, count: 0, layers: [] }
        };
        
        // Conservation area data
        const conservationData = {
            totalLandSeaArea: 12189, // km² (land ~12,200 + EEZ portion)
            mpa: { area: 1850, count: 6, color: '#006994' },
            terrestrial: { area: 245, count: 4, color: '#2d5016' },
            cca: { area: 166, count: 12, color: '#9b59b6' }
        };
        
        function calculateProgress() {
            const totalProtected = conservationData.mpa.area + 
                                  conservationData.terrestrial.area + 
                                  conservationData.cca.area;
            const percentage = (totalProtected / conservationData.totalLandSeaArea * 100);
            const target = 30;
            const gap = target - percentage;
            const gapArea = (gap / 100) * conservationData.totalLandSeaArea;
            
            return {
                totalProtected,
                percentage: percentage.toFixed(1),
                gap: gap.toFixed(1),
                gapArea: Math.round(gapArea)
            };
        }
        
        function updateDashboard() {
            console.log('Updating dashboard...');
            const progress = calculateProgress();
            
            document.getElementById('current-percentage').textContent = progress.percentage;
            document.getElementById('gap-percentage').textContent = progress.gap;
            document.getElementById('protected-area').textContent = progress.totalProtected.toFixed(0);
            document.getElementById('total-area').textContent = conservationData.totalLandSeaArea.toLocaleString();
            document.getElementById('gap-area').textContent = progress.gapArea.toLocaleString();
            
            const progressBar = document.getElementById('progress-bar');
            const progressWidth = (progress.percentage / 30) * 100;
            progressBar.style.width = Math.min(progressWidth, 100) + '%';
            document.getElementById('progress-text').textContent = progress.percentage + '%';
            
            const now = new Date();
            const target = new Date('2030-12-31');
            const yearsLeft = ((target - now) / (1000 * 60 * 60 * 24 * 365)).toFixed(1);
            document.getElementById('years-left').textContent = yearsLeft;
            
            // Update layer coverage displays
            const totalMPA = conservationData.mpa.area + (dynamicCategories.mpa ? dynamicCategories.mpa.area : 0);
            const totalTerrestrial = conservationData.terrestrial.area + (dynamicCategories.terrestrial ? dynamicCategories.terrestrial.area : 0);
            const totalCCA = conservationData.cca.area + (dynamicCategories.cca ? dynamicCategories.cca.area : 0);
            
            document.getElementById('mpa-coverage').textContent = totalMPA.toFixed(0);
            document.getElementById('terrestrial-coverage').textContent = totalTerrestrial.toFixed(0);
            document.getElementById('cca-coverage').textContent = totalCCA.toFixed(0);
            
            const totalMPACount = conservationData.mpa.count + (dynamicCategories.mpa ? dynamicCategories.mpa.count : 0);
            const totalTerrestrialCount = conservationData.terrestrial.count + (dynamicCategories.terrestrial ? dynamicCategories.terrestrial.count : 0);
            const totalCCACount = conservationData.cca.count + (dynamicCategories.cca ? dynamicCategories.cca.count : 0);
            
            document.getElementById('mpa-count').textContent = totalMPACount;
            document.getElementById('terrestrial-count').textContent = totalTerrestrialCount;
            document.getElementById('cca-count').textContent = totalCCACount;
            
            console.log('Dashboard updated successfully');
        }
        
        function createChart() {
            console.log('Creating/updating chart...');
            const ctx = document.getElementById('coverage-chart');
            if (!ctx) {
                console.error('Chart canvas not found');
                return;
            }
            
            // Destroy existing chart if it exists
            if (window.coverageChart) {
                window.coverageChart.destroy();
            }
            
            const totalMPA = conservationData.mpa.area + (dynamicCategories.mpa ? dynamicCategories.mpa.area : 0);
            const totalTerrestrial = conservationData.terrestrial.area + (dynamicCategories.terrestrial ? dynamicCategories.terrestrial.area : 0);
            const totalCCA = conservationData.cca.area + (dynamicCategories.cca ? dynamicCategories.cca.area : 0);
            const totalProtected = totalMPA + totalTerrestrial + totalCCA;
            const unprotected = conservationData.totalLandSeaArea - totalProtected;
            
            window.coverageChart = new Chart(ctx, {
                type: 'doughnut',
                data: {
                    labels: ['Marine Protected Areas', 'Terrestrial Protected', 'Community Conservation', 'Unprotected'],
                    datasets: [{
                        data: [
                            totalMPA,
                            totalTerrestrial,
                            totalCCA,
                            unprotected
                        ],
                        backgroundColor: [
                            conservationData.mpa.color,
                            conservationData.terrestrial.color,
                            conservationData.cca.color,
                            '#e0e0e0'
                        ],
                        borderWidth: 2,
                        borderColor: '#fff'
                    }]
                },
                options: {
                    responsive: true,
                    maintainAspectRatio: true,
                    plugins: {
                        legend: {
                            position: 'bottom',
                            labels: {
                                padding: 15,
                                font: { size: 11 },
                                usePointStyle: true
                            }
                        },
                        tooltip: {
                            callbacks: {
                                label: function(context) {
                                    const value = context.parsed;
                                    const total = context.dataset.data.reduce((a, b) => a + b, 0);
                                    const percentage = ((value / total) * 100).toFixed(1);
                                    return `${context.label}: ${value.toFixed(0)} km² (${percentage}%)`;
                                }
                            }
                        }
                    }
                }
            });
            
            console.log('Chart created successfully');
        }
        
        // Generate sample conservation areas
        function generateMPAs() {
            const mpas = [
                { name: 'West Coast Santo MPA', coords: [[-15.5, 166.8], [-15.3, 166.8], [-15.3, 167.1], [-15.5, 167.1]], area: 450 },
                { name: 'Malekula Marine Reserve', coords: [[-16.4, 167.3], [-16.2, 167.3], [-16.2, 167.6], [-16.4, 167.6]], area: 380 },
                { name: 'Efate Marine Sanctuary', coords: [[-17.8, 168.1], [-17.6, 168.1], [-17.6, 168.4], [-17.8, 168.4]], area: 320 },
                { name: 'South Epi MPA', coords: [[-16.8, 168.2], [-16.7, 168.2], [-16.7, 168.5], [-16.8, 168.5]], area: 280 },
                { name: 'Erromango Coastal Zone', coords: [[-18.9, 168.8], [-18.7, 168.8], [-18.7, 169.1], [-18.9, 169.1]], area: 250 },
                { name: 'Torba Marine Area', coords: [[-13.9, 167.3], [-13.7, 167.3], [-13.7, 167.6], [-13.9, 167.6]], area: 170 }
            ];
            
            const features = mpas.map(mpa => 
                L.rectangle(mpa.coords, {
                    color: conservationData.mpa.color,
                    fillColor: conservationData.mpa.color,
                    fillOpacity: 0.4,
                    weight: 2
                }).bindPopup(`
                    <div style="padding: 10px;">
                        <strong style="font-size: 14px; color: ${conservationData.mpa.color};">${mpa.name}</strong><br>
                        <div style="margin-top: 8px; font-size: 12px;">
                            <strong>Type:</strong> Marine Protected Area<br>
                            <strong>Area:</strong> ${mpa.area} km²<br>
                            <strong>Status:</strong> Legally Protected<br>
                            <strong>Year Established:</strong> 2018-2023
                        </div>
                    </div>
                `)
            );
            
            return L.layerGroup(features);
        }
        
        function generateTerrestrialPAs() {
            const pas = [
                { name: 'Mount Tabwemasana Reserve', coords: [[-15.4, 167.1], [-15.3, 167.1], [-15.3, 167.25], [-15.4, 167.25]], area: 85 },
                { name: 'Loru Conservation Area', coords: [[-15.5, 167.15], [-15.45, 167.15], [-15.45, 167.22], [-15.5, 167.22]], area: 62 },
                { name: 'Vatthe Conservation Area', coords: [[-17.75, 168.25], [-17.7, 168.25], [-17.7, 168.32], [-17.75, 168.32]], area: 58 },
                { name: 'Tanna Volcano Buffer', coords: [[-19.52, 169.28], [-19.48, 169.28], [-19.48, 169.35], [-19.52, 169.35]], area: 40 }
            ];
            
            const features = pas.map(pa => 
                L.rectangle(pa.coords, {
                    color: conservationData.terrestrial.color,
                    fillColor: conservationData.terrestrial.color,
                    fillOpacity: 0.5,
                    weight: 2
                }).bindPopup(`
                    <div style="padding: 10px;">
                        <strong style="font-size: 14px; color: ${conservationData.terrestrial.color};">${pa.name}</strong><br>
                        <div style="margin-top: 8px; font-size: 12px;">
                            <strong>Type:</strong> Terrestrial Protected Area<br>
                            <strong>Area:</strong> ${pa.area} km²<br>
                            <strong>Protection Level:</strong> Strict Nature Reserve<br>
                            <strong>Biodiversity:</strong> High
                        </div>
                    </div>
                `)
            );
            
            return L.layerGroup(features);
        }
        
        function generateCCAs() {
            const ccas = [
                { name: 'South Maewo CCA', lat: -15.2, lon: 168.1, area: 18 },
                { name: 'West Ambrym CCA', lat: -16.25, lon: 168.0, area: 22 },
                { name: 'Pentecost Coastal CCA', lat: -15.85, lon: 168.15, area: 15 },
                { name: 'Epi Community Forest', lat: -16.72, lon: 168.38, area: 12 },
                { name: 'North Efate CCA', lat: -17.65, lon: 168.35, area: 14 },
                { name: 'Malekula Forest CCA', lat: -16.35, lon: 167.52, area: 16 },
                { name: 'Santo Coast CCA', lat: -15.45, lon: 167.18, area: 11 },
                { name: 'Tanna Customary Area', lat: -19.48, lon: 169.30, area: 13 },
                { name: 'Erromango CCA', lat: -18.75, lon: 169.0, area: 10 },
                { name: 'Banks Islands CCA', lat: -13.85, lon: 167.52, area: 9 },
                { name: 'Shepherd Islands CCA', lat: -17.0, lon: 168.5, area: 14 },
                { name: 'Paama Island CCA', lat: -16.45, lon: 168.25, area: 12 }
            ];
            
            const features = ccas.map(cca => 
                L.circle([cca.lat, cca.lon], {
                    radius: Math.sqrt(cca.area) * 1500,
                    color: conservationData.cca.color,
                    fillColor: conservationData.cca.color,
                    fillOpacity: 0.4,
                    weight: 2
                }).bindPopup(`
                    <div style="padding: 10px;">
                        <strong style="font-size: 14px; color: ${conservationData.cca.color};">${cca.name}</strong><br>
                        <div style="margin-top: 8px; font-size: 12px;">
                            <strong>Type:</strong> Community Conservation Area<br>
                            <strong>Area:</strong> ${cca.area} km²<br>
                            <strong>Management:</strong> Community-Led<br>
                            <strong>Recognition:</strong> Locally Managed
                        </div>
                    </div>
                `)
            );
            
            return L.layerGroup(features);
        }
        
        function generateKBAs() {
            const islands = [
                { lat: -15.5, lon: 167.2 }, { lat: -16.3, lon: 167.5 }, { lat: -17.7, lon: 168.3 },
                { lat: -18.8, lon: 169.0 }, { lat: -19.5, lon: 169.3 }, { lat: -15.8, lon: 168.2 },
                { lat: -16.2, lon: 168.1 }, { lat: -16.7, lon: 168.4 }, { lat: -15.0, lon: 168.1 },
                { lat: -13.8, lon: 167.5 }, { lat: -17.0, lon: 168.5 }, { lat: -16.45, lon: 168.25 },
                { lat: -14.2, lon: 167.8 }, { lat: -18.2, lon: 169.2 }, { lat: -16.8, lon: 167.8 }
            ];
            
            const features = islands.map((kba, i) => 
                L.circleMarker([kba.lat, kba.lon], {
                    radius: 8,
                    color: '#e74c3c',
                    fillColor: '#e74c3c',
                    fillOpacity: 0.6,
                    weight: 2
                }).bindPopup(`
                    <div style="padding: 10px;">
                        <strong style="font-size: 14px; color: #e74c3c;">KBA Site ${i + 1}</strong><br>
                        <div style="margin-top: 8px; font-size: 12px;">
                            <strong>Type:</strong> Key Biodiversity Area<br>
                            <strong>Priority:</strong> High<br>
                            <strong>Biodiversity Value:</strong> Significant<br>
                            <strong>Threats:</strong> Habitat Loss, Climate Change
                        </div>
                    </div>
                `)
            );
            
            return L.layerGroup(features);
        }
        
        function generateForestCover() {
            const islands = [
                { name: 'Santo', coords: [[-15.6, 167.0], [-15.3, 167.0], [-15.3, 167.4], [-15.6, 167.4]] },
                { name: 'Malekula', coords: [[-16.5, 167.3], [-16.2, 167.3], [-16.2, 167.7], [-16.5, 167.7]] },
                { name: 'Efate', coords: [[-17.8, 168.2], [-17.6, 168.2], [-17.6, 168.4], [-17.8, 168.4]] },
                { name: 'Erromango', coords: [[-18.9, 168.9], [-18.7, 168.9], [-18.7, 169.1], [-18.9, 169.1]] },
                { name: 'Pentecost', coords: [[-16.0, 168.1], [-15.6, 168.1], [-15.6, 168.3], [-16.0, 168.3]] }
            ];
            
            const features = islands.map(island => 
                L.rectangle(island.coords, {
                    color: '#228B22',
                    fillColor: '#228B22',
                    fillOpacity: 0.3,
                    weight: 1
                }).bindPopup(`
                    <div style="padding: 10px;">
                        <strong style="font-size: 14px;">${island.name} Forest Cover</strong><br>
                        <div style="margin-top: 8px; font-size: 12px;">
                            <strong>Type:</strong> Dense & Open Forest<br>
                            <strong>Condition:</strong> Mixed<br>
                            <strong>Carbon Storage:</strong> Significant
                        </div>
                    </div>
                `)
            );
            
            return L.layerGroup(features);
        }
        
        function generateMangroves() {
            const sites = [
                { lat: -15.5, lon: 167.0 }, { lat: -16.3, lon: 167.4 }, { lat: -17.7, lon: 168.2 },
                { lat: -18.8, lon: 168.9 }, { lat: -16.2, lon: 168.0 }, { lat: -16.7, lon: 168.3 }
            ];
            
            const features = sites.map((site, i) => 
                L.circle([site.lat, site.lon], {
                    radius: 1500,
                    color: '#00CED1',
                    fillColor: '#00CED1',
                    fillOpacity: 0.5,
                    weight: 2
                }).bindPopup(`
                    <div style="padding: 10px;">
                        <strong style="font-size: 14px;">Mangrove Site ${i + 1}</strong><br>
                        <div style="margin-top: 8px; font-size: 12px;">
                            <strong>Type:</strong> Coastal Mangrove<br>
                            <strong>Ecosystem Services:</strong> High<br>
                            <strong>Status:</strong> Monitoring Required
                        </div>
                    </div>
                `)
            );
            
            return L.layerGroup(features);
        }
        
        function toggleLayer(layerName) {
            const checkbox = document.getElementById(`check-${layerName}`);
            const layer = layers[layerName];
            
            if (checkbox.checked && layer) {
                layer.addTo(map);
            } else if (layer) {
                map.removeLayer(layer);
            }
        }
        
        // File upload functions
        function showAlert(message, type) {
            const alert = document.getElementById('upload-alert');
            alert.textContent = message;
            alert.className = `alert alert-${type}`;
            alert.style.display = 'block';
            setTimeout(() => alert.style.display = 'none', 5000);
        }
        
        // AI-powered layer detection
        function detectLayerType(fileName, properties, geometry) {
            const name = fileName.toLowerCase();
            const props = properties ? Object.keys(properties).map(k => k.toLowerCase()).join(' ') : '';
            const allText = (name + ' ' + props).toLowerCase();
            
            // Marine Protected Area detection
            const mpaKeywords = ['marine', 'mpa', 'ocean', 'sea', 'reef', 'coral', 'coastal', 'bay', 'lagoon', 'sanctuary', 'reserve'];
            if (mpaKeywords.some(keyword => allText.includes(keyword))) {
                return { type: 'mpa', confidence: 'high', reason: 'Marine-related keywords detected' };
            }
            
            // Terrestrial Protected Area detection
            const terrestrialKeywords = ['terrestrial', 'park', 'reserve', 'protected', 'national', 'conservation area', 'wildlife', 'nature', 'forest reserve', 'sanctuary'];
            if (terrestrialKeywords.some(keyword => allText.includes(keyword)) && !allText.includes('community')) {
                return { type: 'terrestrial', confidence: 'high', reason: 'Terrestrial protected area keywords detected' };
            }
            
            // Community Conservation Area detection
            const ccaKeywords = ['community', 'cca', 'locally managed', 'customary', 'indigenous', 'village', 'tabu'];
            if (ccaKeywords.some(keyword => allText.includes(keyword))) {
                return { type: 'cca', confidence: 'high', reason: 'Community conservation keywords detected' };
            }
            
            // Key Biodiversity Area detection
            const kbaKeywords = ['kba', 'biodiversity', 'hotspot', 'priority', 'critical', 'important bird'];
            if (kbaKeywords.some(keyword => allText.includes(keyword))) {
                return { type: 'kba', confidence: 'high', reason: 'Biodiversity priority keywords detected' };
            }
            
            // Proposed area detection
            const proposedKeywords = ['proposed', 'candidate', 'potential', 'planned', 'future', 'target'];
            if (proposedKeywords.some(keyword => allText.includes(keyword))) {
                return { type: 'proposed', confidence: 'medium', reason: 'Proposed area keywords detected' };
            }
            
            // Geometry-based detection
            if (geometry) {
                const geomType = geometry.type;
                if (geomType === 'Point' || geomType === 'MultiPoint') {
                    return { type: 'kba', confidence: 'low', reason: 'Point geometry suggests biodiversity site' };
                }
            }
            
            // Property-based detection
            if (properties) {
                // Check for area/size properties
                if (properties.area || properties.Area || properties.AREA || properties.hectares) {
                    const areaVal = properties.area || properties.Area || properties.AREA || properties.hectares || 0;
                    if (areaVal > 100) {
                        return { type: 'terrestrial', confidence: 'medium', reason: 'Large area suggests protected area' };
                    }
                }
                
                // Check for status properties
                if (properties.status || properties.Status || properties.STATUS) {
                    const status = (properties.status || properties.Status || properties.STATUS || '').toLowerCase();
                    if (status.includes('protected') || status.includes('gazetted')) {
                        return { type: 'terrestrial', confidence: 'medium', reason: 'Protected status detected' };
                    }
                }
            }
            
            return { type: 'other', confidence: 'low', reason: 'Unable to determine specific category' };
        }
        
        function calculateGeometryArea(layer) {
            try {
                let totalArea = 0;
                
                layer.eachLayer(function(subLayer) {
                    if (subLayer.getLatLngs) {
                        const latlngs = subLayer.getLatLngs();
                        const coords = Array.isArray(latlngs[0]) ? latlngs[0] : latlngs;
                        totalArea += L.GeometryUtil.geodesicArea(coords) / 1000000; // Convert to km²
                    }
                });
                
                return totalArea;
            } catch (error) {
                console.error('Error calculating area:', error);
                return 0;
            }
        }
        
        function getCategoryColor(category) {
            const colors = {
                'mpa': conservationData.mpa.color,
                'terrestrial': conservationData.terrestrial.color,
                'cca': conservationData.cca.color,
                'kba': '#e74c3c',
                'proposed': '#f39c12',
                'forest': '#228B22',
                'mangrove': '#00CED1',
                'other': '#95a5a6'
            };
            return colors[category] || '#3388ff';
        }
        
        function getCategoryName(category) {
            const names = {
                'mpa': 'Marine Protected Area',
                'terrestrial': 'Terrestrial Protected Area',
                'cca': 'Community Conservation Area',
                'kba': 'Key Biodiversity Area',
                'proposed': 'Proposed Protected Area',
                'forest': 'Forest Cover',
                'mangrove': 'Mangrove Area',
                'other': 'Other Conservation Feature'
            };
            return names[category] || 'Unknown';
        }
        
        function updateCategoryDisplay() {
            const category = document.getElementById('upload-category').value;
            const categoryName = getCategoryName(category);
            const categoryColor = getCategoryColor(category);
            
            document.getElementById('category-display').textContent = categoryName;
            document.getElementById('category-display').style.color = categoryColor;
        }
        
        async function processFile(file) {
            return new Promise(async (resolve, reject) => {
                try {
                    console.log('Processing file:', file.name, 'Type:', file.type, 'Size:', file.size);
                    document.getElementById('loading').style.display = 'block';
                    showAlert('🔍 Processing and analyzing file...', 'info');
                    
                    let geojson;
                    const fileName = file.name.toLowerCase();
                    
                    // Check if it's a zip file (could be shapefile bundle)
                    if (fileName.endsWith('.zip')) {
                        console.log('Detected ZIP file - checking if it contains shapefile');
                        try {
                            const arrayBuffer = await file.arrayBuffer();
                            console.log('ArrayBuffer created, size:', arrayBuffer.byteLength);
                            
                            // Try to parse as shapefile
                            geojson = await shp(arrayBuffer);
                            console.log('ZIP parsed as shapefile successfully:', geojson);
                        } catch (zipError) {
                            console.error('ZIP parsing error:', zipError);
                            document.getElementById('loading').style.display = 'none';
                            showAlert('❌ Error: ZIP file must contain shapefile components (.shp, .shx, .dbf)', 'info');
                            reject(zipError);
                            return;
                        }
                    } else if (fileName.endsWith('.shp')) {
                        console.log('Detected standalone .shp file');
                        showAlert('⚠️ Please upload the complete shapefile as a ZIP (including .shp, .shx, .dbf files)', 'info');
                        document.getElementById('loading').style.display = 'none';
                        reject(new Error('Standalone .shp not supported - use ZIP'));
                        return;
                    } else if (fileName.endsWith('.geojson') || fileName.endsWith('.json')) {
                        console.log('Detected GeoJSON format');
                        const text = await file.text();
                        geojson = JSON.parse(text);
                        console.log('GeoJSON parsed:', geojson);
                    } else if (fileName.endsWith('.kml')) {
                        showAlert('⚠️ KML files need conversion. Please use .geojson or shapefile .zip format', 'info');
                        document.getElementById('loading').style.display = 'none';
                        reject(new Error('KML not supported'));
                        return;
                    } else {
                        showAlert('❌ Unsupported format. Use .zip (shapefile bundle) or .geojson', 'info');
                        document.getElementById('loading').style.display = 'none';
                        reject(new Error('Unsupported format'));
                        return;
                    }
                    
                    if (!geojson) {
                        throw new Error('Failed to parse file - no data returned');
                    }
                    
                    const features = Array.isArray(geojson) ? geojson : [geojson];
                    console.log('Processing', features.length, 'feature(s)');
                    
                    let processedCount = 0;
                    
                    features.forEach(feature => {
                        layerCounter++;
                        const layerId = layerCounter;
                        
                        console.log('Processing feature', layerId);
                        
                        // Detect layer type using AI logic
                        const firstFeature = feature.features ? feature.features[0] : feature;
                        const detection = detectLayerType(
                            file.name,
                            firstFeature.properties,
                            firstFeature.geometry
                        );
                        
                        console.log('Detection result:', detection);
                        
                        const categoryColor = getCategoryColor(detection.type);
                        const categoryName = getCategoryName(detection.type);
                        
                        console.log('Creating layer with color:', categoryColor);
                        
                        // Create layer with detected category color
                        const layer = L.geoJSON(feature, {
                            style: {
                                fillColor: categoryColor,
                                fillOpacity: 0.5,
                                color: categoryColor,
                                weight: 2.5
                            },
                            pointToLayer: function(feature, latlng) {
                                return L.circleMarker(latlng, {
                                    radius: 8,
                                    fillColor: categoryColor,
                                    color: categoryColor,
                                    weight: 2,
                                    opacity: 0.8,
                                    fillOpacity: 0.6
                                });
                            },
                            onEachFeature: (feature, layer) => {
                                if (feature.properties) {
                                    let popup = `<div style="padding: 10px;">
                                        <strong style="font-size: 14px; color: ${categoryColor};">${categoryName}</strong><br>
                                        <div style="margin-top: 8px; padding-top: 8px; border-top: 2px solid ${categoryColor}; font-size: 12px;">
                                        <div style="background: #f0f0f0; padding: 6px; border-radius: 3px; margin-bottom: 8px;">
                                            <strong>🤖 Auto-detected:</strong> ${detection.reason}<br>
                                            <strong>Confidence:</strong> ${detection.confidence.toUpperCase()}
                                        </div>`;
                                    
                                    for (let key in feature.properties) {
                                        if (feature.properties[key]) {
                                            popup += `<strong>${key}:</strong> ${feature.properties[key]}<br>`;
                                        }
                                    }
                                    popup += '</div></div>';
                                    layer.bindPopup(popup);
                                }
                            }
                        });
                        
                        // Add to map FIRST before any other operations
                        console.log('Adding layer to map...');
                        layer.addTo(map);
                        console.log('Layer added to map successfully');
                        
                        // Force map to update
                        map.invalidateSize();
                        
                        // Calculate area
                        const calculatedArea = calculateGeometryArea(layer);
                        console.log('Calculated area:', calculatedArea, 'km²');
                        
                        // Update dynamic categories
                        if (!dynamicCategories[detection.type]) {
                            dynamicCategories[detection.type] = { area: 0, count: 0, layers: [] };
                        }
                        dynamicCategories[detection.type].area += calculatedArea;
                        dynamicCategories[detection.type].count += 1;
                        dynamicCategories[detection.type].layers.push(layerId);
                        
                        // Store layer info
                        const layerObj = {
                            id: layerId,
                            layer: layer,
                            name: file.name,
                            category: detection.type,
                            categoryName: categoryName,
                            detection: detection,
                            area: calculatedArea,
                            color: categoryColor,
                            geojson: feature
                        };
                        
                        uploadedLayers.push(layerObj);
                        console.log('Layer stored, total uploaded layers:', uploadedLayers.length);
                        
                        // Add to category UI
                        addLayerToCategory(layerObj);
                        
                        // Zoom to layer
                        try {
                            if (layer.getBounds && layer.getBounds().isValid()) {
                                map.fitBounds(layer.getBounds(), { padding: [50, 50] });
                                console.log('Zoomed to layer bounds');
                            }
                        } catch (e) {
                            console.warn('Could not zoom to layer:', e);
                        }
                        
                        processedCount++;
                    });
                    
                    console.log('Processed', processedCount, 'feature(s)');
                    
                    // Update statistics and dashboard
                    console.log('Updating statistics...');
                    updateConservationData();
                    
                    console.log('Updating dashboard display...');
                    updateDashboard();
                    
                    console.log('Updating chart...');
                    createChart();
                    
                    console.log('All updates complete');
                    
                    document.getElementById('loading').style.display = 'none';
                    showAlert(`✅ Successfully loaded and categorized: ${file.name} (${processedCount} feature(s))`, 'success');
                    
                    resolve();
                    
                } catch (error) {
                    document.getElementById('loading').style.display = 'none';
                    showAlert(`❌ Error: ${error.message}`, 'info');
                    console.error('File processing error:', error);
                    console.error('Error stack:', error.stack);
                    reject(error);
                }
            });
        }
        
        function updateConservationData() {
            // Update conservation data with uploaded layers
            if (dynamicCategories.mpa.area > 0) {
                conservationData.mpa.area += dynamicCategories.mpa.area;
                conservationData.mpa.count += dynamicCategories.mpa.count;
            }
            if (dynamicCategories.terrestrial.area > 0) {
                conservationData.terrestrial.area += dynamicCategories.terrestrial.area;
                conservationData.terrestrial.count += dynamicCategories.terrestrial.count;
            }
            if (dynamicCategories.cca.area > 0) {
                conservationData.cca.area += dynamicCategories.cca.area;
                conservationData.cca.count += dynamicCategories.cca.count;
            }
        }
        
        function addLayerToCategory(layerObj) {
            const categoryContainer = document.getElementById(`category-${layerObj.category}`);
            if (categoryContainer) {
                categoryContainer.style.display = 'block';
                const filesContainer = categoryContainer.querySelector('.uploaded-files');
                
                const fileItem = document.createElement('div');
                fileItem.className = 'file-item';
                fileItem.id = `file-${layerObj.id}`;
                fileItem.innerHTML = `
                    <div class="file-info">
                        <div style="display: flex; align-items: center; gap: 10px;">
                            <div class="layer-color" style="width: 30px; height: 30px; background: ${layerObj.color};"></div>
                            <div>
                                <div style="font-weight: 700; color: ${layerObj.color}; font-size: 13px;">${layerObj.name}</div>
                                <div style="font-size: 11px; color: #6c757d; margin-top: 2px;">
                                    <strong>Type:</strong> ${layerObj.categoryName}<br>
                                    <strong>Area:</strong> ${layerObj.area.toFixed(2)} km² | 
                                    <strong>Confidence:</strong> ${layerObj.detection.confidence}
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="file-actions">
                        <button class="btn-icon" onclick="event.preventDefault(); event.stopPropagation(); recategorizeLayer(${layerObj.id})" title="Change category">🔄</button>
                        <button class="btn-icon" onclick="event.preventDefault(); event.stopPropagation(); zoomToUploadedLayer(${layerObj.id})" title="Zoom to layer">🔍</button>
                        <button class="btn-icon" onclick="event.preventDefault(); event.stopPropagation(); toggleUploadedLayer(${layerObj.id})" title="Toggle visibility">👁️</button>
                        <button class="btn-icon" onclick="event.preventDefault(); event.stopPropagation(); removeUploadedLayer(${layerObj.id})" title="Remove">❌</button>
                    </div>
                `;
                filesContainer.appendChild(fileItem);
            }
        }
        
        window.recategorizeLayer = function(layerId) {
            const layerObj = uploadedLayers.find(l => l.id === layerId);
            if (!layerObj) return;
            
            const newCategory = prompt(
                `Current category: ${layerObj.categoryName}\n\nChange to:\n` +
                `1 - Marine Protected Area\n` +
                `2 - Terrestrial Protected Area\n` +
                `3 - Community Conservation Area\n` +
                `4 - Key Biodiversity Area\n` +
                `5 - Proposed Protected Area\n` +
                `6 - Forest Cover\n` +
                `7 - Mangrove Areas\n` +
                `8 - Other\n\n` +
                `Enter number (1-8):`,
                '1'
            );
            
            const categoryMap = {
                '1': 'mpa',
                '2': 'terrestrial',
                '3': 'cca',
                '4': 'kba',
                '5': 'proposed',
                '6': 'forest',
                '7': 'mangrove',
                '8': 'other'
            };
            
            const newType = categoryMap[newCategory];
            if (!newType) return;
            
            // Update category
            const oldType = layerObj.category;
            dynamicCategories[oldType].area -= layerObj.area;
            dynamicCategories[oldType].count -= 1;
            
            dynamicCategories[newType].area += layerObj.area;
            dynamicCategories[newType].count += 1;
            
            layerObj.category = newType;
            layerObj.categoryName = getCategoryName(newType);
            layerObj.color = getCategoryColor(newType);
            
            // Update layer style
            layerObj.layer.setStyle({
                fillColor: layerObj.color,
                color: layerObj.color
            });
            
            // Remove from old category UI
            const fileItem = document.getElementById(`file-${layerId}`);
            if (fileItem) fileItem.remove();
            
            // Add to new category UI
            addLayerToCategory(layerObj);
            
            updateConservationData();
            updateDashboard();
            createChart();
            
            showAlert(`✅ Recategorized to: ${layerObj.categoryName}`, 'success');
        };
        
        window.toggleUploadedLayer = function(layerId) {
            const layerObj = uploadedLayers.find(l => l.id === layerId);
            if (layerObj) {
                if (map.hasLayer(layerObj.layer)) {
                    map.removeLayer(layerObj.layer);
                } else {
                    layerObj.layer.addTo(map);
                }
            }
        };
        
        window.zoomToUploadedLayer = function(id) {
            const layerObj = uploadedLayers.find(l => l.id === id);
            if (layerObj && layerObj.layer.getBounds().isValid()) {
                map.fitBounds(layerObj.layer.getBounds(), { padding: [50, 50] });
            }
        };
        
        window.removeUploadedLayer = function(id) {
            const layerObj = uploadedLayers.find(l => l.id === id);
            if (layerObj) {
                // Remove from map
                map.removeLayer(layerObj.layer);
                
                // Update dynamic categories
                if (dynamicCategories[layerObj.category]) {
                    dynamicCategories[layerObj.category].area -= layerObj.area;
                    dynamicCategories[layerObj.category].count -= 1;
                }
                
                // Remove from array
                uploadedLayers = uploadedLayers.filter(l => l.id !== id);
                
                // Remove from UI
                const fileItem = document.getElementById(`file-${id}`);
                if (fileItem) fileItem.remove();
                
                // Hide category container if empty
                const category = layerObj.category;
                const categoryContainer = document.getElementById(`category-${category}`);
                if (categoryContainer) {
                    const filesContainer = categoryContainer.querySelector('.uploaded-files');
                    if (filesContainer && filesContainer.children.length === 0) {
                        categoryContainer.style.display = 'none';
                    }
                }
                
                // Update dashboard
                updateConservationData();
                updateDashboard();
                createChart();
                
                showAlert('Layer removed', 'info');
            }
        };
        
        function startMeasurement() {
            if (!drawnItems) {
                drawnItems = new L.FeatureGroup();
                map.addLayer(drawnItems);
                
                drawControl = new L.Control.Draw({
                    draw: {
                        polygon: true,
                        polyline: false,
                        rectangle: true,
                        circle: false,
                        marker: false,
                        circlemarker: false
                    },
                    edit: {
                        featureGroup: drawnItems
                    }
                });
                map.addControl(drawControl);
                
                map.on('draw:created', function(e) {
                    const layer = e.layer;
                    drawnItems.addLayer(layer);
                    
                    const area = L.GeometryUtil.geodesicArea(layer.getLatLngs()[0]) / 1000000;
                    document.getElementById('measurement-result').style.display = 'block';
                    document.getElementById('measurement-result').innerHTML = `
                        <strong>Measured Area:</strong> ${area.toFixed(2)} km²<br>
                        <strong>Percentage of Total:</strong> ${(area / conservationData.totalLandSeaArea * 100).toFixed(2)}%
                    `;
                });
            }
            
            showAlert('Draw a polygon on the map to calculate its area.', 'info');
        }
        
        function generateReport() {
            const progress = calculateProgress();
            
            // Create report content
            const reportContent = `VANUATU NBSAP TARGET 3 - PROTECTED AREA PROGRESS REPORT
Date: ${new Date().toLocaleDateString()}

========================================
EXECUTIVE SUMMARY
========================================

Current Protected Area Coverage: ${progress.percentage}%
Target for 2030: 30%
Gap to Target: ${progress.gap}% (${progress.gapArea} km²)
Years Remaining: ${document.getElementById('years-left').textContent}

========================================
COVERAGE BREAKDOWN
========================================

Marine Protected Areas:
  - Area: ${conservationData.mpa.area.toFixed(2)} km²
  - Number of Sites: ${conservationData.mpa.count}
  - Percentage: ${(conservationData.mpa.area/conservationData.totalLandSeaArea*100).toFixed(2)}%

Terrestrial Protected Areas:
  - Area: ${conservationData.terrestrial.area.toFixed(2)} km²
  - Number of Sites: ${conservationData.terrestrial.count}
  - Percentage: ${(conservationData.terrestrial.area/conservationData.totalLandSeaArea*100).toFixed(2)}%

Community Conservation Areas:
  - Area: ${conservationData.cca.area.toFixed(2)} km²
  - Number of Sites: ${conservationData.cca.count}
  - Percentage: ${(conservationData.cca.area/conservationData.totalLandSeaArea*100).toFixed(2)}%

Total Protected: ${progress.totalProtected.toFixed(2)} km²
Total Land & Sea Area: ${conservationData.totalLandSeaArea} km²

========================================
UPLOADED LAYERS
========================================
${uploadedLayers.length > 0 ? uploadedLayers.map(l => 
`- ${l.name}
  Category: ${l.categoryName}
  Area: ${l.area.toFixed(2)} km²
  Detection Confidence: ${l.detection.confidence}
`).join('\n') : 'No custom layers uploaded'}

========================================
RECOMMENDATIONS
========================================

1. Additional Protection Needed: ${progress.gapArea} km² to reach 30% target
2. Focus Areas: Marine ecosystems, Key Biodiversity Areas
3. Community Engagement: Expand Community Conservation Areas
4. Timeline: ${document.getElementById('years-left').textContent} years to achieve target

Generated by: Vanuatu NBSAP Target 3 Monitoring Platform
Department of Environmental Protection and Conservation (DEPC)`;

            // Download as text file
            const blob = new Blob([reportContent], { type: 'text/plain' });
            const url = URL.createObjectURL(blob);
            const a = document.createElement('a');
            a.href = url;
            a.download = `NBSAP_Target3_Report_${new Date().toISOString().split('T')[0]}.txt`;
            document.body.appendChild(a);
            a.click();
            document.body.removeChild(a);
            URL.revokeObjectURL(url);
            
            showAlert('📄 Report generated and downloaded!', 'success');
        }
        
        function exportData() {
            const allFeatures = {
                type: 'FeatureCollection',
                features: [],
                metadata: {
                    title: 'Vanuatu NBSAP Target 3 - Protected Areas',
                    date: new Date().toISOString(),
                    total_area_km2: calculateProgress().totalProtected,
                    coverage_percentage: calculateProgress().percentage,
                    target_percentage: 30
                }
            };
            
            // Add all uploaded layers
            uploadedLayers.forEach(layerObj => {
                if (layerObj.geojson) {
                    const features = layerObj.geojson.features || [layerObj.geojson];
                    features.forEach(feature => {
                        // Enhance properties with category info
                        const enrichedFeature = {
                            ...feature,
                            properties: {
                                ...feature.properties,
                                nbsap_category: layerObj.categoryName,
                                nbsap_category_code: layerObj.category,
                                calculated_area_km2: layerObj.area,
                                source_file: layerObj.name,
                                detection_confidence: layerObj.detection.confidence
                            }
                        };
                        allFeatures.features.push(enrichedFeature);
                    });
                }
            });
            
            if (allFeatures.features.length === 0) {
                showAlert('⚠️ No uploaded layers to export. Upload some GIS data first.', 'info');
                return;
            }
            
            // Download as GeoJSON
            const geojsonStr = JSON.stringify(allFeatures, null, 2);
            const blob = new Blob([geojsonStr], { type: 'application/json' });
            const url = URL.createObjectURL(blob);
            const a = document.createElement('a');
            a.href = url;
            a.download = `NBSAP_Target3_AllLayers_${new Date().toISOString().split('T')[0]}.geojson`;
            document.body.appendChild(a);
            a.click();
            document.body.removeChild(a);
            URL.revokeObjectURL(url);
            
            showAlert(`✅ Exported ${allFeatures.features.length} features as GeoJSON!`, 'success');
        }
        
        function exportSummary() {
            const progress = calculateProgress();
            
            // Build CSV with headers
            let csv = 'Category,Area_km2,Number_of_Sites,Percentage_of_Total,Status\n';
            
            // Add baseline data
            csv += `Marine Protected Areas,${conservationData.mpa.area.toFixed(2)},${conservationData.mpa.count},${(conservationData.mpa.area/conservationData.totalLandSeaArea*100).toFixed(2)},Baseline\n`;
            csv += `Terrestrial Protected Areas,${conservationData.terrestrial.area.toFixed(2)},${conservationData.terrestrial.count},${(conservationData.terrestrial.area/conservationData.totalLandSeaArea*100).toFixed(2)},Baseline\n`;
            csv += `Community Conservation Areas,${conservationData.cca.area.toFixed(2)},${conservationData.cca.count},${(conservationData.cca.area/conservationData.totalLandSeaArea*100).toFixed(2)},Baseline\n`;
            
            // Add uploaded layers summary by category
            Object.keys(dynamicCategories).forEach(catKey => {
                const cat = dynamicCategories[catKey];
                if (cat.count > 0) {
                    const catName = getCategoryName(catKey);
                    csv += `${catName},${cat.area.toFixed(2)},${cat.count},${(cat.area/conservationData.totalLandSeaArea*100).toFixed(2)},Uploaded\n`;
                }
            });
            
            // Add totals
            csv += `\nTotal Protected,${progress.totalProtected.toFixed(2)},,${progress.percentage},\n`;
            csv += `Gap to 30% Target,${progress.gapArea.toFixed(2)},,${progress.gap},\n`;
            csv += `Total Area (Land & Sea),${conservationData.totalLandSeaArea},,100,\n`;
            
            // Add metadata
            csv += `\nReport Generated,${new Date().toLocaleString()},,,\n`;
            csv += `Years to Target,${document.getElementById('years-left').textContent},,,\n`;
            
            // Download CSV
            const blob = new Blob([csv], { type: 'text/csv' });
            const url = URL.createObjectURL(blob);
            const a = document.createElement('a');
            a.href = url;
            a.download = `NBSAP_Target3_Summary_${new Date().toISOString().split('T')[0]}.csv`;
            document.body.appendChild(a);
            a.click();
            document.body.removeChild(a);
            URL.revokeObjectURL(url);
            
            showAlert('📊 Summary statistics exported as CSV!', 'success');
        }
        
        // Initialize map
        map = L.map('map').setView([-17.7333, 168.3273], 7);
        
        const satellite = L.tileLayer('https://server.arcgisonline.com/ArcGIS/rest/services/World_Imagery/MapServer/tile/{z}/{y}/{x}', {
            attribution: 'Esri',
            maxZoom: 19
        }).addTo(map);
        
        const osm = L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
            attribution: '© OpenStreetMap',
            maxZoom: 19
        });
        
        L.control.layers({ 'Satellite': satellite, 'Street Map': osm }).addTo(map);
        L.control.scale({ imperial: false, metric: true }).addTo(map);
        
        // Generate and add layers
        layers.mpa = generateMPAs().addTo(map);
        layers.terrestrial = generateTerrestrialPAs().addTo(map);
        layers.cca = generateCCAs().addTo(map);
        layers.kba = generateKBAs();
        layers.forest = generateForestCover();
        layers.mangrove = generateMangroves();
        
        // File upload - Initialize immediately
        (function initializeUpload() {
            const uploadZone = document.getElementById('upload-zone');
            const fileInput = document.getElementById('file-input');
            const uploadCategory = document.getElementById('upload-category');
            
            if (!uploadZone || !fileInput || !uploadCategory) {
                console.error('Upload elements not found!');
                return;
            }
            
            console.log('Upload elements found, initializing...');
            console.log('Upload zone:', uploadZone);
            console.log('File input:', fileInput);
            
            // Category change
            uploadCategory.addEventListener('change', function(e) {
                console.log('Category changed to:', e.target.value);
                updateCategoryDisplay();
            });
            
            // Click to upload
            uploadZone.addEventListener('click', function(e) {
                e.preventDefault();
                e.stopPropagation();
                console.log('Upload zone clicked - triggering file input');
                try {
                    fileInput.click();
                } catch (error) {
                    console.error('Error clicking file input:', error);
                }
                return false;
            }, true);
            
            // File selected
            fileInput.addEventListener('change', function(e) {
                // DO NOT call preventDefault on file input change - it can cause issues
                e.stopPropagation();
                console.log('File input change event fired');
                const files = e.target.files;
                console.log('Files object:', files);
                console.log('Number of files:', files.length);
                
                if (files && files.length > 0) {
                    // Process files asynchronously to prevent blocking
                    setTimeout(() => {
                        for (let i = 0; i < files.length; i++) {
                            const file = files[i];
                            console.log(`File ${i + 1}:`, file.name, 'Size:', file.size, 'Type:', file.type);
                            processFile(file);
                        }
                    }, 0);
                    
                    // Reset after a delay
                    setTimeout(() => {
                        fileInput.value = '';
                        console.log('File input reset');
                    }, 2000);
                } else {
                    console.warn('No files selected');
                }
                
                return false;
            }, false);
            
            // Drag and drop
            uploadZone.addEventListener('dragover', function(e) {
                e.preventDefault();
                e.stopPropagation();
                uploadZone.style.borderColor = '#00a86b';
                uploadZone.style.background = '#e7f9f0';
            }, true);
            
            uploadZone.addEventListener('dragleave', function(e) {
                e.preventDefault();
                e.stopPropagation();
                uploadZone.style.borderColor = '#dee2e6';
                uploadZone.style.background = '#f8f9fa';
            }, true);
            
            uploadZone.addEventListener('drop', function(e) {
                e.preventDefault();
                e.stopPropagation();
                console.log('Drop event fired');
                uploadZone.style.borderColor = '#dee2e6';
                uploadZone.style.background = '#f8f9fa';
                
                const files = e.dataTransfer.files;
                console.log('Dropped files:', files.length);
                
                if (files && files.length > 0) {
                    // Process files asynchronously to prevent blocking
                    setTimeout(() => {
                        for (let i = 0; i < files.length; i++) {
                            const file = files[i];
                            console.log(`Dropped file ${i + 1}:`, file.name);
                            processFile(file);
                        }
                    }, 0);
                } else {
                    console.warn('No files dropped');
                }
                
                return false;
            }, true);
            
            console.log('✅ Upload handlers initialized successfully');
            
            // Test click handler
            setTimeout(() => {
                console.log('Upload zone is clickable:', uploadZone.style.cursor);
            }, 1000);
        })();
        
        // Initialize dashboard
        updateDashboard();
        createChart();
        updateCategoryDisplay();
        
        // Add button event listeners
        document.getElementById('btn-measure').addEventListener('click', function(e) {
            e.preventDefault();
            startMeasurement();
        });
        
        document.getElementById('btn-report').addEventListener('click', function(e) {
            e.preventDefault();
            generateReport();
        });
        
        document.getElementById('btn-export-geojson').addEventListener('click', function(e) {
            e.preventDefault();
            exportData();
        });
        
        document.getElementById('btn-export-csv').addEventListener('click', function(e) {
            e.preventDefault();
            exportSummary();
        });
        
        // Add layer toggle event listeners
        document.getElementById('check-mpa').addEventListener('change', function(e) {
            toggleLayer('mpa');
        });
        
        document.getElementById('check-terrestrial').addEventListener('change', function(e) {
            toggleLayer('terrestrial');
        });
        
        document.getElementById('check-cca').addEventListener('change', function(e) {
            toggleLayer('cca');
        });
        
        document.getElementById('check-kba').addEventListener('change', function(e) {
            toggleLayer('kba');
        });
        
        document.getElementById('check-forest').addEventListener('change', function(e) {
            toggleLayer('forest');
        });
        
        document.getElementById('check-mangrove').addEventListener('change', function(e) {
            toggleLayer('mangrove');
        });
        
        // Add Leaflet.GeometryUtil for area calculation
        L.GeometryUtil = L.extend(L.GeometryUtil || {}, {
            geodesicArea: function(latLngs) {
                let area = 0;
                const len = latLngs.length;
                if (len > 2) {
                    for (let i = 0; i < len; i++) {
                        const j = (i + 1) % len;
                        area += latLngs[i].lng * latLngs[j].lat - latLngs[j].lng * latLngs[i].lat; 
                    }
                    area = Math.abs(area * 6378137 * 6378137 * Math.PI / 360 / 2);
                }
                return area;
            }
        });
    </script>
</body>
</html> 
