---
title: androidManagedStoreAppConfigurationSchemaItem 资源类型
description: Android 应用程序的自定义配置架构内的单个配置项。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6db7a9958599cbc073fa17eef542559a65af2b8e
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42799330"
---
# <a name="androidmanagedstoreappconfigurationschemaitem-resource-type"></a><span data-ttu-id="aed5c-103">androidManagedStoreAppConfigurationSchemaItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="aed5c-103">androidManagedStoreAppConfigurationSchemaItem resource type</span></span>

> <span data-ttu-id="aed5c-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="aed5c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aed5c-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="aed5c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aed5c-106">Android 应用程序的自定义配置架构内的单个配置项。</span><span class="sxs-lookup"><span data-stu-id="aed5c-106">Single configuration item inside an Android application's custom configuration schema.</span></span>

## <a name="properties"></a><span data-ttu-id="aed5c-107">属性</span><span class="sxs-lookup"><span data-stu-id="aed5c-107">Properties</span></span>
|<span data-ttu-id="aed5c-108">属性</span><span class="sxs-lookup"><span data-stu-id="aed5c-108">Property</span></span>|<span data-ttu-id="aed5c-109">类型</span><span class="sxs-lookup"><span data-stu-id="aed5c-109">Type</span></span>|<span data-ttu-id="aed5c-110">说明</span><span class="sxs-lookup"><span data-stu-id="aed5c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aed5c-111">index</span><span class="sxs-lookup"><span data-stu-id="aed5c-111">index</span></span>|<span data-ttu-id="aed5c-112">Int32</span><span class="sxs-lookup"><span data-stu-id="aed5c-112">Int32</span></span>|<span data-ttu-id="aed5c-113">应用程序用来维护嵌套架构项的唯一索引</span><span class="sxs-lookup"><span data-stu-id="aed5c-113">Unique index the application uses to maintain nested schema items</span></span>|
|<span data-ttu-id="aed5c-114">parentIndex</span><span class="sxs-lookup"><span data-stu-id="aed5c-114">parentIndex</span></span>|<span data-ttu-id="aed5c-115">Int32</span><span class="sxs-lookup"><span data-stu-id="aed5c-115">Int32</span></span>|<span data-ttu-id="aed5c-116">用于跟踪嵌套架构项的父架构项的索引</span><span class="sxs-lookup"><span data-stu-id="aed5c-116">Index of parent schema item to track nested schema items</span></span>|
|<span data-ttu-id="aed5c-117">schemaItemKey</span><span class="sxs-lookup"><span data-stu-id="aed5c-117">schemaItemKey</span></span>|<span data-ttu-id="aed5c-118">String</span><span class="sxs-lookup"><span data-stu-id="aed5c-118">String</span></span>|<span data-ttu-id="aed5c-119">应用程序用于标识项的唯一键</span><span class="sxs-lookup"><span data-stu-id="aed5c-119">Unique key the application uses to identify the item</span></span>|
|<span data-ttu-id="aed5c-120">displayName</span><span class="sxs-lookup"><span data-stu-id="aed5c-120">displayName</span></span>|<span data-ttu-id="aed5c-121">字符串</span><span class="sxs-lookup"><span data-stu-id="aed5c-121">String</span></span>|<span data-ttu-id="aed5c-122">用户可读的名称</span><span class="sxs-lookup"><span data-stu-id="aed5c-122">Human readable name</span></span>|
|<span data-ttu-id="aed5c-123">说明</span><span class="sxs-lookup"><span data-stu-id="aed5c-123">description</span></span>|<span data-ttu-id="aed5c-124">String</span><span class="sxs-lookup"><span data-stu-id="aed5c-124">String</span></span>|<span data-ttu-id="aed5c-125">项在应用程序内所控制内容的说明</span><span class="sxs-lookup"><span data-stu-id="aed5c-125">Description of what the item controls within the application</span></span>|
|<span data-ttu-id="aed5c-126">defaultBoolValue</span><span class="sxs-lookup"><span data-stu-id="aed5c-126">defaultBoolValue</span></span>|<span data-ttu-id="aed5c-127">布尔值</span><span class="sxs-lookup"><span data-stu-id="aed5c-127">Boolean</span></span>|<span data-ttu-id="aed5c-128">如果由应用开发人员指定，则为布尔类型项的默认值</span><span class="sxs-lookup"><span data-stu-id="aed5c-128">Default value for boolean type items, if specified by the app developer</span></span>|
|<span data-ttu-id="aed5c-129">defaultIntValue</span><span class="sxs-lookup"><span data-stu-id="aed5c-129">defaultIntValue</span></span>|<span data-ttu-id="aed5c-130">Int32</span><span class="sxs-lookup"><span data-stu-id="aed5c-130">Int32</span></span>|<span data-ttu-id="aed5c-131">如果由应用开发人员指定，则为整数类型项的默认值</span><span class="sxs-lookup"><span data-stu-id="aed5c-131">Default value for integer type items, if specified by the app developer</span></span>|
|<span data-ttu-id="aed5c-132">defaultStringValue</span><span class="sxs-lookup"><span data-stu-id="aed5c-132">defaultStringValue</span></span>|<span data-ttu-id="aed5c-133">String</span><span class="sxs-lookup"><span data-stu-id="aed5c-133">String</span></span>|<span data-ttu-id="aed5c-134">如果由应用开发人员指定，则为字符串类型项的默认值</span><span class="sxs-lookup"><span data-stu-id="aed5c-134">Default value for string type items, if specified by the app developer</span></span>|
|<span data-ttu-id="aed5c-135">defaultStringArrayValue</span><span class="sxs-lookup"><span data-stu-id="aed5c-135">defaultStringArrayValue</span></span>|<span data-ttu-id="aed5c-136">String collection</span><span class="sxs-lookup"><span data-stu-id="aed5c-136">String collection</span></span>|<span data-ttu-id="aed5c-137">如果由应用开发人员指定，则为字符串数组类型项的默认值</span><span class="sxs-lookup"><span data-stu-id="aed5c-137">Default value for string array type items, if specified by the app developer</span></span>|
|<span data-ttu-id="aed5c-138">DataType</span><span class="sxs-lookup"><span data-stu-id="aed5c-138">dataType</span></span>|[<span data-ttu-id="aed5c-139">androidManagedStoreAppConfigurationSchemaItemDataType</span><span class="sxs-lookup"><span data-stu-id="aed5c-139">androidManagedStoreAppConfigurationSchemaItemDataType</span></span>](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitemdatatype.md)|<span data-ttu-id="aed5c-140">此项目描述的值的类型。</span><span class="sxs-lookup"><span data-stu-id="aed5c-140">The type of value this item describes.</span></span> <span data-ttu-id="aed5c-141">可取值为：`bool`、`integer`、`string`、`choice`、`multiselect`、`bundle`、`bundleArray`、`hidden`。</span><span class="sxs-lookup"><span data-stu-id="aed5c-141">Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span></span>|
|<span data-ttu-id="aed5c-142">选择</span><span class="sxs-lookup"><span data-stu-id="aed5c-142">selections</span></span>|<span data-ttu-id="aed5c-143">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="aed5c-143">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="aed5c-144">可为此项（仅 Choice 和 Multiselect 项）设置的有效值的用于可读名称/值对列表</span><span class="sxs-lookup"><span data-stu-id="aed5c-144">List of human readable name/value pairs for the valid values that can be set for this item (Choice and Multiselect items only)</span></span>|

## <a name="relationships"></a><span data-ttu-id="aed5c-145">关系</span><span class="sxs-lookup"><span data-stu-id="aed5c-145">Relationships</span></span>
<span data-ttu-id="aed5c-146">无</span><span class="sxs-lookup"><span data-stu-id="aed5c-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="aed5c-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aed5c-147">JSON Representation</span></span>
<span data-ttu-id="aed5c-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aed5c-148">Here is a JSON representation of the resource.</span></span>
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



