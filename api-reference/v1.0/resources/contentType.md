---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ContentType
localization_priority: Normal
description: ContentType 资源代表 SharePoint 中的内容类型。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: b26f9b7a3bafb7b6185aa781c1f842f7c20adab3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029636"
---
# <a name="contenttype-resource-type"></a><span data-ttu-id="7d871-103">ContentType 资源类型</span><span class="sxs-lookup"><span data-stu-id="7d871-103">ContentType resource type</span></span>

<span data-ttu-id="7d871-104">**ContentType** 资源代表 SharePoint 中的_内容类型_。</span><span class="sxs-lookup"><span data-stu-id="7d871-104">The **contentType** resource represents a _content type_ in SharePoint.</span></span>
<span data-ttu-id="7d871-105">内容类型允许您定义一组列, 这些列必须存在于列表中[\*\*\*\*][listItem]的每个[**列表**][list]中。</span><span class="sxs-lookup"><span data-stu-id="7d871-105">Content types allow you to define a set of columns that must be present on every [**listItem**][listItem] in a [**list**][list].</span></span>

[list]: list.md
[listItem]: listitem.md

## <a name="json-representation"></a><span data-ttu-id="7d871-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7d871-106">JSON representation</span></span>

<span data-ttu-id="7d871-107">下面是 **contentType** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7d871-107">Here is a JSON representation of a **contentType** resource.</span></span>
<!-- {
  "blockType": "resource",
 "baseType": "microsoft.graph.entity",
 "@odata.type": "microsoft.graph.contentType" } -->

```json
{
  "description": "string",
  "group": "string",
  "hidden": false,
  "id": "string",
  "inheritedFrom": { "@type": "microsoft.graph.itemReference" },
  "name": "string",
  "order": { "@type": "microsoft.graph.contentTypeOrder" },
  "parentId": "string",
  "readOnly": false,
  "sealed": false,

  "columnLinks": [{ "@type": "microsoft.graph.columnLink" }]
}
```

## <a name="properties"></a><span data-ttu-id="7d871-108">属性</span><span class="sxs-lookup"><span data-stu-id="7d871-108">Properties</span></span>

