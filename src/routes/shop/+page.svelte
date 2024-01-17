<script>
    import Card from '$lib/components/Card.svelte'
    import whiteCard1 from '$lib/assets/white-tee-card-1-edit.png'
    import whiteCard2 from '$lib/assets/white-tee-card-2-edit.png'
    import whiteCard3 from '$lib/assets/white-tee-card-3-edit.png'
    import whiteCardAlt1 from '$lib/assets/white-tee-card-alt-1-edit.png'
    import whiteCardAlt2 from '$lib/assets/white-tee-card-alt-2-edit.png'
    import whiteCardAlt3 from '$lib/assets/white-tee-card-alt-3-edit.png'

    let outOfStock = false
</script>
  
<div class="grid grid-cols-1 sm:grid-cols-3 gap-4 mt-40 mb-40">
    <Card customText="White" imageUrl={whiteCard1} outOfStock={outOfStock} />
    <Card customText="Gray" imageUrl={whiteCard2} outOfStock={outOfStock} />
    <Card customText="Black" imageUrl={whiteCard3} outOfStock={outOfStock} />
    <Card customText="Red" imageUrl={whiteCardAlt1} outOfStock={outOfStock} />
    <Card customText="Blue" imageUrl={whiteCardAlt2} outOfStock={outOfStock} />
    <Card customText="Navy" imageUrl={whiteCardAlt3} outOfStock={outOfStock} />
</div>