---
title: Microsoft Graph 中的合规性和隐私 API 概述
description: Microsoft Graph 合规性 API 为组织提供了自动执行重复任务并与现有合规性工具集成的功能，以构建符合行业法规通常需要的可预测工作流。
author: mahage-msft
ms.localizationpriority: medium
ms.prod: ediscovery
ms.custom: scenarios:getting-started
ms.openlocfilehash: fd774e77c6f7c7ae2b996daa1d5a99e6f6ab7fb4
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60684041"
---
# <a name="overview-of-compliance-and-privacy-apis-in-microsoft-graph"></a>Microsoft Graph 中的合规性和隐私 API 概述

Microsoft Graph API 实现合规性和隐私，为组织提供了自动执行重复任务并与现有合规性工具集成的功能，以构建符合行业法规通常需要的可预测工作流。

合规性和隐私 API 旨在帮助实现以下愿景：帮助组织适应和扩展 Microsoft 365 合规性，使其符合自己的特定要求，实现现有自定义或第三方解决方案的集成，以及加速和支持在整个企业数字资产中使用 Microsoft 365 解决方案。

## <a name="electronic-discovery-ediscovery-preview"></a>电子数据 (电子数据展示)  (预览) 

### <a name="develop-applications-that-ensure-a-repeatable-predictable-and-standard-process"></a>开发确保可重复、可预测和标准流程的应用程序

组织依靠[Microsoft 365](/microsoft-365/compliance/ediscovery?view=o365-worldwide&preserve-view=true)电子数据展示功能，根据内部或外部要求（如诉讼、调查或监管合规性）了解其组织中所需情况的真实情况。

在许多组织中，电子数据展示工作流是频繁、关键且大量的。 在常见重复任务或大量活动的情况下，API 将有助于提供一种可伸缩的方式，以一致且有效地重复过程。

### <a name="manage-your-ediscovery-workflows"></a>管理电子数据展示工作流

许多组织处理大量的事例和电子数据展示请求，并且希望自动执行某些任务。 Microsoft Graph高级电子数据展示 API 提供对高级电子数据展示解决方案中大多数可用功能的 API 访问权限。

根据当前的系统和流程，组织可能在自动化和集成方面具有各种优先级，从上游流程（如案例创建）到下游（如收集、审阅集查询或导出）。 通过整个高级电子数据展示工作流中的 API 支持工作流提供了灵活性和选项。

### <a name="build-custom-ediscovery-workflows-with-microsoft-graph"></a>使用 Microsoft 服务构建自定义电子数据展示Graph

> [!VIDEO https://www.youtube-nocookie.com/embed/gXqBEHy5K6E]

- 使用案例管理工具自动执行案例管理和同步。

- 向事例添加标准化标记托盘。

- 创建自定义报告以跟踪单个事例的事例负载和进度。

## <a name="privacy-management-by-subject-rights-requests"></a>按主体权限请求的隐私管理

根据全球的某些隐私法规，个人可以请求查看或管理公司收集的有关自己的个人数据。 这些请求在隐私管理解决方案中称为Microsoft 365权限请求;它们有时也称为数据主体请求 (DSR) 或数据主体访问请求 (DSAR) 。 [Microsoft 365隐私](/privacy/solutions/privacymanagement/privacy-management?view=o365-worldwide&preserve-view=true)管理使负责履行主体权利请求的人员可以轻松识别数据主体，并找到 Exchange、SharePoint、OneDrive 和 Teams 中组织数据中的个人信息。 

Microsoft Graph主题权限请求 API 为组织提供了自动执行重复任务并与现有数据主体请求工具集成的功能，以便能够构建可合并到其业务流程中的可重复工作流。 可以使用主题权限请求 API 来帮助你自动执行和扩展组织在 Microsoft 365 中执行主题权限请求搜索的能力，并帮助更有效地满足行业法规。

## <a name="api-reference"></a>API 参考

在查找这些服务的 API 参考？
- [在 Microsoft Graph](/graph/api/resources/ediscovery-ediscoveryapioverview?view=graph-rest-beta&preserve-view=true) beta 版中使用 Microsoft Graph电子数据展示 API
- [使用 Microsoft Graph](/graph/api/resources/subjectrightsrequest-subjectrightsrequestapioverview) v1.0 中的 Microsoft Graph主体权限请求 API
- [在 Microsoft Graph](/graph/api/resources/subjectrightsrequest-subjectrightsrequestapioverview?view=graph-rest-beta&preserve-view=true) beta 版中使用 Microsoft Graph主题权限请求 API

## <a name="next-steps"></a>后续步骤

- 从 Graph 浏览器的[用户](https://developer.microsoft.com/graph/graph-explorer)资源探索自己的数据。
- 浏览[Microsoft Graph合规性 API。](/graph/api/resources/complianceapioverview)
- 浏览 Microsoft Graph[示例和 SDK。](https://developer.microsoft.com/graph/gallery/?filterBy=Samples,SDKs)
