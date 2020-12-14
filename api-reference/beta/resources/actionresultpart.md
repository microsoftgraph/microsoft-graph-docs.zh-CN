---
title: actionResultType 资源类型
description: 为批量操作的响应建模的抽象类型。
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a092fa4a322d0d207550947559cb5dfff4ad4625
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49663998"
---
# <a name="actionresultpart-resource-type"></a><span data-ttu-id="759ae-103">actionResultPart 资源类型</span><span class="sxs-lookup"><span data-stu-id="759ae-103">actionResultPart resource type</span></span>

<span data-ttu-id="759ae-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="759ae-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="759ae-105">用作批量操作响应建模基础的抽象类型。</span><span class="sxs-lookup"><span data-stu-id="759ae-105">An abstract type that serves as a base for modeling responses of bulk operations.</span></span> <span data-ttu-id="759ae-106">根据 **响应** 是否表示错误，选择性地填充错误属性。</span><span class="sxs-lookup"><span data-stu-id="759ae-106">The **error** property is selectively populated based on whether the response represents an error.</span></span>

## <a name="properties"></a><span data-ttu-id="759ae-107">属性</span><span class="sxs-lookup"><span data-stu-id="759ae-107">Properties</span></span>

| <span data-ttu-id="759ae-108">属性</span><span class="sxs-lookup"><span data-stu-id="759ae-108">Property</span></span> | <span data-ttu-id="759ae-109">类型</span><span class="sxs-lookup"><span data-stu-id="759ae-109">Type</span></span>   | <span data-ttu-id="759ae-110">说明</span><span class="sxs-lookup"><span data-stu-id="759ae-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="759ae-111">error</span><span class="sxs-lookup"><span data-stu-id="759ae-111">error</span></span>|[<span data-ttu-id="759ae-112">publicError</span><span class="sxs-lookup"><span data-stu-id="759ae-112">publicError</span></span>](publicerror.md) |<span data-ttu-id="759ae-113">在批量操作过程中发生的错误（如果有）。</span><span class="sxs-lookup"><span data-stu-id="759ae-113">The error that occurred, if any, during the course of the bulk operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="759ae-114">关系</span><span class="sxs-lookup"><span data-stu-id="759ae-114">Relationships</span></span>
<span data-ttu-id="759ae-115">无。</span><span class="sxs-lookup"><span data-stu-id="759ae-115">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="759ae-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="759ae-116">JSON representation</span></span>
<span data-ttu-id="759ae-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="759ae-117">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.actionResultPart"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.actionResultPart",
  "error": {
    "@odata.type": "microsoft.graph.publicError"
  }
}
```
## <a name="see-also"></a><span data-ttu-id="759ae-118">另请参阅</span><span class="sxs-lookup"><span data-stu-id="759ae-118">See also</span></span>

- [<span data-ttu-id="759ae-119">aadUserConversationMemberResult</span><span class="sxs-lookup"><span data-stu-id="759ae-119">aadUserConversationMemberResult</span></span>](aadUserConversationMemberResult.md)
- [<span data-ttu-id="759ae-120">将成员批量添加到团队</span><span class="sxs-lookup"><span data-stu-id="759ae-120">Add members in bulk to team</span></span>](../api/conversationmembers-add.md)

<!-- uuid: 20fd7863-9545-40d4-ae8f-fee2d115a690
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "actionResultPart",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


