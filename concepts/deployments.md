---
title: 区域云部署
description: 除了全球的数据中心网络外，Microsoft 云服务还可用于三个独立的区域云。 这些国家/地区云版本是物理和逻辑网络隔离限制在特定国家/地区的地理边框和由本地人员的 Microsoft 企业云服务的实例。
ms.openlocfilehash: a5f5c5d0ae8611957cb9087de53f5ddd87d1f25d
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571294"
---
# <a name="national-cloud-deployments"></a>区域云部署

除了全球的数据中心网络外，Microsoft 云服务还可用于三个独立的区域云。 这些国家/地区云版本是物理和逻辑网络隔离限制在特定国家/地区的地理边框和由本地人员的 Microsoft 企业云服务的实例。

当前区域云包括：

- Microsoft Cloud for US Government
- Microsoft 云德国
- 由中国的世纪互联运营的 Azure 和 Office 365

每个国家/地区云环境是唯一和 Microsoft 全局环境以外的其他。 非常重要开发应用程序的国家/地区云环境; 时要注意的一些这些主要差异例如，注册应用程序，获取令牌，并调用 Microsoft Graph API 可以不同。

本文提供了有关不同的 Microsoft Graph 国家/地区云部署和内每个开发人员提供的功能的信息。

## <a name="app-registration-and-token-service-root-endpoints"></a>应用程序注册和令牌服务根终结点

调用之前 Microsoft Graph Api，应首先注册您的应用程序，并获取令牌。 下表列出要注册您的应用程序和获取的每个国家/地区云标记的 Azure Active Directory (Azure AD) 终结点的基 Url。

| 国家/地区云 | Azure AD 门户终结点| Azure AD 终结点|
|---------------------------|----------------|----------------|
|Azure AD for US Government |https://portal.azure.us|`https://login.microsoftonline.us`|
|Azure AD 德国 |https://portal.microsoftazure.de|`https://login.microsoftonline.de`|
|由世纪互联运营的 Azure AD 中国 |https://portal.azure.cn|`https://login.chinacloudapi.cn`|
|Azure AD（全局服务）|https://portal.azure.com |`https://login.microsoftonline.com`|

若要了解有关 Azure AD 的详细信息访问令牌和 Microsoft Graph，请参阅[获取身份验证令牌](./auth-overview.md)。 Azure AD 身份验证方案，请参阅[Azure AD 身份验证基础知识](https://docs.microsoft.com/azure/active-directory/develop/authentication-scenarios)。

> **注意：**[Azure AD v2.0 授权和令牌终结点](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)仅在全局服务中可用；它们尚不支持用于区域云部署。


## <a name="microsoft-graph-and-graph-explorer-service-root-endpoints"></a>Microsoft Graph 和图资源管理器服务根终结点

下表显示为每个国家/地区云 Microsoft Graph 和[图资源管理器](https://developer.microsoft.com/graph/graph-explorer)服务根终结点。

| 区域云 | Microsoft Graph | Graph 浏览器 |
|---------------------------|----------------|----------------|
| Microsoft Graph for US Government | https://graph.microsoft.us | 不支持。 |
| Microsoft Graph 德国 | https://graph.microsoft.de | 不支持。 |
| 由世纪互联运营的 Microsoft Graph 中国 | https://microsoftgraph.chinacloudapi.cn | https://developer.microsoft.com/zh-cn/graph/graph-explorer-china |
| Microsoft Graph 全局服务 | https://graph.microsoft.com | https://developer.microsoft.com/graph/graph-explorer |

> **注意**：应用只能通过区域云终结点访问组织数据。 这意味着，应用程序只能访问中的特定国家/地区云中注册的租户数据。 尝试访问通过 Microsoft Graph 个人 Microsoft 帐户相关联的客户数据的应用程序应使用全球服务`https://graph.microsoft.com`。 国家/地区的云部署获取访问令牌不与购置全球服务或任何其他国家/地区云互换。

## <a name="supported-features"></a>支持的功能

以下 Microsoft Graph 功能位于通常`/v1.0`跨所有国家/地区云部署，除非另有说明的终结点。

| Microsoft Graph 功能 | Microsoft Cloud for US Government | Microsoft 云中国由 21Vianet | Microsoft 云德国 |
|---------------------------|----------------|----------------|----------------|
| 用户 | ✔ | ✔ | ✔ |
| 组 | ✔ | ✔ | ✔ |
| Excel | ✔| ✔* | ✔ |
| OneDrive | ✔ | ✔* | ✔ |
| Outlook 邮件 | ✔ | ✔ | ✔ |
| Outlook 日历 | ✔ | ✔ | ✔ |
| 个人联系人 | ✔ | ✔ | ✔ |
| SharePoint| ✔ | ✔* | ✔ |
| Delta 查询 | ✔ | ✔ | ✔ |
| Webhook  | ✔ | ✔ | ✔ |
| 报表  |➖| ✔ |➖|
| Microsoft Planner|➖|➖|➖|
|目录架构扩展 |➖|➖|➖|
| 开放类型扩展|➖|➖|➖|
  
下面的其他 Microsoft Graph 功能均可用，在预览 (在`/beta`终结点) 跨所有国家/地区云部署，除非另有说明：

* 组织联系人
* 应用程序
* 服务主体

(*)此云中此 API 支持有限。

 > **重要说明：** 特定服务和特定区域的全球服务中的功能可能不可用中所有的国家/地区云。 以找出哪些服务是可用，请参阅[区域中的产品](https://azure.microsoft.com/global-infrastructure/services/?products=all&regions=usgov-non-regional,us-dod-central,us-dod-east,usgov-arizona,usgov-iowa,usgov-texas,usgov-virginia,china-non-regional,china-east,china-east-2,china-north,china-north-2,germany-non-regional,germany-central,germany-northeast)。


若要了解有关国家/地区云的详细信息，请参阅以下主题：
- [Microsoft National 云](https://www.microsoft.com/TrustCenter/CloudServices/NationalCloud)
- [Office 365 政府版美国](https://docs.microsoft.com/office365/servicedescriptions/office-365-platform-service-description/office-365-us-government/office-365-us-government)
- [Office 365 由 21Vianet](https://docs.microsoft.com/office365/servicedescriptions/office-365-platform-service-description/office-365-operated-by-21vianet)
- [Office 365 Germany](https://docs.microsoft.com/office365/servicedescriptions/office-365-platform-service-description/office-365-germany)
- [Azure 政府](https://azure.microsoft.com/global-infrastructure/government/)
- [Azure 中国 21Vianet](https://docs.microsoft.com/azure/china/)
- [Azure 德国](https://docs.microsoft.com/azure/germany/)
