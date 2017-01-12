A **shim** is a small library placed in front of an API to transparently intercept API calls in order to handle the call instead of the API, change arguments or redirect the operation.

### Origins

Shim (noun) — a small object or piece of material used between two parts of something to make them fit together, or to prevent them rubbing against each other.<sup>1</sup>

### Examples

I. Not all JS files can be used directly with webpack. The file might be in an unsupported module format, or not even in any module format. Webpack provides several loaders to make these files work with webpack. This is called _shimming_. [Learn more about shimming modules in Webpack](https://webpack.github.io/docs/shimming-modules.html).

II. To facilitate cloud gaming powered by NVIDIA GRID, a software layer for managing multiple concurrent game sessions is needed. This can be implemented without requiring modifications to the application by intercepting API calls from the graphics API and adding the necessary GRID API calls for capture and encode. [Learn more about API Hooking Techniques for GRID Cloud Game Streaming](https://developer.nvidia.com/content/api-hooking-techniques-grid-cloud-game-streaming).

[[/uploads/apihooking3.jpg]]

### Alternative explanation

A shim is a library that brings a new API to an older environment, using only the means of that environment.<sup>2</sup>
II. It’small library makes an older part of an application (that has to be kept and can’t be redone) work with the new additions/changes. Think of it as a compatibility layer.<sup>3</sup>

---

<div class="footnotes">
1. Cambridge Dictionary <br>
2. Dr. Axel Rauschmayer, [[http://www.2ality.com/2011/12/shim-vs-polyfill.html]]<br>
3. Iris Classon, [[http://irisclasson.com/2013/01/30/stupid-question-139-what-is-a-shim/]]
</div>