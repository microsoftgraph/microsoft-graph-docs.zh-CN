---
title: riskyUserHistoryItem 资源类型
description: ''
author: ''
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7143fffecee52747109674e81e5bfbd9860df7f9
ms.sourcegitcommit: 9fd437a77da99d8436d6c852edd99a9ba873f8cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/09/2019
ms.locfileid: "31688497"
---
# <a name="riskyuserhistoryitem-resource-type"></a><span data-ttu-id="84e76-102">riskyUserHistoryItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="84e76-102">riskyUserHistoryItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="84e76-103">属性</span><span class="sxs-lookup"><span data-stu-id="84e76-103">Properties</span></span>

| <span data-ttu-id="84e76-104">属性</span><span class="sxs-lookup"><span data-stu-id="84e76-104">Property</span></span>       | <span data-ttu-id="84e76-105">类型</span><span class="sxs-lookup"><span data-stu-id="84e76-105">Type</span></span>    | <span data-ttu-id="84e76-106">描述</span><span class="sxs-lookup"><span data-stu-id="84e76-106">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="84e76-107">userId</span><span class="sxs-lookup"><span data-stu-id="84e76-107">userId</span></span>         | <span data-ttu-id="84e76-108">string</span><span class="sxs-lookup"><span data-stu-id="84e76-108">string</span></span>  |             |
| <span data-ttu-id="84e76-109">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="84e76-109">initiatedBy</span></span>    | <span data-ttu-id="84e76-110">bool</span><span class="sxs-lookup"><span data-stu-id="84e76-110">bool</span></span>    |             |
| <span data-ttu-id="84e76-111">activity</span><span class="sxs-lookup"><span data-stu-id="84e76-111">activity</span></span>       | [<span data-ttu-id="84e76-112">riskUserActivity</span><span class="sxs-lookup"><span data-stu-id="84e76-112">riskUserActivity</span></span>](riskuseractivity.md)| |

## <a name="json-representation"></a><span data-ttu-id="84e76-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="84e76-113">JSON representation</span></span>

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
