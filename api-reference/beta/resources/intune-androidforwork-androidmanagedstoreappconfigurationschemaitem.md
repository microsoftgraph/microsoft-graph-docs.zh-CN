---
title: androidManagedStoreAppConfigurationSchemaItem 资源类型
description: Android 应用程序的自定义配置架构内的单个配置项。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3f3dc6d00c2d5b579b99a8fe17cca5d3e54482aa
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42494595"
---
# <a name="androidmanagedstoreappconfigurationschemaitem-resource-type"></a><span data-ttu-id="4d7a2-103">androidManagedStoreAppConfigurationSchemaItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="4d7a2-103">androidManagedStoreAppConfigurationSchemaItem resource type</span></span>

<span data-ttu-id="4d7a2-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="4d7a2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4d7a2-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4d7a2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4d7a2-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4d7a2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d7a2-107">Android 应用程序的自定义配置架构内的单个配置项。</span><span class="sxs-lookup"><span data-stu-id="4d7a2-107">Single configuration item inside an Android application's custom configuration schema.</span></span>

## <a name="properties"></a><span data-ttu-id="4d7a2-108">属性</span><span class="sxs-lookup"><span data-stu-id="4d7a2-108">Properties</span></span>
|<span data-ttu-id="4d7a2-109">属性</span><span class="sxs-lookup"><span data-stu-id="4d7a2-109">Property</span></span>|<span data-ttu-id="4d7a2-110">类型</span><span class="sxs-lookup"><span data-stu-id="4d7a2-110">Type</span></span>|<span data-ttu-id="4d7a2-111">说明</span><span class="sxs-lookup"><span data-stu-id="4d7a2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d7a2-112">index</span><span class="sxs-lookup"><span data-stu-id="4d7a2-112">index</span></span>|<span data-ttu-id="4d7a2-113">Int32</span><span class="sxs-lookup"><span data-stu-id="4d7a2-113">Int32</span></span>|<span data-ttu-id="4d7a2-114">应用程序用来维护嵌套架构项的唯一索引</span><span class="sxs-lookup"><span data-stu-id="4d7a2-114">Unique index the application uses to maintain nested schema items</span></span>|
|<span data-ttu-id="4d7a2-115">parentIndex</span><span class="sxs-lookup"><span data-stu-id="4d7a2-115">parentIndex</span></span>|<span data-ttu-id="4d7a2-116">Int32</span><span class="sxs-lookup"><span data-stu-id="4d7a2-116">Int32</span></span>|<span data-ttu-id="4d7a2-117">用于跟踪嵌套架构项的父架构项的索引</span><span class="sxs-lookup"><span data-stu-id="4d7a2-117">Index of parent schema item to track nested schema items</span></span>|
|<span data-ttu-id="4d7a2-118">schemaItemKey</span><span class="sxs-lookup"><span data-stu-id="4d7a2-118">schemaItemKey</span></span>|<span data-ttu-id="4d7a2-119">String</span><span class="sxs-lookup"><span data-stu-id="4d7a2-119">String</span></span>|<span data-ttu-id="4d7a2-120">应用程序用于标识项的唯一键</span><span class="sxs-lookup"><span data-stu-id="4d7a2-120">Unique key the application uses to identify the item</span></span>|
|<span data-ttu-id="4d7a2-121">displayName</span><span class="sxs-lookup"><span data-stu-id="4d7a2-121">displayName</span></span>|<span data-ttu-id="4d7a2-122">字符串</span><span class="sxs-lookup"><span data-stu-id="4d7a2-122">String</span></span>|<span data-ttu-id="4d7a2-123">用户可读的名称</span><span class="sxs-lookup"><span data-stu-id="4d7a2-123">Human readable name</span></span>|
|<span data-ttu-id="4d7a2-124">说明</span><span class="sxs-lookup"><span data-stu-id="4d7a2-124">description</span></span>|<span data-ttu-id="4d7a2-125">String</span><span class="sxs-lookup"><span data-stu-id="4d7a2-125">String</span></span>|<span data-ttu-id="4d7a2-126">项在应用程序内所控制内容的说明</span><span class="sxs-lookup"><span data-stu-id="4d7a2-126">Description of what the item controls within the application</span></span>|
|<span data-ttu-id="4d7a2-127">defaultBoolValue</span><span class="sxs-lookup"><span data-stu-id="4d7a2-127">defaultBoolValue</span></span>|<span data-ttu-id="4d7a2-128">布尔值</span><span class="sxs-lookup"><span data-stu-id="4d7a2-128">Boolean</span></span>|<span data-ttu-id="4d7a2-129">如果由应用开发人员指定，则为布尔类型项的默认值</span><span class="sxs-lookup"><span data-stu-id="4d7a2-129">Default value for boolean type items, if specified by the app developer</span></span>|
|<span data-ttu-id="4d7a2-130">defaultIntValue</span><span class="sxs-lookup"><span data-stu-id="4d7a2-130">defaultIntValue</span></span>|<span data-ttu-id="4d7a2-131">Int32</span><span class="sxs-lookup"><span data-stu-id="4d7a2-131">Int32</span></span>|<span data-ttu-id="4d7a2-132">如果由应用开发人员指定，则为整数类型项的默认值</span><span class="sxs-lookup"><span data-stu-id="4d7a2-132">Default value for integer type items, if specified by the app developer</span></span>|
|<span data-ttu-id="4d7a2-133">defaultStringValue</span><span class="sxs-lookup"><span data-stu-id="4d7a2-133">defaultStringValue</span></span>|<span data-ttu-id="4d7a2-134">String</span><span class="sxs-lookup"><span data-stu-id="4d7a2-134">String</span></span>|<span data-ttu-id="4d7a2-135">如果由应用开发人员指定，则为字符串类型项的默认值</span><span class="sxs-lookup"><span data-stu-id="4d7a2-135">Default value for string type items, if specified by the app developer</span></span>|
|<span data-ttu-id="4d7a2-136">defaultStringArrayValue</span><span class="sxs-lookup"><span data-stu-id="4d7a2-136">defaultStringArrayValue</span></span>|<span data-ttu-id="4d7a2-137">String collection</span><span class="sxs-lookup"><span data-stu-id="4d7a2-137">String collection</span></span>|<span data-ttu-id="4d7a2-138">如果由应用开发人员指定，则为字符串数组类型项的默认值</span><span class="sxs-lookup"><span data-stu-id="4d7a2-138">Default value for string array type items, if specified by the app developer</span></span>|
|<span data-ttu-id="4d7a2-139">DataType</span><span class="sxs-lookup"><span data-stu-id="4d7a2-139">dataType</span></span>|[<span data-ttu-id="4d7a2-140">androidManagedStoreAppConfigurationSchemaItemDataType</span><span class="sxs-lookup"><span data-stu-id="4d7a2-140">androidManagedStoreAppConfigurationSchemaItemDataType</span></span>](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitemdatatype.md)|<span data-ttu-id="4d7a2-141">此项目描述的值的类型。</span><span class="sxs-lookup"><span data-stu-id="4d7a2-141">The type of value this item describes.</span></span> <span data-ttu-id="4d7a2-142">可取值为：`bool`、`integer`、`string`、`choice`、`multiselect`、`bundle`、`bundleArray`、`hidden`。</span><span class="sxs-lookup"><span data-stu-id="4d7a2-142">Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span></span>|
|<span data-ttu-id="4d7a2-143">选择</span><span class="sxs-lookup"><span data-stu-id="4d7a2-143">selections</span></span>|<span data-ttu-id="4d7a2-144">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4d7a2-144">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="4d7a2-145">可为此项（仅 Choice 和 Multiselect 项）设置的有效值的用于可读名称/值对列表</span><span class="sxs-lookup"><span data-stu-id="4d7a2-145">List of human readable name/value pairs for the valid values that can be set for this item (Choice and Multiselect items only)</span></span>|

## <a name="relationships"></a><span data-ttu-id="4d7a2-146">关系</span><span class="sxs-lookup"><span data-stu-id="4d7a2-146">Relationships</span></span>
<span data-ttu-id="4d7a2-147">无</span><span class="sxs-lookup"><span data-stu-id="4d7a2-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4d7a2-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4d7a2-148">JSON Representation</span></span>
<span data-ttu-id="4d7a2-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4d7a2-149">Here is a JSON representation of the resource.</span></span>
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



