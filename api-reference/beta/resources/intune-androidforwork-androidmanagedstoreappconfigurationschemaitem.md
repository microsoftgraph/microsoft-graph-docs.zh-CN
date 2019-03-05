---
title: androidManagedStoreAppConfigurationSchemaItem 资源类型
description: Android 应用程序的自定义配置架构内的单个配置项。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8acd3dc2eddbab3433c30289a8273fd8ca397848
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169200"
---
# <a name="androidmanagedstoreappconfigurationschemaitem-resource-type"></a><span data-ttu-id="b3066-103">androidManagedStoreAppConfigurationSchemaItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="b3066-103">androidManagedStoreAppConfigurationSchemaItem resource type</span></span>

> <span data-ttu-id="b3066-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b3066-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b3066-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b3066-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3066-106">Android 应用程序的自定义配置架构内的单个配置项。</span><span class="sxs-lookup"><span data-stu-id="b3066-106">Single configuration item inside an Android application's custom configuration schema.</span></span>

## <a name="properties"></a><span data-ttu-id="b3066-107">属性</span><span class="sxs-lookup"><span data-stu-id="b3066-107">Properties</span></span>
|<span data-ttu-id="b3066-108">属性</span><span class="sxs-lookup"><span data-stu-id="b3066-108">Property</span></span>|<span data-ttu-id="b3066-109">类型</span><span class="sxs-lookup"><span data-stu-id="b3066-109">Type</span></span>|<span data-ttu-id="b3066-110">说明</span><span class="sxs-lookup"><span data-stu-id="b3066-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3066-111">schemaItemKey</span><span class="sxs-lookup"><span data-stu-id="b3066-111">schemaItemKey</span></span>|<span data-ttu-id="b3066-112">String</span><span class="sxs-lookup"><span data-stu-id="b3066-112">String</span></span>|<span data-ttu-id="b3066-113">应用程序用于标识项的唯一键</span><span class="sxs-lookup"><span data-stu-id="b3066-113">Unique key the application uses to identify the item</span></span>|
|<span data-ttu-id="b3066-114">displayName</span><span class="sxs-lookup"><span data-stu-id="b3066-114">displayName</span></span>|<span data-ttu-id="b3066-115">String</span><span class="sxs-lookup"><span data-stu-id="b3066-115">String</span></span>|<span data-ttu-id="b3066-116">用户可读的名称</span><span class="sxs-lookup"><span data-stu-id="b3066-116">Human readable name</span></span>|
|<span data-ttu-id="b3066-117">说明</span><span class="sxs-lookup"><span data-stu-id="b3066-117">description</span></span>|<span data-ttu-id="b3066-118">String</span><span class="sxs-lookup"><span data-stu-id="b3066-118">String</span></span>|<span data-ttu-id="b3066-119">项在应用程序内所控制内容的说明</span><span class="sxs-lookup"><span data-stu-id="b3066-119">Description of what the item controls within the application</span></span>|
|<span data-ttu-id="b3066-120">defaultBoolValue</span><span class="sxs-lookup"><span data-stu-id="b3066-120">defaultBoolValue</span></span>|<span data-ttu-id="b3066-121">布尔值</span><span class="sxs-lookup"><span data-stu-id="b3066-121">Boolean</span></span>|<span data-ttu-id="b3066-122">如果由应用开发人员指定，则为布尔类型项的默认值</span><span class="sxs-lookup"><span data-stu-id="b3066-122">Default value for boolean type items, if specified by the app developer</span></span>|
|<span data-ttu-id="b3066-123">defaultIntValue</span><span class="sxs-lookup"><span data-stu-id="b3066-123">defaultIntValue</span></span>|<span data-ttu-id="b3066-124">Int32</span><span class="sxs-lookup"><span data-stu-id="b3066-124">Int32</span></span>|<span data-ttu-id="b3066-125">如果由应用开发人员指定，则为整数类型项的默认值</span><span class="sxs-lookup"><span data-stu-id="b3066-125">Default value for integer type items, if specified by the app developer</span></span>|
|<span data-ttu-id="b3066-126">defaultStringValue</span><span class="sxs-lookup"><span data-stu-id="b3066-126">defaultStringValue</span></span>|<span data-ttu-id="b3066-127">String</span><span class="sxs-lookup"><span data-stu-id="b3066-127">String</span></span>|<span data-ttu-id="b3066-128">如果由应用开发人员指定，则为字符串类型项的默认值</span><span class="sxs-lookup"><span data-stu-id="b3066-128">Default value for string type items, if specified by the app developer</span></span>|
|<span data-ttu-id="b3066-129">defaultStringArrayValue</span><span class="sxs-lookup"><span data-stu-id="b3066-129">defaultStringArrayValue</span></span>|<span data-ttu-id="b3066-130">String collection</span><span class="sxs-lookup"><span data-stu-id="b3066-130">String collection</span></span>|<span data-ttu-id="b3066-131">如果由应用开发人员指定，则为字符串数组类型项的默认值</span><span class="sxs-lookup"><span data-stu-id="b3066-131">Default value for string array type items, if specified by the app developer</span></span>|
|<span data-ttu-id="b3066-132">DataType</span><span class="sxs-lookup"><span data-stu-id="b3066-132">dataType</span></span>|[<span data-ttu-id="b3066-133">androidManagedStoreAppConfigurationSchemaItemDataType</span><span class="sxs-lookup"><span data-stu-id="b3066-133">androidManagedStoreAppConfigurationSchemaItemDataType</span></span>](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitemdatatype.md)|<span data-ttu-id="b3066-134">此项目描述的值的类型。</span><span class="sxs-lookup"><span data-stu-id="b3066-134">The type of value this item describes.</span></span> <span data-ttu-id="b3066-135">可取值为：`bool`、`integer`、`string`、`choice`、`multiselect`、`bundle`、`bundleArray`、`hidden`。</span><span class="sxs-lookup"><span data-stu-id="b3066-135">Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span></span>|
|<span data-ttu-id="b3066-136">选择</span><span class="sxs-lookup"><span data-stu-id="b3066-136">selections</span></span>|<span data-ttu-id="b3066-137">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b3066-137">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="b3066-138">可为此项（仅 Choice 和 Multiselect 项）设置的有效值的用于可读名称/值对列表</span><span class="sxs-lookup"><span data-stu-id="b3066-138">List of human readable name/value pairs for the valid values that can be set for this item (Choice and Multiselect items only)</span></span>|

## <a name="relationships"></a><span data-ttu-id="b3066-139">关系</span><span class="sxs-lookup"><span data-stu-id="b3066-139">Relationships</span></span>
<span data-ttu-id="b3066-140">无</span><span class="sxs-lookup"><span data-stu-id="b3066-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b3066-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b3066-141">JSON Representation</span></span>
<span data-ttu-id="b3066-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b3066-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfigurationSchemaItem",
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




