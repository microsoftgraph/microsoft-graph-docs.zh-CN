---
title: 将 Exchange Web 服务 (EWS) 应用程序迁移到 Microsoft Graph
description: 介绍如何将 EWS Exchange Web 服务 (EWS) 迁移到 Microsoft Graph。
author: sumithra-maran
ms.localizationpriority: medium
ms.prod: exchange
doc_type: conceptualPageType
ms.openlocfilehash: 029c27940ee98b9f6b9d9077e79dc704df143e9e
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63516547"
---
# <a name="migrate-exchange-web-services-ews-apps-to-microsoft-graph"></a>将 Exchange Web 服务 (EWS) 应用程序迁移到 Microsoft Graph

[Exchange EWS (EWS) ](/exchange/client-developer/exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange) 是自 2007 以来一直使用的旧Exchange Server协议。 2018 年 8 月[，Microsoft](https://techcommunity.microsoft.com/t5/exchange-team-blog/upcoming-changes-to-exchange-web-services-ews-api-for-office-365/ba-p/608055) 宣布将不会对用于 EWS API 的任何活动Exchange Online。 我们强烈建议将访问 Microsoft Exchange Online的 EWS Graph。

## <a name="why-use-microsoft-graph"></a>为什么使用 Microsoft Graph？

Microsoft Graph 在安全性、简单性和效率方面对 EWS 进行了改进。 切换到 Microsoft Graph利用这些改进，全部通过一个终结点实现。

### <a name="security"></a>安全性

Microsoft Graph OAuth 和粒度范围具有更严格的安全和治理策略，以限制邮箱中的数据访问，而不是 EWS 中的全部访问模型或无访问模型。

### <a name="developer-simplicity"></a>开发人员的简单性

Microsoft Graph提供了[Graph](https://developer.microsoft.com/graph/graph-explorer)资源管理器，以轻松快速地发现和测试 API、使用不同编程语言的 SDK 以及活动的开发人员社区。

### <a name="rest-efficiency"></a>REST 效率

Microsoft Graph API 基于 REST，其中 EWS API 基于 SOAP。 使用基于 REST 的协议的优点包括更快的 JSON 序列化和更低的网络使用率。

## <a name="next-steps"></a>后续步骤

- 了解 Microsoft [Graph](migrate-exchange-web-services-authentication.md) 和 EWS 中的身份验证差异。
- 查看 [API 映射](migrate-exchange-web-services-api-mapping.md)以查找 Microsoft Graph当前使用的 EWS API 的等效项。
- 了解 [Microsoft Graph](/graph/overview)概念和做法。
- 使用[Graph资源管理器](https://developer.microsoft.com/graph/graph-explorer)尝试 Microsoft Graph。
