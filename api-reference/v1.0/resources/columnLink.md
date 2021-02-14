---
author: daspek
ms.date: 09/12/2017
title: ColumnLink
localization_priority: Normal
description: contentType 上的 columnLink 将网站 columnDefinition 附加到该内容类型。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 4087d97dfec976560bac7c8949d34fd962308950
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50240575"
---
# <a name="columnlink-resource-type"></a><span data-ttu-id="8378f-103">ColumnLink 资源类型</span><span class="sxs-lookup"><span data-stu-id="8378f-103">ColumnLink resource type</span></span>

<span data-ttu-id="8378f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8378f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8378f-105">[contentType][] 上的 **columnLink** 将网站 **columnDefinition** 附加到该内容类型。</span><span class="sxs-lookup"><span data-stu-id="8378f-105">A **columnLink** on a [contentType][] attaches a site **columnDefinition** to that content type.</span></span>

[contentType]: contenttype.md

## <a name="json-representation"></a><span data-ttu-id="8378f-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8378f-107">JSON representation</span></span>

<span data-ttu-id="8378f-108">下面是 **columnLink** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8378f-108">Here is a JSON representation of a **columnLink** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="8378f-109">属性</span><span class="sxs-lookup"><span data-stu-id="8378f-109">Properties</span></span>

| <span data-ttu-id="8378f-110">属性名称</span><span class="sxs-lookup"><span data-stu-id="8378f-110">Property name</span></span> | <span data-ttu-id="8378f-111">类型</span><span class="sxs-lookup"><span data-stu-id="8378f-111">Type</span></span>   | <span data-ttu-id="8378f-112">说明</span><span class="sxs-lookup"><span data-stu-id="8378f-112">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="8378f-113">**id**</span><span class="sxs-lookup"><span data-stu-id="8378f-113">**id**</span></span>        | <span data-ttu-id="8378f-114">string</span><span class="sxs-lookup"><span data-stu-id="8378f-114">string</span></span> | <span data-ttu-id="8378f-115">列的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="8378f-115">The unique identifier for the column.</span></span>
| <span data-ttu-id="8378f-116">**name**</span><span class="sxs-lookup"><span data-stu-id="8378f-116">**name**</span></span>      | <span data-ttu-id="8378f-117">string</span><span class="sxs-lookup"><span data-stu-id="8378f-117">string</span></span> | <span data-ttu-id="8378f-118">此内容类型中的列的名称。</span><span class="sxs-lookup"><span data-stu-id="8378f-118">The name of the column  in this content type.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnLink"
} -->

