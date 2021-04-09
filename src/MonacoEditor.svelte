<script lang="ts">
  import loader from "@monaco-editor/loader";

  loader.init().then((monaco) => {
    monaco.editor.create(document.querySelector("#app"), {
      value: "// some comment",
      language: "c",
      theme: "vs-dark",
      scrollbar: {
        arrowSize: 11,
      },
      fontSize: 16,
      wordWrap: "on",
      wordWrapMinified: true,
      minimap: {
        enabled: false,
      },
      lineNumbers: "on",
    });
  });
</script>

<div id="app" />

<style global>
  body {
    height: 100vh;
    font-family: sans-serif;
  }

  #app {
    height: 100%;
  }
</style>
