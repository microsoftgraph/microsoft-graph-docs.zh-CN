---
title: insightIdentity
description: 包含共享项目的属性的复杂类型。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 8718ab248dada75f04d92d6a8717dd4f43ee8106
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333594"
---
# <a name="insightidentity"></a><span data-ttu-id="64eed-103">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="64eed-103">insightIdentity</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64eed-104">包含[共享](insights-shared.md)项目的属性的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="64eed-104">Complex type containing properties of [Shared](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="64eed-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="64eed-105">JSON representation</span></span>
<span data-ttu-id="64eed-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="64eed-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="64eed-107">属性</span><span class="sxs-lookup"><span data-stu-id="64eed-107">Properties</span></span>

| <span data-ttu-id="64eed-108">属性</span><span class="sxs-lookup"><span data-stu-id="64eed-108">Property</span></span>              | <span data-ttu-id="64eed-109">类型</span><span class="sxs-lookup"><span data-stu-id="64eed-109">Type</span></span>          | <span data-ttu-id="64eed-110">说明</span><span class="sxs-lookup"><span data-stu-id="64eed-110">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="64eed-111">displayName</span><span class="sxs-lookup"><span data-stu-id="64eed-111">displayName</span></span>       | <span data-ttu-id="64eed-112">字符串</span><span class="sxs-lookup"><span data-stu-id="64eed-112">String</span></span>          | <span data-ttu-id="64eed-113">共享项目的用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="64eed-113">The display name of the user who shared the item.</span></span> |
| <span data-ttu-id="64eed-114">id</span><span class="sxs-lookup"><span data-stu-id="64eed-114">id</span></span>              | <span data-ttu-id="64eed-115">String</span><span class="sxs-lookup"><span data-stu-id="64eed-115">String</span></span>        | <span data-ttu-id="64eed-116">共享项的用户的 id。</span><span class="sxs-lookup"><span data-stu-id="64eed-116">The id of the user who shared the item.</span></span>     |
| <span data-ttu-id="64eed-117">address</span><span class="sxs-lookup"><span data-stu-id="64eed-117">address</span></span>             | <span data-ttu-id="64eed-118">String</span><span class="sxs-lookup"><span data-stu-id="64eed-118">String</span></span>      | <span data-ttu-id="64eed-119">共享项目的用户的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="64eed-119">The email address of the user who shared the item.</span></span>  |
