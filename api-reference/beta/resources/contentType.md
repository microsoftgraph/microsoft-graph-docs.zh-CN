---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ContentType
ms.openlocfilehash: cda50c2f20df14c733d3bf71e1b84d5b0df225a0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047942"
---
# <a name="contenttype-resource-type"></a><span data-ttu-id="e84c3-102">ContentType 资源类型</span><span class="sxs-lookup"><span data-stu-id="e84c3-102">ContentType resource type</span></span>

> <span data-ttu-id="e84c3-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e84c3-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e84c3-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e84c3-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e84c3-105">**ContentType** 资源代表 SharePoint 中的_内容类型_。</span><span class="sxs-lookup"><span data-stu-id="e84c3-105">The **contentType** resource represents a _content type_ in SharePoint.</span></span>
<span data-ttu-id="e84c3-106">内容类型使你可以定义一组列，这些列必须存在于 [**list**][list] 中的每个 [**listItem**][listItem] 上。</span><span class="sxs-lookup"><span data-stu-id="e84c3-106">Content types allow you to define a set of columns that must be present on every [**listItem**][listItem] in a [**list**][list].</span></span>

[list]: list.md
[listItem]: listitem.md

## <a name="json-representation"></a><span data-ttu-id="e84c3-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e84c3-107">JSON representation</span></span>

<span data-ttu-id="e84c3-108">下面是 **contentType** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e84c3-108">Here is a JSON representation of a **contentType** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="e84c3-109">属性</span><span class="sxs-lookup"><span data-stu-id="e84c3-109">Properties</span></span>

