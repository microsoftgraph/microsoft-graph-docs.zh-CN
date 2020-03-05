---
title: insightIdentity
description: 包含共享项目的属性的复杂类型。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: fee67727e610e44ab8cfcf15f973160310575136
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42495870"
---
# <a name="insightidentity"></a><span data-ttu-id="30c26-103">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="30c26-103">insightIdentity</span></span>

<span data-ttu-id="30c26-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="30c26-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30c26-105">包含[sharedInsight](insights-shared.md)项目的属性的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="30c26-105">Complex type containing properties of [sharedInsight](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="30c26-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="30c26-106">JSON representation</span></span>
<span data-ttu-id="30c26-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="30c26-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="30c26-108">属性</span><span class="sxs-lookup"><span data-stu-id="30c26-108">Properties</span></span>

| <span data-ttu-id="30c26-109">属性</span><span class="sxs-lookup"><span data-stu-id="30c26-109">Property</span></span>              | <span data-ttu-id="30c26-110">类型</span><span class="sxs-lookup"><span data-stu-id="30c26-110">Type</span></span>          | <span data-ttu-id="30c26-111">说明</span><span class="sxs-lookup"><span data-stu-id="30c26-111">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="30c26-112">displayName</span><span class="sxs-lookup"><span data-stu-id="30c26-112">displayName</span></span>       | <span data-ttu-id="30c26-113">字符串</span><span class="sxs-lookup"><span data-stu-id="30c26-113">String</span></span>          | <span data-ttu-id="30c26-114">共享项目的用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="30c26-114">The display name of the user who shared the item.</span></span> |
| <span data-ttu-id="30c26-115">id</span><span class="sxs-lookup"><span data-stu-id="30c26-115">id</span></span>              | <span data-ttu-id="30c26-116">String</span><span class="sxs-lookup"><span data-stu-id="30c26-116">String</span></span>        | <span data-ttu-id="30c26-117">共享项的用户的 id。</span><span class="sxs-lookup"><span data-stu-id="30c26-117">The id of the user who shared the item.</span></span>     |
| <span data-ttu-id="30c26-118">address</span><span class="sxs-lookup"><span data-stu-id="30c26-118">address</span></span>             | <span data-ttu-id="30c26-119">String</span><span class="sxs-lookup"><span data-stu-id="30c26-119">String</span></span>      | <span data-ttu-id="30c26-120">共享项目的用户的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="30c26-120">The email address of the user who shared the item.</span></span>  |
