---
title: outlookItem 资源类型
description: 下面是资源的 JSON 表示形式。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 3bbfe6119d279a1a708b44128a7d134664d7b040
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967047"
---
# <a name="outlookitem-resource-type"></a><span data-ttu-id="3ce98-103">outlookItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="3ce98-103">outlookItem resource type</span></span>



## <a name="json-representation"></a><span data-ttu-id="3ce98-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3ce98-104">JSON representation</span></span>

<span data-ttu-id="3ce98-105">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3ce98-105">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "abstract": true,
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.outlookItem"
}-->

```json
{
  "categories": ["string"],
  "changeKey": "string",
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}

```
## <a name="properties"></a><span data-ttu-id="3ce98-106">属性</span><span class="sxs-lookup"><span data-stu-id="3ce98-106">Properties</span></span>
| <span data-ttu-id="3ce98-107">属性</span><span class="sxs-lookup"><span data-stu-id="3ce98-107">Property</span></span>     | <span data-ttu-id="3ce98-108">类型</span><span class="sxs-lookup"><span data-stu-id="3ce98-108">Type</span></span>   |<span data-ttu-id="3ce98-109">说明</span><span class="sxs-lookup"><span data-stu-id="3ce98-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3ce98-110">categories</span><span class="sxs-lookup"><span data-stu-id="3ce98-110">categories</span></span>|<span data-ttu-id="3ce98-111">String collection</span><span class="sxs-lookup"><span data-stu-id="3ce98-111">String collection</span></span>|<span data-ttu-id="3ce98-112">与项目关联的类别</span><span class="sxs-lookup"><span data-stu-id="3ce98-112">The categories associated with the item</span></span>|
|<span data-ttu-id="3ce98-113">changeKey</span><span class="sxs-lookup"><span data-stu-id="3ce98-113">changeKey</span></span>|<span data-ttu-id="3ce98-114">字符串</span><span class="sxs-lookup"><span data-stu-id="3ce98-114">String</span></span>|<span data-ttu-id="3ce98-115">标识项目的版本。</span><span class="sxs-lookup"><span data-stu-id="3ce98-115">Identifies the version of the item.</span></span> <span data-ttu-id="3ce98-116">每次更改项目时，更改密钥以及更改。</span><span class="sxs-lookup"><span data-stu-id="3ce98-116">Every time the item is changed, changeKey changes as well.</span></span> <span data-ttu-id="3ce98-117">这样，Exchange 更改应用于对象的正确的版本。</span><span class="sxs-lookup"><span data-stu-id="3ce98-117">This allows Exchange to apply changes to the correct version of the object.</span></span> <span data-ttu-id="3ce98-118">只读。</span><span class="sxs-lookup"><span data-stu-id="3ce98-118">Read-only.</span></span>|
|<span data-ttu-id="3ce98-119">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3ce98-119">createdDateTime</span></span>|<span data-ttu-id="3ce98-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ce98-120">DateTimeOffset</span></span>|<span data-ttu-id="3ce98-p102">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="3ce98-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="3ce98-123">id</span><span class="sxs-lookup"><span data-stu-id="3ce98-123">id</span></span>|<span data-ttu-id="3ce98-124">String</span><span class="sxs-lookup"><span data-stu-id="3ce98-124">String</span></span>| <span data-ttu-id="3ce98-125">只读。</span><span class="sxs-lookup"><span data-stu-id="3ce98-125">Read-only.</span></span>|
|<span data-ttu-id="3ce98-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3ce98-126">lastModifiedDateTime</span></span>|<span data-ttu-id="3ce98-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ce98-127">DateTimeOffset</span></span>|<span data-ttu-id="3ce98-p103">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="3ce98-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="3ce98-130">Relationships</span><span class="sxs-lookup"><span data-stu-id="3ce98-130">Relationships</span></span>
<span data-ttu-id="3ce98-131">无</span><span class="sxs-lookup"><span data-stu-id="3ce98-131">None</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
