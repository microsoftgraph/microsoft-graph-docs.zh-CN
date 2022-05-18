---
title: Microsoft Graph 中的主要服务和功能
description: '借助 Microsoft Graph，可以使用 REST API 和客户端库与 Microsoft 365、Windows 以及 Microsoft 365 中的企业移动性 + 安全性服务充分集成。 此外，它提供安全性和社交智能，可以提高用户的工作效率、创造性和团队协作，并保护企业资源和用户数据。 '
author: angelgolfer-ms
ms.localizationpriority: high
ms.custom: scenarios:getting-started
ms.openlocfilehash: ae8f0b29fccbfea9d7c71342a5bc45f08367e943
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461252"
---
# <a name="major-services-and-features-in-microsoft-graph"></a>Microsoft Graph 中的主要服务和功能

借助 Microsoft Graph，可以使用 REST API 和客户端库与 Microsoft 365、Windows 以及 Microsoft 365 中的企业移动性 + 安全性服务充分集成。 此外，它还提供安全性和智能，可以提升用户的工作效率、创意和团队协作，并保护企业资源和用户数据。 

## <a name="users-and-groups"></a>用户和组

Microsoft Graph 的核心是用户和组的概念。 

Microsoft Graph 中的 _用户_ 是数以百万计使用 Microsoft 365 云服务的用户之一。 它是身份受到保护且访问得到妥善管理的焦点。 用户数据是业务发展的驱动力。 Microsoft Graph 服务使这些数据在丰富的上下文、实时更新和深入见解中可供企业使用，并且始终仅在适当的权限下使用这些数据。

Microsoft 365 _组_ 是允许用户进行协作的基本实体。 它与其他服务集成，在任务规划、团队合作、教育等方面提供更丰富的方案。 

|功能     |支持服务  |说明 |更多信息 |
|:-----------|:--------------------|:-----------|:----------------|
| 用户 | Azure AD 和大多数高效工作、协作、智能和教育服务 | 用户是 Microsoft Graph 的核心重点，Microsoft Graph 服务围绕这一点构建以用户为中心的功能。 | [Microsoft Graph 中的用户概述](azuread-users-concept-overview.md)|
|组 | Azure AD、OneDrive、OneNote、Outlook、Planner | Microsoft 365 组为用户提供了基本协作单元，以共享对话、文件、笔记、日历和计划等。 | [Microsoft Graph 中的 Microsoft 365 组概述](office365-groups-concept-overview.md) |

## <a name="connecting-users-data-microsoft-365-services-and-your-apps"></a>连接用户数据、Microsoft 365 服务和你的应用

从核心用户和组开始，Microsoft Graph 构建了一个 Microsoft 365 服务和功能网络，用于管理、保护和提取数据，以支持各种各样的场景。 Microsoft Graph 允许你在始终尊从适当授权的情况下访问这些大量的用户数据。

![Microsoft Graph 将你连接到用户数据](images/microsoft-graph-connects-users-data.png)

### <a name="services-and-features"></a>服务和功能

