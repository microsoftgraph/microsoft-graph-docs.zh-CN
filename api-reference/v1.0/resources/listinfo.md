---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ListInfo
ms.openlocfilehash: eb4952c1a49c41dfae6683153753711158c70f01
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="listinfo-resource"></a><span data-ttu-id="ff61c-102">ListInfo 资源</span><span class="sxs-lookup"><span data-stu-id="ff61c-102">ListInfo resource</span></span>

<span data-ttu-id="ff61c-103">**listInfo** 复杂类型提供有关 [list][] 的其他信息。</span><span class="sxs-lookup"><span data-stu-id="ff61c-103">The **listInfo** complex type provides additional information about a [list][].</span></span>

[list]: list.md

## <a name="json-representation"></a><span data-ttu-id="ff61c-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ff61c-105">JSON representation</span></span>

<span data-ttu-id="ff61c-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ff61c-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.listInfo"
}-->

```json
{
  "contentTypesEnabled": false,
  "hidden": false,
  "template": "documentLibrary | genericList | tasks | survey | links | announcements | contacts | ..."
}
```

## <a name="properties"></a><span data-ttu-id="ff61c-107">属性</span><span class="sxs-lookup"><span data-stu-id="ff61c-107">Properties</span></span>

| <span data-ttu-id="ff61c-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="ff61c-108">Property name</span></span>           | <span data-ttu-id="ff61c-109">类型</span><span class="sxs-lookup"><span data-stu-id="ff61c-109">Type</span></span>    | <span data-ttu-id="ff61c-110">说明</span><span class="sxs-lookup"><span data-stu-id="ff61c-110">Description</span></span>
|:------------------------|:--------|:------------------------------------------------
| <span data-ttu-id="ff61c-111">**contentTypesEnabled**</span><span class="sxs-lookup"><span data-stu-id="ff61c-111">**contentTypesEnabled**</span></span> | <span data-ttu-id="ff61c-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff61c-112">Boolean</span></span> | <span data-ttu-id="ff61c-113">如果值为 `true`，则表示为此列表启用了内容类型。</span><span class="sxs-lookup"><span data-stu-id="ff61c-113">If `true`, indicates that content types are enabled for this list.</span></span>
| <span data-ttu-id="ff61c-114">**hidden**</span><span class="sxs-lookup"><span data-stu-id="ff61c-114">**Hidden**</span></span>              | <span data-ttu-id="ff61c-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff61c-115">Boolean</span></span> | <span data-ttu-id="ff61c-116">如果值为 `true`，则表示该列表在 SharePoint 用户体验中通常不可见。</span><span class="sxs-lookup"><span data-stu-id="ff61c-116">If `true`, indicates that the list is not normally visible in the SharePoint user experience.</span></span>
| <span data-ttu-id="ff61c-117">**template**</span><span class="sxs-lookup"><span data-stu-id="ff61c-117">**Template**</span></span>            | <span data-ttu-id="ff61c-118">String</span><span class="sxs-lookup"><span data-stu-id="ff61c-118">String</span></span>  | <span data-ttu-id="ff61c-119">枚举值，表示创建列表时使用的基本列表模板。</span><span class="sxs-lookup"><span data-stu-id="ff61c-119">An enumerated value that represents the base list template used in creating the list.</span></span> <span data-ttu-id="ff61c-120">可能的值包括 `documentLibrary`、`genericList`、`task`、`survey`、`announcements`、`contacts` 等。</span><span class="sxs-lookup"><span data-stu-id="ff61c-120">Possible values include `documentLibrary`, `genericList`, `task`, `survey`, `announcements`, `contacts`, and more.</span></span>

### <a name="remarks"></a><span data-ttu-id="ff61c-121">备注</span><span class="sxs-lookup"><span data-stu-id="ff61c-121">Remarks</span></span>

<span data-ttu-id="ff61c-122">虽然用户创建的大多数列表将具有上面列出的其中一个值，但也可以使用其他值。</span><span class="sxs-lookup"><span data-stu-id="ff61c-122">While most lists created by users will have one of the values listed above, other values are possible as well.</span></span>
<span data-ttu-id="ff61c-123">应用应准备好处理此处未列出的任何值。</span><span class="sxs-lookup"><span data-stu-id="ff61c-123">Your app should be prepared to handle any values that are not listed here.</span></span>
<span data-ttu-id="ff61c-124">对于熟悉 SharePoint 的 CSOM API 的开发者，`template` 值对应于 `SPListTemplateType` 枚举。</span><span class="sxs-lookup"><span data-stu-id="ff61c-124">For developers familiar with SharePoint's CSOM APIs, the `template` value corresponds to the `SPListTemplateType` enumeration.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
