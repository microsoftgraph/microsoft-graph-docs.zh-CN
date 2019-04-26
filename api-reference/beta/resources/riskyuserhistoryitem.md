---
title: riskyUserHistoryItem 资源类型
description: ''
author: ''
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7143fffecee52747109674e81e5bfbd9860df7f9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343554"
---
# <a name="riskyuserhistoryitem-resource-type"></a><span data-ttu-id="20eaa-102">riskyUserHistoryItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="20eaa-102">riskyUserHistoryItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="20eaa-103">属性</span><span class="sxs-lookup"><span data-stu-id="20eaa-103">Properties</span></span>

| <span data-ttu-id="20eaa-104">属性</span><span class="sxs-lookup"><span data-stu-id="20eaa-104">Property</span></span>       | <span data-ttu-id="20eaa-105">类型</span><span class="sxs-lookup"><span data-stu-id="20eaa-105">Type</span></span>    | <span data-ttu-id="20eaa-106">说明</span><span class="sxs-lookup"><span data-stu-id="20eaa-106">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="20eaa-107">userId</span><span class="sxs-lookup"><span data-stu-id="20eaa-107">userId</span></span>         | <span data-ttu-id="20eaa-108">string</span><span class="sxs-lookup"><span data-stu-id="20eaa-108">string</span></span>  |             |
| <span data-ttu-id="20eaa-109">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="20eaa-109">initiatedBy</span></span>    | <span data-ttu-id="20eaa-110">布尔值</span><span class="sxs-lookup"><span data-stu-id="20eaa-110">bool</span></span>    |             |
| <span data-ttu-id="20eaa-111">activity</span><span class="sxs-lookup"><span data-stu-id="20eaa-111">activity</span></span>       | [<span data-ttu-id="20eaa-112">riskUserActivity</span><span class="sxs-lookup"><span data-stu-id="20eaa-112">riskUserActivity</span></span>](riskuseractivity.md)| |

## <a name="json-representation"></a><span data-ttu-id="20eaa-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="20eaa-113">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.riskyUserHistoryItem",
  "baseType": "microsoft.graph.riskyUser"
}-->

```json
{
    "userId": "string",
    "initiatedBy": "bool",
    "activity": {"@odata.type": "microsoft.graph.riskUserActivity"}
}
```


<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
   
  ]
}
-->
