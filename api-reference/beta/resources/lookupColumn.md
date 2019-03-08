---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: LookupColumn
localization_priority: Normal
ms.openlocfilehash: 1a38cc3e08917b0d4aa2a8df4943ebc932c937d4
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480794"
---
# <a name="lookupcolumn-resource-type"></a><span data-ttu-id="dd3d2-102">LookupColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="dd3d2-102">LookupColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd3d2-103">[columnDefinition](columndefinition.md) 资源上的 **lookupColumn** 指示从网站中的另一个源查找列的值。</span><span class="sxs-lookup"><span data-stu-id="dd3d2-103">The **lookupColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are looked up from another source in the site.</span></span>

## <a name="json-representation"></a><span data-ttu-id="dd3d2-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dd3d2-104">JSON representation</span></span>

<span data-ttu-id="dd3d2-105">下面是 **lookupColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dd3d2-105">Here is a JSON representation of a **lookupColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.lookupColumn" } -->

```json
{
  "allowMultipleValues": true,
  "allowUnlimitedLength": false,
  "columnName": "string",
  "listId": "string",
  "primaryLookupColumnId": "string"
}
```

## <a name="properties"></a><span data-ttu-id="dd3d2-106">属性</span><span class="sxs-lookup"><span data-stu-id="dd3d2-106">Properties</span></span>

| <span data-ttu-id="dd3d2-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="dd3d2-107">Property name</span></span>             | <span data-ttu-id="dd3d2-108">类型</span><span class="sxs-lookup"><span data-stu-id="dd3d2-108">Type</span></span>    | <span data-ttu-id="dd3d2-109">说明</span><span class="sxs-lookup"><span data-stu-id="dd3d2-109">Description</span></span>
|:--------------------------|:--------|:---------------------------------------
| <span data-ttu-id="dd3d2-110">**allowMultipleValues**</span><span class="sxs-lookup"><span data-stu-id="dd3d2-110">**allowMultipleValues**</span></span>   | <span data-ttu-id="dd3d2-111">布尔</span><span class="sxs-lookup"><span data-stu-id="dd3d2-111">boolean</span></span> | <span data-ttu-id="dd3d2-112">指示是否可以从源中选择多个值。</span><span class="sxs-lookup"><span data-stu-id="dd3d2-112">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="dd3d2-113">**allowUnlimitedLength**</span><span class="sxs-lookup"><span data-stu-id="dd3d2-113">**allowUnlimitedLength**</span></span>  | <span data-ttu-id="dd3d2-114">boolean</span><span class="sxs-lookup"><span data-stu-id="dd3d2-114">boolean</span></span> | <span data-ttu-id="dd3d2-115">指示列中的值是否可以超过 255 个字符的标准限制。</span><span class="sxs-lookup"><span data-stu-id="dd3d2-115">Indicates whether values in the column should be able to exceed the standard limit of 255 characters.</span></span>
| <span data-ttu-id="dd3d2-116">**columnName**</span><span class="sxs-lookup"><span data-stu-id="dd3d2-116">**columnName**</span></span>            | <span data-ttu-id="dd3d2-117">string</span><span class="sxs-lookup"><span data-stu-id="dd3d2-117">string</span></span>  | <span data-ttu-id="dd3d2-118">查找源列的名称。</span><span class="sxs-lookup"><span data-stu-id="dd3d2-118">The name of the lookup source column.</span></span>
| <span data-ttu-id="dd3d2-119">**listId**</span><span class="sxs-lookup"><span data-stu-id="dd3d2-119">**listId**</span></span>                | <span data-ttu-id="dd3d2-120">string</span><span class="sxs-lookup"><span data-stu-id="dd3d2-120">string</span></span>  | <span data-ttu-id="dd3d2-121">查找源列表的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="dd3d2-121">The unique identifier of the lookup source list.</span></span>
| <span data-ttu-id="dd3d2-122">**primaryLookupColumnId**</span><span class="sxs-lookup"><span data-stu-id="dd3d2-122">**primaryLookupColumnId**</span></span> | <span data-ttu-id="dd3d2-123">string</span><span class="sxs-lookup"><span data-stu-id="dd3d2-123">string</span></span>  | <span data-ttu-id="dd3d2-124">如果已指定，则此列为*辅助查找*，同时从*主查找*查找的列表项中拉取一个附加字段。</span><span class="sxs-lookup"><span data-stu-id="dd3d2-124">If specified, this column is a *secondary lookup*, pulling an additional field from the list item looked up by the *primary lookup*.</span></span> <span data-ttu-id="dd3d2-125">使用*主查找*查找的列表项作为此处列出的列的源。</span><span class="sxs-lookup"><span data-stu-id="dd3d2-125">Use the list item looked up by the *primary* as the source for the column named here.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/LookupColumn",
  "suppressions": [
    "Error: /api-reference/beta/resources/lookupColumn.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
