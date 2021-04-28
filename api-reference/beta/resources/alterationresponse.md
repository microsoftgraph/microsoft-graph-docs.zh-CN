---
title: 更改response 资源类型
description: 提供与更改响应中的拼写更正有关的信息。
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: e23b94b4e35776b2278c7818efc71f14edcc6cbb
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067996"
---
# <a name="alterationresponse-resource-type"></a><span data-ttu-id="d361f-103">更改response 资源类型</span><span class="sxs-lookup"><span data-stu-id="d361f-103">alterationResponse resource type</span></span>

<span data-ttu-id="d361f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d361f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d361f-105">提供与更改响应中的拼写更正有关的信息。</span><span class="sxs-lookup"><span data-stu-id="d361f-105">Provides information related to spelling corrections in the alteration response.</span></span>

## <a name="properties"></a><span data-ttu-id="d361f-106">属性</span><span class="sxs-lookup"><span data-stu-id="d361f-106">Properties</span></span>

| <span data-ttu-id="d361f-107">属性</span><span class="sxs-lookup"><span data-stu-id="d361f-107">Property</span></span>     | <span data-ttu-id="d361f-108">类型</span><span class="sxs-lookup"><span data-stu-id="d361f-108">Type</span></span>        | <span data-ttu-id="d361f-109">说明</span><span class="sxs-lookup"><span data-stu-id="d361f-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d361f-110">originalQueryString</span><span class="sxs-lookup"><span data-stu-id="d361f-110">originalQueryString</span></span>|<span data-ttu-id="d361f-111">String</span><span class="sxs-lookup"><span data-stu-id="d361f-111">String</span></span>| <span data-ttu-id="d361f-112">定义原始用户查询字符串。</span><span class="sxs-lookup"><span data-stu-id="d361f-112">Defines the original user query string.</span></span>|
|<span data-ttu-id="d361f-113">queryAlteration</span><span class="sxs-lookup"><span data-stu-id="d361f-113">queryAlteration</span></span>|[<span data-ttu-id="d361f-114">searchAlteration</span><span class="sxs-lookup"><span data-stu-id="d361f-114">searchAlteration</span></span>](searchalteration.md)| <span data-ttu-id="d361f-115">定义拼写更正更改信息的详细信息。</span><span class="sxs-lookup"><span data-stu-id="d361f-115">Defines the details of alteration information for the spelling correction.</span></span>|
|<span data-ttu-id="d361f-116">queryAlterationType</span><span class="sxs-lookup"><span data-stu-id="d361f-116">queryAlterationType</span></span>|<span data-ttu-id="d361f-117">searchAlterationType</span><span class="sxs-lookup"><span data-stu-id="d361f-117">searchAlterationType</span></span>| <span data-ttu-id="d361f-118">定义拼写更正的类型。</span><span class="sxs-lookup"><span data-stu-id="d361f-118">Defines the type of the spelling correction.</span></span> <span data-ttu-id="d361f-119">可能的值是 `suggestion` `modification` 、。</span><span class="sxs-lookup"><span data-stu-id="d361f-119">Possible values are `suggestion`, `modification`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d361f-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d361f-120">JSON representation</span></span>

<span data-ttu-id="d361f-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d361f-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alterationResponse",
  "baseType": null
}-->

```json
{
  "originalQueryString": "String",
  "queryAlteration": "String",
  "queryAlterationType": "suggestion"
}
```
