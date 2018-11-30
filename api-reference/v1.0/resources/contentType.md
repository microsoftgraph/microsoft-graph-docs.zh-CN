---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ContentType
ms.openlocfilehash: ee869e5f2925af92fea9eef04fd26ec483baad5b
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="contenttype-resource-type"></a><span data-ttu-id="00eaa-102">ContentType 资源类型</span><span class="sxs-lookup"><span data-stu-id="00eaa-102">ContentType resource type</span></span>

<span data-ttu-id="00eaa-103">**contentType** 资源表示 SharePoint 中的_内容类型_。</span><span class="sxs-lookup"><span data-stu-id="00eaa-103">The **contentType** resource represents a _content type_ in SharePoint.</span></span>
<span data-ttu-id="00eaa-104">内容类型允许定义一组列，这些列必须显示在 [**list**][list] 中的每个 [**listItem**][listItem] 上。</span><span class="sxs-lookup"><span data-stu-id="00eaa-104">Content types allow you to define a set of columns that must be present on every [**listItem**][listItem] in a [**list**][list].</span></span>

[list]: list.md
[listItem]: listItem.md

## <a name="json-representation"></a><span data-ttu-id="00eaa-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="00eaa-105">JSON representation</span></span>

<span data-ttu-id="00eaa-106">下面是 **contentType** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="00eaa-106">Here is a JSON representation of a **baseItem** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.contentType" } -->

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

## <a name="properties"></a><span data-ttu-id="00eaa-107">属性</span><span class="sxs-lookup"><span data-stu-id="00eaa-107">Properties</span></span>

| <span data-ttu-id="00eaa-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="00eaa-108">Property name</span></span>     | <span data-ttu-id="00eaa-109">类型</span><span class="sxs-lookup"><span data-stu-id="00eaa-109">Type</span></span>                 | <span data-ttu-id="00eaa-110">说明</span><span class="sxs-lookup"><span data-stu-id="00eaa-110">Description</span></span>
|:------------------|:---------------------|:----------------------------------
| <span data-ttu-id="00eaa-111">**description**</span><span class="sxs-lookup"><span data-stu-id="00eaa-111">**description**</span></span>   | <span data-ttu-id="00eaa-112">string</span><span class="sxs-lookup"><span data-stu-id="00eaa-112">string</span></span>               | <span data-ttu-id="00eaa-113">项目的描述性文本。</span><span class="sxs-lookup"><span data-stu-id="00eaa-113">The descriptive text for the site.</span></span>
| <span data-ttu-id="00eaa-114">**group**</span><span class="sxs-lookup"><span data-stu-id="00eaa-114">**group**</span></span>         | <span data-ttu-id="00eaa-115">string</span><span class="sxs-lookup"><span data-stu-id="00eaa-115">string</span></span>               | <span data-ttu-id="00eaa-116">此内容类型所属组的名称。</span><span class="sxs-lookup"><span data-stu-id="00eaa-116">The name of the group this content type belongs to.</span></span> <span data-ttu-id="00eaa-117">帮助组织相关的内容类型。</span><span class="sxs-lookup"><span data-stu-id="00eaa-117">Helps organize related content types.</span></span>
| <span data-ttu-id="00eaa-118">**hidden**</span><span class="sxs-lookup"><span data-stu-id="00eaa-118">**hidden**</span></span>        | <span data-ttu-id="00eaa-119">boolean</span><span class="sxs-lookup"><span data-stu-id="00eaa-119">boolean</span></span>              | <span data-ttu-id="00eaa-120">指示内容类型是否在列表的“新建”菜单中隐藏。</span><span class="sxs-lookup"><span data-stu-id="00eaa-120">Indicates whether the content type is hidden in the list's 'New' menu.</span></span>
| <span data-ttu-id="00eaa-121">**id**</span><span class="sxs-lookup"><span data-stu-id="00eaa-121">**id**</span></span>            | <span data-ttu-id="00eaa-122">string</span><span class="sxs-lookup"><span data-stu-id="00eaa-122">string</span></span>               | <span data-ttu-id="00eaa-123">内容类型的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="00eaa-123">The unique identifier of the content type.</span></span>
| <span data-ttu-id="00eaa-124">**inheritedFrom**</span><span class="sxs-lookup"><span data-stu-id="00eaa-124">**inheritedFrom**</span></span> | <span data-ttu-id="00eaa-125">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="00eaa-125">[itemReference][]</span></span>    | <span data-ttu-id="00eaa-126">如果此内容类型继承自另一个范围（如网站），则提供对定义内容类型的项的引用。</span><span class="sxs-lookup"><span data-stu-id="00eaa-126">If this content type is inherited from another scope (like a site), provides a reference to the item where the content type is defined.</span></span>
| <span data-ttu-id="00eaa-127">**name**</span><span class="sxs-lookup"><span data-stu-id="00eaa-127">**name**</span></span>          | <span data-ttu-id="00eaa-128">string</span><span class="sxs-lookup"><span data-stu-id="00eaa-128">string</span></span>               | <span data-ttu-id="00eaa-129">内容类型的名称。</span><span class="sxs-lookup"><span data-stu-id="00eaa-129">The name of the external content type.</span></span>
| <span data-ttu-id="00eaa-130">**order**</span><span class="sxs-lookup"><span data-stu-id="00eaa-130">**order**</span></span>         | <span data-ttu-id="00eaa-131">[contentTypeOrder][]</span><span class="sxs-lookup"><span data-stu-id="00eaa-131">[contentTypeOrder][]</span></span> | <span data-ttu-id="00eaa-132">指定内容类型出现在选择 UI 中的顺序。</span><span class="sxs-lookup"><span data-stu-id="00eaa-132">Specifies the order in which the content type appears in the selection UI.</span></span>
| <span data-ttu-id="00eaa-133">**parentId**</span><span class="sxs-lookup"><span data-stu-id="00eaa-133">**ParentId**</span></span>      | <span data-ttu-id="00eaa-134">string</span><span class="sxs-lookup"><span data-stu-id="00eaa-134">string</span></span>               | <span data-ttu-id="00eaa-135">内容类型的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="00eaa-135">The unique identifier of the content type.</span></span>
| <span data-ttu-id="00eaa-136">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="00eaa-136">**Read-only.**</span></span>      | <span data-ttu-id="00eaa-137">boolean</span><span class="sxs-lookup"><span data-stu-id="00eaa-137">boolean</span></span>              | <span data-ttu-id="00eaa-138">如果值为 `true`，则无法修改内容类型，除非首先将此值设为 `false`。</span><span class="sxs-lookup"><span data-stu-id="00eaa-138">If `true`, the content type cannot be modified unless this value is first set to `false`.</span></span>
| <span data-ttu-id="00eaa-139">**sealed**</span><span class="sxs-lookup"><span data-stu-id="00eaa-139">**sealed**</span></span>        | <span data-ttu-id="00eaa-140">boolean</span><span class="sxs-lookup"><span data-stu-id="00eaa-140">boolean</span></span>              | <span data-ttu-id="00eaa-141">如果值为 `true`，则无法由用户或通过下推操作修改内容类型。</span><span class="sxs-lookup"><span data-stu-id="00eaa-141">If `true`, the content type cannot be modified by users or through push-down operations.</span></span> <span data-ttu-id="00eaa-142">只有网站集管理员才能封装或解封内容类型。</span><span class="sxs-lookup"><span data-stu-id="00eaa-142">Only site collection administrators can seal or unseal content types.</span></span>

