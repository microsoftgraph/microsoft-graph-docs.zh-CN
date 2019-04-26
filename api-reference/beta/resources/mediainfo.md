---
title: mediaInfo 资源类型
description: 在提示操作中使用的媒体信息。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4c6f8e4f4ceea184f9663c433672d0892ed92467
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342637"
---
# <a name="mediainfo-resource-type"></a><span data-ttu-id="8ba6b-103">mediaInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="8ba6b-103">mediaInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ba6b-104">在提示操作中使用的媒体信息。</span><span class="sxs-lookup"><span data-stu-id="8ba6b-104">The media information used in actions for prompts.</span></span>

## <a name="properties"></a><span data-ttu-id="8ba6b-105">属性</span><span class="sxs-lookup"><span data-stu-id="8ba6b-105">Properties</span></span>
| <span data-ttu-id="8ba6b-106">属性</span><span class="sxs-lookup"><span data-stu-id="8ba6b-106">Property</span></span>       | <span data-ttu-id="8ba6b-107">类型</span><span class="sxs-lookup"><span data-stu-id="8ba6b-107">Type</span></span>    | <span data-ttu-id="8ba6b-108">说明</span><span class="sxs-lookup"><span data-stu-id="8ba6b-108">Description</span></span>                      |
|:---------------|:--------|:---------------------------------|
| <span data-ttu-id="8ba6b-109">resourceId</span><span class="sxs-lookup"><span data-stu-id="8ba6b-109">resourceId</span></span>     | <span data-ttu-id="8ba6b-110">String</span><span class="sxs-lookup"><span data-stu-id="8ba6b-110">String</span></span>  | <span data-ttu-id="8ba6b-111">资源的唯一标识。</span><span class="sxs-lookup"><span data-stu-id="8ba6b-111">Unique identity of the resource.</span></span> |
| <span data-ttu-id="8ba6b-112">url</span><span class="sxs-lookup"><span data-stu-id="8ba6b-112">uri</span></span>            | <span data-ttu-id="8ba6b-113">String</span><span class="sxs-lookup"><span data-stu-id="8ba6b-113">String</span></span>  | <span data-ttu-id="8ba6b-114">资源的路径。</span><span class="sxs-lookup"><span data-stu-id="8ba6b-114">Path to the resource.</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="8ba6b-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8ba6b-115">JSON representation</span></span>

<span data-ttu-id="8ba6b-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8ba6b-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mediaInfo"
}-->
```json
{
  "resourceId": "String",
  "uri": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mediaInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
