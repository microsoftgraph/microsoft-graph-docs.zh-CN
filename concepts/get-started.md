# <a name="getting-started-building-microsoft-graph-apps"></a>开始生成 Microsoft Graph 应用

本节中的各篇文章详细介绍了如何生成应用以跨各种语言和开发平台连接到 Microsoft Graph。 每篇文章都从入门项目入手，并逐步介绍连接到 Microsoft Graph 的基本步骤：

 1. 注册应用程序
 2. 验证用户并在应用程序中获取访问令牌
 3. 从应用程序调用 Microsoft Graph
 4. 运行应用程序

若要更快地生成并运行有效解决方案，请尝试[快速入门](https://developer.microsoft.com/graph/quick-start)体验。

完成的每个项目都与相应平台的 [Microsoft Graph 存储库中的 Connect 示例](https://github.com/microsoftgraph?utf8=%E2%9C%93&query=connect)完全相同。

想要查看更多代码？

请浏览 GitHub 中的所有 [Microsoft Graph 示例](https://github.com/microsoftgraph)。 下表列出了本节中示例的其他版本。 它们展示了如何使用两个 ADAL 终结点（v1.0 和 v2.0）验证用户，并使用原始 REST 调用或 Microsoft Graph 客户端库 (SDK) 连接到 Microsoft Graph。

（选择涉及选定验证提供程序和开发平台的文章，再开始连接到 Microsoft Graph。 有关详细信息，请参阅 [v2.0 终结点有何不同之处？](https://docs.microsoft.com/zh-CN/azure/active-directory/develop/active-directory-v2-compare)）


|平台 |Azure AD 终结点 |Azure AD v2.0 终结点 |
|:--- |:--- |:---|
|Android |<a href="https://github.com/microsoftgraph/android-java-connect-sample/tree/last_v1_auth">SDK 示例</a> |<a href="https://github.com/microsoftgraph/android-java-connect-sample">SDK 示例</a>或 <a href="https://github.com/microsoftgraph/android-java-connect-rest-sample">REST 示例</a> |
|AngularJS |<a href="https://github.com/microsoftgraph/angular-connect-rest-sample/tree/last_v1_auth">REST 示例</a> |<a href="https://github.com/microsoftgraph/angular-connect-sample">SDK 示例</a>或 <a href="https://github.com/microsoftgraph/angular-connect-rest-sample">REST 示例</a> |
|ASP.NET |<a href="https://github.com/microsoftgraph/aspnet-connect-rest-sample/tree/last_v1_auth">REST 示例</a> |<a href="https://github.com/microsoftgraph/aspnet-connect-sample">SDK 示例</a>或 <a href="https://github.com/microsoftgraph/aspnet-connect-rest-sample">REST 示例</a> |
|iOS (Obj-C) |<a href="https://github.com/microsoftgraph/ios-objectivec-connect-rest-sample">REST 示例</a> |<a href="https://github.com/microsoftgraph/ios-objectivec-connect-sample">SDK 示例</a> |
|iOS (Swift) |<a href="https://github.com/microsoftgraph/ios-swift-connect-rest-sample">REST 示例</a> |<a href="https://github.com/microsoftgraph/ios-swift-connect-sample">SDK 示例</a> |
|NodeJS |<a href="https://github.com/microsoftgraph/nodejs-connect-rest-sample/tree/last_v1_auth">REST 示例</a> |<a href="https://github.com/microsoftgraph/nodejs-connect-sample">SDK 示例</a>或 <a href="https://github.com/microsoftgraph/nodejs-connect-rest-sample">REST 示例</a> |
|PHP |<a href="https://github.com/microsoftgraph/php-connect-rest-sample/tree/last_v1_auth">REST 示例</a> |<a href="https://github.com/microsoftgraph/php-connect-sample">SDK 示例</a>或 <a href="https://github.com/microsoftgraph/php-connect-rest-sample">REST 示例</a> |
|Python |<a href="https://github.com/microsoftgraph/python-sample-auth/blob/master/sample_adal.py">REST 示例</a> |<a href="https://aka.ms/graph-python-samples">REST 示例</a>
|Ruby |<a href="https://github.com/microsoftgraph/ruby-connect-rest-sample/tree/last_v1_auth">REST 示例</a> |<a href="https://github.com/microsoftgraph/ruby-connect-rest-sample">REST 示例</a> |
|UWP |<a href="https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample/tree/last_v1_auth">REST 示例</a> |<a href="https://github.com/microsoftgraph/uwp-csharp-connect-sample">SDK 示例</a>或 <a href="https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample">REST 示例</a> |
|Xamarin | |<a href="https://github.com/microsoftgraph/xamarin-csharp-connect-sample">SDK 示例</a> |

<br/>

## <a name="see-also"></a>另请参阅

- [在 Graph 浏览器中试调用示例 REST](https://developer.microsoft.com/zh-CN/graph/graph-explorer)
- [Azure AD 终结点文档](https://docs.microsoft.com/zh-CN/azure/active-directory/develop/active-directory-developers-guide)
- [Azure AD v2.0 终结点文档](https://docs.microsoft.com/zh-CN/azure/active-directory/develop/active-directory-appmodel-v2-overview)
