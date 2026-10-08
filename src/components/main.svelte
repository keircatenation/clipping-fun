<script>
    import img1 from '#lib/assets/mag-hugo-mccloud_200.jpg';
    import stairCutout2 from '#lib/assets/stair-cutouts-02.png'
    import stairCutout2b from '#lib/assets/stair-cutouts2b.png'
    import stairCutout3b from '#lib/assets/stair-cutouts3b.svg'
</script>
<main>
    <div class="header">
        <img src={img1} alt=""/>
        <div class="header-text-wrapper">
            <div class="header-text">
                <h1>Welcome to the Memorial Art Gallery</h1>
                <p>7,000 years of art from around the world in Rochester, New York — free for all, forever</p>
                <a href="https://mag.rochester.edu/visit/">Plan your visit</a>
            </div>
        </div>
    </div>
    

</main>
<style>
    .header{
        position: relative;
        aspect-ratio: 16/9;
        .header-text-wrapper{
            position: absolute;
            top:3rem;
            left:3rem;
            height: 40%;
            aspect-ratio: 1.169;
            z-index: 2;
            row-gap: var(--spacing--20);
            clip-path:shape(from 0% 16.46%,line to 14.47% 16.46%,line to 28.75% 0%,line to 42.93% 16.46%,line to 57.2% 0%,line to 71.48% 16.46%,line to 85.85% 0%,line to 85.85% 16.46%,line to 100% 16.46%,line to 71.67% 49.87%,line to 85.56% 66.63%,line to 57.3% 66.63%,line to 28.55% 100%,line to 14.47% 82.85%,line to 0% 82.85%,line to 0% 16.46%,close);
            background-color: var(--color--white);
            .header-text{
                margin-top:2.5rem;
                margin-left:1rem;
                width: 75%;
                display: flex;
                flex-direction: column;
                justify-content: center;
                row-gap:var(--spacing--20);
                *{
                    margin: 0;
                }
                h1{
                    font-size: var(--font-size--xx-large);
                    line-height:1.05;
                }
                p{
                    margin-right:3rem;
                }
            }
        }
        img{
            width: 100%;
            height: 100%;
            object-fit: cover;
            max-height: clamp(300px,70vh,900px);
        }
    }
</style>