Microsoft Graph 中的一些服务是首次推出，其他服务则是我们所熟知的独立服务且目前融入 Microsoft Graph 中。 它们的 API 集遵循 [Microsoft REST API 准则](https://github.com/Microsoft/api-guidelines)中详述的简化设计，现在可通过单个 Microsoft Graph REST 终结点 `https://graph.microsoft.com` 进行访问。 本文其余部分按类别列出了主要服务和功能。 


## <a name="identity-and-access-management"></a>标识和访问管理

|功能     |支持服务  |说明 |更多信息 |
|:-----------|:--------------------|:-----------|:----------------|
| 标识和访问管理 | Azure AD | 创建和管理目录资源，如用户、组和应用程序。 管理对资源和数据的访问。 授权客户登录并访问 Azure AD 中的帐户风险数据。| [Azure AD 标识和访问管理概述](azuread-identity-access-management-concept-overview.md)  |


## <a name="productivity"></a>工作效率

|功能     |支持服务  |说明 |更多信息 |
|:-----------|:--------------------|:-----------|:----------------|
| 日历 | Outlook  | 允许用户在 Web、移动和桌面设备上设置约会和会议。 它是 Microsoft 365 中 Outlook 消息传递通信中心的一部分，还允许用户管理电子邮件和联系人。 | [Outlook 日历概述](outlook-calendar-concept-overview.md)  |
| 文件 | OneDrive 和 SharePoint | 在 OneDrive 和 SharePoint 上管理和共享用户文件。 | [OneDrive 文件存储概述](onedrive-concept-overview.md) |
| 邮件 | Outlook | 允许用户在 Web、移动和桌面设备上进行通信、组织邮件，并管理其工作流中的优先事项。 它是 Microsoft 365 中 Outlook 通信中心的一部分，还允许用户管理联系人和安排会议。 | [Outlook 邮件概述](outlook-mail-concept-overview.md) |
| 笔记 | OneNote | 允许用户规划和组织观点及信息。 | [OneNote 笔记概述](integrate-with-onenote.md) |
| 个人联系人 | Outlook | Web、移动和桌面设备上的联系人管理器。 它是 Microsoft 365 中 Outlook 消息传递通信中心的一部分，还允许用户管理电子邮件和安排会议。  | [Outlook 个人联系人概述](outlook-contacts-concept-overview.md) |
| 工作簿和图表 | Excel | 允许用户使用 Excel 电子表格进行复杂计算、跟踪、分析和可视化数据，并生成专业报表。 | [Excel 工作簿和图表概述](excel-concept-overview.md) |
| 待办任务 | 待办事项 | 允许用户管理工作和生活中的个人任务。它还与 Outlook、Teams、Planner 和 Cortana 集成，使其成为存放 Microsoft 365 中用户个人任务的单一位置。 | [微软待办任务概述](todo-concept-overview.md) |

## <a name="collaboration"></a>协作

<!-- Want to update links to concept overviews as they are created over time. 
-->
|功能     |支持服务  |说明 |更多信息 |
|:-----------|:--------------------|:-----------|:----------------|
| 云通信 | Microsoft Teams, Skype | 允许应用和服务通过各种通信相关功能与用户进行交互，例如，允许聊天机器人处理呼叫、在业务线中集成联机会议、显示用户的当前状态（预览版）和查找通话和联机会议的记录（预览版）。 | [云通信概述](cloud-communications-concept-overview.md) |
| 网站和列表  | SharePoint | 面向用户和 Microsoft 365 组的基于 Web 的平台，以共享、组织、管理和发现内容（包括列表、文件和笔记）。 | [SharePoint 网站和内容概述](sharepoint-concept-overview.md) | 
|任务和计划 | Planner | 使 Microsoft 365 组中的用户能够创建计划、分配任务和跟踪进度。 | [Planner 计划和任务概述](planner-concept-overview.md) |
|团队合作 |  Microsoft Teams | 面向团队的数字中心和基于聊天的工作区，用于共享文件、笔记、日历和计划。 | [Microsoft Teams 团队合作概述](teams-concept-overview.md) |


## <a name="people-and-workplace-intelligence"></a>人员和工作场所智能

|功能     |支持服务  |说明 |更多信息 |
|:-----------|:--------------------|:-----------|:----------------|
| 人员 | Azure AD、Outlook、SharePoint 等 | 获取有关人员的信息，该对象按与用户的相关程度进行排序，相关程度由用户的通信和协作模式以及业务关系决定。  | [Microsoft Graph 中的人员和工作场所智能](social-intel-concept-overview.md) |
| 个人资料（预览版） | 配置文件 | 提供存储和检索有关租户内人员的信息的轻型机制。 | [Microsoft Graph 中的人员和工作场所智能](social-intel-concept-overview.md) |
| 个人资料卡片自定义（预览版） | 个人资料卡片 | 为管理员提供一种轻量级机制，以自定义组织中 Microsoft 365 个人资料卡上显示的内容。 | [Microsoft Graph 中的人员和工作场所智能](social-intel-concept-overview.md) |
| 文档见解  | Delve、OneDrive、Outlook、SharePoint | 使用高级分析和机器学习技术获取常用的文档，以及用户查看、修改或共享的文档。  | [Microsoft Graph 中的人员和工作场所智能](social-intel-concept-overview.md)  |
| 分析（预览版） | Viva Insights | 使用高级分析和机器学习技巧，提供了有关用户如何花费自己时间，以及用户与谁一起花费时间的见解。 此类数据可以帮助用户计划一天的日程安排，深入了解自己的不同工作模式，并帮助用户平衡工作和生活。  | [Microsoft Graph 中的人员和工作场所智能](social-intel-concept-overview.md) |


## <a name="device-and-app-management"></a>设备和应用管理

|功能     |支持服务  |说明 |详细信息 |
|:-----------|:--------------------|:-----------|:----------------|
| 云打印 | 通用打印 | 通用打印是基于 Microsoft 365 云的打印基础设施，可以为用户提供易用、丰富且安全的打印体验，并为 IT 人员减少管理方面的工作。 | [使用通用打印 API 进行云打印](universal-print-concept-overview.md) |
|公司设备和应用管理 | Intune | 注册和配置设备，并管理组织中的移动应用程序。 | [Intune 设备和应用概述](intune-concept-overview.md) |
| 云电脑（预览版） | Windows 365  | Windows 365 是一项基于云的服务，管理员可以轻松地为组织中的用户设置和管理 Windows 365 云电脑。 单个最终用户可以随时使用其云电脑安全地将其丰富的个性化 Windows 体验从 Microsoft 云流式传输到任何设备。 | [通过 Microsoft Graph API 使用 Windows 365 云电脑](cloudpc-concept-overview.md) |
| 设备更新（预览） | 适用于企业的 Windows 更新部署服务 | 可控制对从 Windows 更新网站传送内容的批准、计划、监测和防护。 | [Microsoft Graph 中的 Windows 更新](windowsupdates-concept-overview.md) |
| 多租户管理（预览） | Microsoft 365 Lighthouse | 允许托管服务提供商 （MSP） 远程管理多个客户租户以进行合规性和威胁检测，并帮助使租户设备处于正常且安全的状态。 | [使用 Microsoft 365 Lighthouse 的多租户管理](managedtenants-concept-overview.md) |
| 服务运行状况和通信 | Microsoft 365 和 Dynamics 365 服务 | 提供访问健康状态和关于 Microsoft 云服务的消息中心帖子。 使用服务通信 API 的值得注意的示例是 Microsoft 365 管理中心。 | [在 Microsoft Graph 中访问服务健康和通信](service-communications-concept-overview.md) |


## <a name="security"></a>安全性

|功能     |支持服务  |说明 |更多信息 |
|:-----------|:--------------------|:-----------|:----------------|
| 安全集成 | Azure AD 标识保护、Azure 信息保护、Azure 安全中心、Microsoft Defender for Cloud Apps、Windows Defender 高级威胁防护[等](/graph/api/resources/security-api-overview) | 跨整个 Microsoft 和生态系统合作伙伴提供安全见解和操作的统一网关。 | [Microsoft Graph 中的安全性](security-concept-overview.md) |



## <a name="cross-device-experiences"></a>跨设备体验

|功能     |支持服务  |说明 |更多信息 |
|:-----------|:--------------------|:-----------|:----------------|
| 跨设备体验 | 活动源、设备中继 | 支持超越单一设备的应用体验，同用户在不同设备之间移动，而不考虑设备类型和平台。 | [跨设备体验概述](cross-device-concept-overview.md) |

## <a name="user-notifications-deprecated"></a>用户通知（已弃用）

> [!IMPORTANT]
> Microsoft Graph 通知 API 已弃用，并且已于 2022 年 1 月停止返回数据。 有关其他通知体验，请参阅 [Microsoft Azure 通知中心](/azure/notification-hubs)。 有关详细信息，请参阅[此博客文章](https://devblogs.microsoft.com/microsoft365dev/retiring-microsoft-graph-notifications/)。

|功能     |支持服务  |说明 |详细信息 |
|:-----------|:--------------------|:-----------|:----------------|
| 用户通知 | 用户通知 | 开启应用体验，构建以用户为中心的跨平台通知体验，包括基于用户扇出、全局关闭和访问通知历史记录。 | [利用 Microsoft Graph 通知实现以人为中心的通知体验](notifications-concept-overview.md) |


## <a name="usage-reports"></a>使用率报告

|功能     |支持服务  |说明 |更多信息 |
|:-----------|:--------------------|:-----------|:----------------|
| 报告 | Microsoft Teams、OneDrive、Outlook、SharePoint、Skype for Business、Yammer | 获取支持服务的活动和用法信息。 | [使用情况报表概述](reportroot-concept-overview.md) |


## <a name="education"></a>教育

|功能     |支持服务  |说明 |更多信息 |
|:-----------|:--------------------|:-----------|:----------------|
| 教育 | Azure AD、教育 | 提供了与教育场景相关的信息，包括学校、课堂、学生、教师和作业信息。 支持 ISV 构建面向教室的应用程序，从而节约教师时间并提升团队合作与协作。  | [教育概述](education-concept-overview.md) |


## <a name="business-applications"></a>业务应用程序

|功能     |支持服务  |说明 |更多信息 |
|:-----------|:--------------------|:-----------|:----------------|
| 客户预订（预览） | Microsoft Bookings | 针对组织，使其用户和客户可以直接在 Web 或 Facebook 上预定服务。 让业务提供商管理客户偏好、服务和定价、员工列表和日程安排，以及其他常见的业务信息。 | [Microsoft Bookings API 概述](booking-concept-overview.md) |
| Financials（预览版） | Dynamics 365 业务中心 | 利用一站式商业管理解决方案，实现财务数据管理、供应链自动化和保护、销售管理和改进客户服务、项目管理和运营优化。| [Business Central API 概述](dynamics-business-central-concept-overview.md) |


## <a name="next-steps"></a>后续步骤

<!-- Need to update the destination page titles and URLs as Matt's v-team finalize on the examples and featured scenarios content 
-->

- 在目录的 **了解** 部分，阅读有关 _你_ 可在应用场景中使用的服务和功能。
- 尝试 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中的示例请求。
- 使用此[快速入门](https://developer.microsoft.com/graph/quick-start)设置即可运行的示例应用。
