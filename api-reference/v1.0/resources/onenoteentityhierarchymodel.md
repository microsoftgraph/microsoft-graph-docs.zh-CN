---
title: onenoteEntityHierarchyModel 资源
description: 这是 OneNote 实体的基本类型。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: a25e50f6929ae6b13bbe59839f035d2e4a31a6fb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462618"
---
# <a name="onenoteentityhierarchymodel-resource"></a><span data-ttu-id="75424-103">onenoteEntityHierarchyModel 资源</span><span class="sxs-lookup"><span data-stu-id="75424-103">onenoteEntityHierarchyModel resource</span></span>

<span data-ttu-id="75424-104">这是 OneNote 实体的基本类型。</span><span class="sxs-lookup"><span data-stu-id="75424-104">This is a base type for OneNote entities.</span></span>

## <a name="json-representation"></a><span data-ttu-id="75424-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="75424-105">JSON representation</span></span>

<span data-ttu-id="75424-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="75424-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="75424-107">属性</span><span class="sxs-lookup"><span data-stu-id="75424-107">Properties</span></span>
## <a name="properties"></a><span data-ttu-id="75424-108">属性</span><span class="sxs-lookup"><span data-stu-id="75424-108">Properties</span></span>
| <span data-ttu-id="75424-109">属性</span><span class="sxs-lookup"><span data-stu-id="75424-109">Property</span></span>     | <span data-ttu-id="75424-110">类型</span><span class="sxs-lookup"><span data-stu-id="75424-110">Type</span></span>   |<span data-ttu-id="75424-111">说明</span><span class="sxs-lookup"><span data-stu-id="75424-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="75424-112">displayName</span><span class="sxs-lookup"><span data-stu-id="75424-112">displayName</span></span>|<span data-ttu-id="75424-113">String</span><span class="sxs-lookup"><span data-stu-id="75424-113">String</span></span>|<span data-ttu-id="75424-114">笔记本的名称。</span><span class="sxs-lookup"><span data-stu-id="75424-114">The name of the notebook.</span></span>|
|<span data-ttu-id="75424-115">createdBy</span><span class="sxs-lookup"><span data-stu-id="75424-115">createdBy</span></span>|[<span data-ttu-id="75424-116">identitySet</span><span class="sxs-lookup"><span data-stu-id="75424-116">identitySet</span></span>](identityset.md)|<span data-ttu-id="75424-p101">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="75424-p101">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="75424-119">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="75424-119">lastModifiedBy</span></span>|[<span data-ttu-id="75424-120">identitySet</span><span class="sxs-lookup"><span data-stu-id="75424-120">identitySet</span></span>](identityset.md)|<span data-ttu-id="75424-p102">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="75424-p102">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="75424-123">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="75424-123">lastModifiedDateTime</span></span>|<span data-ttu-id="75424-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75424-124">DateTimeOffset</span></span>|<span data-ttu-id="75424-125">上次修改笔记本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="75424-125">The date and time when the notebook was last modified.</span></span> <span data-ttu-id="75424-126">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="75424-126">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="75424-127">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="75424-127">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="75424-128">只读。</span><span class="sxs-lookup"><span data-stu-id="75424-128">Read-only.</span></span>|

<!-- uuid: 8b1af557-1a7c-4432-86eb-94989c2d4b54
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