| <span data-ttu-id="7d871-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="7d871-109">Property name</span></span>     | <span data-ttu-id="7d871-110">类型</span><span class="sxs-lookup"><span data-stu-id="7d871-110">Type</span></span>                 | <span data-ttu-id="7d871-111">说明</span><span class="sxs-lookup"><span data-stu-id="7d871-111">Description</span></span>
|:------------------|:---------------------|:----------------------------------
| <span data-ttu-id="7d871-112">**说明**</span><span class="sxs-lookup"><span data-stu-id="7d871-112">**description**</span></span>   | <span data-ttu-id="7d871-113">string</span><span class="sxs-lookup"><span data-stu-id="7d871-113">string</span></span>               | <span data-ttu-id="7d871-114">项目的描述性文本。</span><span class="sxs-lookup"><span data-stu-id="7d871-114">The descriptive text for the item.</span></span>
| <span data-ttu-id="7d871-115">**group**</span><span class="sxs-lookup"><span data-stu-id="7d871-115">**group**</span></span>         | <span data-ttu-id="7d871-116">string</span><span class="sxs-lookup"><span data-stu-id="7d871-116">string</span></span>               | <span data-ttu-id="7d871-117">此内容类型所属的组的名称。</span><span class="sxs-lookup"><span data-stu-id="7d871-117">The name of the group this content type belongs to.</span></span> <span data-ttu-id="7d871-118">可以帮助组织相关的内容类型。</span><span class="sxs-lookup"><span data-stu-id="7d871-118">Helps organize related content types.</span></span>
| <span data-ttu-id="7d871-119">**hidden**</span><span class="sxs-lookup"><span data-stu-id="7d871-119">**hidden**</span></span>        | <span data-ttu-id="7d871-120">boolean</span><span class="sxs-lookup"><span data-stu-id="7d871-120">boolean</span></span>              | <span data-ttu-id="7d871-121">指示内容类型是否隐藏于此列表的“新建”菜单中。</span><span class="sxs-lookup"><span data-stu-id="7d871-121">Indicates whether the content type is hidden in the list's 'New' menu.</span></span>
| <span data-ttu-id="7d871-122">**id**</span><span class="sxs-lookup"><span data-stu-id="7d871-122">**id**</span></span>            | <span data-ttu-id="7d871-123">string</span><span class="sxs-lookup"><span data-stu-id="7d871-123">string</span></span>               | <span data-ttu-id="7d871-124">内容类型的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="7d871-124">The unique identifier of the content type.</span></span>
| <span data-ttu-id="7d871-125">**inheritedFrom**</span><span class="sxs-lookup"><span data-stu-id="7d871-125">**inheritedFrom**</span></span> | <span data-ttu-id="7d871-126">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="7d871-126">[itemReference][]</span></span>    | <span data-ttu-id="7d871-127">如果此内容类型继承自另一个作用域（如某个站点），则会提供对在其中定义内容类型的项的引用。</span><span class="sxs-lookup"><span data-stu-id="7d871-127">If this content type is inherited from another scope (like a site), provides a reference to the item where the content type is defined.</span></span>
| <span data-ttu-id="7d871-128">**name**</span><span class="sxs-lookup"><span data-stu-id="7d871-128">**name**</span></span>          | <span data-ttu-id="7d871-129">string</span><span class="sxs-lookup"><span data-stu-id="7d871-129">string</span></span>               | <span data-ttu-id="7d871-130">内容类型的名称。</span><span class="sxs-lookup"><span data-stu-id="7d871-130">The name of the content type.</span></span>
| <span data-ttu-id="7d871-131">**order**</span><span class="sxs-lookup"><span data-stu-id="7d871-131">**order**</span></span>         | <span data-ttu-id="7d871-132">[contentTypeOrder][]</span><span class="sxs-lookup"><span data-stu-id="7d871-132">[contentTypeOrder][]</span></span> | <span data-ttu-id="7d871-133">指定在选择 UI 中显示内容类型的顺序。</span><span class="sxs-lookup"><span data-stu-id="7d871-133">Specifies the order in which the content type appears in the selection UI.</span></span>
| <span data-ttu-id="7d871-134">**parentId**</span><span class="sxs-lookup"><span data-stu-id="7d871-134">**parentId**</span></span>      | <span data-ttu-id="7d871-135">string</span><span class="sxs-lookup"><span data-stu-id="7d871-135">string</span></span>               | <span data-ttu-id="7d871-136">内容类型的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="7d871-136">The unique identifier of the content type.</span></span>
| <span data-ttu-id="7d871-137">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="7d871-137">**readOnly**</span></span>      | <span data-ttu-id="7d871-138">boolean</span><span class="sxs-lookup"><span data-stu-id="7d871-138">boolean</span></span>              | <span data-ttu-id="7d871-139">如果为 `true`，则不能修改内容类型，除非此值首次设置为 `false`。</span><span class="sxs-lookup"><span data-stu-id="7d871-139">If `true`, the content type cannot be modified unless this value is first set to `false`.</span></span>
| <span data-ttu-id="7d871-140">**sealed**</span><span class="sxs-lookup"><span data-stu-id="7d871-140">**sealed**</span></span>        | <span data-ttu-id="7d871-141">boolean</span><span class="sxs-lookup"><span data-stu-id="7d871-141">boolean</span></span>              | <span data-ttu-id="7d871-142">如果为 `true`，则不能由用户或通过下推操作修改内容类型。</span><span class="sxs-lookup"><span data-stu-id="7d871-142">If `true`, the content type cannot be modified by users or through push-down operations.</span></span> <span data-ttu-id="7d871-143">只有网站集管理员可以密封或解封内容类型。</span><span class="sxs-lookup"><span data-stu-id="7d871-143">Only site collection administrators can seal or unseal content types.</span></span>

## <a name="relationships"></a><span data-ttu-id="7d871-144">关系</span><span class="sxs-lookup"><span data-stu-id="7d871-144">Relationships</span></span>

| <span data-ttu-id="7d871-145">属性名</span><span class="sxs-lookup"><span data-stu-id="7d871-145">Property name</span></span>   | <span data-ttu-id="7d871-146">类型</span><span class="sxs-lookup"><span data-stu-id="7d871-146">Type</span></span>                      | <span data-ttu-id="7d871-147">说明</span><span class="sxs-lookup"><span data-stu-id="7d871-147">Description</span></span>
|:----------------|:--------------------------|:-------------------------------
| <span data-ttu-id="7d871-148">**columnLinks**</span><span class="sxs-lookup"><span data-stu-id="7d871-148">**columnLinks**</span></span> | <span data-ttu-id="7d871-149">[columnLink][] 集合</span><span class="sxs-lookup"><span data-stu-id="7d871-149">[columnLink][] collection</span></span> | <span data-ttu-id="7d871-150">此内容类型所需的列集合</span><span class="sxs-lookup"><span data-stu-id="7d871-150">The collection of columns that are required by this content type</span></span>

<span data-ttu-id="7d871-151">请参阅[内容类型和内容类型发布简介][contentTypeIntro]了解详细信息。</span><span class="sxs-lookup"><span data-stu-id="7d871-151">See [Introduction to content types and content type publishing][contentTypeIntro] for more information.</span></span>

[columnLink]: columnlink.md
[contentTypeIntro]: https://support.office.com/en-us/article/Introduction-to-content-types-and-content-type-publishing-e1277a2e-a1e8-4473-9126-91a0647766e5
[itemReference]: itemreference.md
[contentTypeOrder]: contenttypeorder.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentType"
} -->
