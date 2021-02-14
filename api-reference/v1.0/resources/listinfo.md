---
author: JeremyKelley
ms.date: 09/11/2017
title: ListInfo
localization_priority: Normal
ms.prod: sharepoint
description: listInfo 复杂类型提供有关 list 的其他信息。
doc_type: resourcePageType
ms.openlocfilehash: c5d84f5fae89e6ecf433dad20a959f9846f58006
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239357"
---
# <a name="listinfo-resource"></a><span data-ttu-id="95ae5-103">ListInfo 资源</span><span class="sxs-lookup"><span data-stu-id="95ae5-103">ListInfo resource</span></span>

<span data-ttu-id="95ae5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95ae5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="95ae5-105">**listInfo** 复杂类型提供有关 [list][] 的其他信息。</span><span class="sxs-lookup"><span data-stu-id="95ae5-105">The **listInfo** complex type provides additional information about a [list][].</span></span>

[list]: list.md

## <a name="json-representation"></a><span data-ttu-id="95ae5-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="95ae5-107">JSON representation</span></span>

<span data-ttu-id="95ae5-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="95ae5-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="95ae5-109">属性</span><span class="sxs-lookup"><span data-stu-id="95ae5-109">Properties</span></span>

| <span data-ttu-id="95ae5-110">属性名称</span><span class="sxs-lookup"><span data-stu-id="95ae5-110">Property name</span></span>           | <span data-ttu-id="95ae5-111">类型</span><span class="sxs-lookup"><span data-stu-id="95ae5-111">Type</span></span>    | <span data-ttu-id="95ae5-112">说明</span><span class="sxs-lookup"><span data-stu-id="95ae5-112">Description</span></span>
|:------------------------|:--------|:------------------------------------------------
| <span data-ttu-id="95ae5-113">**contentTypesEnabled**</span><span class="sxs-lookup"><span data-stu-id="95ae5-113">**contentTypesEnabled**</span></span> | <span data-ttu-id="95ae5-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="95ae5-114">Boolean</span></span> | <span data-ttu-id="95ae5-115">如果为 `true`，则表明已为此列表启用内容类型。</span><span class="sxs-lookup"><span data-stu-id="95ae5-115">If `true`, indicates that content types are enabled for this list.</span></span>
| <span data-ttu-id="95ae5-116">**hidden**</span><span class="sxs-lookup"><span data-stu-id="95ae5-116">**hidden**</span></span>              | <span data-ttu-id="95ae5-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="95ae5-117">Boolean</span></span> | <span data-ttu-id="95ae5-118">如果为 `true`，则表明该列表通常在 SharePoint 用户体验中不可见。</span><span class="sxs-lookup"><span data-stu-id="95ae5-118">If `true`, indicates that the list is not normally visible in the SharePoint user experience.</span></span>
| <span data-ttu-id="95ae5-119">**template**</span><span class="sxs-lookup"><span data-stu-id="95ae5-119">**template**</span></span>            | <span data-ttu-id="95ae5-120">String</span><span class="sxs-lookup"><span data-stu-id="95ae5-120">String</span></span>  | <span data-ttu-id="95ae5-121">一个枚举值，表示创建列表时使用的基本列表模板。</span><span class="sxs-lookup"><span data-stu-id="95ae5-121">An enumerated value that represents the base list template used in creating the list.</span></span> <span data-ttu-id="95ae5-122">可能的值包括 `documentLibrary`、`genericList`、`task`、`survey`、`announcements`、`contacts` 等。</span><span class="sxs-lookup"><span data-stu-id="95ae5-122">Possible values include `documentLibrary`, `genericList`, `task`, `survey`, `announcements`, `contacts`, and more.</span></span>

### <a name="remarks"></a><span data-ttu-id="95ae5-123">注解</span><span class="sxs-lookup"><span data-stu-id="95ae5-123">Remarks</span></span>

<span data-ttu-id="95ae5-124">虽然用户创建的大多数列表都有上面列出的一个值，但也可能包含其他值。</span><span class="sxs-lookup"><span data-stu-id="95ae5-124">While most lists created by users will have one of the values listed above, other values are possible as well.</span></span>
<span data-ttu-id="95ae5-125">应用应准备好处理未在此处列出的任何值。</span><span class="sxs-lookup"><span data-stu-id="95ae5-125">Your app should be prepared to handle any values that are not listed here.</span></span>
<span data-ttu-id="95ae5-126">对于熟悉 SharePoint CSOM API 的开发人员，`template` 值与 `SPListTemplateType` 枚举对应。</span><span class="sxs-lookup"><span data-stu-id="95ae5-126">For developers familiar with SharePoint's CSOM APIs, the `template` value corresponds to the `SPListTemplateType` enumeration.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/listinfo.md:
      Found potential enums in resource example that weren't defined in a table:(documentLibrary,genericList,tasks,survey,links,announcements,contacts,...) are in resource, but () are in table"
  ],
  "tocPath": ""
}-->

