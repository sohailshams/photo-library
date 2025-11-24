<template>
    <h1>POC Photo Library</h1>

    <lightgallery :settings="{ speed: 500, plugins: plugins }" :onInit="onInit" :onBeforeSlide="onBeforeSlide">
        <a data-lg-size="1400-1400" class="gallery-item"
            data-src="https://images.unsplash.com/photo-1581894158358-5ecd2c518883?ixid=MXwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHw%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=1406&q=80"
            data-sub-html="<h4>Photo by - <a href='https://unsplash.com/@entrycube' >Diego Guzmán </a></h4> <p> Location - <a href='https://unsplash.com/s/photos/fushimi-inari-taisha-shrine-senbontorii%2C-68%E7%95%AA%E5%9C%B0-fukakusa-yabunouchicho%2C-fushimi-ward%2C-kyoto%2C-japan'>Fushimi Ward, Kyoto, Japan</a></p>">
            <img class="img-responsive"
                src="https://images.unsplash.com/photo-1581894158358-5ecd2c518883?ixid=MXwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHw%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=240&q=80" />
        </a>
        <a data-lg-size="1400-1400" class="gallery-item"
            data-src="https://images.unsplash.com/photo-1544550285-f813152fb2fd?ixid=MXwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHw%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=1400&q=80"
            data-sub-html="<h4>Photo by - <a href='https://unsplash.com/@asoshiation' >Shah </a></h4><p> Location - <a href='https://unsplash.com/s/photos/shinimamiya%2C-osaka%2C-japan'>Shinimamiya, Osaka, Japan</a></p>">
            <img class="img-responsive"
                src="https://images.unsplash.com/photo-1544550285-f813152fb2fd?ixid=MXwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHw%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=240&q=80" />
        </a>
        <a data-lg-size="1400-1400" class="gallery-item"
            data-src="https://images.unsplash.com/photo-1584592740039-cddf0671f3d4?ixid=MXwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHw%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=1400&q=80"
            data-sub-html="<h4>Photo by - <a href='https://unsplash.com/@katherine_xx11' >Katherine Gu </a></h4><p> For all those years we were alone and helpless.</p>">
            <img style="width: 200px" class="img-responsive"
                src="https://images.unsplash.com/photo-1584592740039-cddf0671f3d4?ixid=MXwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHw%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=240&q=80" />
        </a>
        <a data-lg-size="1400-1400" class="gallery-item"
            data-video='{"source": [{"src":"https://www.lightgalleryjs.com/videos/video1.mp4", "type":"video/mp4"}], "attributes": {"preload": false, "controls": true}}'
            data-poster=""
            data-sub-html="<h4>Photo by - <a href='https://unsplash.com/@katherine_xx11' >Katherine Gu </a></h4><p> For all those years we were alone and helpless.</p>">
            <img width="200" class="img-responsive"
                src="https://www.lightgalleryjs.com/images/demo/html5-video-poster.jpg" />
        </a>
        <a data-lg-size="1400-1400" class="gallery-item"
            data-src="https://images.unsplash.com/photo-1501785888041-af3ef285b470?auto=format&fit=crop&w=1400&q=80"
            data-sub-html="<h4>Photo by - <a href='https://unsplash.com/@d3signs'>Diego Guzmán</a></h4><p> Location - <a href='https://unsplash.com/photos/photo-1501785888041-af3ef285b470'>Landscape</a></p>">
            <img class="img-responsive"
                src="https://images.unsplash.com/photo-1501785888041-af3ef285b470?auto=format&fit=crop&w=240&q=80" />
        </a>

        <a data-lg-size="1400-1400" class="gallery-item"
            data-src="https://images.unsplash.com/photo-1500530855697-b586d89ba3ee?auto=format&fit=crop&w=1400&q=80"
            data-sub-html="<h4>Photo by - <a href='https://unsplash.com/@shah'>Shah</a></h4><p> Location - <a href='https://unsplash.com/photos/photo-1500530855697-b586d89ba3ee'>Mountain</a></p>">
            <img class="img-responsive"
                src="https://images.unsplash.com/photo-1500530855697-b586d89ba3ee?auto=format&fit=crop&w=240&q=80" />
        </a>

        <a data-lg-size="1400-1400" class="gallery-item"
            data-src="https://images.unsplash.com/photo-1469474968028-56623f02e42e?auto=format&fit=crop&w=1400&q=80"
            data-sub-html="<h4>Photo by - <a href='https://unsplash.com/@photographer1'>Katherine Gu</a></h4><p>Beautiful forest scenery.</p>">
            <img class="img-responsive"
                src="https://images.unsplash.com/photo-1469474968028-56623f02e42e?auto=format&fit=crop&w=240&q=80" />
        </a>

        <a data-lg-size="1400-1400" class="gallery-item"
            data-src="https://images.unsplash.com/photo-1526778548025-fa2f459cd5c1?auto=format&fit=crop&w=1400&q=80"
            data-sub-html="<h4>Photo by - <a href='https://unsplash.com/@photographer2'>Alex Smith</a></h4><p>City skyline at sunset.</p>">
            <img class="img-responsive"
                src="https://images.unsplash.com/photo-1526778548025-fa2f459cd5c1?auto=format&fit=crop&w=240&q=80" />
        </a>

        <a data-lg-size="1400-1400" class="gallery-item"
            data-src="https://images.unsplash.com/photo-1482192596544-9eb780fc7f66?auto=format&fit=crop&w=1400&q=80"
            data-sub-html="<h4>Photo by - <a href='https://unsplash.com/@photographer3'>Lisa Wong</a></h4><p>Beach sunrise view.</p>">
            <img class="img-responsive"
                src="https://images.unsplash.com/photo-1482192596544-9eb780fc7f66?auto=format&fit=crop&w=240&q=80" />
        </a>

        <a data-lg-size="1400-1400" class="gallery-item"
            data-src="https://images.unsplash.com/photo-1508057198894-247b23fe5ade?auto=format&fit=crop&w=1400&q=80"
            data-sub-html="<h4>Photo by - <a href='https://unsplash.com/@photographer4'>John Doe</a></h4><p>Night cityscape.</p>">
            <img class="img-responsive"
                src="https://images.unsplash.com/photo-1508057198894-247b23fe5ade?auto=format&fit=crop&w=240&q=80" />
        </a>

        <a data-lg-size="1400-1400" class="gallery-item"
            data-src="https://images.unsplash.com/photo-1500048993953-d23a436266cf?auto=format&fit=crop&w=1400&q=80"
            data-sub-html="<h4>Photo by - <a href='https://unsplash.com/@photographer5'>Emily Chen</a></h4><p>Historic architecture.</p>">
            <img class="img-responsive"
                src="https://images.unsplash.com/photo-1500048993953-d23a436266cf?auto=format&fit=crop&w=240&q=80" />
        </a>

        <a data-lg-size="1400-1400" class="gallery-item"
            data-src="https://images.unsplash.com/photo-1491553895911-0055eca6402d?auto=format&fit=crop&w=1400&q=80"
            data-sub-html="<h4>Photo by - <a href='https://unsplash.com/@photographer6'>Michael Lee</a></h4><p>River landscape.</p>">
            <img class="img-responsive"
                src="https://images.unsplash.com/photo-1491553895911-0055eca6402d?auto=format&fit=crop&w=240&q=80" />
        </a>

        <a data-lg-size="1400-1400" class="gallery-item"
            data-src="https://images.unsplash.com/photo-1494526585095-c41746248156?auto=format&fit=crop&w=1400&q=80"
            data-sub-html="<h4>Photo by - <a href='https://unsplash.com/@photographer7'>Sara Kim</a></h4><p>Mountain range view.</p>">
            <img class="img-responsive"
                src="https://images.unsplash.com/photo-1494526585095-c41746248156?auto=format&fit=crop&w=240&q=80" />
        </a>

        <a data-lg-size="1400-1400" class="gallery-item"
            data-src="https://images.unsplash.com/photo-1500534623283-312aade485b7?auto=format&fit=crop&w=1400&q=80"
            data-sub-html="<h4>Photo by - <a href='https://unsplash.com/@photographer8'>Anna Brown</a></h4><p>Forest trail.</p>">
            <img class="img-responsive"
                src="https://images.unsplash.com/photo-1500534623283-312aade485b7?auto=format&fit=crop&w=240&q=80" />
        </a>

        <a data-lg-size="1400-1400" class="gallery-item"
            data-src="https://images.unsplash.com/photo-1500534314209-a25ddb2bd429?auto=format&fit=crop&w=1400&q=80"
            data-sub-html="<h4>Photo by - <a href='https://unsplash.com/@photographer9'>Tom Wilson</a></h4><p>Autumn leaves scenery.</p>">
            <img class="img-responsive"
                src="https://images.unsplash.com/photo-1500534314209-a25ddb2bd429?auto=format&fit=crop&w=240&q=80" />
        </a>

    </lightgallery>
</template>

<script>
import Lightgallery from 'lightgallery/vue';
import lgZoom from 'lightgallery/plugins/zoom';
import lgVideo from 'lightgallery/plugins/video';

export default {
    name: 'PhotoLibrary',
    components: {
        Lightgallery,
    },
    data: () => ({
        plugins: [lgZoom, lgVideo],
    }),
};
</script>
<style>
@import url('https://cdn.jsdelivr.net/npm/lightgallery@2.0.0-beta.4/css/lightgallery.css');
@import url('https://cdn.jsdelivr.net/npm/lightgallery@2.0.0-beta.4/css/lg-zoom.css');
@import url('https://cdn.jsdelivr.net/npm/lightgallery@2.0.0-beta.4/css/lg-video.css');

body {
    margin: 0;
}

.gallery-item {
    margin: 5px;
}

.gallery-item img {
    width: 200px;
    height: 150px;
    object-fit: cover;
    border-radius: 6px;
    margin-top: 15px;
}
</style>