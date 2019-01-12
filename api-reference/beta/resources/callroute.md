---
title: callRoute 资源类型
description: CallRoute 类型。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: fd131afcdb5581a719107d9fd3a9a597979d6f21
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933069"
---
# <a name="callroute-resource-type"></a><span data-ttu-id="22654-103">callRoute 资源类型</span><span class="sxs-lookup"><span data-stu-id="22654-103">callRoute resource type</span></span>

> <span data-ttu-id="22654-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="22654-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="22654-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="22654-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="22654-106">CallRoute 类型。</span><span class="sxs-lookup"><span data-stu-id="22654-106">The callRoute type.</span></span>

## <a name="properties"></a><span data-ttu-id="22654-107">属性</span><span class="sxs-lookup"><span data-stu-id="22654-107">Properties</span></span>

| <span data-ttu-id="22654-108">属性</span><span class="sxs-lookup"><span data-stu-id="22654-108">Property</span></span>            | <span data-ttu-id="22654-109">类型</span><span class="sxs-lookup"><span data-stu-id="22654-109">Type</span></span>                          | <span data-ttu-id="22654-110">Description</span><span class="sxs-lookup"><span data-stu-id="22654-110">Description</span></span>                                                  |
| :------------------ | :---------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="22654-111">最终</span><span class="sxs-lookup"><span data-stu-id="22654-111">final</span></span>               | [<span data-ttu-id="22654-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="22654-112">identitySet</span></span>](identityset.md) | <span data-ttu-id="22654-113">解析为呼叫中的标识。</span><span class="sxs-lookup"><span data-stu-id="22654-113">The identity that was resolved to in the call.</span></span>               |
| <span data-ttu-id="22654-114">源语言</span><span class="sxs-lookup"><span data-stu-id="22654-114">original</span></span>            | [<span data-ttu-id="22654-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="22654-115">identitySet</span></span>](identityset.md) | <span data-ttu-id="22654-116">最初在呼叫中使用的标识。</span><span class="sxs-lookup"><span data-stu-id="22654-116">The identity that was originally used in the call.</span></span>           |
| <span data-ttu-id="22654-117">routingType</span><span class="sxs-lookup"><span data-stu-id="22654-117">routingType</span></span>         | <span data-ttu-id="22654-118">字符串</span><span class="sxs-lookup"><span data-stu-id="22654-118">String</span></span>                        | <span data-ttu-id="22654-119">可取值为：`forwarded`、`lookup`、`selfFork`。</span><span class="sxs-lookup"><span data-stu-id="22654-119">Possible values are: `forwarded`, `lookup`, `selfFork`.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="22654-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="22654-120">JSON representation</span></span>

<span data-ttu-id="22654-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="22654-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRoute"
}-->
```json
{
  "final": {"@odata.type": "#microsoft.graph.identitySet"},
  "original": {"@odata.type": "#microsoft.graph.identitySet"},
  "routingType": "forwarded | lookup | selfFork"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "callRoute resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
