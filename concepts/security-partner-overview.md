---
title: 与 Microsoft Graph 安全性 API合作的机会
description: 本文帮助产品经理和业务开发角色了解投资路径，并提供有关合作伙伴价值主张的见解。
ms.localizationpriority: medium
author: preetikr
ms.prod: security
ms.openlocfilehash: 23a155e42030217046b5af7091cac52d47498b62
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66446075"
---
# <a name="partnering-opportunities-with-the-microsoft-graph-security-api"></a>与 Microsoft Graph 安全性 API合作的机会

本文介绍 Microsoft Graph 安全性 API启用的合作伙伴机会。 它旨在帮助产品经理和业务开发角色了解投资路径，并深入了解合作伙伴价值主张。

## <a name="background"></a>背景

大多数组织处理大量的安全数据，并在其企业中拥有数十个安全解决方案，因此集成各种产品和服务的任务令人生畏和复杂。 这些挑战阻碍了组织在快速移动的破坏性攻击世界中检测和修正威胁时快速行动的能力。

技术合作伙伴可以使用 Microsoft Graph 安全性 API 与 Microsoft 平台集成，以应对这些客户挑战。

## <a name="introduction-to-the-microsoft-graph-security-api"></a>Microsoft Graph 安全性 API简介

Microsoft Graph 安全性 API 是一种统一的 API，提供标准界面和统一架构来集成来自多个源的安全警报和威胁智能、丰富警报和数据的上下文信息，并自动化安全操作。

安全 API 是 Microsoft Graph 的一部分，它是一个用于集成来自 Microsoft 和合作伙伴产品和服务的数据和情报的统一 REST API。 使用 Microsoft Graph，客户和合作伙伴可以快速构建仅验证一次的解决方案，并使用单个 API 调用访问来自多个安全解决方案的安全见解或为此采取行动。 浏览 Microsoft 365、Azure Active Directory、 (Intune 等其他 [Microsoft Graph 实体](./overview.md)时，会发现) 其他值，以便将业务上下文与安全见解联系起来。

Microsoft 以两种关键方式启用技术合作伙伴集成。

1. 作为 Microsoft Graph 信息的使用者，可以使用 Microsoft Graph 中包含的信息丰富解决方案，并使用 Microsoft 图形 API代表客户执行任务。
2. 还可以将警报和操作与 Microsoft 提供商一起贡献给 Microsoft Graph。

|如何集成？|可用数据|支持的功能|
|:--------------------|:-------------|:---------------------|
|将应用程序与 Microsoft Graph 安全性 API集成。|<li>来自 Microsoft Graph 安全提供程序的警报</li><li>来自 Microsoft 的安全分数</li>| <li>查询警报/安全分数</li> <li>调用 Microsoft Graph 安全操作</li> <li>更新 Microsoft Graph 安全警报</li> <li>将客户威胁指示器上传到 Microsoft</li> |
|允许其他人通过 Microsoft Graph 安全性 API与产品集成。|<li>来自安全产品的警报</li>|<li>安全产品的安全操作</li>|

让我们更深入地探讨一些常见方案，其中 Microsoft Graph 安全性 API集成放大了安全集成投资以及我们可以一起实现的客户的优势。

## <a name="featured-technology-partner-scenarios"></a>特色技术合作伙伴方案

下面是通过与 Microsoft Graph 安全性 API集成可以获得的三个主要优势：

1. 客户受益于安全有效性和运营方面的改进。
2. 你的客户受益于你的和其他集成合作伙伴产品提供的丰富信息。
3. 简化了技术合作伙伴的工程投资，并通过与 Microsoft Graph 安全性 API 集成来放大客户价值。

### <a name="enhance-threat-protection-with-the-microsoft-graph-security-api"></a>使用 Microsoft Graph 安全性 API增强威胁防护

*启用安全警报的更轻松集成，以通知威胁检测和响应。*

