# GeoGUNDiff: Harmonizing-Geometry-and-Uncertainty-Diffusion-with-Hyperspheres

<meta http-equiv="Cache-Control" content="max-age=86400" />
<!DOCTYPE html>

<html>

<head>
    <style>
        td,
        th {
            border: 0px solid black;
        }

        img {
            padding: 5px;
        }

        .forward {
            float: left;
            width: 50%;

        }
    </style>

    <title> Hyperspheres</title>

    <link href="https://fonts.googleapis.com/css?family=Google+Sans|Noto+Sans|Castoro" rel="stylesheet">

    <link rel="shortcut icon" href="./static/images/logo.png" />

    <link rel="stylesheet" href="./static/css/bulma.min.css">
    <link rel="stylesheet" href="./static/css/bulma-carousel.min.css">
    <link rel="stylesheet" href="./static/css/bulma-slider.min.css">
    <link rel="stylesheet" href="./static/css/fontawesome.all.min.css">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/jpswalsh/academicons@1/css/academicons.min.css">
    <link rel="stylesheet" href="./static/css/index.css">
    <link rel="stylesheet" href="./static/css/leaderboard.css">
    <link rel="icon" href="./static/images/favicon.svg">
    <link rel="stylesheet" href="https://unpkg.com/image-compare-viewer/dist/image-compare-viewer.min.css">

    <script src="https://unpkg.com/image-compare-viewer/dist/image-compare-viewer.min.js"></script>
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
    <script defer src="./static/js/fontawesome.all.min.js"></script>
    <script src="./static/js/bulma-carousel.min.js"></script>
    <script src="./static/js/bulma-slider.min.js"></script>
    <script src="./static/js/index.js"></script>
    <script src="./static/js/explorer-index.js"></script>
    <script src="./static/js/question_card.js"></script>

    <script src="./static/js/leaderboard_testmini.js"></script>
    <script src="./data/results/output_folders.js" defer></script>
    <script src="./data/results/model_scores.js" defer></script>

    <script src="./visualizer/data/data_public.js" defer></script>

</head>

<body>


    <section class="hero">
        <div class="hero-body">
            <div class="container is-max-desktop">
                <div class="columns is-centered">
                    <div class="column has-text-centered">
                        <h2 class="title is-2 publication-title is-bold" style="margin-bottom: 0;">
                            Harmonizing Geometry and Uncertainty: Diffusion with Hyperspheres
                        </h2>
                        <!-- <h2 class="title is-2 publication-title is-bold" style="margin-top: 0;">
                            Orchestrating Linguistic Harmony in a World of Deepfakes
                        </h2> -->
                        <!-- <h2 class="title is-2 publication-title is-bold" style="margin-bottom: 0;">

                        </h2> -->
                        <div class="is-size-5 publication-authors">
                            <div class="authors-group">
                                <span class="author-block">
                                    <a href="" target="_blank">Anonymous Authors</a>
                                </span>
                                <!-- <span class="author-block">
                                    <a href="https://sites.google.com/view/rishabhranjan/" target="_blank">Rishabh Ranjan</a>,
                                </span>
                                <span class="author-block">
                                    <a href="http://home.iitj.ac.in/~mvatsa/" target="_blank">Mayank Vatsa
                                    </a>,
                                </span>
                                <span class="author-block">
                                    <a href="http://home.iitj.ac.in/~richa/"
                                        target="_blank">Richa Singh</a>
                                </span> -->
                            </div>
                        </div>


                        <div class="is-size-5 publication-authors">
                            <span class="author-block">Anonymous University</span>
                        </div>

                        <div class="column has-text-centered">
                            <a href="as"></a>
                            </span>
                        </div>

                        <div class="column has-text-centered">
                            <!-- <div class="publication-links">
                                <span class="link-block">
                                    <a href="https://arxiv.org/abs/2501.10360"
                                        class="external-link button is-normal is-rounded is-dark">
                                        <span class="icon">
                                            <i class="ai ai-arxiv"></i>
                                        </span>
                                        <span>arXiv</span>
                                    </a>
                                </span> -->
