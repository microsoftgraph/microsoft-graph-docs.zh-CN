---
title: 区域云部署
description: 除了全球的数据中心网络外，Microsoft 云服务还可用于三个独立的区域云。
author: arpitha-dhanapathi
ms.openlocfilehash: f4e7a29043a55ddefc5a3f5b7fe5a53911d8ee40
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49754276"
---
# <a name="national-cloud-deployments"></a>区域云部署

除了全球的数据中心网络外，Microsoft 云服务还可用于三个独立的区域云。 这些国家/地区云版本是 Microsoft 企业云服务的物理和逻辑网络隔离实例，它们位于特定国家/地区的地理边界内，由本地人员运营。

当前区域云包括：

* Microsoft Cloud for US Government
* Microsoft 云德国
* 由世纪银行在中国运营的 Azure 和 Microsoft 365

每个国家/地云环境都是唯一的，并且不同于 Microsoft 全球环境。 为国家云环境开发应用程序时，了解其中一些关键差异很重要;例如，注册应用程序、获取令牌和调用 Microsoft Graph API 可能有所不同。

本文提供有关不同 Microsoft Graph 区域云部署以及每个部署中可供开发人员使用的功能的信息。

> **注意：Microsoft** [Graph](./data-connect-concept-overview.md?view=graph-rest-1.0) 数据连接不支持任何区域云部署。

