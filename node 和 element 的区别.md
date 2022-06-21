Dom 文档由Node 层次结构组成，每一个node都可以有一个母节点子节点。
![层次图](https://dmitripavlutin.com/static/75f1711be6313112e996905bd49c9951/ee28a/dom-nodes.webp)

html 是 document tree 的节点
body 有一个节点，其中包括三个孩子

# Node Types
Node.ELEMENT_NODE

Node.ATTRIBUTE_NODE

Node.TEXT_NODE

Node.CDATA_SECTION_NODE

Node.PROCESSING_INSTRUCTION_NODE

Node.COMMENT_NODE

Node.DOCUMENT_NODE

Node.DOCUMENT_TYPE_NODE

Node.DOCUMENT_FRAGMENT_NODE

Node.NOTATION_NODE

# DOM Element

elemen is a node of a specific type(Node.ELEMENT_NODE)
an element is a node that'written using a tag in the HTML document.

 <html>, <head>, <title>, <body>, <h2>, <p> are all elements because they are represented by tags.
  
The document type, the comment, the text nodes aren't elements because they are not written with tags:
