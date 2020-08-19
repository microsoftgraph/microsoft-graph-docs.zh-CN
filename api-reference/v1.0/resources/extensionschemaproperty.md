---
title: extensionSchemaProperty 资源类型
description: 使用 **extensionSchemaProperty** 资源将属性的名称及其类型定义为 schemaExtension 定义的一部分。
localization_priority: Normal
author: keylimesoda
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 623dd4fa92036a3c542bebf791dc802ce0d53520
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812335"
---
# <a name="extensionschemaproperty-resource-type"></a><span data-ttu-id="711cc-103">extensionSchemaProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="711cc-103">extensionSchemaProperty resource type</span></span>

<span data-ttu-id="711cc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="711cc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="711cc-105">使用 **extensionSchemaProperty** 资源将属性的名称及其类型定义为 [schemaExtension](schemaextension.md) 定义的一部分。</span><span class="sxs-lookup"><span data-stu-id="711cc-105">Use the **extensionSchemaProperty** resource to define a property's name and its type, as part of a [schemaExtension](schemaextension.md) definition.</span></span>


## <a name="properties"></a><span data-ttu-id="711cc-106">属性</span><span class="sxs-lookup"><span data-stu-id="711cc-106">Properties</span></span>
| <span data-ttu-id="711cc-107">属性</span><span class="sxs-lookup"><span data-stu-id="711cc-107">Property</span></span>     | <span data-ttu-id="711cc-108">类型</span><span class="sxs-lookup"><span data-stu-id="711cc-108">Type</span></span>   |<span data-ttu-id="711cc-109">说明</span><span class="sxs-lookup"><span data-stu-id="711cc-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="711cc-110">name</span><span class="sxs-lookup"><span data-stu-id="711cc-110">name</span></span>|<span data-ttu-id="711cc-111">String</span><span class="sxs-lookup"><span data-stu-id="711cc-111">String</span></span>| <span data-ttu-id="711cc-112">被定义为架构扩展组成部分的强类型属性的名称。</span><span class="sxs-lookup"><span data-stu-id="711cc-112">The name of the strongly-typed property defined as part of a schema extension.</span></span>|
|<span data-ttu-id="711cc-113">type</span><span class="sxs-lookup"><span data-stu-id="711cc-113">type</span></span>|<span data-ttu-id="711cc-114">String</span><span class="sxs-lookup"><span data-stu-id="711cc-114">String</span></span>| <span data-ttu-id="711cc-p101">被定义为架构扩展组成部分的属性的类型。允许的值为 *Binary、Boolean、DateTime、Integer* 或 *String*。请参阅下表获取更多详细信息。</span><span class="sxs-lookup"><span data-stu-id="711cc-p101">The type of the property that is defined as part of a schema extension.  Allowed values are *Binary, Boolean, DateTime, Integer* or *String*.  See the table below for more details.</span></span>|

#### <a name="supported-property-data-types"></a><span data-ttu-id="711cc-118">受支持的属性数据类型</span><span class="sxs-lookup"><span data-stu-id="711cc-118">Supported property data types</span></span>
<span data-ttu-id="711cc-119">在架构扩展中定义属性时，支持以下数据类型：</span><span class="sxs-lookup"><span data-stu-id="711cc-119">The following data types are supported when defining a property in a schema extension:</span></span>

| <span data-ttu-id="711cc-120">属性类型</span><span class="sxs-lookup"><span data-stu-id="711cc-120">Property Type</span></span> | <span data-ttu-id="711cc-121">备注</span><span class="sxs-lookup"><span data-stu-id="711cc-121">Remarks</span></span> |
|-------------|------------|
| <span data-ttu-id="711cc-122">Binary</span><span class="sxs-lookup"><span data-stu-id="711cc-122">Binary</span></span> | <span data-ttu-id="711cc-123">最多 256 字节。</span><span class="sxs-lookup"><span data-stu-id="711cc-123">256 bytes maximum.</span></span> |
| <span data-ttu-id="711cc-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="711cc-124">Boolean</span></span> | <span data-ttu-id="711cc-125">不受联系人、邮件、活动和帖子支持。</span><span class="sxs-lookup"><span data-stu-id="711cc-125">Not supported for contacts, messages, events and posts.</span></span> |
| <span data-ttu-id="711cc-126">日期时间</span><span class="sxs-lookup"><span data-stu-id="711cc-126">DateTime</span></span> | <span data-ttu-id="711cc-p102">必须以 ISO 8601 格式进行指定。存储为 UTC 格式。</span><span class="sxs-lookup"><span data-stu-id="711cc-p102">Must be specified in ISO 8601 format. Will be stored in UTC.</span></span> |
| <span data-ttu-id="711cc-129">整数</span><span class="sxs-lookup"><span data-stu-id="711cc-129">Integer</span></span> | <span data-ttu-id="711cc-130">32 位值。</span><span class="sxs-lookup"><span data-stu-id="711cc-130">32-bit value.</span></span> <span data-ttu-id="711cc-131">不受联系人、邮件、活动和帖子支持。</span><span class="sxs-lookup"><span data-stu-id="711cc-131">Not supported for contacts, messages, events and posts.</span></span> |
| <span data-ttu-id="711cc-132">字符串</span><span class="sxs-lookup"><span data-stu-id="711cc-132">String</span></span> | <span data-ttu-id="711cc-133">最多 256 个字符。</span><span class="sxs-lookup"><span data-stu-id="711cc-133">256 characters maximum.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="711cc-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="711cc-134">JSON representation</span></span>
<span data-ttu-id="711cc-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="711cc-135">Here is a JSON representation of the resource.</span></span>

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
