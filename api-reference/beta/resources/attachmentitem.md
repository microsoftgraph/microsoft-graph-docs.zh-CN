---
title: attachmentItem 资源类型
description: 表示要附加的项的属性。
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 14213afcaf555b21816a3b3ccf2481c1555c4b90
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48040173"
---
# <a name="attachmentitem-resource-type"></a><span data-ttu-id="21984-103">attachmentItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="21984-103">attachmentItem resource type</span></span>

<span data-ttu-id="21984-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21984-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21984-105">表示要附加的项的属性。</span><span class="sxs-lookup"><span data-stu-id="21984-105">Represents attributes of an item to be attached.</span></span>

## <a name="properties"></a><span data-ttu-id="21984-106">属性</span><span class="sxs-lookup"><span data-stu-id="21984-106">Properties</span></span>

| <span data-ttu-id="21984-107">属性</span><span class="sxs-lookup"><span data-stu-id="21984-107">Property</span></span>     | <span data-ttu-id="21984-108">类型</span><span class="sxs-lookup"><span data-stu-id="21984-108">Type</span></span>        | <span data-ttu-id="21984-109">说明</span><span class="sxs-lookup"><span data-stu-id="21984-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="21984-110">attachmentType</span><span class="sxs-lookup"><span data-stu-id="21984-110">attachmentType</span></span>|<span data-ttu-id="21984-111">String</span><span class="sxs-lookup"><span data-stu-id="21984-111">String</span></span>| <span data-ttu-id="21984-112">附件的类型。</span><span class="sxs-lookup"><span data-stu-id="21984-112">The type of attachment.</span></span> <span data-ttu-id="21984-113">可取值为：`file`、`item`、`reference`。</span><span class="sxs-lookup"><span data-stu-id="21984-113">Possible values are: `file`, `item`, `reference`.</span></span> <span data-ttu-id="21984-114">此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="21984-114">Required.</span></span>|
|<span data-ttu-id="21984-115">contentType</span><span class="sxs-lookup"><span data-stu-id="21984-115">contentType</span></span>|<span data-ttu-id="21984-116">String</span><span class="sxs-lookup"><span data-stu-id="21984-116">String</span></span>|<span data-ttu-id="21984-117">附件中的数据的性质。</span><span class="sxs-lookup"><span data-stu-id="21984-117">The nature of the data in the attachment.</span></span> <span data-ttu-id="21984-118">可选。</span><span class="sxs-lookup"><span data-stu-id="21984-118">Optional.</span></span>|
|<span data-ttu-id="21984-119">isInline</span><span class="sxs-lookup"><span data-stu-id="21984-119">isInline</span></span>|<span data-ttu-id="21984-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="21984-120">Boolean</span></span>|<span data-ttu-id="21984-121">如果附件是内嵌附件，则为 `true`；否则为 `false`。</span><span class="sxs-lookup"><span data-stu-id="21984-121">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span> <span data-ttu-id="21984-122">可选。</span><span class="sxs-lookup"><span data-stu-id="21984-122">Optional.</span></span>|
|<span data-ttu-id="21984-123">name</span><span class="sxs-lookup"><span data-stu-id="21984-123">name</span></span>|<span data-ttu-id="21984-124">String</span><span class="sxs-lookup"><span data-stu-id="21984-124">String</span></span>|<span data-ttu-id="21984-125">附件的显示名称。</span><span class="sxs-lookup"><span data-stu-id="21984-125">The display name of the attachment.</span></span> <span data-ttu-id="21984-126">它可以是描述性字符串，不必是实际的文件名。</span><span class="sxs-lookup"><span data-stu-id="21984-126">This can be a descriptive string and does not have to be the actual file name.</span></span> <span data-ttu-id="21984-127">必需。</span><span class="sxs-lookup"><span data-stu-id="21984-127">Required.</span></span>|
|<span data-ttu-id="21984-128">size</span><span class="sxs-lookup"><span data-stu-id="21984-128">size</span></span>|<span data-ttu-id="21984-129">Int64</span><span class="sxs-lookup"><span data-stu-id="21984-129">Int64</span></span>|<span data-ttu-id="21984-130">附件大小，以字节为单位。</span><span class="sxs-lookup"><span data-stu-id="21984-130">The length of the attachment in bytes.</span></span> <span data-ttu-id="21984-131">此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="21984-131">Required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="21984-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="21984-132">JSON representation</span></span>

<span data-ttu-id="21984-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="21984-133">The following is a JSON representation of the resource.</span></span>

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

