---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ContentType
localization_priority: Normal
description: ContentType 资源代表 SharePoint 中的内容类型。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 71652c2e314cd4f86a7bf0a957b1df937aa0d2e3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48056966"
---
# <a name="contenttype-resource-type"></a><span data-ttu-id="85ad7-103">ContentType 资源类型</span><span class="sxs-lookup"><span data-stu-id="85ad7-103">ContentType resource type</span></span>

<span data-ttu-id="85ad7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85ad7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="85ad7-105">**ContentType** 资源代表 SharePoint 中的_内容类型_。</span><span class="sxs-lookup"><span data-stu-id="85ad7-105">The **contentType** resource represents a _content type_ in SharePoint.</span></span>
<span data-ttu-id="85ad7-106">内容类型允许您定义一组列，这些列必须存在于列表中 [**的**][listItem] 每个 [**列表**][list]中。</span><span class="sxs-lookup"><span data-stu-id="85ad7-106">Content types allow you to define a set of columns that must be present on every [**listItem**][listItem] in a [**list**][list].</span></span>

[list]: list.md
[listItem]: listitem.md

## <a name="json-representation"></a><span data-ttu-id="85ad7-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="85ad7-107">JSON representation</span></span>

<span data-ttu-id="85ad7-108">下面是 **contentType** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="85ad7-108">Here is a JSON representation of a **contentType** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="85ad7-109">属性</span><span class="sxs-lookup"><span data-stu-id="85ad7-109">Properties</span></span>

| <span data-ttu-id="85ad7-110">属性名称</span><span class="sxs-lookup"><span data-stu-id="85ad7-110">Property name</span></span>     | <span data-ttu-id="85ad7-111">类型</span><span class="sxs-lookup"><span data-stu-id="85ad7-111">Type</span></span>                 | <span data-ttu-id="85ad7-112">说明</span><span class="sxs-lookup"><span data-stu-id="85ad7-112">Description</span></span>
|:------------------|:---------------------|:----------------------------------
| <span data-ttu-id="85ad7-113">**说明**</span><span class="sxs-lookup"><span data-stu-id="85ad7-113">**description**</span></span>   | <span data-ttu-id="85ad7-114">string</span><span class="sxs-lookup"><span data-stu-id="85ad7-114">string</span></span>               | <span data-ttu-id="85ad7-115">项目的描述性文本。</span><span class="sxs-lookup"><span data-stu-id="85ad7-115">The descriptive text for the item.</span></span>
| <span data-ttu-id="85ad7-116">**group**</span><span class="sxs-lookup"><span data-stu-id="85ad7-116">**group**</span></span>         | <span data-ttu-id="85ad7-117">string</span><span class="sxs-lookup"><span data-stu-id="85ad7-117">string</span></span>               | <span data-ttu-id="85ad7-118">此内容类型所属的组的名称。</span><span class="sxs-lookup"><span data-stu-id="85ad7-118">The name of the group this content type belongs to.</span></span> <span data-ttu-id="85ad7-119">可以帮助组织相关的内容类型。</span><span class="sxs-lookup"><span data-stu-id="85ad7-119">Helps organize related content types.</span></span>
| <span data-ttu-id="85ad7-120">**hidden**</span><span class="sxs-lookup"><span data-stu-id="85ad7-120">**hidden**</span></span>        | <span data-ttu-id="85ad7-121">boolean</span><span class="sxs-lookup"><span data-stu-id="85ad7-121">boolean</span></span>              | <span data-ttu-id="85ad7-122">指示内容类型是否隐藏于此列表的“新建”菜单中。</span><span class="sxs-lookup"><span data-stu-id="85ad7-122">Indicates whether the content type is hidden in the list's 'New' menu.</span></span>
| <span data-ttu-id="85ad7-123">**id**</span><span class="sxs-lookup"><span data-stu-id="85ad7-123">**id**</span></span>            | <span data-ttu-id="85ad7-124">string</span><span class="sxs-lookup"><span data-stu-id="85ad7-124">string</span></span>               | <span data-ttu-id="85ad7-125">内容类型的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="85ad7-125">The unique identifier of the content type.</span></span>
| <span data-ttu-id="85ad7-126">**inheritedFrom**</span><span class="sxs-lookup"><span data-stu-id="85ad7-126">**inheritedFrom**</span></span> | <span data-ttu-id="85ad7-127">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="85ad7-127">[itemReference][]</span></span>    | <span data-ttu-id="85ad7-128">如果此内容类型继承自另一个作用域（如某个站点），则会提供对在其中定义内容类型的项的引用。</span><span class="sxs-lookup"><span data-stu-id="85ad7-128">If this content type is inherited from another scope (like a site), provides a reference to the item where the content type is defined.</span></span>
| <span data-ttu-id="85ad7-129">**name**</span><span class="sxs-lookup"><span data-stu-id="85ad7-129">**name**</span></span>          | <span data-ttu-id="85ad7-130">string</span><span class="sxs-lookup"><span data-stu-id="85ad7-130">string</span></span>               | <span data-ttu-id="85ad7-131">内容类型的名称。</span><span class="sxs-lookup"><span data-stu-id="85ad7-131">The name of the content type.</span></span>
| <span data-ttu-id="85ad7-132">**order**</span><span class="sxs-lookup"><span data-stu-id="85ad7-132">**order**</span></span>         | <span data-ttu-id="85ad7-133">[contentTypeOrder][]</span><span class="sxs-lookup"><span data-stu-id="85ad7-133">[contentTypeOrder][]</span></span> | <span data-ttu-id="85ad7-134">指定在选择 UI 中显示内容类型的顺序。</span><span class="sxs-lookup"><span data-stu-id="85ad7-134">Specifies the order in which the content type appears in the selection UI.</span></span>
| <span data-ttu-id="85ad7-135">**parentId**</span><span class="sxs-lookup"><span data-stu-id="85ad7-135">**parentId**</span></span>      | <span data-ttu-id="85ad7-136">string</span><span class="sxs-lookup"><span data-stu-id="85ad7-136">string</span></span>               | <span data-ttu-id="85ad7-137">内容类型的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="85ad7-137">The unique identifier of the content type.</span></span>
| <span data-ttu-id="85ad7-138">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="85ad7-138">**readOnly**</span></span>      | <span data-ttu-id="85ad7-139">boolean</span><span class="sxs-lookup"><span data-stu-id="85ad7-139">boolean</span></span>              | <span data-ttu-id="85ad7-140">如果为 `true`，则不能修改内容类型，除非此值首次设置为 `false`。</span><span class="sxs-lookup"><span data-stu-id="85ad7-140">If `true`, the content type cannot be modified unless this value is first set to `false`.</span></span>
| <span data-ttu-id="85ad7-141">**sealed**</span><span class="sxs-lookup"><span data-stu-id="85ad7-141">**sealed**</span></span>        | <span data-ttu-id="85ad7-142">boolean</span><span class="sxs-lookup"><span data-stu-id="85ad7-142">boolean</span></span>              | <span data-ttu-id="85ad7-143">如果为 `true`，则不能由用户或通过下推操作修改内容类型。</span><span class="sxs-lookup"><span data-stu-id="85ad7-143">If `true`, the content type cannot be modified by users or through push-down operations.</span></span> <span data-ttu-id="85ad7-144">只有网站集管理员可以密封或解封内容类型。</span><span class="sxs-lookup"><span data-stu-id="85ad7-144">Only site collection administrators can seal or unseal content types.</span></span>

