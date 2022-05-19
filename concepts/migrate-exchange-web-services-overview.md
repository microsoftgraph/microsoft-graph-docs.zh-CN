---
title: 将 Exchange Web 服务 (EWS) 应用迁移到 Microsoft Graph
description: 介绍如何将 Exchange Web 服务 (EWS) 应用迁移到 Microsoft Graph。
author: sumithra-maran
ms.localizationpriority: medium
ms.prod: exchange
doc_type: conceptualPageType
ms.openlocfilehash: dcc9d75e82fa2a6b09298a8b5068f2c55e2a8be4
ms.sourcegitcommit: 562dc670cea411de0ecc232840ce1c650abbe34c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2022
ms.locfileid: "65549601"
---
# <a name="migrate-exchange-web-services-ews-apps-to-microsoft-graph"></a>将 Exchange Web 服务 (EWS) 应用迁移到 Microsoft Graph

[Exchange Web 服务 (EWS) ](/exchange/client-developer/exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange)是自 2007 Exchange Server以来一直使用的旧协议。 2018 年 8 月，[Microsoft 宣布](https://techcommunity.microsoft.com/t5/exchange-team-blog/upcoming-changes-to-exchange-web-services-ews-api-for-office-365/ba-p/608055)不会对用于 Exchange Online 的 EWS API 进行任何积极投资。 强烈建议将访问Exchange Online的 EWS 应用迁移到 Microsoft Graph。

## <a name="why-use-microsoft-graph"></a>为什么要使用 Microsoft Graph？

Microsoft Graph在安全性、简单性和效率方面对 EWS 进行了改进。 切换到 Microsoft Graph以利用这些改进，所有这些改进都是通过一个终结点实现的。

### <a name="security"></a>安全性

Microsoft Graph具有更严格的安全和治理策略，其中包含 OAuth 和[粒度范围，以限制邮箱中的数据访问，](/graph/permissions-reference)而不是 EWS 中的全部或无访问模型。

### <a name="developer-simplicity"></a>开发人员简单性

Microsoft Graph提供[Graph资源管理器](https://developer.microsoft.com/graph/graph-explorer)，用于轻松快速地发现和测试 API、不同编程语言的 [SDK](/graph/sdks/sdks-overview) 以及活跃的开发人员社区。

### <a name="rest-efficiency"></a>REST 效率

Microsoft Graph API 基于 REST，其中 EWS API 基于 SOAP。 使用基于 REST 的协议的优势包括更快的 JSON 序列化和更低的网络使用率。

## <a name="next-steps"></a>后续步骤

- 了解 Microsoft Graph 和 EWS [中的身份验证差异](migrate-exchange-web-services-authentication.md)。
- 查看 [API 映射](migrate-exchange-web-services-api-mapping.md)，查找当前使用的 EWS API 的 Microsoft Graph 等效项。
- 了解 [Microsoft Graph](/graph/overview)概念和做法。
- 使用[Graph资源管理器](https://developer.microsoft.com/graph/graph-explorer)试验 Microsoft Graph。
