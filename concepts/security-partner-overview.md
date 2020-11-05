---
title: '与 Microsoft Graph 安全 API 合作-技术合作伙伴机会 '
description: '这篇文章介绍了由 Microsoft Graph 安全性 API 启用的合作机会，旨在帮助产品经理和业务开发角色了解投资路径，并提供有关合作价值主张的见解。 '
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: b1c56d7018815f86821e55dc2562d4ea4395a27b
ms.sourcegitcommit: 366178d3fc37439791061082da80a63fba2c27df
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2020
ms.locfileid: "48921632"
---
# <a name="partnering-with-the-microsoft-graph-security-api--technology-partner-opportunities"></a>与 Microsoft Graph 安全 API 合作-技术合作伙伴机会

本文介绍了由 Microsoft Graph 安全性 API 启用的合作机会，旨在帮助产品经理和业务开发角色了解投资路径，并提供有关合作价值主张的见解。

## <a name="background"></a>背景

大多数组织处理大量安全数据，并在企业中拥有数十个安全解决方案，从而使将各种产品和服务的集成变得复杂和复杂的任务变得更加困难。 在对快速移动、中断攻击的世界中检测和修正威胁时，这些挑战会妨碍组织快速移动的能力。

技术合作伙伴可以使用 Microsoft Graph 安全性 API 与 Microsoft 平台集成，以解决这些客户难题。

## <a name="introduction-to-the-microsoft-graph-security-api"></a>Microsoft Graph 安全性 API 简介

Microsoft Graph 安全性 API 是一种统一的 API，提供标准界面和统一架构来集成来自多个源的安全警报和威胁智能、丰富警报和数据的上下文信息，并自动化安全操作。

安全 API 是 Microsoft Graph 的一部分，它是一个用于集成来自 Microsoft 和合作伙伴产品和服务的数据和情报的统一 REST API。 使用 Microsoft Graph，客户和合作伙伴可以快速构建仅验证一次的解决方案，并使用单个 API 调用访问来自多个安全解决方案的安全见解或为此采取行动。 当您浏览其他 [Microsoft Graph 实体](./overview.md) (microsoft 365、Azure Active Directory、Intune 和更多) 以将业务上下文与您的安全见解关联时，会发现其他值。

Microsoft 以两种主要方式启用技术合作伙伴集成。

1. 作为 Microsoft Graph 中信息的使用者，您可以使用 Microsoft graph 中包含的信息来丰富解决方案，也可以使用 Microsoft Graph API 代表客户执行任务。
2. 您还可以将您的通知和操作加入 Microsoft 提供商的 Microsoft Graph。

|如何集成？|数据可用|支持的功能|
|:--------------------|:-------------|:---------------------|
|将应用程序与 Microsoft Graph 安全性 API 集成。|<li>来自 Microsoft Graph 安全提供程序的警报</li><li>Microsoft 的安全分数</li>| <li>查询警报/安全分数</li> <li>调用 Microsoft Graph 安全操作</li> <li>更新 Microsoft Graph 安全警报</li> <li>将客户威胁指示器上传到 Microsoft</li> |
|允许其他人通过 Microsoft Graph 安全性 API 与你的产品集成。|<li>来自安全产品的警报</li>|<li>安全产品的安全操作</li>|

让我们深入探讨一下一些常见方案，其中 Microsoft Graph 安全性 API 集成增加了安全集成投资，以及我们可以一起实现的客户优势。

## <a name="featured-technology-partner-scenarios"></a>特色技术合作伙伴方案

通过与 Microsoft Graph 安全性 API 集成，可以获得以下三个主要好处：

1. 你的客户将从安全效率和运营的改进中受益。
2. 您的客户从自己和其他集成合作伙伴产品提供的丰富信息中获益。
3. 通过与 Microsoft Graph 安全性 API 集成，简化了技术合作伙伴的工程投资，并放大了客户价值。

### <a name="enhance-threat-protection-with-the-microsoft-graph-security-api"></a>使用 Microsoft Graph 安全性 API 增强威胁保护

