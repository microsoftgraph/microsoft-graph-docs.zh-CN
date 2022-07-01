---
title: 将 Exchange Web Services (EWS) 应用迁移到 Microsoft Graph
description: 由于不再对用于Exchange Online的 EWS API 进行积极投资，因此可以将访问 Exchange Online 的 EWS 应用迁移到 Microsoft Graph。
author: sumithra-maran
ms.localizationpriority: medium
ms.prod: exchange
doc_type: conceptualPageType
ms.openlocfilehash: 53fb8e4df5a5211fb275dde9d2b646459b63dfc2
ms.sourcegitcommit: af9489bd42a25dff04836dcfcc57369259fda587
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2022
ms.locfileid: "66577726"
---
# <a name="migrate-exchange-web-services-ews-apps-to-microsoft-graph"></a>将 Exchange Web Services (EWS) 应用迁移到 Microsoft Graph

[Exchange Web Services (EWS) ](/exchange/client-developer/exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange)是自 2007 Exchange Server以来一直使用的旧协议。 2018 年 8 月，[Microsoft 宣布](https://techcommunity.microsoft.com/t5/exchange-team-blog/upcoming-changes-to-exchange-web-services-ews-api-for-office-365/ba-p/608055)不会对用于 Exchange Online 的 EWS API 进行任何积极投资。 强烈建议将访问Exchange Online的 EWS 应用迁移到 Microsoft Graph。

## <a name="why-use-microsoft-graph"></a>为什么要使用 Microsoft Graph？

Microsoft Graph 在安全性、简单性和效率方面提供了对 EWS 的改进。 切换到 Microsoft Graph 以利用这些改进，所有改进都通过一个终结点进行。

### <a name="security"></a>安全性

Microsoft Graph 具有更严格的安全和治理策略，其中包含 OAuth 和 [粒度范围，以限制邮箱中的数据访问，](/graph/permissions-reference) 而不是 EWS 中的全部或无访问模型。

### <a name="developer-simplicity"></a>开发人员简单性

Microsoft Graph 提供 [Graph 资源管理器](https://developer.microsoft.com/graph/graph-explorer) ，用于轻松快速地发现和测试 API、不同编程语言中的 [SDK](/graph/sdks/sdks-overview) 以及活跃的开发人员社区。

### <a name="rest-efficiency"></a>REST 效率

Microsoft Graph API 基于 REST，其中 EWS API 基于 SOAP。 使用基于 REST 的协议的优势包括更快的 JSON 序列化和更低的网络使用率。

## <a name="next-steps"></a>后续步骤

- 了解 Microsoft Graph 和 EWS [中的身份验证差异](migrate-exchange-web-services-authentication.md) 。
- 查看 [API 映射](migrate-exchange-web-services-api-mapping.md) ，查找当前使用的 EWS API 的 Microsoft Graph 等效项。
- 探索 [Microsoft Graph](/graph/overview) 概念和做法。
- 使用 [Graph 资源管理器](https://developer.microsoft.com/graph/graph-explorer) 试验 Microsoft Graph。
