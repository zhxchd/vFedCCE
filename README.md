# `vFedCCE`
A vertical federated learning algorithm for classﬁcation problems with gradient-based optimization.

This algorithm is going to train a shared model on the common IDs (aligned by some private entity resolution technique) between vertically partitioned datasets, as shown in the following figure.

<img src="./docs/images/vertical_data.png" style="zoom: 50%;" />

The algorithm itself can be described by the following sequence diagram.

[![](https://mermaid.ink/img/eyJjb2RlIjoic2VxdWVuY2VEaWFncmFtXG5sb29wIGZvciBlYWNoIGJhdGNoIG9mIHNpemUgTjpcbiAgICBDbGllbnQgMS0tPj5DbGllbnQgMjogU2VuZCBtb2RlbCBvdXRwdXQgYSBhbmQgcGFydGlhbCBncmFkaWVudHNcbiAgICBOb3RlIGxlZnQgb2YgQ2xpZW50IDI6IENhbGN1bGF0ZSBwcmVkaWN0aW9uIHAgPSAoYSArIGIpLzJcbiAgICBOb3RlIGxlZnQgb2YgQ2xpZW50IDI6IENhbGN1bGF0ZSBpdHMgb3duIGdyYWRpZW50XG4gICAgTm90ZSBsZWZ0IG9mIENsaWVudCAyOiBVcGRhdGUgaXRzIHdlaWdodHMgYmFzZWQgb24gZ3JhZGllbnRcbiAgICBOb3RlIGxlZnQgb2YgQ2xpZW50IDI6IEFzc2VtYmxlIGNsaWVudCAxIGdyYWRpZW50XG4gICAgQ2xpZW50IDItLT4-Q2xpZW50IDE6IFNlbmQgYXNzZW1ibGVkIGdyYWRpZW50XG4gICAgTm90ZSByaWdodCBvZiBDbGllbnQgMTogVXBkYXRlIGl0cyB3ZWlnaHRzIGJhc2VkIG9uIGdyYWRpZW50XG5lbmRcbiAgICAgICAgICAgICIsIm1lcm1haWQiOnsidGhlbWUiOiJkZWZhdWx0In0sInVwZGF0ZUVkaXRvciI6dHJ1ZSwiYXV0b1N5bmMiOnRydWUsInVwZGF0ZURpYWdyYW0iOnRydWV9)](https://mermaid-js.github.io/mermaid-live-editor/edit#)

Details of the algorithm can be found in the [report](./docs/report.pdf).

Details of the implementation (with TensorFlow and Keras) can be found under the directory [src](./src/).
