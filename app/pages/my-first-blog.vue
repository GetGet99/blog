<script setup lang="ts">
const clickCount = ref(0)
</script>
<template>
    <div class="flex flex-col items-center">
        <div class="flex flex-col gap-3 max-w-50">
            <h1 class="mt-7">
                Hello! Welcome to my first blog!
            </h1>
            <div class="text-sm text-subtitle">December 5, 2025 - Get</div>
            <p>This is an experimental thing that I am doing today. I'm writing a blog. And I'm going to do that in
                Nuxt,
                with a
                few components copied from SimplyTools.</p>
            <p>Now you might ask why am I copying a lot of stuff from there. Well, I could have a little fun things in
                the
                page.
                For example,</p>
            <Sandbox>
                <Button @click="clickCount++" icon="left">
                    <IconCursorClick />
                    Click me
                </Button>
                <pre v-if="clickCount">You clicked {{ clickCount }} time{{ clickCount >= 2 ? 's' : '' }}</pre>
            </Sandbox>
            <p>Not sure if I'll get to use these interactive contents in the future. Maybe I just put it there because
                it looks cool. ⭐⭐⭐</p>
            <h2>What will I do here?</h2>
            <p>I guess I'll be showcasing my projects. Currently, I'm working on Project QuickMarkup. I like Vue's
                Single File Component (SFC), so I'm trying to recreate one for WinUI.</p>
            <img src="~/assets/my-first-blog/quickmarkup-tests.png" alt="QuickMarkup test case passing" />
            <p>It will look something like that.</p>
            <h2>Not good at blogging, but this is a starting point</h2>
            <p>I just start writing my blog for the first time. I'm not sure what I can put, so this might not be the
                best blog ever. Hopefully, I learn more about them and let's make a more interactive blogs.</p>
            <p class="mb-7">- Get</p>
        </div>
    </div>
</template>