<!--                                 <span class="link-block">
                                    <a href=""
                                        class="external-link button is-normal is-rounded is-dark">
                                        <span class="icon">
                                            <i class="fab fa-github"></i>
                                        </span>
                                        <span>Coming Soon</span>
                                    </a>
                                </span> -->
                            </div>
                        </div>

                    </div>
                </div>
            </div>
        </div>
    </section>

    <section class="section">
        <div class="container" style="margin-bottom: 2vh;">
            <div class="columns is-centered has-text-centered">
                <div class="column is-four-fifths">
                    <h2 class="title is-3">Motivation</h2>
                    <div class="content has-text-justified">
                        <img src="./static/SAFARI_IMAGES/vis_abs.png" alt="" border=0 height=600 width=1500></img>
                        <p>
                            (a) Illustrating class geometry preservation in non-Euclidean hyperspherical spaces. The top
                            row shows Gaussian diffusion, which fails to capture structural relations, whereas the
                            bottom row demonstrates von Mises–Fisher (vMF)-based diffusion, effectively modeling
                            directional uncertainty. Red and Green arrows indicate forward and backward diffusion
                            process, respectively. (b) Comparison of three-class diffusion on the 3D sphere: Gaussian
                            (top) vs. vMF (bottom). Gaussian distorts class boundaries, while vMF maintains the original
                            geometry, preserving angular regions.
                        </p>
                        <p> <i>Do contemporary diffusion models preserve the class geometry of hyperspherical data?</i>
                            Existing diffusion models employ isotropic Gaussian noise in the forward process, inherently
                            biasing the learned distribution toward Euclidean spaces. However, many problems involve
                            distributions living on non-Euclidean spaces, including Hyperspherical manifolds. The design
                            choice of learning in Euclidean spaces overlooks the intrinsic geometric properties of
                            hyperspherical data, where class-specific structures are best represented by directional
                            relationships within <b>hypercones</b>. These models fail to capture the angular
                            subtleties and class geometry required for effective generative modeling on hyperspheres. By
                            introducing directional noise aligned with the data’s hyperspherical structure for angular
                            uncertainty, our approach preserves class geometry while effectively modeling uncertainty.
                            We theoretically and experimentally demonstrate that this method aligns the generative
                            process with the inherent properties of hyperspherical data, enabling more accurate and
                            geometry-aware representations.
                        </p>
                    </div>
                </div>
            </div>
            <div class="container" style="margin-bottom: 2vh;">
                <div class="columns is-centered has-text-centered">
                    <div class="column is-four-fifths">
                        <h2 class="title is-3">Contributions</h2>
                        <div class="content has-text-justified">
                            <p>The key contributions of our work are as follows:
                            </p>
                            <ul>
                                <li>
                                    <b>Introduce a <i>Class-Specific Hypercone</i>
                                        Formalism:</b> We define class hypercones to preserve intra-class angular
                                    concentration
                                    while ensuring inter-class separation on the hypersphere.

                                </li>
                                <li> <b>Design a vMF-Based Forward and Reverse Process:</b> A novel dual-stream approach
                                    combining Whisper
                                    and m-HuBERT encoders with an Audio Feature Unification Module and
                                    large language model integration, designed specifically for multilingual deepfake
                                    detection.
                                </li>
                                <li> <b>Enable Diverse and Hard Sample Generation</b>: Unlike Gaussian noise, our
                                    vMF-based approach avoids simplicity bias, producing a well-spread distribution with
                                    challenging yet realistic samples. We introduce two metrics, <i>Hypercone
                                        Coverage Ratio (HCR) and Hypercone Difficulty Skew (HDS)</i> to assess
                                    distribution spread and sample difficulty.
                                </li>
                                <li> <b>Develop Theoretical Foundations and Empirical Evaluations</b>: We validate our
                                    approach with
                                    experiments, demonstrating improved alignment with intrinsic geometry and robustness
                                    to varying degrees of uncertainty in class-conditional tasks on 4 object datasets
                                    (CIFAR-10, MNIST, CUB-200, Cars-196)
                                    and 2 face datasets (CelebA, D-LORD).
                                </li>
                            </ul>

                            </p>
                        </div>
                    </div>
                </div>
                <!--/ Abstract. -->

                <!-- Paper video. -->

                <section class="section">
                    <div class="container" style="margin-bottom: 2vh;">
                        <!-- Abstract. -->
                        <div class="columns is-centered has-text-centered">
                            <div class="column is-four-fifths">
                                <h2 class="title is-3">Proposed vMF based Diffusion Modeling</h2>
                                <div class="content has-text-justified">
                                    <h5 class="subtitle has-text-centered"></h5>
                                    <div class="forward">
                                        <img src="./static/SAFARI_IMAGES/2.gif" alt="forward" style="width:100%">
                                    </div>
                                    <div class="forward">
                                        <img src="./static/SAFARI_IMAGES/3.gif" alt="reverse" style="width:100%">
                                    </div>
                                    <!-- <p>
                                        Figure 2. Overview of the IndicFake benchmark and SAFARI-LLM. The top panel
                                        shows the IndicFake dataset spanning 18 Indian languages across
                                        three language families, while the bottom panel illustrates our proposed
                                        SAFARI-LLM architecture leveraging dual speech encoders and feature fusion.
                                        Three key research questions
                                        (RQ1-3) guide our investigation of cross-lingual generalization, cross-language
                                        family transfer, and architectural impact on deepfake detection performance
                                    </p> -->


                                </div>
                            </div>
                        </div>
                    </div>
                </section>
                <section class="section">
                    <div class="container" style="margin-bottom: 2vh;">
                        <div class="columns is-centered has-text-centered">
                            <div class="column is-four-fifths">
                                <h2 class="title is-3">Training and Sampling Process</h2>
                                <div class="content has-text-justified" <h5 class="subtitle has-text-centered">
                                    </h5>
                                    <div class="forward">
                                        <img src="./static/SAFARI_IMAGES/1_algo.png" alt="forward"
                                            style="width:100%; height:210px;">
                                    </div>
                                    <div class="forward">
                                        <img src="./static/SAFARI_IMAGES/2_algo.png" alt="reverse"
                                            style="width:100%; height:210px;">
                                    </div>
                                    <!-- <img src="./static/SAFARI_IMAGES/3_algo.png" alt="" border="0" height=500 width=500></img> -->
                                    <!-- <p>
                                        Distribution of real and synthetic speech samples across 17 Indian languages and
                                        English, showing sample counts for different
                                        TTS systems with gender-wise splits and total dataset composition.
                                    </p> -->
                                </div>
                            </div>
                        </div>
                    </div>
                </section>
            </div>
        </div>
    </section>
    <section class="section">
        <div class="container" style="margin-top: -170px; margin-bottom: -100px;">
            <div class="columns is-centered m-6">
                <div class="column is-full has-text-centered content">
                    <div id="results-carousel1" class="carousel results-carousel">
                        <div class="box m-5">
                            <div class="content has-text-centered">
                                <img src="static/SAFARI_IMAGES/samples-2_page-0001.jpg" alt="question distribution"
                                    style="width:84%; height:500px; object-fit: contain;" />
                                <p>Generated samples of birds (left) and facial (right) images using the proposed vMF
                                    based diffusion model trained on CelebA
                                    and CUB-200 dataset, showcasing the preservation key attributes and diversity.
                                </p>
                            </div>
                        </div>
                        <div class="box m-5">
                            <div class="content has-text-centered">
                                <img src="static/SAFARI_IMAGES/cifar10_collage_page-0001.jpg" alt="key statistics"
                                    style="width:84%; height:500px; object-fit: contain;" />
                                <p> Generated samples through proposed vMF based diffusion model trained using CIFAR-10
                                    dataset.
                                </p>
                            </div>
                        </div>
                        <div class="box m-5">
                            <div class="content has-text-centered">
                                <img src="static/SAFARI_IMAGES/mnist_collage_page-0001.jpg" alt="dataset distribution"
                                    style="width:84%; height:500px; object-fit: contain;" />
                                <p> Generated samples through proposed vMF based diffusion model trained using MNIST
                                    dataset.
                                </p>
                            </div>
                        </div>
                        <div class="box m-5">
                            <div class="content has-text-centered">
                                <img src="static/SAFARI_IMAGES/hard_samples_page-0001.jpg" alt="dataset distribution"
                                    style="width:84%; height:500px; object-fit: contain;" />
                                <p> (a) Comparison of generated samples using Gaussian and vMF diffusion models,
                                    highlighting improved variation in pose, illumination, expressions, and quality with
                                    vMF. (b) Scatter + regression plot shows cosine similarity to the class mean, where
                                    vMF generates more challenging samples with broader similarity distribution compared
                                    to Gaussian.
                                </p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section class="section">
        <div class="container" style="margin-bottom: 2vh;">
            <section class="section">
                <div class="container">
                    <div class="columns is-centered">
                        <div class="column is-full has-text-centered content">
                            <h2 class="title is-3" id="example">Results</h2>
                            <div id="results-carousel" class="">
                                <div class="box m-5">
                                    <div class="content has-text-centered">
                                        <img src="static/SAFARI_IMAGES/results.png" alt="Example 1"
                                            style="width:84%; height:700px; object-fit: contain;" />
                                        <p> Performance comparison of Gaussian and vMF models
                                            across six datasets using FID (lower is better), HCR (lower is
                                            better), and HDS (lower indicates harder samples). The vMF
                                            model demonstrates superior capability in generating challenging
                                            samples with better FID and HDS scores.</p>
                                    </div>
                                </div>
                                <!-- <div class="box m-5"> -->
                                    <!-- <div class="content has-text-centered">
                                        <img src="static/SAFARI_IMAGES/decroresult.jpeg" alt="Example 2"
                                            style="width:84%; height:700px; object-fit: contain;" />
                                    </div> -->
                                <!-- </div> -->
                                <!-- <div class="box m-5"> -->
                                    <!-- <div class="content has-text-centered">
                                        <img src="static/SAFARI_IMAGES/setaresult.jpeg" alt="Example 3"
                                            style="width:84%; height:700px; object-fit: contain;" />
                                    </div> -->
                                <!-- </div> -->
                                <!-- <div class="box m-5">
                                                <div class="content has-text-centered">
                                                    <img src="static/images/example_4.png" alt="Example 4"
                                                        style="width:84%; height:700px; object-fit: contain;" />
                                                </div>
                                            </div>
                                            <div class="box m-5">
                                                <div class="content has-text-centered">
                                                    <img src="static/images/example_5.png" alt="Example 5"
                                                        style="width:84%; height:700px; object-fit: contain;" />
                                                </div>
                                            </div>
                                            <div class="box m-5">
                                                <div class="content has-text-centered">
                                                    <img src="static/images/example_6.png" alt="Example 6"
                                                        style="width:84%; height:700px; object-fit: contain;" />
                                                </div>
                                            </div>
                                            <div class="box m-5">
                                                <div class="content has-text-centered">
                                                    <img src="static/images/example_7.png" alt="Example 7"
                                                        style="width:84%; height:700px; object-fit: contain;" />
                                                </div>
                                            </div>
                                            <div class="box m-5">
                                                <div class="content has-text-centered">
                                                    <img src="static/images/example_8.png" alt="Example 8"
                                                        style="width:84%; height:700px; object-fit: contain;" />
                                                </div>
                                            </div>
                                            <div class="box m-5">
                                                <div class="content has-text-centered">
                                                    <img src="static/images/example_9.png" alt="Example 9"
                                                        style="width:84%; height:700px; object-fit: contain;" />
                                                </div>
                                            </div>
                                            <div class="box m-5">
                                                <div class="content has-text-centered">
                                                    <img src="static/images/example_10.png" alt="Example 10"
                                                        style="width:84%; height:700px; object-fit: contain;" />
                                                </div>
                                            </div>
                                            <div class="box m-5">
                                                <div class="content has-text-centered">
                                                    <img src="static/images/example_11.png" alt="Example 11"
                                                        style="width:84%; height:700px; object-fit: contain;" />
                                                </div>
                                            </div>
                                            <div class="box m-5">
                                                <div class="content has-text-centered">
                                                    <img src="static/images/example_12.png" alt="Example 12"
                                                        style="width:84%; height:700px; object-fit: contain;" />
                                                </div>
                                            </div>
                                            <div class="box m-5">
                                                <div class="content has-text-centered">
                                                    <img src="static/images/example_13.png" alt="Example 13"
                                                        style="width:84%; height:700px; object-fit: contain;" />
                                                </div>
                                            </div>
                                            <div class="box m-5">
                                                <div class="content has-text-centered">
                                                    <img src="static/images/example_14.png" alt="Example 14"
                                                        style="width:84%; height:700px; object-fit: contain;" />
                                                </div>
                                            </div> -->
                            </div>
                        </div>
                    </div>
                </div>
            </section>

            <!-- <section class="section">
                            <div class="container" style="margin-bottom: 2vh;">
                                <div class="columns is-centered has-text-centered">
                                    <div class="column is-four-fifths">
                                        <h2 class="title is-3">Results</h2>
                                        <div class="content has-text-justified">
                                            <h5 class="subtitle has-text-centered"></h5>
                                            <img src="./static/images/results.png" alt="" border="0" height=500
                                                width=1500></img>
                                            <p>
                                                Table 1. Results of different models on the FaceXBench. We categorize
                                                the
                                                open-source models in three categories based on
                                                parameter size:
                                                (a) Open source MLLMs (<4B parameters), (b) Open source MLLMs (4B-13B
                                                    parameters), (c) Open source MLLMs (>13B
                                                    parameters).
                                                    Additionally, we evaluate (d) proprietary models. The best model
                                                    in each category is highlighted in <b style="color: blue;">bold</b>.
                                            </p>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </section>
                    </div>
            </div>
    </section> -->

            <!-- <section class="section" id="BibTeX">
        <div class="container" style="margin-top: -200px; margin-bottom: -100px;"></div>
        <div class="container is-max-desktop">
            <h2 class="title">BibTeX</h2>
            <pre>Coming Soon ... !!!
            </pre>
        </div>
    </section> -->

            <section class="section">
                <div class="container is-max-desktop">
                    <h5 class="title" style="font-size: 10px;"> Acknowledgement: The website template is taken from
                        <span class="author-block">
                            <a href="https://nerfies.github.io/" target="_blank">Nerfies</a>
                    </h5>
                </div>
            </section>

            <script>
                const viewers = document.querySelectorAll(".image-compare");
                viewers.forEach((element) => {
                    let view = new ImageCompare(element, {
                        hoverStart: true,
                        addCircle: true
                    }).mount();
                });

                $(document).ready(function () {
                    var editor = CodeMirror.fromTextArea(document.getElementById("bibtex"), {
                        lineNumbers: false,
                        lineWrapping: true,
                        readOnly: true
                    });
                    $(function () {
                        $('[data-toggle="tooltip"]').tooltip()
                    })
                });

                // Carousel Initialization
                document.addEventListener("DOMContentLoaded", () => {
                    bulmaCarousel.attach('#example-carousel', {
                        slidesToScroll: 1,
                        slidesToShow: 1,
                        autoplay: true,
                        loop: true,
                        pauseOnHover: true,
                        navigation: true,
                        pagination: true,
                    });
                });
            </script>

</body>

</html>
