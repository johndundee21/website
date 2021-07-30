<script lang="ts">
  import RecentArticlesPreview from "./recent-articles-preview.svelte";
  import NewsletterSignup from "./newsletter-signup.svelte";
  import PostContentLayout from "../post-content-layout.svelte";
</script>

<PostContentLayout 
  imagesDirectoryName="blog"
  baseUrl="https://www.gitpod.io/blog/"
  {...$$restProps}
>
  <slot />
</PostContentLayout>

<NewsletterSignup class="mx-auto mt-large mb-huge" />
<RecentArticlesPreview />
