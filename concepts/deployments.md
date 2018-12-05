---
title: 区域云部署
description: 除了全球的数据中心网络外，Microsoft 云服务还可用于三个独立的区域云。 这些区域云版本是 Microsoft 企业云服务的物理和逻辑网络隔离实例，它们仅限于特定国家/地区的地理边界内，由当地人员运营。 若要了解详细信息，请参阅Microsoft 区域云。
ms.openlocfilehash: b0f2ab257773faa14fe59566992bb1ed0dd77959
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091754"
---
# <a name="national-cloud-deployments"></a>区域云部署


除了全球的数据中心网络外，Microsoft 云服务还可用于三个独立的区域云。 这些区域云版本是 Microsoft 企业云服务的物理和逻辑网络隔离实例，它们仅限于特定国家/地区的地理边界内，由当地人员运营。 若要了解详细信息，请参阅[Microsoft 区域云](https://www.microsoft.com/en-us/TrustCenter/CloudServices/NationalCloud)。

当前区域云包括：

- Microsoft Cloud for US Government
- Microsoft 云德国
- 由中国的世纪互联运营的 Azure 和 Office 365

本文提供了有关 Microsoft Graph 的不同区域云部署及每个部署内可供开发人员使用的功能信息。

## <a name="microsoft-graph-and-microsoft-graph-explorer-service-root-endpoints"></a>Microsoft Graph 和 Microsoft Graph 浏览器服务根终结点

下表显示了每个区域云的 Microsoft Graph 和 Microsoft Graph 浏览器的服务根终结点。

| 区域云 | Microsoft Graph | Microsoft Graph 浏览器
|---------------------------|----------------|----------------|
| 由世纪互联运营的 Microsoft Graph 中国 | https://microsoftgraph.chinacloudapi.cn | https://developer.microsoft.com/zh-cn/graph/graph-explorer-china |
| Microsoft Graph 德国 | https://graph.microsoft.de | 不支持。 |
| Microsoft Graph for US Government | https://graph.microsoft.com | 不支持。 |
| Microsoft Graph 全局服务 | https://graph.microsoft.com | https://developer.microsoft.com/graph/graph-explorer |

> **注意**：应用只能通过区域云终结点访问组织数据。 这意味着仅能访问在特定区域云中注册的租户内的数据。 尝试通过 Microsoft Graph 访问与个人 Microsoft 帐户关联的使用者数据的应用应使用全局服务 (https://graph.microsoft.com)。 为区域云部署获取的访问令牌不可与为全局服务获取的访问令牌互换。

## <a name="azure-ad-openid-connect-and-oauth20-endpoints"></a>Azure AD OpenID Connect 和 OAuth2.0 终结点

下表列出了用于为每个区域云获取令牌以调用 Microsoft Graph 的 Azure Active Directory (Azure AD) 终结点的基本 URL。

| 区域云 | Azure AD 根终结点 |
|---------------------------|----------------|
| 由世纪互联运营的 Azure AD 中国 |https://login.chinacloudapi.cn |
| Azure AD 德国 | https://login.microsoftonline.de |
| Azure AD for US Government | https://login.microsoftonline.us |
| Azure AD（全局服务） | https://login.microsoftonline.com |

可以使用相应的区域特定的基本 URL 来生成对 Azure AD 授权或令牌终结点的请求。例如，在德国：

- 授权常见终结点是 https://login.microsoftonline.de/common/oauth2/authorize。
- 令牌常见终结点是 https://login.microsoftonline.de/common/oauth2/token。

可以通过使用租户 ID 或租户的验证域替换上述 URL 中的“common”来生成租户特定的终结点。是使用常用终结点还是租户特定的终结点将取决于应用的要求和用于获取令牌的身份验证流。要了解有关 Azure AD 访问令牌和 Microsoft Graph 的详细信息，请参阅[获取身份验证令牌](./auth-overview.md)。

> **注意：**[Azure AD v2.0 授权和令牌终结点](https://azure.microsoft.com/en-us/documentation/articles/active-directory-appmodel-v2-overview/)仅在全局服务中可用；它们尚不支持用于区域云部署。

## <a name="supported-features"></a>支持的功能

除非另有说明，否则以下 Microsoft Graph 功能通常在所有区域云部署中（在 `/v1.0` 终结点上）可用：

* 用户
* 组
* Excel（在由中国世纪互联运营的 Microsoft Graph 上支持的功能受限。）
* OneDrive（在由中国世纪互联运营的 Microsoft Graph 上支持的功能受限。）
* Outlook 邮件
* Outlook 日历
* 个人联系人 
* SharePoint（在由中国世纪互联运营的 Microsoft Graph 上支持的功能受限。）
* Delta 查询（对每个区域云部署上的不同资源的支持各不相同。）
* Webhook（对每个区域云部署上的不同资源的支持各不相同。）

除非另有说明，否则以下其他 Microsoft Graph 功能在所有区域云部署中（在 `/beta` 终结点上）可用于预览：

* 组织联系人
* 应用程序
* 服务主体

区域云部署尚不支持以下 Microsoft Graph 功能：

* Microsoft Planner
* 目录架构扩展
* 开放类型扩展
