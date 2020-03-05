---
title: callRoute 资源类型
description: CallRoute 类型。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 9a2ac5e0e8656cf6d7dcde2528d7ca000368d640
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507794"
---
# <a name="callroute-resource-type"></a><span data-ttu-id="9d092-103">callRoute 资源类型</span><span class="sxs-lookup"><span data-stu-id="9d092-103">callRoute resource type</span></span>

<span data-ttu-id="9d092-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="9d092-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d092-105">CallRoute 类型。</span><span class="sxs-lookup"><span data-stu-id="9d092-105">The callRoute type.</span></span>

## <a name="properties"></a><span data-ttu-id="9d092-106">属性</span><span class="sxs-lookup"><span data-stu-id="9d092-106">Properties</span></span>

| <span data-ttu-id="9d092-107">属性</span><span class="sxs-lookup"><span data-stu-id="9d092-107">Property</span></span>            | <span data-ttu-id="9d092-108">类型</span><span class="sxs-lookup"><span data-stu-id="9d092-108">Type</span></span>                          | <span data-ttu-id="9d092-109">说明</span><span class="sxs-lookup"><span data-stu-id="9d092-109">Description</span></span>                                                  |
| :------------------ | :---------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="9d092-110">终稿</span><span class="sxs-lookup"><span data-stu-id="9d092-110">final</span></span>               | [<span data-ttu-id="9d092-111">identitySet</span><span class="sxs-lookup"><span data-stu-id="9d092-111">identitySet</span></span>](identityset.md) | <span data-ttu-id="9d092-112">在呼叫中解析为的标识。</span><span class="sxs-lookup"><span data-stu-id="9d092-112">The identity that was resolved to in the call.</span></span>               |
| <span data-ttu-id="9d092-113">源语言</span><span class="sxs-lookup"><span data-stu-id="9d092-113">original</span></span>            | [<span data-ttu-id="9d092-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="9d092-114">identitySet</span></span>](identityset.md) | <span data-ttu-id="9d092-115">最初在呼叫中使用的标识。</span><span class="sxs-lookup"><span data-stu-id="9d092-115">The identity that was originally used in the call.</span></span>           |
| <span data-ttu-id="9d092-116">routingType</span><span class="sxs-lookup"><span data-stu-id="9d092-116">routingType</span></span>         | <span data-ttu-id="9d092-117">String</span><span class="sxs-lookup"><span data-stu-id="9d092-117">String</span></span>                        | <span data-ttu-id="9d092-118">可取值为：`forwarded`、`lookup`、`selfFork`。</span><span class="sxs-lookup"><span data-stu-id="9d092-118">Possible values are: `forwarded`, `lookup`, `selfFork`.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="9d092-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9d092-119">JSON representation</span></span>

<span data-ttu-id="9d092-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9d092-120">The following is a JSON representation of the resource.</span></span>

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
