---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ContentType
ms.openlocfilehash: 38142299b06313da43637fd0a15ba95f3da362e2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009148"
---
# <a name="contenttype-resource-type"></a><span data-ttu-id="d1025-102">ContentType 资源类型</span><span class="sxs-lookup"><span data-stu-id="d1025-102">ContentType resource type</span></span>

<span data-ttu-id="d1025-103">**ContentType** 资源代表 SharePoint 中的_内容类型_。</span><span class="sxs-lookup"><span data-stu-id="d1025-103">The **contentType** resource represents a _content type_ in SharePoint.</span></span>
<span data-ttu-id="d1025-104">内容类型使你可以定义一组列，这些列必须存在于 [**list**][list] 中的每个 [**listItem**][listItem] 上。</span><span class="sxs-lookup"><span data-stu-id="d1025-104">Content types allow you to define a set of columns that must be present on every [**listItem**][listItem] in a [**list**][list].</span></span>

[list]: list.md
[listItem]: listitem.md

## <a name="json-representation"></a><span data-ttu-id="d1025-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d1025-105">JSON representation</span></span>

<span data-ttu-id="d1025-106">下面是 **contentType** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d1025-106">Here is a JSON representation of a **contentType** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="d1025-107">属性</span><span class="sxs-lookup"><span data-stu-id="d1025-107">Properties</span></span>

| <span data-ttu-id="d1025-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="d1025-108">Property name</span></span>     | <span data-ttu-id="d1025-109">类型</span><span class="sxs-lookup"><span data-stu-id="d1025-109">Type</span></span>                 | <span data-ttu-id="d1025-110">说明</span><span class="sxs-lookup"><span data-stu-id="d1025-110">Description</span></span>
|:------------------|:---------------------|:----------------------------------
| <span data-ttu-id="d1025-111">**description**</span><span class="sxs-lookup"><span data-stu-id="d1025-111">**description**</span></span>   | <span data-ttu-id="d1025-112">string</span><span class="sxs-lookup"><span data-stu-id="d1025-112">string</span></span>               | <span data-ttu-id="d1025-113">项目的描述性文本。</span><span class="sxs-lookup"><span data-stu-id="d1025-113">The descriptive text for the item.</span></span>
| <span data-ttu-id="d1025-114">**group**</span><span class="sxs-lookup"><span data-stu-id="d1025-114">**group**</span></span>         | <span data-ttu-id="d1025-115">string</span><span class="sxs-lookup"><span data-stu-id="d1025-115">string</span></span>               | <span data-ttu-id="d1025-116">此内容类型所属的组的名称。</span><span class="sxs-lookup"><span data-stu-id="d1025-116">The name of the group this content type belongs to.</span></span> <span data-ttu-id="d1025-117">可以帮助组织相关的内容类型。</span><span class="sxs-lookup"><span data-stu-id="d1025-117">Helps organize related content types.</span></span>
| <span data-ttu-id="d1025-118">**hidden**</span><span class="sxs-lookup"><span data-stu-id="d1025-118">**hidden**</span></span>        | <span data-ttu-id="d1025-119">boolean</span><span class="sxs-lookup"><span data-stu-id="d1025-119">boolean</span></span>              | <span data-ttu-id="d1025-120">指示内容类型是否隐藏于此列表的“新建”菜单中。</span><span class="sxs-lookup"><span data-stu-id="d1025-120">Indicates whether the content type is hidden in the list's 'New' menu.</span></span>
| <span data-ttu-id="d1025-121">**id**</span><span class="sxs-lookup"><span data-stu-id="d1025-121">**id**</span></span>            | <span data-ttu-id="d1025-122">string</span><span class="sxs-lookup"><span data-stu-id="d1025-122">string</span></span>               | <span data-ttu-id="d1025-123">内容类型的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d1025-123">The unique identifier of the content type.</span></span>
| <span data-ttu-id="d1025-124">**inheritedFrom**</span><span class="sxs-lookup"><span data-stu-id="d1025-124">**inheritedFrom**</span></span> | <span data-ttu-id="d1025-125">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="d1025-125">[itemReference][]</span></span>    | <span data-ttu-id="d1025-126">如果此内容类型继承自另一个作用域（如某个站点），则会提供对在其中定义内容类型的项的引用。</span><span class="sxs-lookup"><span data-stu-id="d1025-126">If this content type is inherited from another scope (like a site), provides a reference to the item where the content type is defined.</span></span>
| <span data-ttu-id="d1025-127">**name**</span><span class="sxs-lookup"><span data-stu-id="d1025-127">**name**</span></span>          | <span data-ttu-id="d1025-128">string</span><span class="sxs-lookup"><span data-stu-id="d1025-128">string</span></span>               | <span data-ttu-id="d1025-129">内容类型的名称。</span><span class="sxs-lookup"><span data-stu-id="d1025-129">The name of the content type.</span></span>
| <span data-ttu-id="d1025-130">**order**</span><span class="sxs-lookup"><span data-stu-id="d1025-130">**order**</span></span>         | <span data-ttu-id="d1025-131">[contentTypeOrder][]</span><span class="sxs-lookup"><span data-stu-id="d1025-131">[contentTypeOrder][]</span></span> | <span data-ttu-id="d1025-132">指定在选择 UI 中显示内容类型的顺序。</span><span class="sxs-lookup"><span data-stu-id="d1025-132">Specifies the order in which the content type appears in the selection UI.</span></span>
| <span data-ttu-id="d1025-133">**parentId**</span><span class="sxs-lookup"><span data-stu-id="d1025-133">**parentId**</span></span>      | <span data-ttu-id="d1025-134">string</span><span class="sxs-lookup"><span data-stu-id="d1025-134">string</span></span>               | <span data-ttu-id="d1025-135">内容类型的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d1025-135">The unique identifier of the content type.</span></span>
| <span data-ttu-id="d1025-136">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="d1025-136">**readOnly**</span></span>      | <span data-ttu-id="d1025-137">boolean</span><span class="sxs-lookup"><span data-stu-id="d1025-137">boolean</span></span>              | <span data-ttu-id="d1025-138">如果为 `true`，则不能修改内容类型，除非此值首次设置为 `false`。</span><span class="sxs-lookup"><span data-stu-id="d1025-138">If `true`, the content type cannot be modified unless this value is first set to `false`.</span></span>
| <span data-ttu-id="d1025-139">**sealed**</span><span class="sxs-lookup"><span data-stu-id="d1025-139">**sealed**</span></span>        | <span data-ttu-id="d1025-140">boolean</span><span class="sxs-lookup"><span data-stu-id="d1025-140">boolean</span></span>              | <span data-ttu-id="d1025-141">如果为 `true`，则不能由用户或通过下推操作修改内容类型。</span><span class="sxs-lookup"><span data-stu-id="d1025-141">If `true`, the content type cannot be modified by users or through push-down operations.</span></span> <span data-ttu-id="d1025-142">只有网站集管理员可以密封或解封内容类型。</span><span class="sxs-lookup"><span data-stu-id="d1025-142">Only site collection administrators can seal or unseal content types.</span></span>

