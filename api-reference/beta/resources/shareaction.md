---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ShareAction
ms.openlocfilehash: c9f06c7a4a6351b8a6554c944c0efe9af379e030
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045648"
---
# <a name="shareaction-resource-type"></a><span data-ttu-id="199fd-102">ShareAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="199fd-102">ShareAction resource type</span></span>

> <span data-ttu-id="199fd-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="199fd-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="199fd-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="199fd-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="199fd-105">**ShareAction** 资源提供了有关共享项的[活动][activity]的信息。</span><span class="sxs-lookup"><span data-stu-id="199fd-105">The **ShareAction** resource provides information about an [activity][activity] that shared an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="199fd-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="199fd-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="199fd-107">属性</span><span class="sxs-lookup"><span data-stu-id="199fd-107">Properties</span></span>

| <span data-ttu-id="199fd-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="199fd-108">Property name</span></span> | <span data-ttu-id="199fd-109">类型</span><span class="sxs-lookup"><span data-stu-id="199fd-109">Type</span></span>                       | <span data-ttu-id="199fd-110">说明</span><span class="sxs-lookup"><span data-stu-id="199fd-110">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="199fd-111">recipients</span><span class="sxs-lookup"><span data-stu-id="199fd-111">recipients</span></span>    | <span data-ttu-id="199fd-112">[identitySet][] 集合</span><span class="sxs-lookup"><span data-stu-id="199fd-112">[identitySet][] collection</span></span> | <span data-ttu-id="199fd-113">项在此操作中共享的标识。</span><span class="sxs-lookup"><span data-stu-id="199fd-113">The identities the item was shared with in this action.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="199fd-115">注解</span><span class="sxs-lookup"><span data-stu-id="199fd-115">Remarks</span></span>

<span data-ttu-id="199fd-116">项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="199fd-116">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The ShareAction object provides information about who an item was shared to in a share action.",
  "keywords": "activities,activity,action,mention",
  "section": "documentation",
  "tocPath": "Resources/ShareAction"
} -->
