<script>
	import EditorJS from '@editorjs/editorjs';
  import Header from '@editorjs/header'; 
  import List from '@editorjs/list'; 
  import CheckList from '@editorjs/checklist';
  // import LinkTool from '@editorjs/link';
  import Table from '@editorjs/table';


	let editor = new EditorJS({
    holderId: 'md-editor',
    autofocus: true,
    tools: {
      header: {
        class: Header,
        defaultLevel: 1,
        levels: [1, 2, 3, 4, 5, 6],
      },
      list: List,
      checklist: CheckList,
      // linkTool: LinkTool,
      table: {
        class: Table,
        inlineToolbar: true,
      },
    },
  });
</script>

<div id="md-editor" />

<style>
</style>