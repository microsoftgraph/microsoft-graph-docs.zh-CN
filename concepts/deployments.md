---
title: 区域云部署
description: 除了全球的数据中心网络外，Microsoft 云服务还可用于三个独立的区域云。
author: arpitha-dhanapathi
ms.localizationpriority: medium
ms.openlocfilehash: a6c3ecbcb5cbb48d76c678c2496349e562721b8d
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61226902"
---
# <a name="national-cloud-deployments"></a>区域云部署

除了全球的数据中心网络外，Microsoft 云服务还可用于三个独立的区域云。 这些国家/地区云版本是 Microsoft 企业云服务的物理和逻辑网络隔离实例，它们限制在特定国家/地区的地理边界内，由本地人员运营。

当前区域云包括：

* Microsoft Cloud for US Government
* Microsoft 云德国
* Azure 由世纪互联运营的 Microsoft 365中国

每个国家/地云环境都是唯一的，并且不同于 Microsoft 全球环境。 为国家云环境开发应用程序时，了解其中一些关键差异非常重要;例如，注册应用程序、获取令牌和调用 Microsoft Graph API 可能有所不同。

本文提供有关不同 Microsoft Graph国家云部署的信息，以及每个部署中可供开发人员使用的功能。

> **注意**[Microsoft Graph 数据连接](./data-connect-concept-overview.md)不支持任何国家云部署。

