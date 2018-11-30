---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ColumnLink
ms.openlocfilehash: ef7fef6fb6ca35f1117433b452de0841691282a0
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="columnlink-resource-type"></a><span data-ttu-id="8abe9-102">ColumnLink 资源类型</span><span class="sxs-lookup"><span data-stu-id="8abe9-102">ColumnLink resource type</span></span>

<span data-ttu-id="8abe9-103">[contentType][] 上的 **columnLink** 将网站 **columnDefinition** 附加到该内容类型。</span><span class="sxs-lookup"><span data-stu-id="8abe9-103">A **columnLink** on a [contentType][] attaches a site **columnDefinition** to that content type.</span></span>

[contentType]: contentType.md

## <a name="json-representation"></a><span data-ttu-id="8abe9-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8abe9-105">JSON representation</span></span>

<span data-ttu-id="8abe9-106">下面是 **columnLink** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8abe9-106">Here is a JSON representation of a **baseItem** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.columnLink" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a><span data-ttu-id="8abe9-107">属性</span><span class="sxs-lookup"><span data-stu-id="8abe9-107">Properties</span></span>

| <span data-ttu-id="8abe9-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="8abe9-108">Property name</span></span> | <span data-ttu-id="8abe9-109">类型</span><span class="sxs-lookup"><span data-stu-id="8abe9-109">Type</span></span>   | <span data-ttu-id="8abe9-110">说明</span><span class="sxs-lookup"><span data-stu-id="8abe9-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="8abe9-111">**id**</span><span class="sxs-lookup"><span data-stu-id="8abe9-111">**id**</span></span>        | <span data-ttu-id="8abe9-112">string</span><span class="sxs-lookup"><span data-stu-id="8abe9-112">string</span></span> | <span data-ttu-id="8abe9-113">列的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="8abe9-113">The unique identifier for the column.</span></span>
| <span data-ttu-id="8abe9-114">**name**</span><span class="sxs-lookup"><span data-stu-id="8abe9-114">**name**</span></span>      | <span data-ttu-id="8abe9-115">string</span><span class="sxs-lookup"><span data-stu-id="8abe9-115">string</span></span> | <span data-ttu-id="8abe9-116">此内容类型中的列的名称。</span><span class="sxs-lookup"><span data-stu-id="8abe9-116">The name of the column  in this content type.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnLink"
} -->
