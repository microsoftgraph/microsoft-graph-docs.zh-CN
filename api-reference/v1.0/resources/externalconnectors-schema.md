---
title: 架构资源类型
description: 连接架构确定添加到连接的内容如何用于各种 Microsoft Graph体验。
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: c0ca5e88d9d4ac7d7b63dea49f8ff4aace8cc348
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467258"
---
# <a name="schema-resource-type"></a><span data-ttu-id="c0c80-103">架构资源类型</span><span class="sxs-lookup"><span data-stu-id="c0c80-103">schema resource type</span></span>

<span data-ttu-id="c0c80-104">命名空间：microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="c0c80-104">Namespace: microsoft.graph.externalConnectors</span></span>

<span data-ttu-id="c0c80-105">[连接](externalconnectors-externalconnection.md)架构确定外部内容如何用于各种 Microsoft Graph体验。</span><span class="sxs-lookup"><span data-stu-id="c0c80-105">The [connection](externalconnectors-externalconnection.md) schema determines how your external content will be used in various Microsoft Graph experiences.</span></span> <span data-ttu-id="c0c80-106">架构是计划添加到连接中的所有属性的简单列表及其属性、标签和别名。</span><span class="sxs-lookup"><span data-stu-id="c0c80-106">Schema is a flat list of all the properties that you plan to add to the connection along with their attributes, labels, and aliases.</span></span> <span data-ttu-id="c0c80-107">向连接添加项目前，必须注册架构。</span><span class="sxs-lookup"><span data-stu-id="c0c80-107">You must register the schema before adding items into the connection.</span></span>

## <a name="methods"></a><span data-ttu-id="c0c80-108">方法</span><span class="sxs-lookup"><span data-stu-id="c0c80-108">Methods</span></span>
|<span data-ttu-id="c0c80-109">方法</span><span class="sxs-lookup"><span data-stu-id="c0c80-109">Method</span></span>|<span data-ttu-id="c0c80-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="c0c80-110">Return type</span></span>|<span data-ttu-id="c0c80-111">说明</span><span class="sxs-lookup"><span data-stu-id="c0c80-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c0c80-112">创建架构</span><span class="sxs-lookup"><span data-stu-id="c0c80-112">Create schema</span></span>](../api/externalconnectors-schema-create.md)|[<span data-ttu-id="c0c80-113">schema</span><span class="sxs-lookup"><span data-stu-id="c0c80-113">schema</span></span>](../resources/externalconnectors-schema.md)|<span data-ttu-id="c0c80-114">创建新的 [架构](../resources/externalconnectors-schema.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c0c80-114">Create a new [schema](../resources/externalconnectors-schema.md) object.</span></span>|
|[<span data-ttu-id="c0c80-115">获取架构</span><span class="sxs-lookup"><span data-stu-id="c0c80-115">Get schema</span></span>](../api/externalconnectors-schema-get.md)|[<span data-ttu-id="c0c80-116">schema</span><span class="sxs-lookup"><span data-stu-id="c0c80-116">schema</span></span>](../resources/externalconnectors-schema.md)|<span data-ttu-id="c0c80-117">读取架构 [对象的属性和](../resources/externalconnectors-schema.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="c0c80-117">Read the properties and relationships of a [schema](../resources/externalconnectors-schema.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c0c80-118">属性</span><span class="sxs-lookup"><span data-stu-id="c0c80-118">Properties</span></span>
|<span data-ttu-id="c0c80-119">属性</span><span class="sxs-lookup"><span data-stu-id="c0c80-119">Property</span></span>|<span data-ttu-id="c0c80-120">类型</span><span class="sxs-lookup"><span data-stu-id="c0c80-120">Type</span></span>|<span data-ttu-id="c0c80-121">说明</span><span class="sxs-lookup"><span data-stu-id="c0c80-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0c80-122">baseType</span><span class="sxs-lookup"><span data-stu-id="c0c80-122">baseType</span></span>|<span data-ttu-id="c0c80-123">String</span><span class="sxs-lookup"><span data-stu-id="c0c80-123">String</span></span>|<span data-ttu-id="c0c80-124">必须设置为 `microsoft.graph.externalConnector.externalItem`。</span><span class="sxs-lookup"><span data-stu-id="c0c80-124">Must be set to `microsoft.graph.externalConnector.externalItem`.</span></span> <span data-ttu-id="c0c80-125">必需项。</span><span class="sxs-lookup"><span data-stu-id="c0c80-125">Required.</span></span>|
|<span data-ttu-id="c0c80-126">properties</span><span class="sxs-lookup"><span data-stu-id="c0c80-126">properties</span></span>|<span data-ttu-id="c0c80-127">[property](../resources/externalconnectors-property.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c0c80-127">[property](../resources/externalconnectors-property.md) collection</span></span>|<span data-ttu-id="c0c80-128">为连接中的项目定义的属性。</span><span class="sxs-lookup"><span data-stu-id="c0c80-128">The properties defined for the items in the connection.</span></span> <span data-ttu-id="c0c80-129">最小属性数为 1，最大值为 128。</span><span class="sxs-lookup"><span data-stu-id="c0c80-129">The minimum number of properties is one, the maximum is 128.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c0c80-130">关系</span><span class="sxs-lookup"><span data-stu-id="c0c80-130">Relationships</span></span>
<span data-ttu-id="c0c80-131">无。</span><span class="sxs-lookup"><span data-stu-id="c0c80-131">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c0c80-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c0c80-132">JSON representation</span></span>
<span data-ttu-id="c0c80-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c0c80-133">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalConnectors.schema",
  "openType": false
}
-->
``` json
{
  "baseType": "String",
  "properties": [
    {
      "name": "String",
      "type": "String",
    }
  ]
}
```

