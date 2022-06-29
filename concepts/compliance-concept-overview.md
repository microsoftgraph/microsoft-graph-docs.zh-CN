---
title: Microsoft Graph 中的合规性和隐私 API 概述
description: 使用 Microsoft Graph 符合性和隐私 API 自动执行重复性任务，并与合规性工具集成，以满足所需的行业法规。
author: mahage-msft
ms.localizationpriority: medium
ms.prod: ediscovery
ms.custom: scenarios:getting-started
ms.openlocfilehash: d571615b3431f2ef4707ea90ce8277643deb9b81
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66442132"
---
# <a name="overview-of-compliance-and-privacy-apis-in-microsoft-graph"></a>Microsoft Graph 中的合规性和隐私 API 概述

适用于合规性和隐私的 Microsoft Graph API 为组织提供了自动执行重复性任务的功能，并与现有合规性工具集成，以生成通常需要满足行业法规要求的可预测工作流。

合规性和隐私 API 旨在帮助组织根据自己的特定要求调整和扩展 Microsoft 365 合规性，为现有自定义或第三方解决方案启用集成，并加速和支持在整个企业数字资产中使用 Microsoft 365 解决方案的愿景。

## <a name="electronic-discovery-ediscovery-preview"></a>电子发现 (电子数据展示)  (预览) 

### <a name="develop-applications-that-ensure-a-repeatable-predictable-and-standard-process"></a>开发可确保可重复、可预测和标准流程的应用程序

组织依靠 [Microsoft 365 电子数据展示](/microsoft-365/compliance/ediscovery?view=o365-worldwide&preserve-view=true) 功能来满足要求，根据内部或外部要求（例如诉讼、调查或法规合规性）查找组织中所发生情况的真相。

在许多组织中，电子数据展示工作流频繁、关键且数量大。 在存在常见重复任务或大量活动的情况下，API 将帮助提供一种可缩放的方式来一致且有效地重复进程。

### <a name="manage-your-ediscovery-workflows"></a>管理电子数据展示工作流

许多组织处理大量案例和电子数据展示请求，并且希望自动执行某些任务。 用于高级电子数据展示的 Microsoft Graph API 提供对高级电子数据展示解决方案中可用的大多数函数的 API 访问权限。

根据当前的系统和流程，组织可能具有自动化和集成的各种优先级，从上游流程（如案例创建）到下游流程（如收集、审阅集查询或导出）。 在整个高级电子数据展示工作流中通过 API 支持工作流提供了灵活性和选项。

### <a name="build-custom-ediscovery-workflows-with-microsoft-graph"></a>使用 Microsoft Graph 构建自定义电子数据展示工作流

> [!VIDEO https://www.youtube-nocookie.com/embed/gXqBEHy5K6E]

- 使用案例管理工具自动执行案例管理和同步。

- 将标准化标记托盘添加到案例。

- 创建自定义报告以跟踪案例负载和各个案例的进度。

## <a name="privacy-management-by-subject-rights-requests"></a>按主题权限请求进行隐私管理

根据世界各地的某些隐私法规，个人可以请求查看或管理公司收集的有关自己的个人数据。 这些请求在 Microsoft 365 隐私管理解决方案中称为使用者权利请求;它们有时也称为数据主体请求 (DSR) 或数据主体访问请求 (DSAR) 。 [Microsoft 365 隐私管理](/privacy/solutions/privacymanagement/privacy-management?view=o365-worldwide&preserve-view=true) 使负责满足主体权利请求的人员能够轻松识别数据主体，并在 Exchange、SharePoint、OneDrive 和 Teams 中的组织数据中查找其个人信息。 

使用者权限请求的 Microsoft Graph API 为组织提供了自动执行重复任务和与现有数据主体请求工具集成的功能，以便生成可合并到其业务流程的可重复工作流。 可以使用主题权限请求 API 来帮助你自动化和扩展组织在 Microsoft 365 中执行主题权限请求搜索的能力，并帮助更高效地满足行业法规。

## <a name="records-management-preview"></a>记录管理 (预览) 

所有类型的组织都需要记录管理解决方案来管理其公司数据中的关键记录。 [Microsoft Purview 记录管理](/microsoft-365/compliance/records-management) 可帮助组织管理其法律义务、提供证明遵守法规的能力，以及通过定期处置不再需要的项目来提高效率。

大量组织使用记录管理解决方案来保护、标记、保留或删除其数据。 用于记录管理的 Microsoft Graph API 允许组织更高效地管理标签和标签关联的功能、自动执行重复性任务，并为客户提供灵活的选项。


## <a name="api-reference"></a>API 参考

在查找这些服务的 API 参考？

- [Microsoft Graph 电子数据展示 API beta](/graph/api/resources/ediscovery-ediscoveryapioverview?view=graph-rest-beta&preserve-view=true)
- [Microsoft Graph 使用者权限请求 API v1.0](/graph/api/resources/subjectrightsrequest-subjectrightsrequestapioverview)
- [Microsoft Graph 主题权限请求 API beta](/graph/api/resources/subjectrightsrequest-subjectrightsrequestapioverview?view=graph-rest-beta&preserve-view=true)

## <a name="next-steps"></a>后续步骤

- 从 Graph 浏览器的[用户](https://developer.microsoft.com/graph/graph-explorer)资源探索自己的数据。
- 浏览 [Microsoft Graph 符合性 API](/graph/api/resources/complianceapioverview)。
- 浏览 Microsoft Graph [示例和 SDK](https://developer.microsoft.com/graph/gallery/?filterBy=Samples,SDKs)。