*实现安全警报的更简单集成，以通知威胁检测和响应。*

- 将来自 Microsoft Graph 安全提供程序的警报/检测与您的检测相关联，以改进调查结果并支持自动脚本。
- 通过 Microsoft Graph 访问检测和上下文，以改进威胁响应–会审、调查和修正。
- 访问客户威胁智能 (哈希、IP、URL、域等 ) 以阻止/通知恶意活动。

### <a name="streamline-it-and-security-management"></a>优化 IT 和安全管理

*提供对事件生命周期的更好的可视性和简化管理。*

- 聚合来自多个提供程序的警报以创建事件。
- 访问其他上下文以通知警报优先顺序和响应。
- 使警报状态在管理警报的系统之间保持同步。
- 深入了解安全状态，并提供有关如何使用安全分数进行改进的建议。

### <a name="share-threat-intelligence-to-enable-custom-detections"></a>共享威胁智能以启用自定义检测

*利用威胁情报对 Microsoft 解决方案中的自定义检测进行电源自定义。*

- 自动将威胁指示器发送到 Microsoft 安全解决方案，以启用警报、阻止或允许操作。
- 启用 swift 操作以防御新的威胁，如安全工具和工作流中的阻止文件、URL、域和 IP 地址。
- 客户提供的 TI 仅用于提供的客户，而不适用于任何其他 Microsoft 客户。

## <a name="technical-integrations-overview"></a>技术集成概述

Microsoft Graph 安全性 API 合作机会通过两个主要的集成途径提供，可独立使用或一起使用。  我们将概述高级要求，并深入了解如何考虑在这里购买这些途径，但详细的技术说明将留给本文档后面提到的文档。

支持的实体：

