---
title: resourceReference 资源类型
description: 包含见解的属性的复杂类型。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: accd2b0b12f8068ea990fbd611b46053f66d6de4
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339984"
---
# <a name="resourcereference-resource-type"></a><span data-ttu-id="d75fd-103">resourceReference 资源类型</span><span class="sxs-lookup"><span data-stu-id="d75fd-103">resourceReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d75fd-104">包含[见解](officegraphinsights.md)的属性的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="d75fd-104">Complex type containing properties of [insights](officegraphinsights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="d75fd-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d75fd-105">JSON representation</span></span>

<span data-ttu-id="d75fd-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d75fd-106">Here is a JSON representation of the resource</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.resourceReference"
}-->
```json
{
  "webUrl": "string",
  "id": "string",
  "type": "string"
}
```

## <a name="properties"></a><span data-ttu-id="d75fd-107">属性</span><span class="sxs-lookup"><span data-stu-id="d75fd-107">Properties</span></span>

| <span data-ttu-id="d75fd-108">属性</span><span class="sxs-lookup"><span data-stu-id="d75fd-108">Property</span></span>      | <span data-ttu-id="d75fd-109">类型</span><span class="sxs-lookup"><span data-stu-id="d75fd-109">Type</span></span>      | <span data-ttu-id="d75fd-110">说明</span><span class="sxs-lookup"><span data-stu-id="d75fd-110">Description</span></span>  |
| ------------- |-----------| -------------|
| <span data-ttu-id="d75fd-111">WebUrl</span><span class="sxs-lookup"><span data-stu-id="d75fd-111">webUrl</span></span>        | <span data-ttu-id="d75fd-112">String</span><span class="sxs-lookup"><span data-stu-id="d75fd-112">String</span></span>    | <span data-ttu-id="d75fd-113">指向引用项的 URL。</span><span class="sxs-lookup"><span data-stu-id="d75fd-113">A URL leading to the referenced item.</span></span> |
| <span data-ttu-id="d75fd-114">id</span><span class="sxs-lookup"><span data-stu-id="d75fd-114">id</span></span>            | <span data-ttu-id="d75fd-115">String</span><span class="sxs-lookup"><span data-stu-id="d75fd-115">String</span></span>    | <span data-ttu-id="d75fd-116">项目的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d75fd-116">The item's unique identifier.</span></span>           |
| <span data-ttu-id="d75fd-117">type</span><span class="sxs-lookup"><span data-stu-id="d75fd-117">type</span></span>          | <span data-ttu-id="d75fd-118">String</span><span class="sxs-lookup"><span data-stu-id="d75fd-118">String</span></span>    | <span data-ttu-id="d75fd-119">一个可用于对项目进行分类的字符串值, 例如 "driveItem"</span><span class="sxs-lookup"><span data-stu-id="d75fd-119">A string value that can be used to classify the item, such as "microsoft.graph.driveItem"</span></span> |
