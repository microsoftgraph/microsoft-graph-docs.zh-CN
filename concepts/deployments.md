---
title: 区域云部署
description: 除了全球的数据中心网络外，Microsoft 云服务还可用于三个独立的区域云。
author: arpitha-dhanapathi
ms.localizationpriority: medium
ms.openlocfilehash: 06f3b34d8a1f41116f2e8e719ff81939f4999ecd
ms.sourcegitcommit: 69b150e408c0b9a0705bf33229269f6e5371bc6c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/07/2022
ms.locfileid: "65924077"
---
# <a name="national-cloud-deployments"></a>区域云部署

除了全球的数据中心网络外，Microsoft 云服务还可用于三个独立的区域云。 这些国家/地区云版本是 Microsoft 企业云服务的物理和逻辑网络隔离实例，这些实例局限于特定国家/地区的地理边界内，由当地人员运营。

当前区域云包括：

* Microsoft Cloud for US Government
* Microsoft 云德国
* Azure 和 Microsoft 365 由世纪互联在中国运营

每个国家/地区云环境都是独一无二的，不同于 Microsoft 全球环境。 开发适用于国家云环境的应用程序时，请务必注意这些主要差异：例如，注册应用程序、获取令牌和调用 Microsoft Graph API 可能有所不同。

本文提供有关不同 Microsoft Graph 国家云部署以及每个云中开发人员可用的功能的信息。

> **注意：**[Microsoft Graph 数据连接](./data-connect-concept-overview.md)不支持任何国家云部署。