## <a name="relationships"></a><span data-ttu-id="00eaa-143">关系</span><span class="sxs-lookup"><span data-stu-id="00eaa-143">Relationships</span></span>

| <span data-ttu-id="00eaa-144">属性名称</span><span class="sxs-lookup"><span data-stu-id="00eaa-144">Property name</span></span>   | <span data-ttu-id="00eaa-145">类型</span><span class="sxs-lookup"><span data-stu-id="00eaa-145">Type</span></span>                      | <span data-ttu-id="00eaa-146">说明</span><span class="sxs-lookup"><span data-stu-id="00eaa-146">Description</span></span>
|:----------------|:--------------------------|:-------------------------------
| <span data-ttu-id="00eaa-147">**columnLinks**</span><span class="sxs-lookup"><span data-stu-id="00eaa-147">**columnLinks**</span></span> | <span data-ttu-id="00eaa-148">[columnLink][] 集合</span><span class="sxs-lookup"><span data-stu-id="00eaa-148">[columnLink][] collection</span></span> | <span data-ttu-id="00eaa-149">此内容类型所需列的集合</span><span class="sxs-lookup"><span data-stu-id="00eaa-149">The collection of columns that are required by this content type</span></span>

<span data-ttu-id="00eaa-150">有关详细信息，请参阅[内容类型和内容类型发布简介][contentTypeIntro]。</span><span class="sxs-lookup"><span data-stu-id="00eaa-150">See [Introduction to content types and content type publishing][contentTypeIntro] for more information.</span></span>

[columnLink]: columnLink.md
[contentTypeIntro]: https://support.office.com/en-us/article/Introduction-to-content-types-and-content-type-publishing-e1277a2e-a1e8-4473-9126-91a0647766e5
[itemReference]: itemReference.md
[contentTypeOrder]: contentTypeOrder.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentType"
} -->
