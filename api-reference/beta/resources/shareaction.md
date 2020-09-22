---
author: daspek
description: ShareAction 资源提供了有关共享项的活动的信息。
ms.date: 09/14/2017
title: ShareAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 6d855b4c42a51e6ff9c9330f0a22e8076778d456
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48010190"
---
# <a name="shareaction-resource-type"></a><span data-ttu-id="86cdc-103">ShareAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="86cdc-103">ShareAction resource type</span></span>

<span data-ttu-id="86cdc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86cdc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86cdc-105">**ShareAction** 资源提供了有关共享项的[活动][activity]的信息。</span><span class="sxs-lookup"><span data-stu-id="86cdc-105">The **ShareAction** resource provides information about an [activity][activity] that shared an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="86cdc-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="86cdc-106">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.shareAction"
}-->

```json
{
  "recipients": [{"@odata.type": "microsoft.graph.identitySet"}]
}
```

## <a name="properties"></a><span data-ttu-id="86cdc-107">属性</span><span class="sxs-lookup"><span data-stu-id="86cdc-107">Properties</span></span>

| <span data-ttu-id="86cdc-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="86cdc-108">Property name</span></span> | <span data-ttu-id="86cdc-109">类型</span><span class="sxs-lookup"><span data-stu-id="86cdc-109">Type</span></span>                       | <span data-ttu-id="86cdc-110">说明</span><span class="sxs-lookup"><span data-stu-id="86cdc-110">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="86cdc-111">recipients</span><span class="sxs-lookup"><span data-stu-id="86cdc-111">recipients</span></span>    | <span data-ttu-id="86cdc-112">[identitySet][] 集合</span><span class="sxs-lookup"><span data-stu-id="86cdc-112">[identitySet][] collection</span></span> | <span data-ttu-id="86cdc-113">项在此操作中共享的标识。</span><span class="sxs-lookup"><span data-stu-id="86cdc-113">The identities the item was shared with in this action.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="86cdc-115">注解</span><span class="sxs-lookup"><span data-stu-id="86cdc-115">Remarks</span></span>

<span data-ttu-id="86cdc-116">项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="86cdc-116">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The ShareAction object provides information about who an item was shared to in a share action.",
  "keywords": "activities,activity,action,mention",
  "section": "documentation",
  "tocPath": "Resources/ShareAction",
  "suppressions": []
}
-->


