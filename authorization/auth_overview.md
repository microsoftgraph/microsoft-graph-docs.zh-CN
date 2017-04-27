# <a name="app-authentication-with-microsoft-graph"></a>Microsoft Graph 的应用身份验证

若要访问用户的 Microsoft 数据，应用程序必须允许用户验证他们的身份并使用户同意应用代表他们执行操作。

Microsoft Graph 支持两种身份验证提供程序：

- 若要对使用 Microsoft 个人帐户的用户进行身份验证，如 _live.com_ 或 _outlook.com_ 帐户等，请使用 [Azure Active Directory (Azure AD) v2.0 终结点](converged_auth.md)。
- 若要对使用企业（即工作或学校）帐户的用户进行身份验证，请使用 [Azure AD](app_authorization.md)。


> **为企业客户生成应用？**如果企业客户启用企业移动性安全功能，如<a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">条件性设备访问</a>，应用可能无法运行。  

> 若要在**所有企业场景**中支持**所有企业客户**，必须使用 Azure AD 终结点并使用 [Azure 管理门户](https://aka.ms/aadapplist) 管理应用。

![Microsoft Graph 应用程序堆栈将身份验证显示为应用和各种 Microsoft Graph 资源之间的一个层。](./images/MSGraph_DevStack_v2Auth.png)

## <a name="deciding-between-the-azure-ad-and-azure-ad-v20-endpoints"></a>在 Azure AD 和 Azure AD v2.0 终结点之间做选择

下表总结了 Azure AD 和 Azure AD v2.0 终结点支持的主要功能，并提供了指向额外信息的链接。这些功能的相对重要性以及因而在应用中选择实施哪种身份验证提供程序主要取决于以下内容：

- 应用需要支持的帐户类型（企业或客户）
- 要生成的应用类型
- 所需的身份验证流 

<table style="width:100%">
  <tr>
    <th></th>
    <th>Azure AD 终结点</th> 
    <th>Azure AD v2.0 终结点</th>
   </tr>
  <tr>
    <td>支持的授权类型</td>
    <td style="vertical-align: text-top;"><p>授权代码</p><p>隐式</p><p>客户端凭据</p><p>资源所有者密码凭据</p></td> 
    <td style="vertical-align: text-top;"><p>授权代码</p><p>隐式</p><p>客户端凭据</p></td>
   </tr>
  <tr>
    <td>支持的应用类型</td>
    <td style="vertical-align: text-top;"><p>Web 应用</p><p>Web API</p><p>移动和本机应用</p><p>单页应用 (SPA)</p><p>独立 Web API</p><p>守护程序/服务器端应用</p><p>云解决方案提供商应用</p><p><a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-authentication-scenarios/" target="_newtab">详细信息</a></p></td> 
    <td style="vertical-align: text-top;"><p>Web 应用</p><p>Web API</p><p>移动和本机应用</p><p>单页应用 (SPA)</p><p>守护程序/服务器端应用</p><p><a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-flows/" target="_newtab">详细信息</a></td>
   </tr>
  <tr>
    <td>条件访问设备策略</td>
     <td><a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">支持</a></td> 
    <td>目前尚不支持</td>
   </tr>
  <tr>
    <td>兼容 OAuth 2.0 和 OpenID Connect</td>
    <td>否</td> 
    <td>是</td>
  </tr>
  <tr>
    <td>权限</td>
    <td>静态：应用注册期间已指定 </td> 
    <td><a href ="https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-compare/#scopes-not-resources" target="_newtab">动态：</a>应用运行时期间请求；包括增量许可</td>
  </tr>
  <tr>
    <td>帐户类型</td>
    <td> <p>工作或学校</p></td> 
    <td><p>工作或学校</p><p>个人</p> </td>
  </tr>
  <tr>
    <td>应用程序 ID </td>
    <td>各个平台的单独应用程序 ID</td> 
    <td><a href ="https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-compare/#one-app-id-for-all-platforms" target="_newtab">多个平台的单个应用程序 ID</a></td>
  </tr>
  <tr>
    <td>注册门户 </td>
    <td><a href ="https://manage.windowsazure.com/" target="_newtab">Microsoft Azure 管理</a></td> 
    <td><a href ="https://apps.dev.microsoft.com" target="_newtab">Microsoft 应用程序注册</a></td>
  </tr>
  <tr>
    <td>客户端库 </td>
    <td>适用于大多数开发平台的 Active Directory 身份验证 (ADAL) SDK</td> 
    <td><p><a href="https://www.nuget.org/packages/Microsoft.Identity.Client" target="_newtab">Microsoft 身份验证库（预览）</a></p><p><a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-limitations/#restrictions-on-libraries-amp-sdks" target="_newtab">开放源代码 OAuth 2.0 库（列表）</a></p> </td>
  </tr>
  <tr>
    <td>其他功能 </td>
    <td><p>Azure AD 用户的组声明</p><p>应用程序角色和角色声明</p></td> 
    <td></td>
  </tr>
</table> 

此外，两种身份验证提供程序所需的权限范围及各种令牌中返回的声明均存在差异。有关详细详细，请参阅 [v2.0 终结点有何不同？](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-compare/) 中的 [已知范围](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-compare/#well-known-scopes) 和 [令牌声明](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-compare/#token-claims)。

此外，Azure AD v2.0 终结点处于积极开发过程中，未来会添加其他功能和支持场景。有关 Azure AD v2.0 终结点的限制和约束的最新列表，请参阅 [是否应使用 v2.0 终结点？](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-limitations/)。

## <a name="registering-your-app-for-authentication"></a>注册应用进行身份验证 

在确定符合应用要求的身份验证提供程序后，需要在该身份验证提供程序的门户注册此应用。注册应用可以使用该身份验证提供程序创建应用的身份，并且允许应用在提交来自用户的身份验证请求时指定自身身份。

- 若要使用 Azure AD 注册应用，请使用 [Azure 门户](https://portal.azure.com/)。

    <!--For Azure AD, you'll also need to associate your Office 365 account with Azure AD subscription in order to manage your apps.-->

- 若要 [使用 Azure AD v2.0 终结点注册应用](auth_register_app_v2.md)，请使用 [Microsoft 应用程序注册门户](https://apps.dev.microsoft.com)。


## <a name="resources-for-implementing-authentication-in-your-microsoft-graph-app"></a>在 Microsoft Graph 应用中实施身份验证的资源 

使用相应的身份验证门户注册应用并具备创建应用身份所需的应用注册信息（应用程序 ID、应用机密，适用情况下则还有重定向 URL）后，则在应用中实施身份验证已准备就绪。 

同样，根据要生成的应用类型、开发平台、选择的身份验证流和应用的任何特定身份验证要求的不同，这也会有所不同。 

### <a name="connect-samples-by-authentication-provider-and-platform"></a>身份验证提供程序和平台的连接示例

下表列出了身份验证提供程序和平台的 Connect 示例，并标注其是否使用 REST 或 Microsoft Graph 客户端库连接到 Microsoft Graph。

<table>
  <tr>
    <th>平台</th>
    <th>Azure AD 终结点</th> 
    <th>Azure AD v2.0 终结点</th>
  </tr>
  <tr>
    <td>Android</td>
    <td>
        <a href="https://github.com/microsoftgraph/android-java-connect-rest-sample">REST 示例</a>或 <a href="https://github.com/microsoftgraph/android-java-connect-sample/tree/last_v1_auth">SDK 示例</a>
    </td> 
    <td>
        <a href="https://github.com/microsoftgraph/android-java-connect-sample">SDK 示例</a>
    </td> 
  </tr>
  <tr>
    <td>ASP.NET</td>
    <td>
        <a href="https://github.com/microsoftgraph/aspnet-connect-rest-sample">REST 示例</a>
    </td>     
    <td>
        <a href="https://github.com/microsoftgraph/aspnet-connect-sample">SDK 示例</a>
    </td> 
  </tr>
  <tr>
    <td>iOS (Obj-C)</td>
    <td>
        <a href="https://github.com/microsoftgraph/ios-objectivec-connect-rest-sample">REST 示例</a>
    </td>     
    <td>
        <a href="https://github.com/microsoftgraph/ios-objectivec-connect-sample">SDK 示例</a>
    </td> 
  </tr>
  <tr>
    <td>iOS (Swift)</td>
    <td>
        <a href="https://github.com/microsoftgraph/ios-swift-connect-rest-sample">REST 示例</a>
    </td>     
    <td>
        <a href="https://github.com/microsoftgraph/ios-swift-connect-sample">SDK 示例</a>
    </td> 
  </tr>
  <tr>
    <td>Node.js</td>
    <td>
        <a href="https://github.com/microsoftgraph/nodejs-connect-rest-sample/tree/last_v1_auth">REST 示例</a>
    </td>     
    <td>
        <a href="https://github.com/microsoftgraph/nodejs-connect-rest-sample">REST 示例</a>
    </td> 
  </tr>
  <tr>
    <td>PHP</td>
    <td>
        <a href="https://github.com/microsoftgraph/php-connect-rest-sample/tree/last_v1_auth">REST 示例</a>
    </td>     
    <td>
        <a href="https://github.com/microsoftgraph/php-connect-rest-sample">REST 示例</a>
    </td> 
  </tr>
  <tr>
    <td>Python</td>
    <td>
        <a href="https://github.com/microsoftgraph/python3-connect-rest-sample">REST 示例</a>
    </td>     
    <td>
    </td> 
  </tr>
  <tr>
    <td>Ruby</td>
    <td>
        <a href="https://github.com/microsoftgraph/ruby-connect-rest-sample/tree/last_v1_auth">REST 示例</a>
    </td>     
    <td>
        <a href="https://github.com/microsoftgraph/ruby-connect-rest-sample">REST 示例</a>
    </td> 
  </tr>
  <tr>
    <td>UWP</td>
    <td>
        <a href="https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample/tree/last_v1_auth">REST 示例</a>
    </td>     
    <td>
        <a href="https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample">REST 示例</a>或 <a href="https://github.com/microsoftgraph/uwp-csharp-connect-sample">SDK 示例</a>
    </td> 
  </tr>
  <tr>
    <td>Xamarin</td>
    <td>
    </td>     
    <td>
        <a href="https://github.com/microsoftgraph/xamarin-csharp-connect-sample">SDK 示例</a>
    </td> 
  </tr>
</table>

若要浏览通过各种技术连接到 Microsoft Graph 的多个项目，请访问 GitHub 上的 [Microsoft Graph 存储库](https://github.com/microsoftgraph)。 

### <a name="get-started"></a>入门  


  [入门](http://developer.microsoft.com/en-us/graph/docs/platform/get-started) 部分包含详细的文章，为你演示如何使用 Azure AD v2.0 终结点创建表中列出的应用，并包括在各个平台上所使用的身份验证库。 

## <a name="see-also"></a>另请参阅

- <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-authentication-scenarios/#basics-of-authentication-in-azure-ad" target="_newtab">Azure AD 的身份验证场景</a>
- <a href="https://azure.microsoft.com/en-us/documentation/articles/?product=active-directory&term=v2.0+endpoint" target="_newtab">Azure.com 上的 Azure AD v2.0 终结点文档</a>
- <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-app-registration/#build-a-quick-start-app" target="_newtab">Azure.com 上的 Azure AD v2.0 代码快速入门</a>