> [!VIDEO https://www.youtube-nocookie.com/embed/R\_3E0IVypRM]

## <a name="app-registration-and-token-service-root-endpoints"></a>应用注册和令牌服务根终结点

在调用 Microsoft Graph API 之前，应先注册应用程序并获取令牌。 下表列出了 Azure Active Directory (Azure AD) 终结点的基本 URL，以注册应用程序并获取每个国家/地区云的令牌。

| 国家/地区云 | Azure AD 门户终结点 | Azure AD 终结点 |
| -------------- | ------------------------ | ----------------- |
| Azure AD（全局服务） | https://portal.azure.com | `https://login.microsoftonline.com` |
| Azure AD for US Government | https://portal.azure.us | `https://login.microsoftonline.us` |
| Azure AD 德国 | https://portal.microsoftazure.de | `https://login.microsoftonline.de` |
| 由世纪互联运营的 Azure AD 中国 | https://portal.azure.cn | `https://login.chinacloudapi.cn` |

若要详细了解访问令牌和 Microsoft Graph，请参阅 [身份验证基础知识](./auth/auth-concepts.md)。 有关 Azure AD 身份验证方案，请参阅 [Azure AD 身份验证基础知识](/azure/active-directory/develop/authentication-scenarios)。

## <a name="microsoft-graph-and-graph-explorer-service-root-endpoints"></a>Microsoft Graph 和 Graph Explorer 服务根终结点

下表显示了每个国家/地区云的 Microsoft Graph 和 [Graph 资源管理器](https://developer.microsoft.com/graph/graph-explorer) 的服务根终结点。

| 区域云 | Microsoft Graph | Graph 浏览器 |
| -------------- | --------------- | -------------- |
| Microsoft Graph 全局服务 | https://graph.microsoft.com | https://developer.microsoft.com/graph/graph-explorer |
| Microsoft Graph for US Government L4 | https://graph.microsoft.us | 不支持。 |
| Microsoft Graph for US Government L5 (DOD)  | https://dod-graph.microsoft.us | 不支持。 |
| Microsoft Graph 德国 | https://graph.microsoft.de | 不支持。 |
| 由世纪互联运营的 Microsoft Graph 中国 | https://microsoftgraph.chinacloudapi.cn | https://developer.microsoft.com/zh-cn/graph/graph-explorer-china |

> [!IMPORTANT]
> 对于美国政府中的应用：
>
> * 如果你在 Microsoft 365 GCC 环境中工作，请继续使用全球终结点： `https://graph.microsoft.com` 和 `https://portal.azure.com`。
> * 如果你在 Microsoft 365 GCC High 环境中工作，请使用 `https://portal.azure.us` 和 `https://graph.microsoft.us`使用。
> * 如果在 Microsoft 365 DoD 环境中工作，请使用 `https://portal.azure.us` 和 `https://dod-graph.microsoft.us`使用。

> [!NOTE]
> 应用只能通过国家云终结点访问组织数据。 这意味着应用只能访问在特定国家云中注册的租户中的数据。 尝试通过 Microsoft Graph 访问与 Microsoft 个人帐户关联的使用者数据的应用应使用全局服务 `https://graph.microsoft.com`。 为国家云部署获取的访问令牌不能与为全球服务或任何其他国家云获取的访问令牌互换。

## <a name="supported-features"></a>支持的功能

以下 Microsoft Graph 功能在所有国家云部署的 `/v1.0` 终结点上正式发布，但所述除外。

| Microsoft Graph 功能 | Microsoft Cloud for US Government | 由世纪互联运营的 Microsoft Cloud 中国 | Microsoft 云德国 |
| ------------------------ | --------------------------------- | ------------------------------------------ | ----------------------- |
| 访问审查 | ✔ | ✔ | ➖ |
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
| Privileged Identity Management | ✔ | ✔ | ➖ |
| Planner | ✔ | ✔ | ✔ |
| 报告 | ➖ | ➖ | ➖ |
| 搜索 (Microsoft 搜索)  | ✔ | ➖ | ➖ |
| 安全性 | ✔ | ✔ | ✔ |
| 服务运行状况和通信 | ✔ | ✔ | ✔ |
| 服务主体 | ✔ | ➖ | ➖ |
| SharePoint | ✔ | ✔ | ✔ |
| Teams | ✔ | ✔ | ✔ |
| 用户 | ✔ | ✔ | ✔ |

以下 Microsoft Graph 功能在 Microsoft Cloud China 和 Microsoft Cloud Germany (`/beta` v1.0 终结点的终结点) 的预览版 (中提供，这些功能仅) 在 Microsoft Cloud 中提供：

* 组织联系人
* 应用程序
* 服务主体

\* () 仅限 Exchange 和 OneDrive 服务的支持。 不支持 Azure AD 服务。

> [!IMPORTANT]
> 全球服务的特定区域中的某些服务和功能可能无法在所有国家云中使用。 若要了解哪些服务可用，请 [参阅按区域提供的产品](https://azure.microsoft.com/global-infrastructure/services/?products=all&regions=usgov-non-regional,us-dod-central,us-dod-east,usgov-arizona,usgov-iowa,usgov-texas,usgov-virginia,china-non-regional,china-east,china-east-2,china-north,china-north-2,germany-non-regional,germany-central,germany-northeast)。

若要详细了解国家云，请参阅以下主题：

* [Microsoft 国家/地区云](https://www.microsoft.com/TrustCenter/CloudServices/NationalCloud)
* [Microsoft 365 for US Government](/office365/servicedescriptions/office-365-platform-service-description/office-365-us-government/office-365-us-government)
* [由世纪互联运营的 Microsoft 365](/office365/servicedescriptions/office-365-platform-service-description/office-365-operated-by-21vianet)
* [Office 365 德国版](/office365/servicedescriptions/office-365-platform-service-description/office-365-germany)
* [Azure 政府版](https://azure.microsoft.com/global-infrastructure/government/)
* [Azure 中国世纪互联](/azure/china/)
* [Azure Germany](/azure/germany/)

了解在国家云部署中对 Azure 和 Microsoft 365 进行身份验证和使用的示例：

* [通过适用于美国政府的 Microsoft Graph 使用 Azure](https://github.com/SteveWinward/Azure-Samples/blob/master/AAD/SampleAadToken_AzureForGovernment.ps1)
* [使用 Microsoft Graph PowerShell 连接到美国政府 O365 环境 (GCC、GCC High 和 GCC DoD) ](https://github.com/microsoft/Federal-Business-Applications/tree/main/demos/powershell-gov-samples#microsoft-graph-powershell)

