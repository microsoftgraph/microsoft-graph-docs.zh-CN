---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: ListInfo
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 5b3618610a803f86852a95ed1cb662f98cfb6e3f
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482131"
---
# <a name="listinfo-resource"></a><span data-ttu-id="6d44d-102">ListInfo 资源</span><span class="sxs-lookup"><span data-stu-id="6d44d-102">ListInfo resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d44d-103">**listInfo** 复杂类型提供有关 [list][] 的其他信息。</span><span class="sxs-lookup"><span data-stu-id="6d44d-103">The **listInfo** complex type provides additional information about a [list][].</span></span>

[list]: list.md

## <a name="json-representation"></a><span data-ttu-id="6d44d-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6d44d-105">JSON representation</span></span>

<span data-ttu-id="6d44d-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6d44d-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="6d44d-107">属性</span><span class="sxs-lookup"><span data-stu-id="6d44d-107">Properties</span></span>

| <span data-ttu-id="6d44d-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="6d44d-108">Property name</span></span>           | <span data-ttu-id="6d44d-109">类型</span><span class="sxs-lookup"><span data-stu-id="6d44d-109">Type</span></span>    | <span data-ttu-id="6d44d-110">说明</span><span class="sxs-lookup"><span data-stu-id="6d44d-110">Description</span></span>
|:------------------------|:--------|:------------------------------------------------
| <span data-ttu-id="6d44d-111">**contentTypesEnabled**</span><span class="sxs-lookup"><span data-stu-id="6d44d-111">**contentTypesEnabled**</span></span> | <span data-ttu-id="6d44d-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d44d-112">Boolean</span></span> | <span data-ttu-id="6d44d-113">如果为 `true`，则表明已为此列表启用内容类型。</span><span class="sxs-lookup"><span data-stu-id="6d44d-113">If `true`, indicates that content types are enabled for this list.</span></span>
| <span data-ttu-id="6d44d-114">**hidden**</span><span class="sxs-lookup"><span data-stu-id="6d44d-114">**hidden**</span></span>              | <span data-ttu-id="6d44d-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d44d-115">Boolean</span></span> | <span data-ttu-id="6d44d-116">如果为 `true`，则表明该列表通常在 SharePoint 用户体验中不可见。</span><span class="sxs-lookup"><span data-stu-id="6d44d-116">If `true`, indicates that the list is not normally visible in the SharePoint user experience.</span></span>
| <span data-ttu-id="6d44d-117">**template**</span><span class="sxs-lookup"><span data-stu-id="6d44d-117">**template**</span></span>            | <span data-ttu-id="6d44d-118">String</span><span class="sxs-lookup"><span data-stu-id="6d44d-118">String</span></span>  | <span data-ttu-id="6d44d-119">一个枚举值，表示创建列表时使用的基本列表模板。</span><span class="sxs-lookup"><span data-stu-id="6d44d-119">An enumerated value that represents the base list template used in creating the list.</span></span> <span data-ttu-id="6d44d-120">可能的值包括 `documentLibrary`、`genericList`、`task`、`survey`、`announcements`、`contacts` 等。</span><span class="sxs-lookup"><span data-stu-id="6d44d-120">Possible values include `documentLibrary`, `genericList`, `task`, `survey`, `announcements`, `contacts`, and more.</span></span>

### <a name="remarks"></a><span data-ttu-id="6d44d-121">注解</span><span class="sxs-lookup"><span data-stu-id="6d44d-121">Remarks</span></span>

<span data-ttu-id="6d44d-122">虽然用户创建的大多数列表都有上面列出的一个值，但也可能包含其他值。</span><span class="sxs-lookup"><span data-stu-id="6d44d-122">While most lists created by users will have one of the values listed above, other values are possible as well.</span></span>
<span data-ttu-id="6d44d-123">应用应准备好处理未在此处列出的任何值。</span><span class="sxs-lookup"><span data-stu-id="6d44d-123">Your app should be prepared to handle any values that are not listed here.</span></span>
<span data-ttu-id="6d44d-124">对于熟悉 SharePoint CSOM API 的开发人员，`template` 值与 `SPListTemplateType` 枚举对应。</span><span class="sxs-lookup"><span data-stu-id="6d44d-124">For developers familiar with SharePoint's CSOM APIs, the `template` value corresponds to the `SPListTemplateType` enumeration.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/listinfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
