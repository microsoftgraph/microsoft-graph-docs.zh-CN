---
title: '与 Microsoft Graph 安全性 API 合作 - 技术合作伙伴机会 '
description: '本文介绍由 Microsoft Graph 安全性 API 启用的合作伙伴机会，旨在帮助产品经理和业务开发角色了解投资路径，并提供对合作伙伴价值主张的见解。 '
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 2e8025bbcb3b2858db467444d155cd8186e57dce
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921936"
---
# <a name="partnering-with-the-microsoft-graph-security-api--technology-partner-opportunities"></a>与 Microsoft Graph 安全性 API 合作 - 技术合作伙伴机会

本文介绍了由 Microsoft Graph 安全性 API 启用的合作伙伴机会，旨在帮助产品经理和业务开发角色了解投资路径，并提供对合作伙伴价值主张的见解。

## <a name="background"></a>背景

大多数组织处理大量安全数据，并且企业中具有数十个安全解决方案，使得集成各种产品和服务的任务变得困难和复杂。 在快速移动的破坏性攻击中检测和修正威胁时，这些问题阻碍组织快速移动的能力。

技术合作伙伴可以使用 Microsoft Graph 安全性 API 与 Microsoft 平台集成，以解决这些客户难题。

## <a name="introduction-to-the-microsoft-graph-security-api"></a>Microsoft Graph 安全性 API 简介

Microsoft Graph 安全性 API 是一种统一的 API，提供标准界面和统一架构来集成来自多个源的安全警报和威胁智能、丰富警报和数据的上下文信息，并自动化安全操作。

安全 API 是 Microsoft Graph 的一部分，它是一个用于集成来自 Microsoft 和合作伙伴产品和服务的数据和情报的统一 REST API。 使用 Microsoft Graph，客户和合作伙伴可以快速构建仅验证一次的解决方案，并使用单个 API 调用访问来自多个安全解决方案的安全见解或为此采取行动。 在浏览 Microsoft 365、Azure Active Directory、Intune (Microsoft Graph 实体等其他 [Microsoft Graph](./overview.md) 实体时，) 发现其他价值，以将业务上下文与安全见解关联起来。

Microsoft 以两种关键方式实现技术合作伙伴集成。

1. 作为 Microsoft Graph 信息的使用者，可以使用 Microsoft Graph 中包含的信息丰富解决方案，并使用 Microsoft Graph API 代表客户执行任务。
2. 还可以与 Microsoft 提供程序一起向 Microsoft Graph 提供警报和操作。

|如何集成？|可用数据|支持的功能|
|:--------------------|:-------------|:---------------------|
|将应用程序与 Microsoft Graph 安全性 API 集成。|<li>来自 Microsoft Graph 安全提供程序的警报</li><li>Microsoft 的安全分数</li>| <li>查询警报/安全分数</li> <li>调用 Microsoft Graph 安全性操作</li> <li>更新 Microsoft Graph 安全性警报</li> <li>将客户威胁指示器上载到 Microsoft</li> |
|使其他人可以通过 Microsoft Graph 安全性 API 与产品集成。|<li>来自安全产品的警报</li>|<li>安全产品的安全操作</li>|

让我们深入探讨一些常见方案，其中 Microsoft Graph 安全性 API 集成可以放大安全集成投资以及我们可以一起实现的好处。

## <a name="featured-technology-partner-scenarios"></a>特色技术合作伙伴方案

通过与 Microsoft Graph 安全性 API 集成，你可以获得以下三个关键优势：

1. 客户从安全性有效性和运营方面的改进中获益。
2. 你的客户从你的和其他集成合作伙伴产品提供的丰富信息中获益。
3. 通过与 Microsoft Graph 安全性 API 集成，简化了技术合作伙伴的工程投资，并放大了客户价值。

### <a name="enhance-threat-protection-with-the-microsoft-graph-security-api"></a>使用 Microsoft Graph 安全性 API 增强威胁防护

*允许更轻松地集成安全警报，以通知威胁检测和响应。*