- 将来自 Microsoft Graph 安全提供程序的警报/检测与检测相关联，以改进调查结果并支持自动化。
- 通过 Microsoft Graph 访问检测和上下文，以改进威胁响应 - 会审、调查、修正。
- 访问客户威胁智能 (哈希、IP、URL、域等) 阻止/警报恶意活动。

### <a name="streamline-it-and-security-management"></a>简化 IT 和安全管理

*为事件生命周期提供更高的可见性和精简管理。*

- 聚合来自多个提供程序的警报以创建事件。
- 访问其他上下文以通知警报优先级和响应。
- 在管理警报的系统之间保持警报状态同步。
- 了解安全状况并建议如何使用安全分数对其进行改进。

### <a name="share-threat-intelligence-to-enable-custom-detections"></a>共享威胁智能以启用自定义检测

*利用威胁智能为 Microsoft 解决方案中的自定义检测提供支持。*

- 自动将威胁指示器发送到 Microsoft 安全解决方案，以启用警报、阻止或允许操作。
- 启用快速操作来抵御新威胁，例如安全工具和工作流中的块文件、URL、域、IP 地址。
- 客户提供的 TI 仅用于供应客户，而不用于任何其他 Microsoft 客户。

## <a name="technical-integrations-overview"></a>技术集成概述

Microsoft Graph 安全性 API合作伙伴机会通过两个主要集成路径提供，这些路径可以单独使用或一起使用。  我们将概述高级要求，并提供一些见解，了解如何考虑在此处投资这些路径，但详细的技术解释将留给本文档后面引用的文档。

支持的实体：

