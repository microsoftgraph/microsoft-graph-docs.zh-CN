---
title: androidManagedStoreAppConfigurationSchemaItem 资源类型
description: Android 应用程序的自定义配置架构内的单个配置项。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 744715e3169dd0b6b7aa4fa9a7fd9be1f341720f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43467873"
---
# <a name="androidmanagedstoreappconfigurationschemaitem-resource-type"></a><span data-ttu-id="53e5f-103">androidManagedStoreAppConfigurationSchemaItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="53e5f-103">androidManagedStoreAppConfigurationSchemaItem resource type</span></span>

<span data-ttu-id="53e5f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53e5f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="53e5f-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="53e5f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="53e5f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="53e5f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53e5f-107">Android 应用程序的自定义配置架构内的单个配置项。</span><span class="sxs-lookup"><span data-stu-id="53e5f-107">Single configuration item inside an Android application's custom configuration schema.</span></span>

## <a name="properties"></a><span data-ttu-id="53e5f-108">属性</span><span class="sxs-lookup"><span data-stu-id="53e5f-108">Properties</span></span>
|<span data-ttu-id="53e5f-109">属性</span><span class="sxs-lookup"><span data-stu-id="53e5f-109">Property</span></span>|<span data-ttu-id="53e5f-110">类型</span><span class="sxs-lookup"><span data-stu-id="53e5f-110">Type</span></span>|<span data-ttu-id="53e5f-111">说明</span><span class="sxs-lookup"><span data-stu-id="53e5f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53e5f-112">index</span><span class="sxs-lookup"><span data-stu-id="53e5f-112">index</span></span>|<span data-ttu-id="53e5f-113">Int32</span><span class="sxs-lookup"><span data-stu-id="53e5f-113">Int32</span></span>|<span data-ttu-id="53e5f-114">应用程序用来维护嵌套架构项的唯一索引</span><span class="sxs-lookup"><span data-stu-id="53e5f-114">Unique index the application uses to maintain nested schema items</span></span>|
|<span data-ttu-id="53e5f-115">parentIndex</span><span class="sxs-lookup"><span data-stu-id="53e5f-115">parentIndex</span></span>|<span data-ttu-id="53e5f-116">Int32</span><span class="sxs-lookup"><span data-stu-id="53e5f-116">Int32</span></span>|<span data-ttu-id="53e5f-117">用于跟踪嵌套架构项的父架构项的索引</span><span class="sxs-lookup"><span data-stu-id="53e5f-117">Index of parent schema item to track nested schema items</span></span>|
|<span data-ttu-id="53e5f-118">schemaItemKey</span><span class="sxs-lookup"><span data-stu-id="53e5f-118">schemaItemKey</span></span>|<span data-ttu-id="53e5f-119">String</span><span class="sxs-lookup"><span data-stu-id="53e5f-119">String</span></span>|<span data-ttu-id="53e5f-120">应用程序用于标识项的唯一键</span><span class="sxs-lookup"><span data-stu-id="53e5f-120">Unique key the application uses to identify the item</span></span>|
|<span data-ttu-id="53e5f-121">displayName</span><span class="sxs-lookup"><span data-stu-id="53e5f-121">displayName</span></span>|<span data-ttu-id="53e5f-122">字符串</span><span class="sxs-lookup"><span data-stu-id="53e5f-122">String</span></span>|<span data-ttu-id="53e5f-123">用户可读的名称</span><span class="sxs-lookup"><span data-stu-id="53e5f-123">Human readable name</span></span>|
|<span data-ttu-id="53e5f-124">description</span><span class="sxs-lookup"><span data-stu-id="53e5f-124">description</span></span>|<span data-ttu-id="53e5f-125">String</span><span class="sxs-lookup"><span data-stu-id="53e5f-125">String</span></span>|<span data-ttu-id="53e5f-126">项在应用程序内所控制内容的说明</span><span class="sxs-lookup"><span data-stu-id="53e5f-126">Description of what the item controls within the application</span></span>|
|<span data-ttu-id="53e5f-127">defaultBoolValue</span><span class="sxs-lookup"><span data-stu-id="53e5f-127">defaultBoolValue</span></span>|<span data-ttu-id="53e5f-128">布尔值</span><span class="sxs-lookup"><span data-stu-id="53e5f-128">Boolean</span></span>|<span data-ttu-id="53e5f-129">如果由应用开发人员指定，则为布尔类型项的默认值</span><span class="sxs-lookup"><span data-stu-id="53e5f-129">Default value for boolean type items, if specified by the app developer</span></span>|
|<span data-ttu-id="53e5f-130">defaultIntValue</span><span class="sxs-lookup"><span data-stu-id="53e5f-130">defaultIntValue</span></span>|<span data-ttu-id="53e5f-131">Int32</span><span class="sxs-lookup"><span data-stu-id="53e5f-131">Int32</span></span>|<span data-ttu-id="53e5f-132">如果由应用开发人员指定，则为整数类型项的默认值</span><span class="sxs-lookup"><span data-stu-id="53e5f-132">Default value for integer type items, if specified by the app developer</span></span>|
|<span data-ttu-id="53e5f-133">defaultStringValue</span><span class="sxs-lookup"><span data-stu-id="53e5f-133">defaultStringValue</span></span>|<span data-ttu-id="53e5f-134">String</span><span class="sxs-lookup"><span data-stu-id="53e5f-134">String</span></span>|<span data-ttu-id="53e5f-135">如果由应用开发人员指定，则为字符串类型项的默认值</span><span class="sxs-lookup"><span data-stu-id="53e5f-135">Default value for string type items, if specified by the app developer</span></span>|
|<span data-ttu-id="53e5f-136">defaultStringArrayValue</span><span class="sxs-lookup"><span data-stu-id="53e5f-136">defaultStringArrayValue</span></span>|<span data-ttu-id="53e5f-137">String collection</span><span class="sxs-lookup"><span data-stu-id="53e5f-137">String collection</span></span>|<span data-ttu-id="53e5f-138">如果由应用开发人员指定，则为字符串数组类型项的默认值</span><span class="sxs-lookup"><span data-stu-id="53e5f-138">Default value for string array type items, if specified by the app developer</span></span>|
|<span data-ttu-id="53e5f-139">DataType</span><span class="sxs-lookup"><span data-stu-id="53e5f-139">dataType</span></span>|[<span data-ttu-id="53e5f-140">androidManagedStoreAppConfigurationSchemaItemDataType</span><span class="sxs-lookup"><span data-stu-id="53e5f-140">androidManagedStoreAppConfigurationSchemaItemDataType</span></span>](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitemdatatype.md)|<span data-ttu-id="53e5f-141">此项目描述的值的类型。</span><span class="sxs-lookup"><span data-stu-id="53e5f-141">The type of value this item describes.</span></span> <span data-ttu-id="53e5f-142">可取值为：`bool`、`integer`、`string`、`choice`、`multiselect`、`bundle`、`bundleArray`、`hidden`。</span><span class="sxs-lookup"><span data-stu-id="53e5f-142">Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span></span>|
|<span data-ttu-id="53e5f-143">选择</span><span class="sxs-lookup"><span data-stu-id="53e5f-143">selections</span></span>|<span data-ttu-id="53e5f-144">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="53e5f-144">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="53e5f-145">可为此项（仅 Choice 和 Multiselect 项）设置的有效值的用于可读名称/值对列表</span><span class="sxs-lookup"><span data-stu-id="53e5f-145">List of human readable name/value pairs for the valid values that can be set for this item (Choice and Multiselect items only)</span></span>|

## <a name="relationships"></a><span data-ttu-id="53e5f-146">关系</span><span class="sxs-lookup"><span data-stu-id="53e5f-146">Relationships</span></span>
<span data-ttu-id="53e5f-147">无</span><span class="sxs-lookup"><span data-stu-id="53e5f-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="53e5f-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="53e5f-148">JSON Representation</span></span>
<span data-ttu-id="53e5f-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="53e5f-149">Here is a JSON representation of the resource.</span></span>
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



