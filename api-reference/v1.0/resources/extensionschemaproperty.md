---
title: extensionSchemaProperty 资源类型
description: 使用 **extensionSchemaProperty** 资源将属性的名称及其类型定义为 schemaExtension 定义的一部分。
localization_priority: Normal
author: keylimesoda
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 0ba79f634432b6f481bb94be3b70b6821fb84e7d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48018429"
---
# <a name="extensionschemaproperty-resource-type"></a><span data-ttu-id="c9ce0-103">extensionSchemaProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="c9ce0-103">extensionSchemaProperty resource type</span></span>

<span data-ttu-id="c9ce0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9ce0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c9ce0-105">使用 **extensionSchemaProperty** 资源将属性的名称及其类型定义为 [schemaExtension](schemaextension.md) 定义的一部分。</span><span class="sxs-lookup"><span data-stu-id="c9ce0-105">Use the **extensionSchemaProperty** resource to define a property's name and its type, as part of a [schemaExtension](schemaextension.md) definition.</span></span>


## <a name="properties"></a><span data-ttu-id="c9ce0-106">属性</span><span class="sxs-lookup"><span data-stu-id="c9ce0-106">Properties</span></span>
| <span data-ttu-id="c9ce0-107">属性</span><span class="sxs-lookup"><span data-stu-id="c9ce0-107">Property</span></span>     | <span data-ttu-id="c9ce0-108">类型</span><span class="sxs-lookup"><span data-stu-id="c9ce0-108">Type</span></span>   |<span data-ttu-id="c9ce0-109">说明</span><span class="sxs-lookup"><span data-stu-id="c9ce0-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c9ce0-110">name</span><span class="sxs-lookup"><span data-stu-id="c9ce0-110">name</span></span>|<span data-ttu-id="c9ce0-111">String</span><span class="sxs-lookup"><span data-stu-id="c9ce0-111">String</span></span>| <span data-ttu-id="c9ce0-112">被定义为架构扩展组成部分的强类型属性的名称。</span><span class="sxs-lookup"><span data-stu-id="c9ce0-112">The name of the strongly-typed property defined as part of a schema extension.</span></span>|
|<span data-ttu-id="c9ce0-113">type</span><span class="sxs-lookup"><span data-stu-id="c9ce0-113">type</span></span>|<span data-ttu-id="c9ce0-114">String</span><span class="sxs-lookup"><span data-stu-id="c9ce0-114">String</span></span>| <span data-ttu-id="c9ce0-p101">被定义为架构扩展组成部分的属性的类型。允许的值为 *Binary、Boolean、DateTime、Integer* 或 *String*。请参阅下表获取更多详细信息。</span><span class="sxs-lookup"><span data-stu-id="c9ce0-p101">The type of the property that is defined as part of a schema extension.  Allowed values are *Binary, Boolean, DateTime, Integer* or *String*.  See the table below for more details.</span></span>|

#### <a name="supported-property-data-types"></a><span data-ttu-id="c9ce0-118">受支持的属性数据类型</span><span class="sxs-lookup"><span data-stu-id="c9ce0-118">Supported property data types</span></span>
<span data-ttu-id="c9ce0-119">在架构扩展中定义属性时，支持以下数据类型：</span><span class="sxs-lookup"><span data-stu-id="c9ce0-119">The following data types are supported when defining a property in a schema extension:</span></span>

| <span data-ttu-id="c9ce0-120">属性类型</span><span class="sxs-lookup"><span data-stu-id="c9ce0-120">Property Type</span></span> | <span data-ttu-id="c9ce0-121">备注</span><span class="sxs-lookup"><span data-stu-id="c9ce0-121">Remarks</span></span> |
|-------------|------------|
| <span data-ttu-id="c9ce0-122">Binary</span><span class="sxs-lookup"><span data-stu-id="c9ce0-122">Binary</span></span> | <span data-ttu-id="c9ce0-123">最多 256 字节。</span><span class="sxs-lookup"><span data-stu-id="c9ce0-123">256 bytes maximum.</span></span> |
| <span data-ttu-id="c9ce0-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9ce0-124">Boolean</span></span> | <span data-ttu-id="c9ce0-125">不受联系人、邮件、活动和帖子支持。</span><span class="sxs-lookup"><span data-stu-id="c9ce0-125">Not supported for contacts, messages, events and posts.</span></span> |
| <span data-ttu-id="c9ce0-126">日期时间</span><span class="sxs-lookup"><span data-stu-id="c9ce0-126">DateTime</span></span> | <span data-ttu-id="c9ce0-p102">必须以 ISO 8601 格式进行指定。存储为 UTC 格式。</span><span class="sxs-lookup"><span data-stu-id="c9ce0-p102">Must be specified in ISO 8601 format. Will be stored in UTC.</span></span> |
| <span data-ttu-id="c9ce0-129">整数</span><span class="sxs-lookup"><span data-stu-id="c9ce0-129">Integer</span></span> | <span data-ttu-id="c9ce0-130">32 位值。</span><span class="sxs-lookup"><span data-stu-id="c9ce0-130">32-bit value.</span></span> <span data-ttu-id="c9ce0-131">不受联系人、邮件、活动和帖子支持。</span><span class="sxs-lookup"><span data-stu-id="c9ce0-131">Not supported for contacts, messages, events and posts.</span></span> |
| <span data-ttu-id="c9ce0-132">字符串</span><span class="sxs-lookup"><span data-stu-id="c9ce0-132">String</span></span> | <span data-ttu-id="c9ce0-133">最多 256 个字符。</span><span class="sxs-lookup"><span data-stu-id="c9ce0-133">256 characters maximum.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c9ce0-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c9ce0-134">JSON representation</span></span>
<span data-ttu-id="c9ce0-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c9ce0-135">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "extensionSchemaProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

