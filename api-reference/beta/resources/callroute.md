---
title: callRoute 资源类型
description: CallRoute 类型。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9978bffd55f62f0646f84d2405df70eba6232d68
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974052"
---
# <a name="callroute-resource-type"></a><span data-ttu-id="53e4b-103">callRoute 资源类型</span><span class="sxs-lookup"><span data-stu-id="53e4b-103">callRoute resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53e4b-104">CallRoute 类型。</span><span class="sxs-lookup"><span data-stu-id="53e4b-104">The callRoute type.</span></span>

## <a name="properties"></a><span data-ttu-id="53e4b-105">属性</span><span class="sxs-lookup"><span data-stu-id="53e4b-105">Properties</span></span>

| <span data-ttu-id="53e4b-106">属性</span><span class="sxs-lookup"><span data-stu-id="53e4b-106">Property</span></span>            | <span data-ttu-id="53e4b-107">类型</span><span class="sxs-lookup"><span data-stu-id="53e4b-107">Type</span></span>                          | <span data-ttu-id="53e4b-108">说明</span><span class="sxs-lookup"><span data-stu-id="53e4b-108">Description</span></span>                                                  |
| :------------------ | :---------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="53e4b-109">终稿</span><span class="sxs-lookup"><span data-stu-id="53e4b-109">final</span></span>               | [<span data-ttu-id="53e4b-110">identitySet</span><span class="sxs-lookup"><span data-stu-id="53e4b-110">identitySet</span></span>](identityset.md) | <span data-ttu-id="53e4b-111">在呼叫中解析为的标识。</span><span class="sxs-lookup"><span data-stu-id="53e4b-111">The identity that was resolved to in the call.</span></span>               |
| <span data-ttu-id="53e4b-112">源语言</span><span class="sxs-lookup"><span data-stu-id="53e4b-112">original</span></span>            | [<span data-ttu-id="53e4b-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="53e4b-113">identitySet</span></span>](identityset.md) | <span data-ttu-id="53e4b-114">最初在呼叫中使用的标识。</span><span class="sxs-lookup"><span data-stu-id="53e4b-114">The identity that was originally used in the call.</span></span>           |
| <span data-ttu-id="53e4b-115">routingType</span><span class="sxs-lookup"><span data-stu-id="53e4b-115">routingType</span></span>         | <span data-ttu-id="53e4b-116">String</span><span class="sxs-lookup"><span data-stu-id="53e4b-116">String</span></span>                        | <span data-ttu-id="53e4b-117">可取值为：`forwarded`、`lookup`、`selfFork`。</span><span class="sxs-lookup"><span data-stu-id="53e4b-117">Possible values are: `forwarded`, `lookup`, `selfFork`.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="53e4b-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="53e4b-118">JSON representation</span></span>

<span data-ttu-id="53e4b-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="53e4b-119">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "callRoute resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
