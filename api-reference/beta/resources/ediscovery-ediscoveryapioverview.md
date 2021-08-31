---
title: 使用 Microsoft Graph 电子数据展示 API
description: Microsoft 365 电子数据展示 API 为组织提供了自动执行重复任务的功能，并与现有电子数据展示工具集成，以构建基于行业法规可能需要的可重复工作流。可以使用能够电子数据展示 API 帮助满足你的法律需求。
ms.localizationpriority: high
author: mahage-msft
ms.prod: ediscovery
doc_type: conceptualPageType
ms.openlocfilehash: 239704caecba229e66959276effa77091965efa1
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/30/2021
ms.locfileid: "58696398"
---
# <a name="use-the-microsoft-graph-ediscovery-api"></a>使用 Microsoft Graph 电子数据展示 API

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Graph 电子数据展示 API 为组织提供了自动执行重复任务的功能，并与现有电子数据展示工具集成，以构建基于行业法规可能需要的可重复工作流。可以使用能够电子数据展示 API 帮助满足你的法律需求。

> [!IMPORTANT]
> 用于电子数据展示的 Microsoft Graph API 旨在用于诉讼、调查和法规请求的电子数据展示操作。 不应将这些 API 用作 Microsoft 365 系统或任何其他成批下载的日记数据的替代项。

> [!NOTE]
> 在预览版中，使用这些 API 可能需要订阅特定 Microsoft 产品，并且受 [Microsoft API 使用条款](/legal/microsoft-apis/terms-of-use?context=graph%252fcontext)的约束。  发行正式版后，Microsoft 可能会要求你或你的客户支付额外费用。
>
> 目前，Microsoft Graph 中的电子数据展示 API 仅适用于高级电子数据展示用例。

电子数据展示 API 在 OData 子名称space，microsoft.graph.ediscovery 中定义。 Microsoft Graph API 包括以下关键实体。

| 名称 | 类型       | 用例 |
|:-|:-|:-|
| 情况 | [microsoft.graph.ediscovery.case](ediscovery-case.md) | 电子数据展示事例是所有电子数据展示对象（包括保管人、保留、搜索、审阅集和导出）的容器。 |
| Custodian | [microsoft.graph.ediscovery.custodian](ediscovery-custodian.md) | 某人及其拥有管理控制权的数据。 识别保管人后， *高级电子数据* 可保留、搜索、挑选和导出其数据。 有关详细信息，请参阅 [电子数据展示服务中的保管人和非疑源](/microsoft-365/compliance/managing-custodians)。|
| 合法持有 | [microsoft.graph.ediscovery.legalHold](ediscovery-legalhold.md) | 用于保存内容以用于诉讼和法律目的。 不能混淆法定保留或将保留用作保留保留，保留通常用于遵守政府或行业法规。 若要了解有关详细信息，请参阅 [电子数据展示管理中的保留](https://docs.microsoft.com/microsoft-365/compliance/managing-holds)。|
| 审阅集| [microsoft.graph.ediscovery.reviewSet](ediscovery-reviewset.md) | 电子数据展示审阅集是一组以电子形式存储的信息静态集，用于诉讼、调查或法规请求。 |
| 创建审阅集查询 | [microsoft.graph.ediscovery.reviewSetQuery](ediscovery-reviewsetquery.md) | 电子数据展示审阅集查询用于发现、挑选、审阅和标记 [ESI](https://en.wikipedia.org/wiki/Electronically_stored_information_(Federal_Rules_of_Civil_Procedure))，最终目标是向请求者或对方法律顾问提供产品。|
| 源集合| [microsoft.graph.ediscovery.sourceCollection](ediscovery-sourcecollection.md)| 通常称为搜索，允许您从 Microsoft 365 实时服务（如 Exchange、SharePoint 和 Teams）收集数据。 可以将源集合添加到审阅集，以进一步挑选和最终导出与大小写相关的数据。 有关详细信息，请参阅 [电子数据展示中收集](/microsoft-365/compliance/collecting-data-for-ediscovery)。|
| 标记 | [microsoft.graph.ediscovery.tag](ediscovery-tag.md) | 用于审阅期间设置的审阅集，或挑选从无响应数据中挑选响应式数据，识别特权内容，或一般帮助完成审阅过程。  若要了解有关详细信息，请参阅 [电子数据展示功能中的审阅集内标记](/microsoft-365/compliance/tagging-documents)。|
