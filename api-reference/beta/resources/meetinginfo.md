---
title: meetingInfo 资源类型
description: 指定用于创建或加入会议的会议信息。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: da3e89e0aa28868debd4b6ea98291fa88b42bb0b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966851"
---
# <a name="meetinginfo-resource-type"></a><span data-ttu-id="ab2f6-103">meetingInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="ab2f6-103">meetingInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab2f6-104">指定用于创建或加入会议的会议信息。</span><span class="sxs-lookup"><span data-stu-id="ab2f6-104">Meeting information specified to create or join a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="ab2f6-105">属性</span><span class="sxs-lookup"><span data-stu-id="ab2f6-105">Properties</span></span>

| <span data-ttu-id="ab2f6-106">属性</span><span class="sxs-lookup"><span data-stu-id="ab2f6-106">Property</span></span>       | <span data-ttu-id="ab2f6-107">类型</span><span class="sxs-lookup"><span data-stu-id="ab2f6-107">Type</span></span>    | <span data-ttu-id="ab2f6-108">说明</span><span class="sxs-lookup"><span data-stu-id="ab2f6-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ab2f6-109">allowConversationWithoutHost</span><span class="sxs-lookup"><span data-stu-id="ab2f6-109">allowConversationWithoutHost</span></span> | <span data-ttu-id="ab2f6-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="ab2f6-110">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="ab2f6-111">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ab2f6-111">JSON representation</span></span>

<span data-ttu-id="ab2f6-112">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ab2f6-112">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
