# RESTful 设计原则

## 客户端-服务器架构，即前后端分离

> 客户端和服务器之间的通信通过 HTTP 协议完成，客户端和服务器之间没有关于请求的状态信息，每个组件都可以独立修改而不影响其他组件。

## 无状态 请求独立，互不影响
RESTful 服务应该是无状态的。这意味着服务器不应该保存关于客户端请求的任何状态信息。每个请求都应该包含足够的信息来完成该请求，而不需要依赖之前的请求或状态。这样可以使得系统更加简单和可伸缩。

## 缓存 支持http缓存，通知客户端资源是否缓存
RESTful 服务应该支持缓存。服务器应该在响应中包含缓存控制信息，以告知客户端该资源是否可以被缓存。这样可以提高系统的性能和可伸缩性，减少网络带宽的消耗。

## 统一接口
RESTful 服务应该提供统一的接口，包括资源的标识、资源的操作方法、资源的表示形式和超媒体控制信息。这样可以简化客户端和服务器之间的通信，使得客户端和服务器之间的耦合度更低。

## 服务分层，资源表示形式和业务逻辑分离
RESTful 服务应该是分层的。这意味着服务器应该将资源的表示形式和业务逻辑分离。这样可以提高系统的可伸缩性和灵活性，使得系统更易于维护和扩展。

## 按需代码，通过传输代码来扩展功能
RESTful 服务应该可以通过传输代码来扩展其功能，但是这种方式不是必需的。如果需要扩展功能，可以使用例如 JavaScript 或 Flash 等技术来传输代码。这样可以使得系统更加灵活和可扩展。

## 面相资源，每个资源有唯一URL
RESTful 服务应该是面向资源的。每个资源都应该有一个唯一的标识符（URI），并且应该通过 HTTP 方法（例如 GET、POST、PUT、DELETE 等）对资源进行操作。这样可以使得系统更加具有可读性和可维护性。