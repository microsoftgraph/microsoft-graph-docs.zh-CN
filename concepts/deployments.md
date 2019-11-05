---
title: 区域云部署
description: 除了全球的数据中心网络外，Microsoft 云服务还可用于三个独立的区域云。 这些国家/地区云版本是物理和逻辑网络隔离的 Microsoft 企业云服务实例，这些实例限制在特定国家/地区的地理边界内，并由当地人员运营。
ms.openlocfilehash: 4da5570719cf64ba8fc329039e4ba4fcef7348b5
ms.sourcegitcommit: b1e1f614299f668453916bd85761ef7b6c8d6eff
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37969841"
---
# <a name="national-cloud-deployments"></a>区域云部署

除了全球的数据中心网络外，Microsoft 云服务还可用于三个独立的区域云。 这些国家/地区云版本是物理和逻辑网络隔离的 Microsoft 企业云服务实例，这些实例限制在特定国家/地区的地理边界内，并由当地人员运营。

当前区域云包括：

- Microsoft Cloud for US Government
- Microsoft 云德国
- 由中国的世纪互联运营的 Azure 和 Office 365

每个国家/地区云环境都是唯一的，与 Microsoft 全局环境不同。 在开发适用于国家/地区云环境的应用程序时，请务必注意其中的一些关键区别;例如，注册应用程序、获取令牌和调用 Microsoft Graph API 可能会有所不同。

本文提供了有关不同 Microsoft Graph 国家云部署的信息，以及每个区域中的开发人员可用的功能。

>**注意：** [Microsoft Graph 数据连接](https://docs.microsoft.com/graph/data-connect-concept-overview?view=graph-rest-1.0)不支持任何国家云部署。 

> [!VIDEO https://www.youtube-nocookie.com/embed/R_3E0IVypRM]

## <a name="app-registration-and-token-service-root-endpoints"></a>应用注册和令牌服务根终结点

在调用 Microsoft Graph Api 之前，应先注册您的应用程序并获取一个令牌。 下表列出了 Azure Active Directory （Azure AD）终结点的基 Url，这些终结点用于注册应用程序并获取每个国家/地区云的令牌。

| 国家云 | Azure AD 门户终结点| Azure AD 终结点|
|---------------------------|----------------|----------------|
|Azure AD for US Government |https://portal.azure.us|`https://login.microsoftonline.us`|
|Azure AD 德国 |https://portal.microsoftazure.de|`https://login.microsoftonline.de`|
|由世纪互联运营的 Azure AD 中国 |https://portal.azure.cn|`https://login.chinacloudapi.cn`|
|Azure AD（全局服务）|https://portal.azure.com |`https://login.microsoftonline.com`|

若要了解有关 Azure AD 访问令牌和 Microsoft Graph 的详细信息，请参阅[身份验证基础](./auth/auth-concepts.md)。 对于 Azure AD 身份验证方案，请参阅[AZURE ad 身份验证基础](https://docs.microsoft.com/azure/active-directory/develop/authentication-scenarios)。


## <a name="microsoft-graph-and-graph-explorer-service-root-endpoints"></a>Microsoft Graph 和 Graph 浏览器服务根终结点

下表显示了每个国家/地区群的 Microsoft Graph 和[Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)的服务根终结点。

| 区域云 | Microsoft Graph | Graph 浏览器 |
|---------------------------|----------------|----------------|
| 适用于美国政府 L4 的 Microsoft Graph | https://graph.microsoft.us | 不支持。 |
| Microsoft Graph for 美国政府版 L5 （DOD） | https://dod-graph.microsoft.us | 不支持。 |
| Microsoft Graph 德国 | https://graph.microsoft.de | 不支持。 |
| 由世纪互联运营的 Microsoft Graph 中国 | https://microsoftgraph.chinacloudapi.cn | https://developer.microsoft.com/zh-cn/graph/graph-explorer-china |
| Microsoft Graph 全局服务 | https://graph.microsoft.com | https://developer.microsoft.com/graph/graph-explorer |

>**重要说明：** 如果你已在美国政府版中使用了一个应用程序，并且你`https://graph.microsoft.com`使用的是全球终结点， `https://graph.microsoft.us`我们建议切换到新终结点。 使用全球终结点访问美国政府数据当前可以正常运行，但在不久的将来将被禁用。

> **注意**：应用只能通过区域云终结点访问组织数据。 这意味着应用只能访问在特定国家云中注册的租户中的数据。 尝试通过 Microsoft Graph 访问与 Microsoft 个人帐户关联的用户数据的应用程序应使用全局服务`https://graph.microsoft.com`。 为国家云部署获取的访问令牌与为全局服务或任何其他国家云获取的访问令牌不可互换。

## <a name="supported-features"></a>支持的功能

以下 Microsoft Graph 功能在`/v1.0`终结点上通常在所有国家/地区云部署上可用，除非另有说明。

| Microsoft Graph 功能 | Microsoft Cloud for US Government | 由世纪互联运营的 Microsoft 云中国 | Microsoft 云德国 |
|---------------------------|----------------|----------------|----------------|
| 用户 | ✔ | ✔ | ✔ |
| 组 | ✔ | ✔ | ✔ |
| Excel | ✔| ✔* | ✔ |
| OneDrive | ✔ | ✔* | ✔ |
| Outlook 邮件 | ✔ | ✔ | ✔ |
| Outlook 日历 | ✔ | ✔ | ✔ |
| 个人联系人 | ✔ | ✔ | ✔ |
| SharePoint| ✔ | ✔ | ✔ |
| Planner|✔ |✔ |✔ |
| 报表  |➖| ✔ |➖|
| 更改通知（Webhook）  | ➖|✔* |✔* |
| Delta 查询 | ➖ | ➖| ➖ |
| 目录架构扩展 |➖|➖|➖|
| 开放类型扩展|➖|➖|➖|
  
以下其他 Microsoft Graph 功能在所有国家/地区云部署的`/beta`预览（在终结点上）中可用，但在另有说明的情况除外：

* 组织联系人
* 应用程序
* 服务主体
* 更改通知（Webhook）

(*)仅对 Exchange 和 OneDrive 服务的有限支持。 Azure AD services 不受支持。 

 > **重要说明：** 全局服务特定区域中的某些服务和功能在所有国家/地区群中可能不可用。 若要了解哪些服务可用，请参阅[地区提供的产品](https://azure.microsoft.com/global-infrastructure/services/?products=all&regions=usgov-non-regional,us-dod-central,us-dod-east,usgov-arizona,usgov-iowa,usgov-texas,usgov-virginia,china-non-regional,china-east,china-east-2,china-north,china-north-2,germany-non-regional,germany-central,germany-northeast)。


若要了解有关国家/地区云的详细信息，请参阅下列主题：
- [Microsoft 国家/地区群](https://www.microsoft.com/TrustCenter/CloudServices/NationalCloud)
- [适用于美国政府的 Office 365](https://docs.microsoft.com/office365/servicedescriptions/office-365-platform-service-description/office-365-us-government/office-365-us-government)
- [由世纪互联运营的 Office 365](https://docs.microsoft.com/office365/servicedescriptions/office-365-platform-service-description/office-365-operated-by-21vianet)
- [Office 365 德国版](https://docs.microsoft.com/office365/servicedescriptions/office-365-platform-service-description/office-365-germany)
- [Azure 政府](https://azure.microsoft.com/global-infrastructure/government/)
- [Azure 中国世纪互联](https://docs.microsoft.com/azure/china/)
- [Azure 德国](https://docs.microsoft.com/azure/germany/)
