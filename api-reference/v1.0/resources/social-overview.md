---
title: 使用 Microsoft Graph API 在应用程序中集成人员智能
description: Microsoft Graph 允许访问相关人员的有用数据以及与之交互的文档。
author: simonhult
ms.localizationpriority: high
ms.prod: insights
doc_type: conceptualPageType
ms.openlocfilehash: 4d78275f1a2a7489233d49ce950cd349efe1dea9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59032144"
---
# <a name="use-the-microsoft-graph-api-to-integrate-people-intelligence-in-an-app"></a>使用 Microsoft Graph API 在应用程序中集成人员智能

Microsoft Graph 允许访问相关人员的有用数据以及与之交互的文档。

## <a name="aggregate-and-extract-specific-information-about-people"></a>聚合并提取有关人员的特定信息

功能：人员

可使用 [person](../resources/person.md) 资源和人员 API 从邮件、联系人和社交网络中收集某位用户的相关信息。 根据多个通信和协作模式及业务关系按相关性对结果进行排序。 通过此 API 可基于自己的条件对人员进行浏览、排序、选择、筛选或搜索。

有关应用场景及示例，请参阅[获取相关人员的信息](/graph/people-example)。

若要使用此 API，请参阅下列内容：

- [列出人员](../api/user-list-people.md)


## <a name="help-users-get-the-most-relevant-documents-for-their-work"></a>帮助用户获得最相关的工作文档

功能：文档见解

使用见解 API 为用户标识最相关的文档：

- 列出用户[常用的](../api/insights-list-trending.md)文档
- 列出用户[使用的](../api/insights-list-used.md)文档
- 列出[与用户共享或由用户共享的](../api/insights-list-shared.md)文档

## <a name="whats-new"></a>最近更新
了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。