| <span data-ttu-id="e84c3-110">属性名称</span><span class="sxs-lookup"><span data-stu-id="e84c3-110">Property name</span></span>     | <span data-ttu-id="e84c3-111">类型</span><span class="sxs-lookup"><span data-stu-id="e84c3-111">Type</span></span>                 | <span data-ttu-id="e84c3-112">说明</span><span class="sxs-lookup"><span data-stu-id="e84c3-112">Description</span></span>
|:------------------|:---------------------|:----------------------------------
| <span data-ttu-id="e84c3-113">**说明**</span><span class="sxs-lookup"><span data-stu-id="e84c3-113">**description**</span></span>   | <span data-ttu-id="e84c3-114">string</span><span class="sxs-lookup"><span data-stu-id="e84c3-114">string</span></span>               | <span data-ttu-id="e84c3-115">项目的描述性文本。</span><span class="sxs-lookup"><span data-stu-id="e84c3-115">The descriptive text for the item.</span></span>
| <span data-ttu-id="e84c3-116">**group**</span><span class="sxs-lookup"><span data-stu-id="e84c3-116">**group**</span></span>         | <span data-ttu-id="e84c3-117">string</span><span class="sxs-lookup"><span data-stu-id="e84c3-117">string</span></span>               | <span data-ttu-id="e84c3-118">此内容类型所属的组的名称。</span><span class="sxs-lookup"><span data-stu-id="e84c3-118">The name of the group this content type belongs to.</span></span> <span data-ttu-id="e84c3-119">可以帮助组织相关的内容类型。</span><span class="sxs-lookup"><span data-stu-id="e84c3-119">Helps organize related content types.</span></span>
| <span data-ttu-id="e84c3-120">**hidden**</span><span class="sxs-lookup"><span data-stu-id="e84c3-120">**hidden**</span></span>        | <span data-ttu-id="e84c3-121">boolean</span><span class="sxs-lookup"><span data-stu-id="e84c3-121">boolean</span></span>              | <span data-ttu-id="e84c3-122">指示内容类型是否隐藏于此列表的“新建”菜单中。</span><span class="sxs-lookup"><span data-stu-id="e84c3-122">Indicates whether the content type is hidden in the list's 'New' menu.</span></span>
| <span data-ttu-id="e84c3-123">**id**</span><span class="sxs-lookup"><span data-stu-id="e84c3-123">**id**</span></span>            | <span data-ttu-id="e84c3-124">string</span><span class="sxs-lookup"><span data-stu-id="e84c3-124">string</span></span>               | <span data-ttu-id="e84c3-125">内容类型的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e84c3-125">The unique identifier of the content type.</span></span>
| <span data-ttu-id="e84c3-126">**inheritedFrom**</span><span class="sxs-lookup"><span data-stu-id="e84c3-126">**inheritedFrom**</span></span> | <span data-ttu-id="e84c3-127">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="e84c3-127">[itemReference][]</span></span>    | <span data-ttu-id="e84c3-128">如果此内容类型继承自另一个作用域（如某个站点），则会提供对在其中定义内容类型的项的引用。</span><span class="sxs-lookup"><span data-stu-id="e84c3-128">If this content type is inherited from another scope (like a site), provides a reference to the item where the content type is defined.</span></span>
| <span data-ttu-id="e84c3-129">**name**</span><span class="sxs-lookup"><span data-stu-id="e84c3-129">**name**</span></span>          | <span data-ttu-id="e84c3-130">string</span><span class="sxs-lookup"><span data-stu-id="e84c3-130">string</span></span>               | <span data-ttu-id="e84c3-131">内容类型的名称。</span><span class="sxs-lookup"><span data-stu-id="e84c3-131">The name of the content type.</span></span>
| <span data-ttu-id="e84c3-132">**order**</span><span class="sxs-lookup"><span data-stu-id="e84c3-132">**order**</span></span>         | <span data-ttu-id="e84c3-133">[contentTypeOrder][]</span><span class="sxs-lookup"><span data-stu-id="e84c3-133">[contentTypeOrder][]</span></span> | <span data-ttu-id="e84c3-134">指定在选择 UI 中显示内容类型的顺序。</span><span class="sxs-lookup"><span data-stu-id="e84c3-134">Specifies the order in which the content type appears in the selection UI.</span></span>
| <span data-ttu-id="e84c3-135">**parentId**</span><span class="sxs-lookup"><span data-stu-id="e84c3-135">**parentId**</span></span>      | <span data-ttu-id="e84c3-136">string</span><span class="sxs-lookup"><span data-stu-id="e84c3-136">string</span></span>               | <span data-ttu-id="e84c3-137">内容类型的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e84c3-137">The unique identifier of the content type.</span></span>
| <span data-ttu-id="e84c3-138">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="e84c3-138">**readOnly**</span></span>      | <span data-ttu-id="e84c3-139">boolean</span><span class="sxs-lookup"><span data-stu-id="e84c3-139">boolean</span></span>              | <span data-ttu-id="e84c3-140">如果为 `true`，则不能修改内容类型，除非此值首次设置为 `false`。</span><span class="sxs-lookup"><span data-stu-id="e84c3-140">If `true`, the content type cannot be modified unless this value is first set to `false`.</span></span>
| <span data-ttu-id="e84c3-141">**sealed**</span><span class="sxs-lookup"><span data-stu-id="e84c3-141">**sealed**</span></span>        | <span data-ttu-id="e84c3-142">boolean</span><span class="sxs-lookup"><span data-stu-id="e84c3-142">boolean</span></span>              | <span data-ttu-id="e84c3-143">如果为 `true`，则不能由用户或通过下推操作修改内容类型。</span><span class="sxs-lookup"><span data-stu-id="e84c3-143">If `true`, the content type cannot be modified by users or through push-down operations.</span></span> <span data-ttu-id="e84c3-144">只有网站集管理员可以密封或解封内容类型。</span><span class="sxs-lookup"><span data-stu-id="e84c3-144">Only site collection administrators can seal or unseal content types.</span></span>

## <a name="relationships"></a><span data-ttu-id="e84c3-145">关系</span><span class="sxs-lookup"><span data-stu-id="e84c3-145">Relationships</span></span>

| <span data-ttu-id="e84c3-146">属性名称</span><span class="sxs-lookup"><span data-stu-id="e84c3-146">Property name</span></span>   | <span data-ttu-id="e84c3-147">类型</span><span class="sxs-lookup"><span data-stu-id="e84c3-147">Type</span></span>                      | <span data-ttu-id="e84c3-148">说明</span><span class="sxs-lookup"><span data-stu-id="e84c3-148">Description</span></span>
|:----------------|:--------------------------|:-------------------------------
| <span data-ttu-id="e84c3-149">**columnLinks**</span><span class="sxs-lookup"><span data-stu-id="e84c3-149">**columnLinks**</span></span> | <span data-ttu-id="e84c3-150">[columnLink][] 集合</span><span class="sxs-lookup"><span data-stu-id="e84c3-150">[columnLink][] collection</span></span> | <span data-ttu-id="e84c3-151">此内容类型所需的列集合</span><span class="sxs-lookup"><span data-stu-id="e84c3-151">The collection of columns that are required by this content type</span></span>

<span data-ttu-id="e84c3-152">请参阅[内容类型和内容类型发布简介][contentTypeIntro]了解详细信息。</span><span class="sxs-lookup"><span data-stu-id="e84c3-152">See [Introduction to content types and content type publishing][contentTypeIntro] for more information.</span></span>

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
