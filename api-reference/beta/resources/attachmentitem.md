---
title: attachmentItem 资源类型
description: 表示要附加的项目的属性。
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: a469ff035b63c16b422a23d4ffad91dbc361157f
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130288"
---
# <a name="attachmentitem-resource-type"></a><span data-ttu-id="e68aa-103">attachmentItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="e68aa-103">attachmentItem resource type</span></span>

<span data-ttu-id="e68aa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e68aa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e68aa-105">表示要附加的项目的属性。</span><span class="sxs-lookup"><span data-stu-id="e68aa-105">Represents attributes of an item to be attached.</span></span>

## <a name="properties"></a><span data-ttu-id="e68aa-106">属性</span><span class="sxs-lookup"><span data-stu-id="e68aa-106">Properties</span></span>

| <span data-ttu-id="e68aa-107">属性</span><span class="sxs-lookup"><span data-stu-id="e68aa-107">Property</span></span>     | <span data-ttu-id="e68aa-108">类型</span><span class="sxs-lookup"><span data-stu-id="e68aa-108">Type</span></span>        | <span data-ttu-id="e68aa-109">说明</span><span class="sxs-lookup"><span data-stu-id="e68aa-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e68aa-110">attachmentType</span><span class="sxs-lookup"><span data-stu-id="e68aa-110">attachmentType</span></span>|<span data-ttu-id="e68aa-111">字符串</span><span class="sxs-lookup"><span data-stu-id="e68aa-111">String</span></span>| <span data-ttu-id="e68aa-112">附件的类型。</span><span class="sxs-lookup"><span data-stu-id="e68aa-112">The type of attachment.</span></span> <span data-ttu-id="e68aa-113">可取值为：`file`、`item`、`reference`。</span><span class="sxs-lookup"><span data-stu-id="e68aa-113">Possible values are: `file`, `item`, `reference`.</span></span> <span data-ttu-id="e68aa-114">此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="e68aa-114">Required.</span></span>|
|<span data-ttu-id="e68aa-115">contentType</span><span class="sxs-lookup"><span data-stu-id="e68aa-115">contentType</span></span>|<span data-ttu-id="e68aa-116">String</span><span class="sxs-lookup"><span data-stu-id="e68aa-116">String</span></span>|<span data-ttu-id="e68aa-117">附件中数据的性质。</span><span class="sxs-lookup"><span data-stu-id="e68aa-117">The nature of the data in the attachment.</span></span> <span data-ttu-id="e68aa-118">可选。</span><span class="sxs-lookup"><span data-stu-id="e68aa-118">Optional.</span></span>|
|<span data-ttu-id="e68aa-119">isInline</span><span class="sxs-lookup"><span data-stu-id="e68aa-119">isInline</span></span>|<span data-ttu-id="e68aa-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="e68aa-120">Boolean</span></span>|<span data-ttu-id="e68aa-121">如果附件是内嵌附件，则为 `true`；否则为 `false`。</span><span class="sxs-lookup"><span data-stu-id="e68aa-121">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span> <span data-ttu-id="e68aa-122">可选。</span><span class="sxs-lookup"><span data-stu-id="e68aa-122">Optional.</span></span>|
|<span data-ttu-id="e68aa-123">name</span><span class="sxs-lookup"><span data-stu-id="e68aa-123">name</span></span>|<span data-ttu-id="e68aa-124">String</span><span class="sxs-lookup"><span data-stu-id="e68aa-124">String</span></span>|<span data-ttu-id="e68aa-125">附件的显示名称。</span><span class="sxs-lookup"><span data-stu-id="e68aa-125">The display name of the attachment.</span></span> <span data-ttu-id="e68aa-126">它可以是一个描述性字符串，不一定就是实际的文件名。</span><span class="sxs-lookup"><span data-stu-id="e68aa-126">This can be a descriptive string and does not have to be the actual file name.</span></span> <span data-ttu-id="e68aa-127">必填。</span><span class="sxs-lookup"><span data-stu-id="e68aa-127">Required.</span></span>|
|<span data-ttu-id="e68aa-128">size</span><span class="sxs-lookup"><span data-stu-id="e68aa-128">size</span></span>|<span data-ttu-id="e68aa-129">Int64</span><span class="sxs-lookup"><span data-stu-id="e68aa-129">Int64</span></span>|<span data-ttu-id="e68aa-130">附件大小，以字节为单位。</span><span class="sxs-lookup"><span data-stu-id="e68aa-130">The length of the attachment in bytes.</span></span> <span data-ttu-id="e68aa-131">此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="e68aa-131">Required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e68aa-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e68aa-132">JSON representation</span></span>

<span data-ttu-id="e68aa-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e68aa-133">The following is a JSON representation of the resource.</span></span>

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

