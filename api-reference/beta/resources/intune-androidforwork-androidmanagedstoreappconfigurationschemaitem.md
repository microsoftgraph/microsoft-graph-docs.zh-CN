---
title: androidManagedStoreAppConfigurationSchemaItem 资源类型
description: Android 应用程序的自定义配置架构内的单个配置项。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 39f7bb07e28875ec2d0280eb02a9d3c90b5a82e3
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36366208"
---
# <a name="androidmanagedstoreappconfigurationschemaitem-resource-type"></a><span data-ttu-id="d1972-103">androidManagedStoreAppConfigurationSchemaItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="d1972-103">androidManagedStoreAppConfigurationSchemaItem resource type</span></span>

> <span data-ttu-id="d1972-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d1972-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1972-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d1972-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1972-106">Android 应用程序的自定义配置架构内的单个配置项。</span><span class="sxs-lookup"><span data-stu-id="d1972-106">Single configuration item inside an Android application's custom configuration schema.</span></span>

## <a name="properties"></a><span data-ttu-id="d1972-107">属性</span><span class="sxs-lookup"><span data-stu-id="d1972-107">Properties</span></span>
|<span data-ttu-id="d1972-108">属性</span><span class="sxs-lookup"><span data-stu-id="d1972-108">Property</span></span>|<span data-ttu-id="d1972-109">类型</span><span class="sxs-lookup"><span data-stu-id="d1972-109">Type</span></span>|<span data-ttu-id="d1972-110">说明</span><span class="sxs-lookup"><span data-stu-id="d1972-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1972-111">index</span><span class="sxs-lookup"><span data-stu-id="d1972-111">index</span></span>|<span data-ttu-id="d1972-112">Int32</span><span class="sxs-lookup"><span data-stu-id="d1972-112">Int32</span></span>|<span data-ttu-id="d1972-113">应用程序用来维护嵌套架构项的唯一索引</span><span class="sxs-lookup"><span data-stu-id="d1972-113">Unique index the application uses to maintain nested schema items</span></span>|
|<span data-ttu-id="d1972-114">parentIndex</span><span class="sxs-lookup"><span data-stu-id="d1972-114">parentIndex</span></span>|<span data-ttu-id="d1972-115">Int32</span><span class="sxs-lookup"><span data-stu-id="d1972-115">Int32</span></span>|<span data-ttu-id="d1972-116">用于跟踪嵌套架构项的父架构项的索引</span><span class="sxs-lookup"><span data-stu-id="d1972-116">Index of parent schema item to track nested schema items</span></span>|
|<span data-ttu-id="d1972-117">schemaItemKey</span><span class="sxs-lookup"><span data-stu-id="d1972-117">schemaItemKey</span></span>|<span data-ttu-id="d1972-118">String</span><span class="sxs-lookup"><span data-stu-id="d1972-118">String</span></span>|<span data-ttu-id="d1972-119">应用程序用于标识项的唯一键</span><span class="sxs-lookup"><span data-stu-id="d1972-119">Unique key the application uses to identify the item</span></span>|
|<span data-ttu-id="d1972-120">displayName</span><span class="sxs-lookup"><span data-stu-id="d1972-120">displayName</span></span>|<span data-ttu-id="d1972-121">字符串</span><span class="sxs-lookup"><span data-stu-id="d1972-121">String</span></span>|<span data-ttu-id="d1972-122">用户可读的名称</span><span class="sxs-lookup"><span data-stu-id="d1972-122">Human readable name</span></span>|
|<span data-ttu-id="d1972-123">说明</span><span class="sxs-lookup"><span data-stu-id="d1972-123">description</span></span>|<span data-ttu-id="d1972-124">String</span><span class="sxs-lookup"><span data-stu-id="d1972-124">String</span></span>|<span data-ttu-id="d1972-125">项在应用程序内所控制内容的说明</span><span class="sxs-lookup"><span data-stu-id="d1972-125">Description of what the item controls within the application</span></span>|
|<span data-ttu-id="d1972-126">defaultBoolValue</span><span class="sxs-lookup"><span data-stu-id="d1972-126">defaultBoolValue</span></span>|<span data-ttu-id="d1972-127">布尔值</span><span class="sxs-lookup"><span data-stu-id="d1972-127">Boolean</span></span>|<span data-ttu-id="d1972-128">如果由应用开发人员指定，则为布尔类型项的默认值</span><span class="sxs-lookup"><span data-stu-id="d1972-128">Default value for boolean type items, if specified by the app developer</span></span>|
|<span data-ttu-id="d1972-129">defaultIntValue</span><span class="sxs-lookup"><span data-stu-id="d1972-129">defaultIntValue</span></span>|<span data-ttu-id="d1972-130">Int32</span><span class="sxs-lookup"><span data-stu-id="d1972-130">Int32</span></span>|<span data-ttu-id="d1972-131">如果由应用开发人员指定，则为整数类型项的默认值</span><span class="sxs-lookup"><span data-stu-id="d1972-131">Default value for integer type items, if specified by the app developer</span></span>|
|<span data-ttu-id="d1972-132">defaultStringValue</span><span class="sxs-lookup"><span data-stu-id="d1972-132">defaultStringValue</span></span>|<span data-ttu-id="d1972-133">String</span><span class="sxs-lookup"><span data-stu-id="d1972-133">String</span></span>|<span data-ttu-id="d1972-134">如果由应用开发人员指定，则为字符串类型项的默认值</span><span class="sxs-lookup"><span data-stu-id="d1972-134">Default value for string type items, if specified by the app developer</span></span>|
|<span data-ttu-id="d1972-135">defaultStringArrayValue</span><span class="sxs-lookup"><span data-stu-id="d1972-135">defaultStringArrayValue</span></span>|<span data-ttu-id="d1972-136">String collection</span><span class="sxs-lookup"><span data-stu-id="d1972-136">String collection</span></span>|<span data-ttu-id="d1972-137">如果由应用开发人员指定，则为字符串数组类型项的默认值</span><span class="sxs-lookup"><span data-stu-id="d1972-137">Default value for string array type items, if specified by the app developer</span></span>|
|<span data-ttu-id="d1972-138">DataType</span><span class="sxs-lookup"><span data-stu-id="d1972-138">dataType</span></span>|[<span data-ttu-id="d1972-139">androidManagedStoreAppConfigurationSchemaItemDataType</span><span class="sxs-lookup"><span data-stu-id="d1972-139">androidManagedStoreAppConfigurationSchemaItemDataType</span></span>](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitemdatatype.md)|<span data-ttu-id="d1972-140">此项目描述的值的类型。</span><span class="sxs-lookup"><span data-stu-id="d1972-140">The type of value this item describes.</span></span> <span data-ttu-id="d1972-141">可取值为：`bool`、`integer`、`string`、`choice`、`multiselect`、`bundle`、`bundleArray`、`hidden`。</span><span class="sxs-lookup"><span data-stu-id="d1972-141">Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span></span>|
|<span data-ttu-id="d1972-142">选择</span><span class="sxs-lookup"><span data-stu-id="d1972-142">selections</span></span>|<span data-ttu-id="d1972-143">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d1972-143">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="d1972-144">可为此项（仅 Choice 和 Multiselect 项）设置的有效值的用于可读名称/值对列表</span><span class="sxs-lookup"><span data-stu-id="d1972-144">List of human readable name/value pairs for the valid values that can be set for this item (Choice and Multiselect items only)</span></span>|

## <a name="relationships"></a><span data-ttu-id="d1972-145">关系</span><span class="sxs-lookup"><span data-stu-id="d1972-145">Relationships</span></span>
<span data-ttu-id="d1972-146">无</span><span class="sxs-lookup"><span data-stu-id="d1972-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d1972-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d1972-147">JSON Representation</span></span>
<span data-ttu-id="d1972-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d1972-148">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfigurationSchemaItem",
  "index": 1024,
  "parentIndex": 1024,
  "schemaItemKey": "String",
  "displayName": "String",
  "description": "String",
  "defaultBoolValue": true,
  "defaultIntValue": 1024,
  "defaultStringValue": "String",
  "defaultStringArrayValue": [
    "String"
  ],
  "dataType": "String",
  "selections": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ]
}
```



