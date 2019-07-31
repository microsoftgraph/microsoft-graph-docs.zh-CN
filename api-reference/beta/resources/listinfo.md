---
author: JeremyKelley
description: listInfo 复杂类型提供有关 list 的其他信息。
ms.date: 09/11/2017
title: ListInfo
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 962fc4928bac69489cf2ae2a4c77f3b72169ce0c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966942"
---
# <a name="listinfo-resource"></a><span data-ttu-id="659d9-103">ListInfo 资源</span><span class="sxs-lookup"><span data-stu-id="659d9-103">ListInfo resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="659d9-104">**listInfo** 复杂类型提供有关 [list][] 的其他信息。</span><span class="sxs-lookup"><span data-stu-id="659d9-104">The **listInfo** complex type provides additional information about a [list][].</span></span>

[list]: list.md

## <a name="json-representation"></a><span data-ttu-id="659d9-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="659d9-106">JSON representation</span></span>

<span data-ttu-id="659d9-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="659d9-107">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="659d9-108">属性</span><span class="sxs-lookup"><span data-stu-id="659d9-108">Properties</span></span>

| <span data-ttu-id="659d9-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="659d9-109">Property name</span></span>           | <span data-ttu-id="659d9-110">类型</span><span class="sxs-lookup"><span data-stu-id="659d9-110">Type</span></span>    | <span data-ttu-id="659d9-111">说明</span><span class="sxs-lookup"><span data-stu-id="659d9-111">Description</span></span>
|:------------------------|:--------|:------------------------------------------------
| <span data-ttu-id="659d9-112">**contentTypesEnabled**</span><span class="sxs-lookup"><span data-stu-id="659d9-112">**contentTypesEnabled**</span></span> | <span data-ttu-id="659d9-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="659d9-113">Boolean</span></span> | <span data-ttu-id="659d9-114">如果为 `true`，则表明已为此列表启用内容类型。</span><span class="sxs-lookup"><span data-stu-id="659d9-114">If `true`, indicates that content types are enabled for this list.</span></span>
| <span data-ttu-id="659d9-115">**hidden**</span><span class="sxs-lookup"><span data-stu-id="659d9-115">**hidden**</span></span>              | <span data-ttu-id="659d9-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="659d9-116">Boolean</span></span> | <span data-ttu-id="659d9-117">如果为 `true`，则表明该列表通常在 SharePoint 用户体验中不可见。</span><span class="sxs-lookup"><span data-stu-id="659d9-117">If `true`, indicates that the list is not normally visible in the SharePoint user experience.</span></span>
| <span data-ttu-id="659d9-118">**template**</span><span class="sxs-lookup"><span data-stu-id="659d9-118">**template**</span></span>            | <span data-ttu-id="659d9-119">String</span><span class="sxs-lookup"><span data-stu-id="659d9-119">String</span></span>  | <span data-ttu-id="659d9-120">一个枚举值，表示创建列表时使用的基本列表模板。</span><span class="sxs-lookup"><span data-stu-id="659d9-120">An enumerated value that represents the base list template used in creating the list.</span></span> <span data-ttu-id="659d9-121">可能的值包括 `documentLibrary`、`genericList`、`task`、`survey`、`announcements`、`contacts` 等。</span><span class="sxs-lookup"><span data-stu-id="659d9-121">Possible values include `documentLibrary`, `genericList`, `task`, `survey`, `announcements`, `contacts`, and more.</span></span>

### <a name="remarks"></a><span data-ttu-id="659d9-122">注解</span><span class="sxs-lookup"><span data-stu-id="659d9-122">Remarks</span></span>

<span data-ttu-id="659d9-123">虽然用户创建的大多数列表都有上面列出的一个值，但也可能包含其他值。</span><span class="sxs-lookup"><span data-stu-id="659d9-123">While most lists created by users will have one of the values listed above, other values are possible as well.</span></span>
<span data-ttu-id="659d9-124">应用应准备好处理未在此处列出的任何值。</span><span class="sxs-lookup"><span data-stu-id="659d9-124">Your app should be prepared to handle any values that are not listed here.</span></span>
<span data-ttu-id="659d9-125">对于熟悉 SharePoint CSOM API 的开发人员，`template` 值与 `SPListTemplateType` 枚举对应。</span><span class="sxs-lookup"><span data-stu-id="659d9-125">For developers familiar with SharePoint's CSOM APIs, the `template` value corresponds to the `SPListTemplateType` enumeration.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