> [!VIDEO https://www.youtube-nocookie.com/embed/R\_3E0IVypRM]

## <a name="app-registration-and-token-service-root-endpoints"></a>应用注册和令牌服务根终结点

在调用 Microsoft Graph API 之前，应首先注册应用程序并获取令牌。 下表列出了 Azure Active Directory (Azure AD) 终结点的基本 URL，用于注册应用程序并获取每个区域云的令牌。

| 国家云 | Azure AD 门户终结点 | Azure AD 终结点 |
| -------------- | ------------------------ | ----------------- |
| Azure AD（全局服务） | https://portal.azure.com | `https://login.microsoftonline.com` |
| Azure AD for US Government | https://portal.azure.us | `https://login.microsoftonline.us` |
| Azure AD 德国 | https://portal.microsoftazure.de | `https://login.microsoftonline.de` |
| 由世纪互联运营的 Azure AD 中国 | https://portal.azure.cn | `https://login.chinacloudapi.cn` |

若要了解有关 Azure AD 访问令牌和 Microsoft Graph 的信息，请参阅 [身份验证基础知识](./auth/auth-concepts.md)。 有关 Azure AD 身份验证方案，请参阅 [Azure AD 身份验证基础知识](/azure/active-directory/develop/authentication-scenarios)。

## <a name="microsoft-graph-and-graph-explorer-service-root-endpoints"></a>Microsoft Graph 和 Graph 浏览器服务根终结点

下表显示了适用于每个区域云的 Microsoft Graph 和 [Graph 资源管理器](https://developer.microsoft.com/graph/graph-explorer) 的服务根终结点。

| 区域云 | Microsoft Graph | Graph 浏览器 |
| -------------- | --------------- | -------------- |
| Microsoft Graph 全局服务 | https://graph.microsoft.com | https://developer.microsoft.com/graph/graph-explorer |
| Microsoft Graph 美国政府版 L4 | https://graph.microsoft.us | 不支持。 |
| Microsoft Graph 美国政府版 L5 (DOD)  | https://dod-graph.microsoft.us | 不支持。 |
| Microsoft Graph 德国 | https://graph.microsoft.de | 不支持。 |
| 由世纪互联运营的 Microsoft Graph 中国 | https://microsoftgraph.chinacloudapi.cn | https://developer.microsoft.com/zh-cn/graph/graph-explorer-china |

> [!IMPORTANT]
> 对于美国政府的应用：
> 
> 
> * 如果你在 Microsoft 365 GCC 环境中工作，请继续使用全球终结点： 和 `https://graph.microsoft.com` `https://portal.azure.com` 。
> * 如果你在 Microsoft 365 GCC High 环境中工作，请使用： `https://portal.azure.us` 和 `https://graph.microsoft.us` 。
> * 如果你在 Microsoft 365 DoD 环境中工作，请使用 `https://portal.azure.us` `https://dod-graph.microsoft.us` 和 。
> 
> 
> 使用全球终结点访问美国政府数据将在近期内禁用。

> [!NOTE]
> 应用只能通过国家云终结点访问组织数据。 这意味着应用只能访问特定国家云中注册的租户数据。 尝试通过 Microsoft Graph 访问与 Microsoft 个人帐户关联的消费者数据的应用应该使用全局服务 `https://graph.microsoft.com` 。 为国家云部署获取的访问令牌不可与为全局服务或任何其他国家云获取的访问令牌互换。

## <a name="supported-features"></a>支持的功能

以下 Microsoft Graph 功能通常在终结点上跨所有国家/地区云部署提供， `/v1.0` 除非有说明。

| Microsoft Graph 功能 | Microsoft Cloud for US Government | 由世纪银行运营的 Microsoft 云中国 | Microsoft 云德国 |
| ------------------------ | --------------------------------- | ------------------------------------------ | ----------------------- |
| 用户 | ✔ | ✔ | ✔ |
| 组 | ✔ | ✔ | ✔ |
| Excel | ✔ | ✔\* | ✔ |
| OneDrive | ✔ | ✔\* | ✔ |
| Outlook 邮件 | ✔ | ✔ | ✔ |
| Outlook 日历 | ✔ | ✔ | ✔ |
| 个人联系人 | ✔ | ✔ | ✔ |
| 安全性 | ✔ | ✔ | ✔ |
| SharePoint | ✔ | ✔ | ✔ |
| Teams | ✔ | ✔ | ✔ |
| Planner | ✔ | ✔ | ✔ |
| 报告 | ➖ | ✔ | ➖ |
| 组织联系人 | ✔ | ➖ | ➖ |
| 应用程序 | ✔ | ➖ | ➖ |
| 服务主体 | ✔ | ➖ | ➖ |
| 更改通知（Webhook） | ✔ | ✔ | ✔\* |
| Delta 查询 | ✔ | ✔ | ➖ |
| 目录架构扩展 | ✔ | ✔ | ➖ |
| 开放类型扩展 | ✔ | ➖ | ➖ |
| 搜索 (Microsoft 搜索)  | ➖ | ➖ | ➖ |
 
以下 Microsoft Graph 功能在 Microsoft 云中国终结点)  (和 `/beta` Microsoft Cloud Germany (V1.0 终结点上的预览版 (中提供，仅在美国政府 Microsoft 云中) ：

* 组织联系人
* 应用程序
* 服务主体

 () \* Exchange 和 OneDrive 服务提供有限支持。 不支持 Azure AD 服务。

> [!IMPORTANT]
> 全局服务的特定区域的某些服务和功能可能无法在所有区域云中提供。 若要了解哪些服务可用，请参阅 [按地区提供的产品](https://azure.microsoft.com/global-infrastructure/services/?products=all&regions=usgov-non-regional,us-dod-central,us-dod-east,usgov-arizona,usgov-iowa,usgov-texas,usgov-virginia,china-non-regional,china-east,china-east-2,china-north,china-north-2,germany-non-regional,germany-central,germany-northeast)。

若要了解有关国家云的信息，请参阅下列主题：

* [Microsoft 国家云](https://www.microsoft.com/TrustCenter/CloudServices/NationalCloud)
* [Microsoft 365 美国政府版](/office365/servicedescriptions/office-365-platform-service-description/office-365-us-government/office-365-us-government)
* [由世纪银行运营的 Microsoft 365](/office365/servicedescriptions/office-365-platform-service-description/office-365-operated-by-21vianet)
* [Office 365 德国版](/office365/servicedescriptions/office-365-platform-service-description/office-365-germany)
* [Azure 政府](https://azure.microsoft.com/global-infrastructure/government/)
* [Azure China 21Vianet](/azure/china/)
* [Azure Germany](/azure/germany/)