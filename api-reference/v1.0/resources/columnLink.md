---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ColumnLink
localization_priority: Normal
ms.openlocfilehash: 435696cc596f73830104ea8ec0619bf40a462d62
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32565784"
---
# <a name="columnlink-resource-type"></a><span data-ttu-id="7e681-102">ColumnLink 资源类型</span><span class="sxs-lookup"><span data-stu-id="7e681-102">ColumnLink resource type</span></span>

<span data-ttu-id="7e681-103">[contentType][] 上的 **columnLink** 将网站 **columnDefinition** 附加到该内容类型。</span><span class="sxs-lookup"><span data-stu-id="7e681-103">A **columnLink** on a [contentType][] attaches a site **columnDefinition** to that content type.</span></span>

[contentType]: contenttype.md

## <a name="json-representation"></a><span data-ttu-id="7e681-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7e681-105">JSON representation</span></span>

<span data-ttu-id="7e681-106">下面是 **columnLink** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7e681-106">Here is a JSON representation of a **columnLink** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="7e681-107">属性</span><span class="sxs-lookup"><span data-stu-id="7e681-107">Properties</span></span>

| <span data-ttu-id="7e681-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="7e681-108">Property name</span></span> | <span data-ttu-id="7e681-109">类型</span><span class="sxs-lookup"><span data-stu-id="7e681-109">Type</span></span>   | <span data-ttu-id="7e681-110">说明</span><span class="sxs-lookup"><span data-stu-id="7e681-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="7e681-111">**id**</span><span class="sxs-lookup"><span data-stu-id="7e681-111">**id**</span></span>        | <span data-ttu-id="7e681-112">string</span><span class="sxs-lookup"><span data-stu-id="7e681-112">string</span></span> | <span data-ttu-id="7e681-113">列的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="7e681-113">The unique identifier for the column.</span></span>
| <span data-ttu-id="7e681-114">**name**</span><span class="sxs-lookup"><span data-stu-id="7e681-114">**name**</span></span>      | <span data-ttu-id="7e681-115">string</span><span class="sxs-lookup"><span data-stu-id="7e681-115">string</span></span> | <span data-ttu-id="7e681-116">此内容类型中的列的名称。</span><span class="sxs-lookup"><span data-stu-id="7e681-116">The name of the column  in this content type.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnLink"
} -->
