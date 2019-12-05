---
title: insightIdentity
description: 包含共享项目的属性的复杂类型。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 1dc952ba931e1a0cb4302dac881f2d5ec015c591
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/05/2019
ms.locfileid: "39844356"
---
# <a name="insightidentity"></a><span data-ttu-id="753d1-103">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="753d1-103">insightIdentity</span></span>

<span data-ttu-id="753d1-104">包含[sharedInsight](insights-shared.md)项目的属性的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="753d1-104">Complex type containing properties of [sharedInsight](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="753d1-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="753d1-105">JSON representation</span></span>
<span data-ttu-id="753d1-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="753d1-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="753d1-107">属性</span><span class="sxs-lookup"><span data-stu-id="753d1-107">Properties</span></span>

| <span data-ttu-id="753d1-108">属性</span><span class="sxs-lookup"><span data-stu-id="753d1-108">Property</span></span>              | <span data-ttu-id="753d1-109">类型</span><span class="sxs-lookup"><span data-stu-id="753d1-109">Type</span></span>          | <span data-ttu-id="753d1-110">说明</span><span class="sxs-lookup"><span data-stu-id="753d1-110">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="753d1-111">displayName</span><span class="sxs-lookup"><span data-stu-id="753d1-111">displayName</span></span>       | <span data-ttu-id="753d1-112">字符串</span><span class="sxs-lookup"><span data-stu-id="753d1-112">String</span></span>          | <span data-ttu-id="753d1-113">共享项目的用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="753d1-113">The display name of the user who shared the item.</span></span> |
| <span data-ttu-id="753d1-114">id</span><span class="sxs-lookup"><span data-stu-id="753d1-114">id</span></span>              | <span data-ttu-id="753d1-115">String</span><span class="sxs-lookup"><span data-stu-id="753d1-115">String</span></span>        | <span data-ttu-id="753d1-116">共享项的用户的 id。</span><span class="sxs-lookup"><span data-stu-id="753d1-116">The id of the user who shared the item.</span></span>     |
| <span data-ttu-id="753d1-117">address</span><span class="sxs-lookup"><span data-stu-id="753d1-117">address</span></span>             | <span data-ttu-id="753d1-118">String</span><span class="sxs-lookup"><span data-stu-id="753d1-118">String</span></span>      | <span data-ttu-id="753d1-119">共享项目的用户的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="753d1-119">The email address of the user who shared the item.</span></span>  |