## <a name="relationships"></a><span data-ttu-id="d1025-143">关系</span><span class="sxs-lookup"><span data-stu-id="d1025-143">Relationships</span></span>

| <span data-ttu-id="d1025-144">属性名称</span><span class="sxs-lookup"><span data-stu-id="d1025-144">Property name</span></span>   | <span data-ttu-id="d1025-145">类型</span><span class="sxs-lookup"><span data-stu-id="d1025-145">Type</span></span>                      | <span data-ttu-id="d1025-146">说明</span><span class="sxs-lookup"><span data-stu-id="d1025-146">Description</span></span>
|:----------------|:--------------------------|:-------------------------------
| <span data-ttu-id="d1025-147">**columnLinks**</span><span class="sxs-lookup"><span data-stu-id="d1025-147">**columnLinks**</span></span> | <span data-ttu-id="d1025-148">[columnLink][] 集合</span><span class="sxs-lookup"><span data-stu-id="d1025-148">[columnLink][] collection</span></span> | <span data-ttu-id="d1025-149">此内容类型所需的列集合</span><span class="sxs-lookup"><span data-stu-id="d1025-149">The collection of columns that are required by this content type</span></span>

<span data-ttu-id="d1025-150">请参阅[内容类型和内容类型发布简介][contentTypeIntro]了解详细信息。</span><span class="sxs-lookup"><span data-stu-id="d1025-150">See [Introduction to content types and content type publishing][contentTypeIntro] for more information.</span></span>

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
