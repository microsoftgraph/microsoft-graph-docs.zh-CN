# <a name="working-with-intune-in-microsoft-graph"></a>在 Microsoft Graph 中使用 Intune  

> **注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://www.microsoft.com/zh-CN/cloud-platform/microsoft-intune-pricing) Intune 服务。

适用于 Intune 的 Microsoft Graph API 允许以编程方式访问租户的 Intune 信息；API 会执行与可通过 **Azure 门户**执行的相同 Intune 操作。  

对于移动设备管理 (MDM) 场景，适用于 Intune 的 Graph API 支持独立部署；不支持 Intune [混合部署](https://docs.microsoft.com/zh-CN/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management)。 

## <a name="using-the-intune-graph-api"></a>使用 Intune Graph API

Intune 向 Microsoft Graph API 提供数据的方式与其他云服务相同，具有丰富的实体信息和关系导航。  使用 Microsoft Graph API 将来自其他服务和 Intune 的信息进行组合，为 IT 专业人员和最终用户构建丰富的跨服务应用程序。     

以下是如何能够确定是否在用户的设备上安装了应用程序的方法示例： 

1. 从 Azure Active Directory 获取注册到用户的设备列表： 

    https://graph.microsoft.com/users/{user}/ownedDevices 

2. 然后，查看租户的应用程序列表： 

    https://graph.microsoft.com/deviceAppManagement/mobileApps  

3. 从应用程序中获取 ID，并确定应用程序（以及用户）的安装状态：

    https://graph.microsoft.com/deviceAppManagement/mobileApps/{id}/deviceStatuses/


## <a name="using-permission-scopes"></a>使用权限范围

Microsoft Graph API 可以使用权限范围控制对资源的访问。 作为开发者，你必须指定访问 Intune 资源需要的权限范围。 通常情况下，可以在 Azure Active Directory 门户中指定需要的权限范围。 有关详细信息，请参阅 [Microsoft Graph 权限范围](https://developer.microsoft.com/zh-CN/graph/docs/authorization/permission_scopes)和 [Intune 权限范围](https://developer.microsoft.com/zh-CN/graph/docs/authorization/permission_scopes#permission-scopes-in-preview)。

