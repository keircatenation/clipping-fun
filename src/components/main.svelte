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
            height:clamp(250px,50vh,700px);
            width:500px;
            z-index: 2;
            row-gap: var(--spacing--20);
            clip-path:polygon(0% 15%, 15% 15%, 27% 0%, 40% 15%, 55% 0%, 70% 15%, 82.5% 0%, 84.9% 15%, 98.6% 15%, 72.4% 50%, 86.6% 69.8%, 56.8% 70.3%, 29.4% 100%, 13.9% 87%, 0% 86.9%);
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