> [!VIDEO https://www.youtube-nocookie.com/embed/R\_3E0IVypRM]

## <a name="app-registration-and-token-service-root-endpoints"></a>应用注册和令牌服务根终结点

在调用 Microsoft Graph API 之前，应首先注册应用程序并获取令牌。 下表列出了用于注册应用程序并获取每个区域云Azure Active Directory (Azure AD) 终结点的基本 URL。

| 国家云 | Azure AD门户终结点 | Azure AD 终结点 |
| -------------- | ------------------------ | ----------------- |
| Azure AD（全局服务） | https://portal.azure.com | `https://login.microsoftonline.com` |
| Azure AD for US Government | https://portal.azure.us | `https://login.microsoftonline.us` |
| Azure AD 德国 | https://portal.microsoftazure.de | `https://login.microsoftonline.de` |
| 由世纪互联运营的 Azure AD 中国 | https://portal.azure.cn | `https://login.chinacloudapi.cn` |

若要了解有关访问Azure AD和 Microsoft Graph，请参阅身份验证[基础知识](./auth/auth-concepts.md)。 有关Azure AD方案，请参阅Azure AD[基本身份验证。](/azure/active-directory/develop/authentication-scenarios)

## <a name="microsoft-graph-and-graph-explorer-service-root-endpoints"></a>Microsoft Graph 和 Graph Explorer 服务根终结点

下表显示了每个区域云的 Microsoft Graph 和 Graph [Explorer](https://developer.microsoft.com/graph/graph-explorer)的服务根终结点。

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
> * 如果你正在一个Microsoft 365 GCC环境中工作，请继续使用全球终结点： `https://graph.microsoft.com` 和 `https://portal.azure.com` 。
> * 如果你在高Microsoft 365 GCC工作，请使用： `https://portal.azure.us` 和 `https://graph.microsoft.us` 。
> * 如果你在 DoD 环境中Microsoft 365，请使用 `https://portal.azure.us` `https://dod-graph.microsoft.us` 和 。
>
>
> 使用全球终结点访问美国政府数据将将于近期内禁用。

> [!NOTE]
> 应用仅能通过国家云终结点访问组织数据。 这意味着应用只能访问特定区域云中注册的租户数据。 尝试通过 Microsoft 帐户访问与 Microsoft 个人帐户关联的消费者数据Graph应该使用全局服务 `https://graph.microsoft.com` 。 为国家云部署获取的访问令牌不可与为全局服务或其他任何国家云获取的访问令牌互换。

## <a name="supported-features"></a>支持的功能

以下 Microsoft Graph功能通常在终结点上跨所有区域云部署提供 `/v1.0` ，除非已指出。

| Microsoft Graph 功能 | Microsoft Cloud for US Government | 由世纪银行运营的 Microsoft 云中国 | Microsoft 云德国 |
| ------------------------ | --------------------------------- | ------------------------------------------ | ----------------------- |
| 应用程序 | ✔ | ➖ | ➖ |
| 更改通知（Webhook） | ✔ | ✔ | ✔\* |
| Delta 查询 | ✔ | ✔ | ➖ |
| 目录架构扩展 | ✔ | ✔ | ➖ |
| Excel | ✔ | ➖ | ✔ |
| 组 | ✔ | ✔ | ✔ |
| OneDrive | ✔ | ✔\* | ✔ |
| 开放类型扩展 | ✔ | ➖ | ➖ |
| 组织联系人 | ✔ | ➖ | ➖ |
| Outlook 日历 | ✔ | ✔ | ✔ |
| Outlook 邮件 | ✔ | ✔ | ✔ |
| 个人联系人 | ✔ | ✔ | ✔ |
| Planner | ✔ | ✔ | ✔ |
| 报表 | ➖ | ✔ | ➖ |
| 搜索 (Microsoft 搜索)  | ➖ | ➖ | ➖ |
| 安全性 | ✔ | ✔ | ✔ |
| 服务运行状况和通信 | ✔ | ✔ | ✔ |
| 服务主体 | ✔ | ➖ | ➖ |
| SharePoint | ✔ | ✔ | ✔ |
| Teams | ✔ | ✔ | ✔ |
| 用户 | ✔ | ✔ | ✔ |

以下 Microsoft Graph 功能在 Microsoft Cloud China 和 `/beta` Microsoft Cloud Germany (V1.0 终结点上的) 终结点上的预览版 (中提供，这些功能仅在 Microsoft Cloud for US Government) ：

* 组织联系人
* 应用程序
* 服务主体

\* () 仅对 Exchange 和 OneDrive 服务提供有限支持。 Azure AD服务不受支持。

> [!IMPORTANT]
> 全局服务的特定区域的某些服务和功能可能无法在所有区域云中提供。 若要了解哪些服务可用，请参阅按 [地区提供的产品](https://azure.microsoft.com/global-infrastructure/services/?products=all&regions=usgov-non-regional,us-dod-central,us-dod-east,usgov-arizona,usgov-iowa,usgov-texas,usgov-virginia,china-non-regional,china-east,china-east-2,china-north,china-north-2,germany-non-regional,germany-central,germany-northeast)。

若要详细了解国家云，请参阅以下主题：

* [Microsoft 国家云](https://www.microsoft.com/TrustCenter/CloudServices/NationalCloud)
* [Microsoft 365美国政府](/office365/servicedescriptions/office-365-platform-service-description/office-365-us-government/office-365-us-government)
* [由世纪互联运营的 Microsoft 365](/office365/servicedescriptions/office-365-platform-service-description/office-365-operated-by-21vianet)
* [Office 365 德国版](/office365/servicedescriptions/office-365-platform-service-description/office-365-germany)
* [Azure 政府](https://azure.microsoft.com/global-infrastructure/government/)
* [Azure China 21Vianet](/azure/china/)
* [Azure Germany](/azure/germany/)

探索用于国家云部署中的 Azure 和 Microsoft 365进行身份验证和运行的示例：

* [通过美国政府 Microsoft Graph Azure 合作](https://github.com/SteveWinward/Azure-Samples/blob/master/AAD/SampleAadToken_AzureForGovernment.ps1)
* [连接 Microsoft Graph PowerShell (GCC、GCC High 和 GCC DoD) 美国政府 O365 环境](https://github.com/microsoft/Federal-Business-Applications/tree/main/demos/powershell-gov-samples#microsoft-graph-powershell)

