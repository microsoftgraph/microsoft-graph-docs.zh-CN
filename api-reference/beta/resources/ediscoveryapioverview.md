---
title: 使用 Microsoft Graph 电子数据展示 API
description: Microsoft 365 电子数据展示 API 为组织提供了自动化重复任务的功能，并与现有的电子数据展示工具集成，以构建基于行业法规可能需要的可重复工作流。 可使用电子数据展示 API 来协助你的法律需求。
localization_priority: Priority
author: mahage-msft
ms.prod: compliance
doc_type: conceptualPageType
ms.openlocfilehash: c9ae9561908456b0954060e95a08abdc394c9767
ms.sourcegitcommit: 82f9200355841c30f7a7487861d79e17256ff788
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/15/2020
ms.locfileid: "48479933"
---
# <a name="use-the-microsoft-graph-ediscovery-api"></a>使用 Microsoft Graph 电子数据展示 API

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于电子数据展示的 Microsoft Graph API 为组织提供了自动化重复任务的功能，并与现有的电子数据展示工具集成，以构建基于行业法规可能需要的可重复工作流。 可使用电子数据展示 API 来协助你的法律需求。

> [!IMPORTANT]
> 用于电子数据展示的 Microsoft Graph API 旨在用于诉讼、调查和法规请求的电子数据展示操作。 不应将这些 API 用作 Microsoft 365 系统或任何其他成批下载的日记数据的替代项。

> [!NOTE]
> 在预览版中，使用这些 API 可能需要订阅特定 Microsoft 产品，并且受 [Microsoft API 使用条款](/legal/microsoft-apis/terms-of-use?context=graph%252fcontext)的约束。  发行正式版后，Microsoft 可能会要求你或你的客户支付额外费用。
>
> 目前，Microsoft Graph 中的电子数据展示 API 仅适用于高级电子数据展示用例。

Microsoft Graph API 包括以下关键实体。

| 名称 | 类型       | 用例 |
|:-|:-|:-|
| 电子数据展示事例 | [ediscoveryCase](ediscoverycase.md) | 电子数据展示事例是所有电子数据展示对象（包括保管人、保留、搜索、审阅集和导出）的容器。 |
| 电子数据展示审阅集| [reviewSet](reviewset.md) | 电子数据展示审阅集是一组以电子形式存储的信息静态集，用于诉讼、调查或法规请求。 |
| 电子数据展示审阅集查询 | [reviewSetQuery](reviewsetquery.md) | 电子数据展示审阅集查询用于发现、挑选、审阅和标记 [ESI](https://en.wikipedia.org/wiki/Electronically_stored_information_(Federal_Rules_of_Civil_Procedure))，最终目标是向请求者或对方法律顾问提供产品。
