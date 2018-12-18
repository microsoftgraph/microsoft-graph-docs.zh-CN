---
title: outlookItem 资源类型
description: 下面是资源的 JSON 表示形式。
author: angelgolfer-ms
ms.openlocfilehash: 750239156e6f4e2874783ae160a7018fb58e259d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332513"
---
# <a name="outlookitem-resource-type"></a><span data-ttu-id="85de6-103">outlookItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="85de6-103">outlookItem resource type</span></span>



## <a name="json-representation"></a><span data-ttu-id="85de6-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="85de6-104">JSON representation</span></span>

<span data-ttu-id="85de6-105">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="85de6-105">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="85de6-106">属性</span><span class="sxs-lookup"><span data-stu-id="85de6-106">Properties</span></span>
| <span data-ttu-id="85de6-107">属性</span><span class="sxs-lookup"><span data-stu-id="85de6-107">Property</span></span>     | <span data-ttu-id="85de6-108">类型</span><span class="sxs-lookup"><span data-stu-id="85de6-108">Type</span></span>   |<span data-ttu-id="85de6-109">说明</span><span class="sxs-lookup"><span data-stu-id="85de6-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="85de6-110">categories</span><span class="sxs-lookup"><span data-stu-id="85de6-110">categories</span></span>|<span data-ttu-id="85de6-111">String collection</span><span class="sxs-lookup"><span data-stu-id="85de6-111">String collection</span></span>|<span data-ttu-id="85de6-112">与项目关联的类别</span><span class="sxs-lookup"><span data-stu-id="85de6-112">The categories associated with the item</span></span>|
|<span data-ttu-id="85de6-113">changeKey</span><span class="sxs-lookup"><span data-stu-id="85de6-113">changeKey</span></span>|<span data-ttu-id="85de6-114">字符串</span><span class="sxs-lookup"><span data-stu-id="85de6-114">String</span></span>|<span data-ttu-id="85de6-115">标识项目的版本。</span><span class="sxs-lookup"><span data-stu-id="85de6-115">Identifies the version of the item.</span></span> <span data-ttu-id="85de6-116">每次更改项目时，更改密钥以及更改。</span><span class="sxs-lookup"><span data-stu-id="85de6-116">Every time the item is changed, changeKey changes as well.</span></span> <span data-ttu-id="85de6-117">这样，Exchange 更改应用于对象的正确的版本。</span><span class="sxs-lookup"><span data-stu-id="85de6-117">This allows Exchange to apply changes to the correct version of the object.</span></span> <span data-ttu-id="85de6-118">只读。</span><span class="sxs-lookup"><span data-stu-id="85de6-118">Read-only.</span></span>|
|<span data-ttu-id="85de6-119">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="85de6-119">createdDateTime</span></span>|<span data-ttu-id="85de6-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85de6-120">DateTimeOffset</span></span>|<span data-ttu-id="85de6-p102">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="85de6-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="85de6-123">id</span><span class="sxs-lookup"><span data-stu-id="85de6-123">id</span></span>|<span data-ttu-id="85de6-124">String</span><span class="sxs-lookup"><span data-stu-id="85de6-124">String</span></span>| <span data-ttu-id="85de6-125">只读。</span><span class="sxs-lookup"><span data-stu-id="85de6-125">Read-only.</span></span>|
|<span data-ttu-id="85de6-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="85de6-126">lastModifiedDateTime</span></span>|<span data-ttu-id="85de6-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85de6-127">DateTimeOffset</span></span>|<span data-ttu-id="85de6-p103">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="85de6-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="85de6-130">Relationships</span><span class="sxs-lookup"><span data-stu-id="85de6-130">Relationships</span></span>
<span data-ttu-id="85de6-131">无</span><span class="sxs-lookup"><span data-stu-id="85de6-131">None</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
