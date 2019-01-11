---
title: extensionSchemaProperty 资源类型
description: 使用 **extensionSchemaProperty** 资源将属性的名称及其类型定义为 schemaExtension 定义的一部分。
localization_priority: Normal
ms.openlocfilehash: 44769bab4a4f4b40a80d896bed2311554ea5e8ad
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889857"
---
# <a name="extensionschemaproperty-resource-type"></a><span data-ttu-id="6093f-103">extensionSchemaProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="6093f-103">extensionSchemaProperty resource type</span></span>

> <span data-ttu-id="6093f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6093f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6093f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6093f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6093f-106">使用 **extensionSchemaProperty** 资源将属性的名称及其类型定义为 [schemaExtension](schemaextension.md) 定义的一部分。</span><span class="sxs-lookup"><span data-stu-id="6093f-106">Use the **extensionSchemaProperty** resource to define a property's name and its type, as part of a [schemaExtension](schemaextension.md) definition.</span></span>


## <a name="properties"></a><span data-ttu-id="6093f-107">属性</span><span class="sxs-lookup"><span data-stu-id="6093f-107">Properties</span></span>
| <span data-ttu-id="6093f-108">属性</span><span class="sxs-lookup"><span data-stu-id="6093f-108">Property</span></span>     | <span data-ttu-id="6093f-109">类型</span><span class="sxs-lookup"><span data-stu-id="6093f-109">Type</span></span>   |<span data-ttu-id="6093f-110">说明</span><span class="sxs-lookup"><span data-stu-id="6093f-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6093f-111">name</span><span class="sxs-lookup"><span data-stu-id="6093f-111">name</span></span>|<span data-ttu-id="6093f-112">字符串</span><span class="sxs-lookup"><span data-stu-id="6093f-112">String</span></span>| <span data-ttu-id="6093f-113">架构扩展的一部分定义的强类型属性的名称。</span><span class="sxs-lookup"><span data-stu-id="6093f-113">The name of the strongly typed property defined as part of a schema extension.</span></span>|
|<span data-ttu-id="6093f-114">type</span><span class="sxs-lookup"><span data-stu-id="6093f-114">type</span></span>|<span data-ttu-id="6093f-115">String</span><span class="sxs-lookup"><span data-stu-id="6093f-115">String</span></span>| <span data-ttu-id="6093f-p102">被定义为架构扩展组成部分的属性的类型。允许的值为 *Binary、Boolean、DateTime、Integer* 或 *String*。请参阅下表获取更多详细信息。</span><span class="sxs-lookup"><span data-stu-id="6093f-p102">The type of the property that is defined as part of a schema extension.  Allowed values are *Binary, Boolean, DateTime, Integer* or *String*.  See the table below for more details.</span></span>|

#### <a name="supported-property-data-types"></a><span data-ttu-id="6093f-119">受支持的属性数据类型</span><span class="sxs-lookup"><span data-stu-id="6093f-119">Supported property data types</span></span> 
<span data-ttu-id="6093f-120">在架构扩展中定义属性时，支持以下数据类型：</span><span class="sxs-lookup"><span data-stu-id="6093f-120">The following data types are supported when defining a property in a schema extension:</span></span>

| <span data-ttu-id="6093f-121">属性类型</span><span class="sxs-lookup"><span data-stu-id="6093f-121">Property Type</span></span> | <span data-ttu-id="6093f-122">备注</span><span class="sxs-lookup"><span data-stu-id="6093f-122">Remarks</span></span> |
|-------------|------------|
| <span data-ttu-id="6093f-123">Binary</span><span class="sxs-lookup"><span data-stu-id="6093f-123">Binary</span></span> | <span data-ttu-id="6093f-124">最多 256 字节。</span><span class="sxs-lookup"><span data-stu-id="6093f-124">256 bytes maximum.</span></span> |
| <span data-ttu-id="6093f-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="6093f-125">Boolean</span></span> | <span data-ttu-id="6093f-126">不支持消息、活动和帖子。</span><span class="sxs-lookup"><span data-stu-id="6093f-126">Not supported for messages, events and posts.</span></span> |
| <span data-ttu-id="6093f-127">日期时间</span><span class="sxs-lookup"><span data-stu-id="6093f-127">DateTime</span></span> | <span data-ttu-id="6093f-p103">必须以 ISO 8601 格式进行指定。存储为 UTC 格式。</span><span class="sxs-lookup"><span data-stu-id="6093f-p103">Must be specified in ISO 8601 format. Will be stored in UTC.</span></span> |
| <span data-ttu-id="6093f-130">整数</span><span class="sxs-lookup"><span data-stu-id="6093f-130">Integer</span></span> | <span data-ttu-id="6093f-p104">32 位值。不支持消息、活动和帖子。</span><span class="sxs-lookup"><span data-stu-id="6093f-p104">32-bit value. Not supported for messages, events and posts.</span></span> |
| <span data-ttu-id="6093f-133">字符串</span><span class="sxs-lookup"><span data-stu-id="6093f-133">String</span></span> | <span data-ttu-id="6093f-134">最多 256 个字符。</span><span class="sxs-lookup"><span data-stu-id="6093f-134">256 characters maximum.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6093f-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6093f-135">JSON representation</span></span>
<span data-ttu-id="6093f-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6093f-136">Here is a JSON representation of the resource.</span></span>

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
