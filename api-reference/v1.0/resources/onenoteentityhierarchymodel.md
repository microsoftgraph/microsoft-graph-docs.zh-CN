---
title: onenoteEntityHierarchyModel 资源
description: 这是 OneNote 实体的基本类型。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 8547839597e5f98cf0bcceef80f28814888d539e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48079023"
---
# <a name="onenoteentityhierarchymodel-resource"></a><span data-ttu-id="d281e-103">onenoteEntityHierarchyModel 资源</span><span class="sxs-lookup"><span data-stu-id="d281e-103">onenoteEntityHierarchyModel resource</span></span>

<span data-ttu-id="d281e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d281e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d281e-105">这是 OneNote 实体的基本类型。</span><span class="sxs-lookup"><span data-stu-id="d281e-105">This is a base type for OneNote entities.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d281e-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d281e-106">JSON representation</span></span>

<span data-ttu-id="d281e-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d281e-107">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.onenoteEntitySchemaObjectModel",
  "optionalProperties": [
    "self"
  ],
  "@odata.type": "microsoft.graph.onenoteEntityHierarchyModel"
}-->

```json
{
  "displayName": "string",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)"
}

```
## <a name="properties"></a><span data-ttu-id="d281e-108">属性</span><span class="sxs-lookup"><span data-stu-id="d281e-108">Properties</span></span>
## <a name="properties"></a><span data-ttu-id="d281e-109">属性</span><span class="sxs-lookup"><span data-stu-id="d281e-109">Properties</span></span>
| <span data-ttu-id="d281e-110">属性</span><span class="sxs-lookup"><span data-stu-id="d281e-110">Property</span></span>     | <span data-ttu-id="d281e-111">类型</span><span class="sxs-lookup"><span data-stu-id="d281e-111">Type</span></span>   |<span data-ttu-id="d281e-112">说明</span><span class="sxs-lookup"><span data-stu-id="d281e-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d281e-113">displayName</span><span class="sxs-lookup"><span data-stu-id="d281e-113">displayName</span></span>|<span data-ttu-id="d281e-114">String</span><span class="sxs-lookup"><span data-stu-id="d281e-114">String</span></span>|<span data-ttu-id="d281e-115">笔记本的名称。</span><span class="sxs-lookup"><span data-stu-id="d281e-115">The name of the notebook.</span></span>|
|<span data-ttu-id="d281e-116">createdBy</span><span class="sxs-lookup"><span data-stu-id="d281e-116">createdBy</span></span>|[<span data-ttu-id="d281e-117">identitySet</span><span class="sxs-lookup"><span data-stu-id="d281e-117">identitySet</span></span>](identityset.md)|<span data-ttu-id="d281e-p101">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="d281e-p101">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="d281e-120">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="d281e-120">lastModifiedBy</span></span>|[<span data-ttu-id="d281e-121">identitySet</span><span class="sxs-lookup"><span data-stu-id="d281e-121">identitySet</span></span>](identityset.md)|<span data-ttu-id="d281e-p102">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="d281e-p102">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="d281e-124">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d281e-124">lastModifiedDateTime</span></span>|<span data-ttu-id="d281e-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d281e-125">DateTimeOffset</span></span>|<span data-ttu-id="d281e-126">上次修改笔记本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d281e-126">The date and time when the notebook was last modified.</span></span> <span data-ttu-id="d281e-127">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="d281e-127">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d281e-128">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="d281e-128">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="d281e-129">只读。</span><span class="sxs-lookup"><span data-stu-id="d281e-129">Read-only.</span></span>|

<!-- uuid: 8b1af557-1a7c-4432-86eb-94989c2d4b54
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