- 将来自 Microsoft Graph 安全提供程序的警报/检测与你的检测关联，以改进你的调查结果和支持自动化。
- 通过 Microsoft Graph 访问检测和上下文，以改进威胁响应 – 会审、调查、修正。
- 访问客户威胁情报 (哈希、IP、URL、域等) 恶意活动进行阻止/警报。

### <a name="streamline-it-and-security-management"></a>简化 IT 和安全管理

*提供更高的可见性并简化事件生命周期的管理。*

- 聚合来自多个提供商的警报以创建事件。
- 访问其他上下文，以通知警报优先顺序和响应。
- 在管理警报的系统之间保持警报状态同步。
- 深入了解安全状态，并推荐如何使用安全分数改进安全状态。

### <a name="share-threat-intelligence-to-enable-custom-detections"></a>共享威胁智能以启用自定义检测

*利用威胁情报在 Microsoft 解决方案中支持自定义检测。*

- 自动将威胁指示器发送到 Microsoft 安全解决方案，以启用警报、阻止或允许操作。
- 启用快速操作以抵御新威胁，如安全工具和工作流中的阻止文件、URL、域、IP 地址。
- 客户提供的 TI 仅用于提供客户，而不是任何其他 Microsoft 客户。

## <a name="technical-integrations-overview"></a>技术集成概述

Microsoft Graph 安全性 API 合作伙伴机会通过两个主要集成路径提供，可以单独使用，也可以一起使用。  我们将概述这些高级要求，并提供一些见解，了解如何考虑在此处投资这些途径，但本文档稍后将介绍详细的技术解释。

支持的实体：

