---
title: insightIdentity
description: 包含共享项目的属性的复杂类型。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 418b991ff24613fa46c3adc6e7a98474ffa4e2b1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021887"
---
# <a name="insightidentity"></a><span data-ttu-id="46a62-103">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="46a62-103">insightIdentity</span></span>

<span data-ttu-id="46a62-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46a62-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46a62-105">包含 [sharedInsight](insights-shared.md) 项目的属性的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="46a62-105">Complex type containing properties of [sharedInsight](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="46a62-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="46a62-106">JSON representation</span></span>
<span data-ttu-id="46a62-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="46a62-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.insightIdentity"
}-->
```json
{
  "displayName": "string",
  "id": "string",
  "address": "string"
}
```

## <a name="properties"></a><span data-ttu-id="46a62-108">属性</span><span class="sxs-lookup"><span data-stu-id="46a62-108">Properties</span></span>

| <span data-ttu-id="46a62-109">属性</span><span class="sxs-lookup"><span data-stu-id="46a62-109">Property</span></span>              | <span data-ttu-id="46a62-110">类型</span><span class="sxs-lookup"><span data-stu-id="46a62-110">Type</span></span>          | <span data-ttu-id="46a62-111">说明</span><span class="sxs-lookup"><span data-stu-id="46a62-111">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="46a62-112">displayName</span><span class="sxs-lookup"><span data-stu-id="46a62-112">displayName</span></span>       | <span data-ttu-id="46a62-113">String</span><span class="sxs-lookup"><span data-stu-id="46a62-113">String</span></span>          | <span data-ttu-id="46a62-114">共享项目的用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="46a62-114">The display name of the user who shared the item.</span></span> |
| <span data-ttu-id="46a62-115">id</span><span class="sxs-lookup"><span data-stu-id="46a62-115">id</span></span>              | <span data-ttu-id="46a62-116">String</span><span class="sxs-lookup"><span data-stu-id="46a62-116">String</span></span>        | <span data-ttu-id="46a62-117">共享项的用户的 id。</span><span class="sxs-lookup"><span data-stu-id="46a62-117">The id of the user who shared the item.</span></span>     |
| <span data-ttu-id="46a62-118">address</span><span class="sxs-lookup"><span data-stu-id="46a62-118">address</span></span>             | <span data-ttu-id="46a62-119">String</span><span class="sxs-lookup"><span data-stu-id="46a62-119">String</span></span>      | <span data-ttu-id="46a62-120">共享项目的用户的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="46a62-120">The email address of the user who shared the item.</span></span>  |


