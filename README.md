# `vFedCCE`
A vertical federated learning algorithm for classﬁcation problems with gradient-based optimization.

This algorithm is going to train a shared model on the common IDs (aligned by some private entity resolution technique) between vertically partitioned datasets, as shown in the following figure.

<img src="./docs/images/vertical_data.png" style="zoom: 50%;" />

The algorithm itself can be described by the following sequence diagram.

[![](https://mermaid.ink/img/eyJjb2RlIjoic2VxdWVuY2VEaWFncmFtXG5Ob3RlIHJpZ2h0IG9mIENsaWVudCAxOiBHZW5lcmF0ZSBwdWJsaWMgYW5kIHByaXZhdGUga2V5c1xuQ2xpZW50IDEgLS0-PiBDbGllbnQgMjogU2VuZCBwdWJsaWMga2V5XG5sb29wIGluIGVhY2ggZXBvY2g6XG4gICAgbG9vcCBmb3IgZWFjaCBiYXRjaCBvZiBzaXplIE46XG4gICAgICAgIE5vdGUgcmlnaHQgb2YgQ2xpZW50IDE6IENhbGN1bGF0ZSBtb2RlbCBvdXRwdXQgYVxuICAgICAgICBOb3RlIHJpZ2h0IG9mIENsaWVudCAxOiBDYWxjdWxhdGUgcGFydGlhbCBncmFkaWVudHMgYSdfaWpcbiAgICAgICAgTm90ZSByaWdodCBvZiBDbGllbnQgMTogRW5jcnlwdCBhJ19paiB3aXRoIHB1YmxpYyBrZXk6IFtbYSdfaWpdXVxuICAgICAgICBDbGllbnQgMS0tPj5DbGllbnQgMjogU2VuZCBhIGFuZCBbW2EnX2lqXV1cbiAgICAgICAgTm90ZSBsZWZ0IG9mIENsaWVudCAyOiBDYWxjdWxhdGUgcHJlZGljdGlvbiBwID0gKGEgKyBiKS8yXG4gICAgICAgIE5vdGUgbGVmdCBvZiBDbGllbnQgMjogTG9zcyBvZiBwIGFnYWluc3QgbGFiZWxzIHlcbiAgICAgICAgTm90ZSBsZWZ0IG9mIENsaWVudCAyOiBDYWxjdWxhdGUgZ3JhZGllbnQgZzJcbiAgICAgICAgTm90ZSBsZWZ0IG9mIENsaWVudCAyOiBVcGRhdGUgaXRzIHdlaWdodHMgYmFzZWQgb24gZzJcbiAgICAgICAgTm90ZSBsZWZ0IG9mIENsaWVudCAyOiBBc3NlbWJsZSBbW2cxXV0gdmlhIFtbYSdfaWpdXVxuICAgICAgICBDbGllbnQgMi0tPj5DbGllbnQgMTogU2VuZCBjbGllbnQgMSdzIGdyYWRpZW50IFtbZzFdXSAoc3RpbGwgZW5jcnlwdGVkKVxuICAgICAgICBOb3RlIHJpZ2h0IG9mIENsaWVudCAxOiBEZWNyeXB0IFtbZzFdXSBmb3IgZ3JhZGllbnQgZzEgd2l0aCBwcml2YXRlIGtleVxuICAgICAgICBOb3RlIHJpZ2h0IG9mIENsaWVudCAxOiBVcGRhdGUgaXRzIHdlaWdodHMgYmFzZWQgb24gZzFcbiAgICBlbmRcbmVuZFxuICAgICAgICAgICAgIiwibWVybWFpZCI6eyJ0aGVtZSI6ImRlZmF1bHQifSwidXBkYXRlRWRpdG9yIjpmYWxzZSwiYXV0b1N5bmMiOnRydWUsInVwZGF0ZURpYWdyYW0iOmZhbHNlfQ)](https://mermaid-js.github.io/mermaid-live-editor/edit#)

Details of the algorithm can be found in the [report](./docs/report.pdf).

Details of the implementation (with TensorFlow and Keras) can be found under the directory [src](./src/).
