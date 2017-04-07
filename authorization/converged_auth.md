# <a name="authenticate-microsoft-graph-apps-with-the-azure-ad-v20-endpoint"></a>使用 Azure AD v2.0 终结点对 Microsoft Graph 应用进行身份验证

> **为企业客户生成应用？**如果企业客户启用企业移动性安全功能，如<a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">条件性设备访问</a>，应用可能无法运行。  

> 若要在**所有企业场景**中支持**所有企业客户**，必须使用 Azure AD 终结点并使用 [Azure 管理门户](https://aka.ms/aadapplist) 管理应用。有关详细信息，请参阅 [在 Azure AD 和 Azure AD v2.0 终结点之间做选择](auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints)。


通过使用 Azure AD v2.0 终结点，可以创建接受工作、学校 (Azure Active Directory) 以及个人（Microsoft 帐户）身份的应用。

过去，如果想开发支持 Microsoft 帐户和 Azure Active Directory 两者的应用，则必须集成两个完全独立的系统。借助 Azure AD v2.0 终结点，现在则可以通过单一集成同时支持这两种帐户类型 - 这种集成是一个简单的过程，可将受众范围扩展到同时具有个人和工作/学校帐户的数百万用户。  

使用 Azure AD v2.0 终结点集成应用后，应用可以立即访问可用于个人和工作或学校帐户的 Microsoft Graph 终结点，例如： 

| 数据              | 终结点                                       |
|:------------------|:-----------------------------------------------|
| 用户配置文件      | `https://graph.microsoft.com/v1.0/me`          |
| Outlook 邮件      | `https://graph.microsoft.com/v1.0/me/messages` |
| Outlook 联系人  | `https://graph.microsoft.com/v1.0/me/contacts` |
| Outlook 日历 | `https://graph.microsoft.com/v1.0/me/events`   |
| OneDrive          | `https://graph.microsoft.com/v1.0/me/drive`    |

 >**注意：**某些 Microsoft Graph 终结点（如组和任务）不适用于个人帐户。  

## <a name="microsoft-graph-authentication-scopes"></a>Microsoft Graph 身份验证范围

Azure AD v2.0 终结点支持 [Microsoft Graph 权限范围](permission_scopes.md) 中列出的所有权限范围。 

若要详细了解 Azure AD v2.0 终结点的使用范围，以及其与 Azure AD 中的使用资源有何不同，请参阅<a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-compare/#scopes-not-resources" target="_newtab">范围，而非资源</a>。

## <a name="see-it-in-action"></a>查看实际操作

[Microsoft Graph 存储库中的 Connect 示例](https://github.com/microsoftgraph?utf8=%E2%9C%93&query=connect) 提供了如何对用户进行身份验证并跨多种平台连接到 Microsoft Graph 的简单示例。

此外，[入门](http://developer.microsoft.com/en-us/graph/docs/platform/get-started) 部分包括介绍如何创建这些示例应用（包含用于各个平台的身份验证库）的文章。

## <a name="see-also"></a>另请参阅

- [使用 Azure AD v2.0 终结点注册应用](auth_register_app_v2.md)
- [Microsoft Graph 的应用身份验证](auth_overview.md)
- <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-compare" target="_newtab">Azure AD v2.0 模型的新增功能</a>
- <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-limitations/" target="_newtab">是否应使用 Azure AD v2.0 终结点？</a>
- <a href="https://azure.microsoft.com/en-us/documentation/articles/?product=active-directory&term=azure+ad+v2.0" target="_newtab">Azure.com 上的 Azure AD v2.0 终结点文档</a>
- <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-app-registration/#build-a-quick-start-app" target="_newtab">Azure.com 上的 Azure AD v2.0 代码快速入门</a>

