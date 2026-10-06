<script>
    import img1 from '#lib/assets/mag-hugo-mccloud_200.jpg';
    import stairCutout2 from '#lib/assets/stair-cutouts-02.png'
    import stairCutout2b from '#lib/assets/stair-cutouts2b.png'
    import stairCutout3b from '#lib/assets/stair-cutouts3b.svg'
</script>
<main>
    <div class="header">
        <div class="header-text">
            <h1>Welcome to the Memorial Art Gallery</h1>
            <p>7,000 years of art from around the world in Rochester, New York — free for all, forever</p>
            <a href="https://mag.rochester.edu/visit/">Plan your visit</a>
        </div>
        <img src={img1} alt=""/>
    </div>
    

</main>
<style>
    .header{
        position: relative;
        display: grid;
        overflow: hidden;
        .header-text{
            grid-column: 1;
            grid-row: 1;
            z-index: 2;
            display: flex;
            flex-direction: column;
            justify-content: center;
            row-gap: var(--spacing--20);
            margin-left:calc(2 * var(--spacing--padding));
            margin-right:auto;
            align-self: center;
            padding:4rem 2rem 6rem;
            max-width:50%;
            height: auto;
            aspect-ratio:400/250;
            clip-path:polygon(0% 10%, 15% 10%, 27% 0%, 41.2% 10%, 57.6% 0%, 72% 10%, 82.5% 0%, 84.9% 13.4%, 98.6% 14.8%, 72.4% 50%, 86.6% 69.8%, 56.8% 70.3%, 29.4% 100%, 13.9% 87%, 0% 86.9%);
            background-color: var(--color--white);
            *{
                margin: 0;
            }
            h1{
                font-size: var(--font-size--xxx-large);
                line-height:1.05;
            }
        }
        img{
            grid-column: 1;
            grid-row: 1;
            mask-repeat: repeat-x;
            mask-position: 45%;
            width: 100%;
            height: 100%;
            max-height: 600px;
            object-fit: cover;
        }
    }
</style>