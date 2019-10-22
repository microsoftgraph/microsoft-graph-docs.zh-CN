---
title: attachmentItem 资源类型
description: 表示要附加的项的属性。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: b6570b44bab06c0ab4b8b6788ea585276b43c3cc
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2019
ms.locfileid: "37621636"
---
# <a name="attachmentitem-resource-type"></a><span data-ttu-id="b2c9a-103">attachmentItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="b2c9a-103">attachmentItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2c9a-104">表示要附加的项的属性。</span><span class="sxs-lookup"><span data-stu-id="b2c9a-104">Represents attributes of an item to be attached.</span></span>

## <a name="properties"></a><span data-ttu-id="b2c9a-105">属性</span><span class="sxs-lookup"><span data-stu-id="b2c9a-105">Properties</span></span>

| <span data-ttu-id="b2c9a-106">属性</span><span class="sxs-lookup"><span data-stu-id="b2c9a-106">Property</span></span>     | <span data-ttu-id="b2c9a-107">类型</span><span class="sxs-lookup"><span data-stu-id="b2c9a-107">Type</span></span>        | <span data-ttu-id="b2c9a-108">说明</span><span class="sxs-lookup"><span data-stu-id="b2c9a-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b2c9a-109">attachmentType</span><span class="sxs-lookup"><span data-stu-id="b2c9a-109">attachmentType</span></span>|<span data-ttu-id="b2c9a-110">String</span><span class="sxs-lookup"><span data-stu-id="b2c9a-110">String</span></span>| <span data-ttu-id="b2c9a-111">附件的类型。</span><span class="sxs-lookup"><span data-stu-id="b2c9a-111">The type of attachment.</span></span> <span data-ttu-id="b2c9a-112">可取值为：`file`、`item`、`reference`。</span><span class="sxs-lookup"><span data-stu-id="b2c9a-112">Possible values are: `file`, `item`, `reference`.</span></span> <span data-ttu-id="b2c9a-113">此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="b2c9a-113">Required.</span></span>|
|<span data-ttu-id="b2c9a-114">contentType</span><span class="sxs-lookup"><span data-stu-id="b2c9a-114">contentType</span></span>|<span data-ttu-id="b2c9a-115">String</span><span class="sxs-lookup"><span data-stu-id="b2c9a-115">String</span></span>|<span data-ttu-id="b2c9a-116">附件中的数据的性质。</span><span class="sxs-lookup"><span data-stu-id="b2c9a-116">The nature of the data in the attachment.</span></span> <span data-ttu-id="b2c9a-117">可选。</span><span class="sxs-lookup"><span data-stu-id="b2c9a-117">Optional.</span></span>|
|<span data-ttu-id="b2c9a-118">isInline</span><span class="sxs-lookup"><span data-stu-id="b2c9a-118">isInline</span></span>|<span data-ttu-id="b2c9a-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2c9a-119">Boolean</span></span>|<span data-ttu-id="b2c9a-120">如果附件是内嵌附件，则为 `true`；否则为 `false`。</span><span class="sxs-lookup"><span data-stu-id="b2c9a-120">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span> <span data-ttu-id="b2c9a-121">可选。</span><span class="sxs-lookup"><span data-stu-id="b2c9a-121">Optional.</span></span>|
|<span data-ttu-id="b2c9a-122">name</span><span class="sxs-lookup"><span data-stu-id="b2c9a-122">name</span></span>|<span data-ttu-id="b2c9a-123">String</span><span class="sxs-lookup"><span data-stu-id="b2c9a-123">String</span></span>|<span data-ttu-id="b2c9a-124">附件的显示名称。</span><span class="sxs-lookup"><span data-stu-id="b2c9a-124">The display name of the attachment.</span></span> <span data-ttu-id="b2c9a-125">它可以是描述性字符串，不必是实际的文件名。</span><span class="sxs-lookup"><span data-stu-id="b2c9a-125">This can be a descriptive string and does not have to be the actual file name.</span></span> <span data-ttu-id="b2c9a-126">必填。</span><span class="sxs-lookup"><span data-stu-id="b2c9a-126">Required.</span></span>|
|<span data-ttu-id="b2c9a-127">size</span><span class="sxs-lookup"><span data-stu-id="b2c9a-127">size</span></span>|<span data-ttu-id="b2c9a-128">Int64</span><span class="sxs-lookup"><span data-stu-id="b2c9a-128">Int64</span></span>|<span data-ttu-id="b2c9a-129">附件大小，以字节为单位。</span><span class="sxs-lookup"><span data-stu-id="b2c9a-129">The length of the attachment in bytes.</span></span> <span data-ttu-id="b2c9a-130">此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="b2c9a-130">Required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b2c9a-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b2c9a-131">JSON representation</span></span>

<span data-ttu-id="b2c9a-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b2c9a-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "contentType",
    "isInline"
  ],
  "@odata.type": "microsoft.graph.attachmentItem",
  "baseType": null
}-->

```json
{
  "attachmentType": "String",
  "contentType": "String",
  "isInline": true,
  "name": "String",
  "size": 1024
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attachmentItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->