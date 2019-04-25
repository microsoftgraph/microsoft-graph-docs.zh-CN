---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ColumnLink
localization_priority: Normal
ms.openlocfilehash: d5b1d068202057bc6a07982d04ff77b6bf07f028
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543467"
---
# <a name="columnlink-resource-type"></a><span data-ttu-id="0d4b3-102">ColumnLink 资源类型</span><span class="sxs-lookup"><span data-stu-id="0d4b3-102">ColumnLink resource type</span></span>

<span data-ttu-id="0d4b3-103">[contentType][] 上的 **columnLink** 将网站 **columnDefinition** 附加到该内容类型。</span><span class="sxs-lookup"><span data-stu-id="0d4b3-103">A **columnLink** on a [contentType][] attaches a site **columnDefinition** to that content type.</span></span>

[contentType]: contenttype.md

## <a name="json-representation"></a><span data-ttu-id="0d4b3-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0d4b3-105">JSON representation</span></span>

<span data-ttu-id="0d4b3-106">下面是 **columnLink** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0d4b3-106">Here is a JSON representation of a **columnLink** resource.</span></span>
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.columnLink" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a><span data-ttu-id="0d4b3-107">属性</span><span class="sxs-lookup"><span data-stu-id="0d4b3-107">Properties</span></span>

| <span data-ttu-id="0d4b3-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="0d4b3-108">Property name</span></span> | <span data-ttu-id="0d4b3-109">类型</span><span class="sxs-lookup"><span data-stu-id="0d4b3-109">Type</span></span>   | <span data-ttu-id="0d4b3-110">说明</span><span class="sxs-lookup"><span data-stu-id="0d4b3-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="0d4b3-111">**id**</span><span class="sxs-lookup"><span data-stu-id="0d4b3-111">**id**</span></span>        | <span data-ttu-id="0d4b3-112">string</span><span class="sxs-lookup"><span data-stu-id="0d4b3-112">string</span></span> | <span data-ttu-id="0d4b3-113">列的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="0d4b3-113">The unique identifier for the column.</span></span>
| <span data-ttu-id="0d4b3-114">**name**</span><span class="sxs-lookup"><span data-stu-id="0d4b3-114">**name**</span></span>      | <span data-ttu-id="0d4b3-115">string</span><span class="sxs-lookup"><span data-stu-id="0d4b3-115">string</span></span> | <span data-ttu-id="0d4b3-116">此内容类型中的列的名称。</span><span class="sxs-lookup"><span data-stu-id="0d4b3-116">The name of the column  in this content type.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnLink"
} -->