## <a name="relationships"></a><span data-ttu-id="85ad7-145">关系</span><span class="sxs-lookup"><span data-stu-id="85ad7-145">Relationships</span></span>

| <span data-ttu-id="85ad7-146">属性名称</span><span class="sxs-lookup"><span data-stu-id="85ad7-146">Property name</span></span>   | <span data-ttu-id="85ad7-147">类型</span><span class="sxs-lookup"><span data-stu-id="85ad7-147">Type</span></span>                      | <span data-ttu-id="85ad7-148">说明</span><span class="sxs-lookup"><span data-stu-id="85ad7-148">Description</span></span>
|:----------------|:--------------------------|:-------------------------------
| <span data-ttu-id="85ad7-149">**columnLinks**</span><span class="sxs-lookup"><span data-stu-id="85ad7-149">**columnLinks**</span></span> | <span data-ttu-id="85ad7-150">[columnLink][] 集合</span><span class="sxs-lookup"><span data-stu-id="85ad7-150">[columnLink][] collection</span></span> | <span data-ttu-id="85ad7-151">此内容类型所需的列集合</span><span class="sxs-lookup"><span data-stu-id="85ad7-151">The collection of columns that are required by this content type</span></span>

<span data-ttu-id="85ad7-152">请参阅[内容类型和内容类型发布简介][contentTypeIntro]了解详细信息。</span><span class="sxs-lookup"><span data-stu-id="85ad7-152">See [Introduction to content types and content type publishing][contentTypeIntro] for more information.</span></span>

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