- **警报** 是"具有安全影响的结果"，而不是原始日志数据或其他未记录的信息。 [了解详细信息](/graph/api/resources/security-api-overview#alerts)。
- **威胁指示器**（也称为入侵指示器或 IoC）表示有关已知威胁的数据，例如恶意文件、URL、域和 IP 地址。 客户可以通过内部威胁情报收集生成指示器，或者从威胁情报社区、许可源和其他来源获取指示器。 [了解详细信息](/graph/api/resources/tiindicator)。
- **安全操作** 使技术合作伙伴可以通过 Graph 公开功能。  例如，如果安全解决方案支持阻止 IP 地址的功能，可以将"阻止 IP"公开为 Graph 中的一项功能。 其他 Graph 安全性 API 产品可以通过 Graph 调用你的操作。 [了解详细信息](/graph/api/resources/securityaction)。
- **安全分数**... [了解详细信息](/graph/api/resources/securescores)。

### <a name="integrate-your-application-with-the-microsoft-graph-security-api"></a>将应用程序与 Microsoft Graph 安全性 API 集成

所有集成应用程序 [都必须在](./auth-register-app-v2.md) Microsoft Graph 中注册。 支持单个客户使用的两种应用程序以及许多客户 (租户) 的应用程序。  在任一情况下，客户都必须同意你的应用程序。 调用 Microsoft Graph 时，来自应用程序的每个请求都将包含应用程序标识符和代表您呼叫的客户。 支持以下类型的请求：

- **获取警报** – 根据需要通过筛选获取警报信息。  例如：显示特定用户、主机等的所有高优先级警报或"所有高优先级警报"。
- **更新警报状态** – 启用警报生命周期管理。  例如：将警报状态从"正在进行"设置为"已解决"，或向警报添加注释。
- **获取安全分数** – Microsoft 安全分数是 Microsoft 产品安全配置的"信用评分"类型值。
- **订阅** - 允许通知通知或查询的更改。
- **源自定义威胁指示器** - 自动将威胁指示器发送到 Microsoft 安全解决方案，以启用警报、阻止或允许操作。 直接使用 Microsoft Graph 安全性 API 或利用与领先威胁情报平台的集成。
- **调用 Microsoft Graph 安全性操作** – 立即采取措施，使用 Microsoft Graph 安全性 [securityActions](/graph/api/resources/securityaction) 实体抵御威胁。

### <a name="enable-others-to-integrate-with-your-products-through-the-microsoft-graph-security-api"></a>允许其他人通过 Microsoft Graph 安全性 API 与产品集成

Microsoft Graph 安全提供程序通过 Microsoft Graph 向其他人提供其安全警报。  生成安全警报的 Microsoft 产品均具有向 Microsoft Graph 公开其各自警报的提供程序。 此外，Microsoft Graph 安全性 API 还允许外部提供商（作为 Microsoft 技术合作伙伴）在 Microsoft Graph 中共享来自应用程序的相关安全警报，以便客户使用。 除了警报之外，Microsoft Graph 安全性操作还支持技术合作伙伴通过 Microsoft Graph 公开功能。  例如，如果你的安全解决方案支持阻止 IP 地址的功能，你可以将"阻止 IP"公开为 Microsoft Graph 中的一项功能。 其他 Microsoft Graph 安全性产品可以通过 Microsoft Graph 调用你的操作。

Microsoft Graph 安全提供程序实质上是一个云终结点，它响应来自 Microsoft Graph 安全性 API 的请求，并返回相关的安全警报或为相互客户执行操作。 客户身份验证和服务到服务身份验证可确保访问客户警报和操作的安全。

提供程序方案各不相同。 计划载入过程从确定相关方案开始。 一旦就方案达成一致，文档、示例代码和开发环境即可用于支持 Microsoft Graph 安全提供程序的开发。

## <a name="get-started"></a>开始行动

### <a name="onboarding-guides-and-technical-documentation"></a>载入指南和技术文档

- [Microsoft Graph 安全性 API 概述](./security-concept-overview.md)
- [API 参考](/graph/api/resources/security-api-overview)
- [警报架构](/graph/api/resources/alert)
- [tiIndicator 架构](/graph/api/resources/tiindicator)
- [安全操作架构](/graph/api/resources/securityaction)
- [安全分数架构](/graph/api/resources/securescores)

### <a name="sample-code"></a>示例代码

- [Microsoft Graph 安全性示例](https://aka.ms/graphsecurityapicode)
- [参与 Microsoft Graph 安全性示例](https://aka.ms/graphsecurityapicodecontribute)

### <a name="help-and-support"></a>帮助和支持

- 如果你对应用程序或服务或与 Microsoft Graph 安全性 API 的产品集成有疑问，请联系使用 [Microsoft 安全图形 API 技术社区](https://techcommunity.microsoft.com/t5/Using-Microsoft-Graph-Security/bd-p/SecurityGraphAPI)
- 关注 Microsoft [问答&标记](/answers/topics/microsoft-graph-security.html)  ：microsoft-graph-security。
- 如果你在示例或文档请求中发现 Bug，或者在各自的示例存储库中发现 Bug [文件问题](https://github.com/microsoftgraph/security-api-solutions/blob/master/sample-repos.md)。
- 如果你有新的示例请求或问题，但范围不是单个示例，则 Microsoft Graph[](https://github.com/microsoftgraph/security-api-solutions/issues/new)安全性解决方案存储库中[的文件问题](https://github.com/microsoftgraph/security-api-solutions)。

### <a name="getting-to-market"></a>进入市场

- [Microsoft 合作伙伴网络](https://partner.microsoft.com/) – 与 Microsoft 合作的主要计划是 Microsoft 合作伙伴网络。 Microsoft Graph 安全性集成属于 [MPN 独立软件供应商 (ISV) ](https://partner.microsoft.com/isv-resource-hub) 跟踪。
- [Microsoft Intelligent Security Association](https://www.microsoft.com/security/partnerships/intelligent-security-association) 是专为 Microsoft 安全合作伙伴计划，可帮助丰富安全产品并提高客户对 Microsoft 安全产品的集成可发现性。
- Microsoft AppSource – 作为 Microsoft Graph 安全性 API 合作伙伴，可以在 [Microsoft AppSource](https://appsource.microsoft.com/partners/signup)Marketplace 中列出 Microsoft Graph 集成。