- **警报** 是 "对安全影响的结论"，而不是原始日志数据或其他不相关的信息。 [了解详细信息](/graph/api/resources/security-api-overview#alerts)。
- **威胁指示器** （也称为 "危害" 或 "IoCs" 的指示符）表示有关已知威胁（如恶意文件、url、域和 IP 地址）的数据。 客户可以通过内部威胁情报生成指示器，并从威胁智能社区、许可源和其他源中获取指示器。 [了解详细信息](/graph/api/resources/tiindicator)。
- 通过 **安全操作** ，技术合作伙伴可以通过图形公开功能功能。  例如，如果您的安全解决方案支持阻止 IP 地址的功能，则可以公开 "阻止 IP" 作为图形中的一项功能。 其他 Graph 安全 API 产品可以通过图形调用您的操作。 [了解详细信息](/graph/api/resources/securityaction)。
- **安全分数**.。。 [了解详细信息](/graph/api/resources/securescores)。

### <a name="integrate-your-application-with-the-microsoft-graph-security-api"></a>将应用程序与 Microsoft Graph 安全性 API 集成

所有集成的应用程序都 [必须注册](./auth-register-app-v2.md) 到 Microsoft Graph。 由单个客户使用的两个应用程序以及由许多客户使用的那些应用程序 (多租户) 受支持。  在这两种情况下，客户都必须向您的应用程序授予许可。 调用 Microsoft Graph 时，应用程序中的每个请求都将包含你的应用程序标识符和你代表其呼叫的客户。 支持以下类型的请求：

- **获取通知** –根据需要在筛选时获取警报信息。  例如：向我显示特定用户、主机等的所有高优先级警报或 "所有高优先级警报"。
- **更新警报状态** -启用通知生命周期管理。  例如：将警报状态设置为 "正在进行中" 或向警报添加注释。
- **获取安全分数** – Microsoft 安全分数是 microsoft 产品安全配置的 "信用等级" 类型值。
- **订阅** -允许通知通知或查询更改。
- **订阅源自定义威胁指标** -自动将威胁指示器发送到 Microsoft 安全解决方案，以启用警报、阻止或允许操作。 直接使用 Microsoft Graph 安全 API 或利用与主要威胁智能平台的集成。
- **调用 Microsoft Graph 安全操作** -立即采取行动以使用 Microsoft Graph security [securityActions](/graph/api/resources/securityaction) 实体防御威胁。

### <a name="enable-others-to-integrate-with-your-products-through-the-microsoft-graph-security-api"></a>允许其他人通过 Microsoft Graph 安全性 API 与你的产品集成

Microsoft Graph 安全提供程序通过 Microsoft Graph 让其他人可以使用其安全警报。  生成安全警报的 Microsoft 产品都具有将其各自的警报公开给 Microsoft Graph 的提供程序。 此外，Microsoft Graph 安全性 API 允许外部提供程序（作为 Microsoft 技术合作伙伴）共享来自 Microsoft Graph 中的应用程序的相关安全警报，供客户使用。 除了警报之外，Microsoft Graph Security securityActions 使技术合作伙伴能够通过 Microsoft Graph 公开功能功能。  例如，如果您的安全解决方案支持阻止 IP 地址的功能，则可以在 Microsoft Graph 中公开 "阻止 IP" 的功能。 其他 Microsoft Graph 安全产品可以通过 Microsoft Graph 调用您的操作。

Microsoft Graph 安全提供程序实质上是一个云终结点，它响应来自 Microsoft Graph 安全性 API 的请求，并返回相关的安全警报或对共同客户执行操作。 客户和服务到服务身份验证确保对客户通知和操作的访问受到保护。

提供程序方案的范围多种多样。 Curated 载入过程从确定相关方案开始。 在同意方案后，文档、示例代码和开发环境可用于支持 Microsoft Graph 安全提供程序的开发。

## <a name="get-started"></a>入门

### <a name="onboarding-guides-and-technical-documentation"></a>载入指南和技术文档

- [Microsoft Graph 安全性 API 概述](./security-concept-overview.md)
- [API 参考](/graph/api/resources/security-api-overview)
- [警报架构](/graph/api/resources/alert)
- [tiIndicator 架构](/graph/api/resources/tiindicator)
- [安全操作架构](/graph/api/resources/securityaction)
- [安全分数架构](/graph/api/resources/securescores)

### <a name="sample-code"></a>示例代码

- [Microsoft Graph 安全示例](https://aka.ms/graphsecurityapicode)
- [参与 Microsoft Graph 安全示例](https://aka.ms/graphsecurityapicodecontribute)

### <a name="help-and-support"></a>帮助和支持

- 如果你对使用 Microsoft Graph 安全 API 的应用程序或服务或产品集成有疑问，请访问 [Microsoft 安全图 API 技术社区](https://techcommunity.microsoft.com/t5/Using-Microsoft-Graph-Security/bd-p/SecurityGraphAPI)
- 在 [堆栈溢出](https://aka.ms/graphsecuritystackoverflow) 时跟踪标记： microsoft-安全性的讨论。
- 如果在各个 [示例存储库](https://github.com/microsoftgraph/security-api-solutions/blob/master/sample-repos.md)中发现示例或文档请求或 bug 文件中的 bug。
- 如果您有新的示例请求或不属于单个示例的问题，则[Microsoft Graph 安全解决方案存储库](https://github.com/microsoftgraph/security-api-solutions)中的[文件问题](https://github.com/microsoftgraph/security-api-solutions/issues/new)。

### <a name="getting-to-market"></a>进入市场

- [Microsoft 合作伙伴网络](https://partner.microsoft.com/) –与 microsoft 合作的主要计划是 Microsoft 合作伙伴网络。 Microsoft Graph 安全集成分为 [MPN 独立软件供应商 (ISV) ](https://partner.microsoft.com/isv-resource-hub) 班组。
- [Microsoft 智能安全关联](https://www.microsoft.com/security/partnerships/intelligent-security-association) 是专门为 Microsoft 安全合作伙伴提供的一种程序，可帮助丰富安全产品，并改进客户与 Microsoft 安全产品的集成的发现。
- Microsoft AppSource –作为 Microsoft Graph 安全性 API 合作伙伴，您可以 [在 Microsoft AppSource 市场中](https://appsource.microsoft.com/partners/signup)列出 microsoft graph 集成。