- **警报** 是“具有安全影响的结论”，而不是原始日志数据或其他未关联的信息。 [了解详细信息](/graph/api/resources/security-api-overview#alerts)。
- **威胁指示器**（也称为入侵指标或 IoC）表示有关已知威胁的数据，例如恶意文件、URL、域和 IP 地址。 客户可以通过内部威胁情报收集或从威胁情报社区、许可源和其他来源获取指标来生成指标。 [了解详细信息](/graph/api/resources/tiindicator)。
- **安全操作** 使技术合作伙伴能够通过 Graph 公开功能功能。  例如，如果安全解决方案支持阻止 IP 地址的功能，则可以在 Graph 中公开“阻止 IP”作为功能。 其他 Graph 安全性 API产品可以通过 Graph 调用操作。 [了解详细信息](/graph/api/resources/securityaction)。
- **安全分数**... [了解详细信息](/graph/api/resources/securescores)。

### <a name="integrate-your-application-with-the-microsoft-graph-security-api"></a>将应用程序与 Microsoft Graph 安全性 API集成

[所有集成应用程序都必须注册](./auth-register-app-v2.md)到 Microsoft Graph。 支持单个客户使用的两个应用程序，以及许多客户使用的应用程序 (多租户) 。  在任一情况下，客户都必须为应用程序授予许可。 调用 Microsoft Graph 时，应用程序发出的每个请求将包含应用程序标识符和你代表其调用的客户。 支持以下类型的请求：

- **获取警报** – 根据需要通过筛选获取警报信息。  例如：显示特定用户、主机等的所有高优先级警报或“所有高优先级警报”。
- **更新警报状态** - 启用警报生命周期的管理。  例如：将警报状态设置为“已解决”，从“正在进行”或向警报添加注释。
- **获取安全分数** - Microsoft 安全分数是 Microsoft 产品安全配置的“信用评级”类型值。
- **订阅** - 允许通知警报或查询的更改。
- **源自定义威胁指示器** - 自动将威胁指示器发送到 Microsoft 安全解决方案，以启用警报、阻止或允许操作。 直接使用 Microsoft Graph 安全性 API或利用与主要威胁情报平台的集成。
- **调用 Microsoft Graph 安全操作** - 立即采取措施，使用 Microsoft Graph [Security SecurityActions](/graph/api/resources/securityaction) 实体防范威胁。

### <a name="enable-others-to-integrate-with-your-products-through-the-microsoft-graph-security-api"></a>让其他人通过 Microsoft Graph 安全性 API与产品集成

Microsoft Graph 安全提供商通过 Microsoft Graph 向其他人提供其安全警报。  生成安全警报的 Microsoft 产品都具有向 Microsoft Graph 公开其各自警报的提供程序。 此外，Microsoft Graph 安全性 API允许外部提供商以 Microsoft 技术合作伙伴的身份在 Microsoft Graph 中共享应用程序的相关安全警报，供客户使用。 除了警报，Microsoft Graph 安全性操作还使技术合作伙伴能够通过 Microsoft Graph 公开功能功能。  例如，如果安全解决方案支持阻止 IP 地址的功能，则可以在 Microsoft Graph 中公开“阻止 IP”作为功能。 其他 Microsoft Graph 安全产品可以通过 Microsoft Graph 调用操作。

Microsoft Graph 安全提供程序本质上是一个云终结点，它响应来自 Microsoft Graph 安全性 API的请求，并返回相关安全警报或为共同客户执行操作。 客户和服务到服务的身份验证可确保对客户警报和操作的访问受到保护。

提供程序方案种类繁多。 精心策划的载入过程从标识相关方案开始。 达成一致后，可以使用文档、示例代码和开发环境来支持 Microsoft Graph 安全提供程序的开发。

## <a name="get-started"></a>入门

### <a name="onboarding-guides-and-technical-documentation"></a>载入指南和技术文档

- [Microsoft Graph 安全性 API概述](./security-concept-overview.md)
- [API 参考](/graph/api/resources/security-api-overview)
- [警报架构](/graph/api/resources/alert)
- [tiIndicator 架构](/graph/api/resources/tiindicator)
- [安全操作架构](/graph/api/resources/securityaction)
- [安全评分架构](/graph/api/resources/securescores)

### <a name="sample-code"></a>示例代码

- [Microsoft Graph 安全性示例](https://aka.ms/graphsecurityapicode)
- [为 Microsoft Graph 安全性示例做出贡献](https://aka.ms/graphsecurityapicodecontribute)

### <a name="help-and-support"></a>帮助和支持

- 如果对应用程序、服务或产品与 Microsoft Graph 安全性 API集成有疑问，请联系[使用 Microsoft 安全图形 API技术社区](https://techcommunity.microsoft.com/t5/Using-Microsoft-Graph-Security/bd-p/SecurityGraphAPI)
- 按照有关 [Microsoft Q&A](/answers/topics/microsoft-graph-security.html)  和标记：microsoft-graph-security 的讨论进行操作。
- 如果在示例或文档请求中发现 bug，或者在相应的 [示例存储库](https://github.com/microsoftgraph/security-api-solutions/blob/master/sample-repos.md)中发现 bug 文件问题。
- 如果有新的示例请求或未限于单个示例的问题，则 [Microsoft Graph 安全解决方案存储库](https://github.com/microsoftgraph/security-api-solutions)中[的文件问题](https://github.com/microsoftgraph/security-api-solutions/issues/new)。

### <a name="getting-to-market"></a>进入市场

- [Microsoft 合作伙伴网络](https://partner.microsoft.com/) - 与 Microsoft 合作的主要计划是 Microsoft 合作伙伴网络。 Microsoft Graph 安全集成属于 [MPN 独立软件供应商 (ISV) ](https://partner.microsoft.com/isv-resource-hub) 跟踪。
- [Microsoft 智能安全协会](https://www.microsoft.com/security/partnerships/intelligent-security-association) 是专门为 Microsoft 安全合作伙伴提供的程序，旨在帮助丰富安全产品，提高客户对 Microsoft Security 产品的集成的可发现性。
- Microsoft AppSource – 作为 Microsoft Graph 安全性 API合作伙伴，可以在 [Microsoft AppSource 市场中](https://appsource.microsoft.com/partners/signup)列出 Microsoft Graph 集成。
