---
title: extensionSchemaProperty 资源类型
description: 使用 **extensionSchemaProperty** 资源将属性的名称及其类型定义为 schemaExtension 定义的一部分。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a684d71aa25267c1b2f19f13d35d796825783544
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531451"
---
# <a name="extensionschemaproperty-resource-type"></a><span data-ttu-id="af88d-103">extensionSchemaProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="af88d-103">extensionSchemaProperty resource type</span></span>

<span data-ttu-id="af88d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af88d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="af88d-105">使用 **extensionSchemaProperty** 资源将属性的名称及其类型定义为 [schemaExtension](schemaextension.md) 定义的一部分。</span><span class="sxs-lookup"><span data-stu-id="af88d-105">Use the **extensionSchemaProperty** resource to define a property's name and its type, as part of a [schemaExtension](schemaextension.md) definition.</span></span>


## <a name="properties"></a><span data-ttu-id="af88d-106">属性</span><span class="sxs-lookup"><span data-stu-id="af88d-106">Properties</span></span>
| <span data-ttu-id="af88d-107">属性</span><span class="sxs-lookup"><span data-stu-id="af88d-107">Property</span></span>     | <span data-ttu-id="af88d-108">类型</span><span class="sxs-lookup"><span data-stu-id="af88d-108">Type</span></span>   |<span data-ttu-id="af88d-109">说明</span><span class="sxs-lookup"><span data-stu-id="af88d-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="af88d-110">name</span><span class="sxs-lookup"><span data-stu-id="af88d-110">name</span></span>|<span data-ttu-id="af88d-111">String</span><span class="sxs-lookup"><span data-stu-id="af88d-111">String</span></span>| <span data-ttu-id="af88d-112">被定义为架构扩展组成部分的强类型属性的名称。</span><span class="sxs-lookup"><span data-stu-id="af88d-112">The name of the strongly-typed property defined as part of a schema extension.</span></span>|
|<span data-ttu-id="af88d-113">type</span><span class="sxs-lookup"><span data-stu-id="af88d-113">type</span></span>|<span data-ttu-id="af88d-114">字符串</span><span class="sxs-lookup"><span data-stu-id="af88d-114">String</span></span>| <span data-ttu-id="af88d-p101">被定义为架构扩展组成部分的属性的类型。允许的值为 *Binary、Boolean、DateTime、Integer* 或 *String*。请参阅下表获取更多详细信息。</span><span class="sxs-lookup"><span data-stu-id="af88d-p101">The type of the property that is defined as part of a schema extension.  Allowed values are *Binary, Boolean, DateTime, Integer* or *String*.  See the table below for more details.</span></span>|

#### <a name="supported-property-data-types"></a><span data-ttu-id="af88d-118">受支持的属性数据类型</span><span class="sxs-lookup"><span data-stu-id="af88d-118">Supported property data types</span></span> 
<span data-ttu-id="af88d-119">在架构扩展中定义属性时，支持以下数据类型：</span><span class="sxs-lookup"><span data-stu-id="af88d-119">The following data types are supported when defining a property in a schema extension:</span></span>

| <span data-ttu-id="af88d-120">属性类型</span><span class="sxs-lookup"><span data-stu-id="af88d-120">Property Type</span></span> | <span data-ttu-id="af88d-121">备注</span><span class="sxs-lookup"><span data-stu-id="af88d-121">Remarks</span></span> |
|-------------|------------|
| <span data-ttu-id="af88d-122">Binary</span><span class="sxs-lookup"><span data-stu-id="af88d-122">Binary</span></span> | <span data-ttu-id="af88d-123">最多 256 字节。</span><span class="sxs-lookup"><span data-stu-id="af88d-123">256 bytes maximum.</span></span> |
| <span data-ttu-id="af88d-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="af88d-124">Boolean</span></span> | <span data-ttu-id="af88d-125">不受联系人、邮件、活动和帖子支持。</span><span class="sxs-lookup"><span data-stu-id="af88d-125">Not supported for contacts, messages, events and posts.</span></span> |
| <span data-ttu-id="af88d-126">日期时间</span><span class="sxs-lookup"><span data-stu-id="af88d-126">DateTime</span></span> | <span data-ttu-id="af88d-p102">必须以 ISO 8601 格式进行指定。存储为 UTC 格式。</span><span class="sxs-lookup"><span data-stu-id="af88d-p102">Must be specified in ISO 8601 format. Will be stored in UTC.</span></span> |
| <span data-ttu-id="af88d-129">整数</span><span class="sxs-lookup"><span data-stu-id="af88d-129">Integer</span></span> | <span data-ttu-id="af88d-130">32 位值。</span><span class="sxs-lookup"><span data-stu-id="af88d-130">32-bit value.</span></span> <span data-ttu-id="af88d-131">不受联系人、邮件、活动和帖子支持。</span><span class="sxs-lookup"><span data-stu-id="af88d-131">Not supported for contacts, messages, events and posts.</span></span> |
| <span data-ttu-id="af88d-132">字符串</span><span class="sxs-lookup"><span data-stu-id="af88d-132">String</span></span> | <span data-ttu-id="af88d-133">最多 256 个字符。</span><span class="sxs-lookup"><span data-stu-id="af88d-133">256 characters maximum.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="af88d-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="af88d-134">JSON representation</span></span>
<span data-ttu-id="af88d-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="af88d-135">Here is a JSON representation of the resource.</span></span>

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
