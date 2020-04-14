---
title: outlookItem 资源类型
description: 下面是资源的 JSON 表示形式。
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 88436021375c85e85fc009611b2279705801ad12
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43463239"
---
# <a name="outlookitem-resource-type"></a><span data-ttu-id="17228-103">outlookItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="17228-103">outlookItem resource type</span></span>

<span data-ttu-id="17228-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17228-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="17228-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="17228-105">JSON representation</span></span>

<span data-ttu-id="17228-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="17228-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
## <a name="properties"></a><span data-ttu-id="17228-107">属性</span><span class="sxs-lookup"><span data-stu-id="17228-107">Properties</span></span>
| <span data-ttu-id="17228-108">属性</span><span class="sxs-lookup"><span data-stu-id="17228-108">Property</span></span>     | <span data-ttu-id="17228-109">类型</span><span class="sxs-lookup"><span data-stu-id="17228-109">Type</span></span>   |<span data-ttu-id="17228-110">说明</span><span class="sxs-lookup"><span data-stu-id="17228-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="17228-111">categories</span><span class="sxs-lookup"><span data-stu-id="17228-111">categories</span></span>|<span data-ttu-id="17228-112">String collection</span><span class="sxs-lookup"><span data-stu-id="17228-112">String collection</span></span>||
|<span data-ttu-id="17228-113">changeKey</span><span class="sxs-lookup"><span data-stu-id="17228-113">changeKey</span></span>|<span data-ttu-id="17228-114">String</span><span class="sxs-lookup"><span data-stu-id="17228-114">String</span></span>||
|<span data-ttu-id="17228-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="17228-115">createdDateTime</span></span>|<span data-ttu-id="17228-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17228-116">DateTimeOffset</span></span>|<span data-ttu-id="17228-p101">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="17228-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="17228-119">id</span><span class="sxs-lookup"><span data-stu-id="17228-119">id</span></span>|<span data-ttu-id="17228-120">字符串</span><span class="sxs-lookup"><span data-stu-id="17228-120">String</span></span>| <span data-ttu-id="17228-121">只读。</span><span class="sxs-lookup"><span data-stu-id="17228-121">Read-only.</span></span>|
|<span data-ttu-id="17228-122">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="17228-122">lastModifiedDateTime</span></span>|<span data-ttu-id="17228-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17228-123">DateTimeOffset</span></span>|<span data-ttu-id="17228-p102">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="17228-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="17228-126">关系</span><span class="sxs-lookup"><span data-stu-id="17228-126">Relationships</span></span>
<span data-ttu-id="17228-127">无</span><span class="sxs-lookup"><span data-stu-id="17228-127">None</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
