---
author: JeremyKelley
description: listInfo 复杂类型提供有关 list 的其他信息。
ms.date: 09/11/2017
title: ListInfo
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 5f36e7f08d8a5ce29316e97ff8f03f14063a4d36
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055286"
---
# <a name="listinfo-resource"></a><span data-ttu-id="31390-103">ListInfo 资源</span><span class="sxs-lookup"><span data-stu-id="31390-103">ListInfo resource</span></span>

<span data-ttu-id="31390-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31390-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31390-105">**listInfo** 复杂类型提供有关 [list][] 的其他信息。</span><span class="sxs-lookup"><span data-stu-id="31390-105">The **listInfo** complex type provides additional information about a [list][].</span></span>

[list]: list.md

## <a name="json-representation"></a><span data-ttu-id="31390-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="31390-107">JSON representation</span></span>

<span data-ttu-id="31390-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="31390-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="31390-109">属性</span><span class="sxs-lookup"><span data-stu-id="31390-109">Properties</span></span>

| <span data-ttu-id="31390-110">属性名称</span><span class="sxs-lookup"><span data-stu-id="31390-110">Property name</span></span>           | <span data-ttu-id="31390-111">类型</span><span class="sxs-lookup"><span data-stu-id="31390-111">Type</span></span>    | <span data-ttu-id="31390-112">说明</span><span class="sxs-lookup"><span data-stu-id="31390-112">Description</span></span>
|:------------------------|:--------|:------------------------------------------------
| <span data-ttu-id="31390-113">**contentTypesEnabled**</span><span class="sxs-lookup"><span data-stu-id="31390-113">**contentTypesEnabled**</span></span> | <span data-ttu-id="31390-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="31390-114">Boolean</span></span> | <span data-ttu-id="31390-115">如果为 `true`，则表明已为此列表启用内容类型。</span><span class="sxs-lookup"><span data-stu-id="31390-115">If `true`, indicates that content types are enabled for this list.</span></span>
| <span data-ttu-id="31390-116">**hidden**</span><span class="sxs-lookup"><span data-stu-id="31390-116">**hidden**</span></span>              | <span data-ttu-id="31390-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="31390-117">Boolean</span></span> | <span data-ttu-id="31390-118">如果为 `true`，则表明该列表通常在 SharePoint 用户体验中不可见。</span><span class="sxs-lookup"><span data-stu-id="31390-118">If `true`, indicates that the list is not normally visible in the SharePoint user experience.</span></span>
| <span data-ttu-id="31390-119">**template**</span><span class="sxs-lookup"><span data-stu-id="31390-119">**template**</span></span>            | <span data-ttu-id="31390-120">String</span><span class="sxs-lookup"><span data-stu-id="31390-120">String</span></span>  | <span data-ttu-id="31390-121">一个枚举值，表示创建列表时使用的基本列表模板。</span><span class="sxs-lookup"><span data-stu-id="31390-121">An enumerated value that represents the base list template used in creating the list.</span></span> <span data-ttu-id="31390-122">可能的值包括 `documentLibrary`、`genericList`、`task`、`survey`、`announcements`、`contacts` 等。</span><span class="sxs-lookup"><span data-stu-id="31390-122">Possible values include `documentLibrary`, `genericList`, `task`, `survey`, `announcements`, `contacts`, and more.</span></span>

### <a name="remarks"></a><span data-ttu-id="31390-123">注解</span><span class="sxs-lookup"><span data-stu-id="31390-123">Remarks</span></span>

<span data-ttu-id="31390-124">虽然用户创建的大多数列表都有上面列出的一个值，但也可能包含其他值。</span><span class="sxs-lookup"><span data-stu-id="31390-124">While most lists created by users will have one of the values listed above, other values are possible as well.</span></span>
<span data-ttu-id="31390-125">应用应准备好处理未在此处列出的任何值。</span><span class="sxs-lookup"><span data-stu-id="31390-125">Your app should be prepared to handle any values that are not listed here.</span></span>
<span data-ttu-id="31390-126">对于熟悉 SharePoint CSOM API 的开发人员，`template` 值与 `SPListTemplateType` 枚举对应。</span><span class="sxs-lookup"><span data-stu-id="31390-126">For developers familiar with SharePoint's CSOM APIs, the `template` value corresponds to the `SPListTemplateType` enumeration.</span></span>

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


