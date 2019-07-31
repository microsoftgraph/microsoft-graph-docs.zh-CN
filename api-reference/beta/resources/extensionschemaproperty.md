---
title: extensionSchemaProperty 资源类型
description: 使用 **extensionSchemaProperty** 资源将属性的名称及其类型定义为 schemaExtension 定义的一部分。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: d36cf90e82e0240842fd9631e2471f9ee834fcb7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972059"
---
# <a name="extensionschemaproperty-resource-type"></a><span data-ttu-id="97523-103">extensionSchemaProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="97523-103">extensionSchemaProperty resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97523-104">使用 **extensionSchemaProperty** 资源将属性的名称及其类型定义为 [schemaExtension](schemaextension.md) 定义的一部分。</span><span class="sxs-lookup"><span data-stu-id="97523-104">Use the **extensionSchemaProperty** resource to define a property's name and its type, as part of a [schemaExtension](schemaextension.md) definition.</span></span>


## <a name="properties"></a><span data-ttu-id="97523-105">属性</span><span class="sxs-lookup"><span data-stu-id="97523-105">Properties</span></span>
| <span data-ttu-id="97523-106">属性</span><span class="sxs-lookup"><span data-stu-id="97523-106">Property</span></span>     | <span data-ttu-id="97523-107">类型</span><span class="sxs-lookup"><span data-stu-id="97523-107">Type</span></span>   |<span data-ttu-id="97523-108">说明</span><span class="sxs-lookup"><span data-stu-id="97523-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="97523-109">name</span><span class="sxs-lookup"><span data-stu-id="97523-109">name</span></span>|<span data-ttu-id="97523-110">String</span><span class="sxs-lookup"><span data-stu-id="97523-110">String</span></span>| <span data-ttu-id="97523-111">定义为架构扩展的一部分的强类型属性的名称。</span><span class="sxs-lookup"><span data-stu-id="97523-111">The name of the strongly typed property defined as part of a schema extension.</span></span>|
|<span data-ttu-id="97523-112">type</span><span class="sxs-lookup"><span data-stu-id="97523-112">type</span></span>|<span data-ttu-id="97523-113">String</span><span class="sxs-lookup"><span data-stu-id="97523-113">String</span></span>| <span data-ttu-id="97523-p101">被定义为架构扩展组成部分的属性的类型。允许的值为 *Binary、Boolean、DateTime、Integer* 或 *String*。请参阅下表获取更多详细信息。</span><span class="sxs-lookup"><span data-stu-id="97523-p101">The type of the property that is defined as part of a schema extension.  Allowed values are *Binary, Boolean, DateTime, Integer* or *String*.  See the table below for more details.</span></span>|

#### <a name="supported-property-data-types"></a><span data-ttu-id="97523-117">受支持的属性数据类型</span><span class="sxs-lookup"><span data-stu-id="97523-117">Supported property data types</span></span> 
<span data-ttu-id="97523-118">在架构扩展中定义属性时，支持以下数据类型：</span><span class="sxs-lookup"><span data-stu-id="97523-118">The following data types are supported when defining a property in a schema extension:</span></span>

| <span data-ttu-id="97523-119">属性类型</span><span class="sxs-lookup"><span data-stu-id="97523-119">Property Type</span></span> | <span data-ttu-id="97523-120">备注</span><span class="sxs-lookup"><span data-stu-id="97523-120">Remarks</span></span> |
|-------------|------------|
| <span data-ttu-id="97523-121">Binary</span><span class="sxs-lookup"><span data-stu-id="97523-121">Binary</span></span> | <span data-ttu-id="97523-122">最多 256 字节。</span><span class="sxs-lookup"><span data-stu-id="97523-122">256 bytes maximum.</span></span> |
| <span data-ttu-id="97523-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="97523-123">Boolean</span></span> | <span data-ttu-id="97523-124">不支持消息、活动和帖子。</span><span class="sxs-lookup"><span data-stu-id="97523-124">Not supported for messages, events and posts.</span></span> |
| <span data-ttu-id="97523-125">日期时间</span><span class="sxs-lookup"><span data-stu-id="97523-125">DateTime</span></span> | <span data-ttu-id="97523-p102">必须以 ISO 8601 格式进行指定。存储为 UTC 格式。</span><span class="sxs-lookup"><span data-stu-id="97523-p102">Must be specified in ISO 8601 format. Will be stored in UTC.</span></span> |
| <span data-ttu-id="97523-128">整数</span><span class="sxs-lookup"><span data-stu-id="97523-128">Integer</span></span> | <span data-ttu-id="97523-p103">32 位值。不支持消息、活动和帖子。</span><span class="sxs-lookup"><span data-stu-id="97523-p103">32-bit value. Not supported for messages, events and posts.</span></span> |
| <span data-ttu-id="97523-131">字符串</span><span class="sxs-lookup"><span data-stu-id="97523-131">String</span></span> | <span data-ttu-id="97523-132">最多 256 个字符。</span><span class="sxs-lookup"><span data-stu-id="97523-132">256 characters maximum.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="97523-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="97523-133">JSON representation</span></span>
<span data-ttu-id="97523-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="97523-134">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.extensionSchemaProperty"
}-->

```json
{
  "name": "String",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "extensionSchemaProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
