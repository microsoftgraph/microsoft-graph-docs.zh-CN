---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ListInfo
localization_priority: Normal
ms.openlocfilehash: c1a29099264c46f32e09b375a97ff49c13c99c6f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858455"
---
# <a name="listinfo-resource"></a><span data-ttu-id="72ef6-102">ListInfo 资源</span><span class="sxs-lookup"><span data-stu-id="72ef6-102">ListInfo resource</span></span>

> <span data-ttu-id="72ef6-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="72ef6-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="72ef6-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="72ef6-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="72ef6-105">**listInfo** 复杂类型提供有关 [list][] 的其他信息。</span><span class="sxs-lookup"><span data-stu-id="72ef6-105">The **listInfo** complex type provides additional information about a [list][].</span></span>

[list]: list.md

## <a name="json-representation"></a><span data-ttu-id="72ef6-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="72ef6-107">JSON representation</span></span>

<span data-ttu-id="72ef6-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="72ef6-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="72ef6-109">属性</span><span class="sxs-lookup"><span data-stu-id="72ef6-109">Properties</span></span>

| <span data-ttu-id="72ef6-110">属性名称</span><span class="sxs-lookup"><span data-stu-id="72ef6-110">Property name</span></span>           | <span data-ttu-id="72ef6-111">类型</span><span class="sxs-lookup"><span data-stu-id="72ef6-111">Type</span></span>    | <span data-ttu-id="72ef6-112">说明</span><span class="sxs-lookup"><span data-stu-id="72ef6-112">Description</span></span>
|:------------------------|:--------|:------------------------------------------------
| <span data-ttu-id="72ef6-113">**contentTypesEnabled**</span><span class="sxs-lookup"><span data-stu-id="72ef6-113">**contentTypesEnabled**</span></span> | <span data-ttu-id="72ef6-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="72ef6-114">Boolean</span></span> | <span data-ttu-id="72ef6-115">如果为 `true`，则表明已为此列表启用内容类型。</span><span class="sxs-lookup"><span data-stu-id="72ef6-115">If `true`, indicates that content types are enabled for this list.</span></span>
| <span data-ttu-id="72ef6-116">**hidden**</span><span class="sxs-lookup"><span data-stu-id="72ef6-116">**hidden**</span></span>              | <span data-ttu-id="72ef6-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="72ef6-117">Boolean</span></span> | <span data-ttu-id="72ef6-118">如果为 `true`，则表明该列表通常在 SharePoint 用户体验中不可见。</span><span class="sxs-lookup"><span data-stu-id="72ef6-118">If `true`, indicates that the list is not normally visible in the SharePoint user experience.</span></span>
| <span data-ttu-id="72ef6-119">**template**</span><span class="sxs-lookup"><span data-stu-id="72ef6-119">**template**</span></span>            | <span data-ttu-id="72ef6-120">String</span><span class="sxs-lookup"><span data-stu-id="72ef6-120">String</span></span>  | <span data-ttu-id="72ef6-121">一个枚举值，表示创建列表时使用的基本列表模板。</span><span class="sxs-lookup"><span data-stu-id="72ef6-121">An enumerated value that represents the base list template used in creating the list.</span></span> <span data-ttu-id="72ef6-122">可能的值包括 `documentLibrary`、`genericList`、`task`、`survey`、`announcements`、`contacts` 等。</span><span class="sxs-lookup"><span data-stu-id="72ef6-122">Possible values include `documentLibrary`, `genericList`, `task`, `survey`, `announcements`, `contacts`, and more.</span></span>

### <a name="remarks"></a><span data-ttu-id="72ef6-123">备注</span><span class="sxs-lookup"><span data-stu-id="72ef6-123">Remarks</span></span>

<span data-ttu-id="72ef6-124">虽然用户创建的大多数列表都有上面列出的一个值，但也可能包含其他值。</span><span class="sxs-lookup"><span data-stu-id="72ef6-124">While most lists created by users will have one of the values listed above, other values are possible as well.</span></span>
<span data-ttu-id="72ef6-125">应用应准备好处理未在此处列出的任何值。</span><span class="sxs-lookup"><span data-stu-id="72ef6-125">Your app should be prepared to handle any values that are not listed here.</span></span>
<span data-ttu-id="72ef6-126">对于熟悉 SharePoint CSOM API 的开发人员，`template` 值与 `SPListTemplateType` 枚举对应。</span><span class="sxs-lookup"><span data-stu-id="72ef6-126">For developers familiar with SharePoint's CSOM APIs, the `template` value corresponds to the `SPListTemplateType` enumeration.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
