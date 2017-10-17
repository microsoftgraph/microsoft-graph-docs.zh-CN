---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: LookupColumn
ms.openlocfilehash: 07dba3c223ffc3993be1fc284572810a7aa3ccf8
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="lookupcolumn-resource-type"></a><span data-ttu-id="8206e-102">LookupColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="8206e-102">LookupColumn resource type</span></span>

<span data-ttu-id="8206e-103">[columnDefinition](columnDefinition.md) 资源上的 **lookupColumn** 指示从网站中的另一个源查找列的值。</span><span class="sxs-lookup"><span data-stu-id="8206e-103">The **lookupColumn** on a [columnDefinition](columnDefinition.md) resource indicates that the column's values are looked up from another source in the site.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8206e-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8206e-104">JSON representation</span></span>

<span data-ttu-id="8206e-105">下面是 **lookupColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8206e-105">Here is a JSON representation of a **driveItem** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="8206e-106">属性</span><span class="sxs-lookup"><span data-stu-id="8206e-106">Properties</span></span>

| <span data-ttu-id="8206e-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="8206e-107">Property name</span></span>             | <span data-ttu-id="8206e-108">类型</span><span class="sxs-lookup"><span data-stu-id="8206e-108">Type</span></span>    | <span data-ttu-id="8206e-109">说明</span><span class="sxs-lookup"><span data-stu-id="8206e-109">Description</span></span>
|:--------------------------|:--------|:---------------------------------------
| <span data-ttu-id="8206e-110">**allowMultipleValues**</span><span class="sxs-lookup"><span data-stu-id="8206e-110">**allowMultipleValues**</span></span>   | <span data-ttu-id="8206e-111">boolean</span><span class="sxs-lookup"><span data-stu-id="8206e-111">boolean</span></span> | <span data-ttu-id="8206e-112">指示是否可以从源中选择多个值。</span><span class="sxs-lookup"><span data-stu-id="8206e-112">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="8206e-113">**allowUnlimitedLength**</span><span class="sxs-lookup"><span data-stu-id="8206e-113">**allowUnlimitedLength**</span></span>  | <span data-ttu-id="8206e-114">boolean</span><span class="sxs-lookup"><span data-stu-id="8206e-114">boolean</span></span> | <span data-ttu-id="8206e-115">指示列中的值是否可以超过 255 个字符的标准限制。</span><span class="sxs-lookup"><span data-stu-id="8206e-115">Indicates whether values in the column should be able to exceed the standard limit of 255 characters.</span></span>
| <span data-ttu-id="8206e-116">**columnName**</span><span class="sxs-lookup"><span data-stu-id="8206e-116">**columnName**</span></span>            | <span data-ttu-id="8206e-117">string</span><span class="sxs-lookup"><span data-stu-id="8206e-117">string</span></span>  | <span data-ttu-id="8206e-118">查找源列的名称。</span><span class="sxs-lookup"><span data-stu-id="8206e-118">The name of the lookup source column.</span></span>
| <span data-ttu-id="8206e-119">**listId**</span><span class="sxs-lookup"><span data-stu-id="8206e-119">**listId**</span></span>                | <span data-ttu-id="8206e-120">string</span><span class="sxs-lookup"><span data-stu-id="8206e-120">string</span></span>  | <span data-ttu-id="8206e-121">查找源列表的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="8206e-121">The unique identifier of the lookup source list.</span></span>
| <span data-ttu-id="8206e-122">**primaryLookupColumnId**</span><span class="sxs-lookup"><span data-stu-id="8206e-122">**primaryLookupColumnId**</span></span> | <span data-ttu-id="8206e-123">string</span><span class="sxs-lookup"><span data-stu-id="8206e-123">string</span></span>  | <span data-ttu-id="8206e-124">如果已指定，则此列为“辅助查找”**，同时从“主查找”**查找的列表项中拉取一个附加字段。</span><span class="sxs-lookup"><span data-stu-id="8206e-124">If specified, this column is a *secondary lookup*, pulling an additional field from the list item looked up by the *primary lookup*.</span></span> <span data-ttu-id="8206e-125">使用“主查找”查找**的列表项作为此处命名的列的源。</span><span class="sxs-lookup"><span data-stu-id="8206e-125">Use the list item looked up by the *primary* as the source for the column named here.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/LookupColumn"
} -->
