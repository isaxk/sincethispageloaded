<script lang="ts">
</script>

<div class="header">
	<div class="content">
		<div class="title">
			<a href="/">Since this page loaded...</a>
		</div>
		<div class="links">
			<a href="https://github.com/isaxk/sincethispageloaded">GitHub</a>
			<a href="https://www.isaxk.com">isaxk.com</a>
		</div>
	</div>
</div>

<style>
	.header {
		position: -webkit-sticky;
		position: sticky;
        top: 0;
		height: 50px;
		background-color: var(--header-background-color);
		padding: 0px 20px;
        display: flex;
        align-items: center;
	}
    .content {
        width: 100%;
        max-width: 1150px;
        display: grid;
        margin: auto;
		align-items: center;
		grid-template-columns: 1fr max-content;
    }
	.title {
		font-size: 20px;
		font-weight: 500;
	}
	a {
		color: var(--text-color);
		text-decoration: none;
	}
	.links a {
		margin: 0px 0px 0px 10px;
	}
</style>