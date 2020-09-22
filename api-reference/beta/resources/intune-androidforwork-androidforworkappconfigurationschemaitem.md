---
title: androidForWorkAppConfigurationSchemaItem 资源类型
description: Android for Work 应用程序的自定义配置架构内的单个配置项。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 13af3b581498a4285773b2fda02d5596127c3012
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48019668"
---
# <a name="androidforworkappconfigurationschemaitem-resource-type"></a><span data-ttu-id="d10f7-103">androidForWorkAppConfigurationSchemaItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="d10f7-103">androidForWorkAppConfigurationSchemaItem resource type</span></span>

<span data-ttu-id="d10f7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d10f7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d10f7-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d10f7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d10f7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d10f7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d10f7-107">Android for Work 应用程序的自定义配置架构内的单个配置项。</span><span class="sxs-lookup"><span data-stu-id="d10f7-107">Single configuration item inside an Android for Work application's custom configuration schema.</span></span>

## <a name="properties"></a><span data-ttu-id="d10f7-108">属性</span><span class="sxs-lookup"><span data-stu-id="d10f7-108">Properties</span></span>
|<span data-ttu-id="d10f7-109">属性</span><span class="sxs-lookup"><span data-stu-id="d10f7-109">Property</span></span>|<span data-ttu-id="d10f7-110">类型</span><span class="sxs-lookup"><span data-stu-id="d10f7-110">Type</span></span>|<span data-ttu-id="d10f7-111">说明</span><span class="sxs-lookup"><span data-stu-id="d10f7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d10f7-112">schemaItemKey</span><span class="sxs-lookup"><span data-stu-id="d10f7-112">schemaItemKey</span></span>|<span data-ttu-id="d10f7-113">String</span><span class="sxs-lookup"><span data-stu-id="d10f7-113">String</span></span>|<span data-ttu-id="d10f7-114">应用程序用于标识项的唯一键</span><span class="sxs-lookup"><span data-stu-id="d10f7-114">Unique key the application uses to identify the item</span></span>|
|<span data-ttu-id="d10f7-115">displayName</span><span class="sxs-lookup"><span data-stu-id="d10f7-115">displayName</span></span>|<span data-ttu-id="d10f7-116">String</span><span class="sxs-lookup"><span data-stu-id="d10f7-116">String</span></span>|<span data-ttu-id="d10f7-117">用户可读的名称</span><span class="sxs-lookup"><span data-stu-id="d10f7-117">Human readable name</span></span>|
|<span data-ttu-id="d10f7-118">description</span><span class="sxs-lookup"><span data-stu-id="d10f7-118">description</span></span>|<span data-ttu-id="d10f7-119">String</span><span class="sxs-lookup"><span data-stu-id="d10f7-119">String</span></span>|<span data-ttu-id="d10f7-120">项在应用程序内所控制内容的说明</span><span class="sxs-lookup"><span data-stu-id="d10f7-120">Description of what the item controls within the application</span></span>|
|<span data-ttu-id="d10f7-121">defaultBoolValue</span><span class="sxs-lookup"><span data-stu-id="d10f7-121">defaultBoolValue</span></span>|<span data-ttu-id="d10f7-122">布尔值</span><span class="sxs-lookup"><span data-stu-id="d10f7-122">Boolean</span></span>|<span data-ttu-id="d10f7-123">如果由应用开发人员指定，则为布尔类型项的默认值</span><span class="sxs-lookup"><span data-stu-id="d10f7-123">Default value for boolean type items, if specified by the app developer</span></span>|
|<span data-ttu-id="d10f7-124">defaultIntValue</span><span class="sxs-lookup"><span data-stu-id="d10f7-124">defaultIntValue</span></span>|<span data-ttu-id="d10f7-125">Int32</span><span class="sxs-lookup"><span data-stu-id="d10f7-125">Int32</span></span>|<span data-ttu-id="d10f7-126">如果由应用开发人员指定，则为整数类型项的默认值</span><span class="sxs-lookup"><span data-stu-id="d10f7-126">Default value for integer type items, if specified by the app developer</span></span>|
|<span data-ttu-id="d10f7-127">defaultStringValue</span><span class="sxs-lookup"><span data-stu-id="d10f7-127">defaultStringValue</span></span>|<span data-ttu-id="d10f7-128">String</span><span class="sxs-lookup"><span data-stu-id="d10f7-128">String</span></span>|<span data-ttu-id="d10f7-129">如果由应用开发人员指定，则为字符串类型项的默认值</span><span class="sxs-lookup"><span data-stu-id="d10f7-129">Default value for string type items, if specified by the app developer</span></span>|
|<span data-ttu-id="d10f7-130">defaultStringArrayValue</span><span class="sxs-lookup"><span data-stu-id="d10f7-130">defaultStringArrayValue</span></span>|<span data-ttu-id="d10f7-131">String collection</span><span class="sxs-lookup"><span data-stu-id="d10f7-131">String collection</span></span>|<span data-ttu-id="d10f7-132">如果由应用开发人员指定，则为字符串数组类型项的默认值</span><span class="sxs-lookup"><span data-stu-id="d10f7-132">Default value for string array type items, if specified by the app developer</span></span>|
|<span data-ttu-id="d10f7-133">DataType</span><span class="sxs-lookup"><span data-stu-id="d10f7-133">dataType</span></span>|[<span data-ttu-id="d10f7-134">androidForWorkAppConfigurationSchemaItemDataType</span><span class="sxs-lookup"><span data-stu-id="d10f7-134">androidForWorkAppConfigurationSchemaItemDataType</span></span>](../resources/intune-androidforwork-androidforworkappconfigurationschemaitemdatatype.md)|<span data-ttu-id="d10f7-135">此项目描述的值的类型。</span><span class="sxs-lookup"><span data-stu-id="d10f7-135">The type of value this item describes.</span></span> <span data-ttu-id="d10f7-136">可取值为：`bool`、`integer`、`string`、`choice`、`multiselect`、`bundle`、`bundleArray`、`hidden`。</span><span class="sxs-lookup"><span data-stu-id="d10f7-136">Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span></span>|
|<span data-ttu-id="d10f7-137">选择</span><span class="sxs-lookup"><span data-stu-id="d10f7-137">selections</span></span>|<span data-ttu-id="d10f7-138">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d10f7-138">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="d10f7-139">可为此项（仅 Choice 和 Multiselect 项）设置的有效值的用于可读名称/值对列表</span><span class="sxs-lookup"><span data-stu-id="d10f7-139">List of human readable name/value pairs for the valid values that can be set for this item (Choice and Multiselect items only)</span></span>|

## <a name="relationships"></a><span data-ttu-id="d10f7-140">关系</span><span class="sxs-lookup"><span data-stu-id="d10f7-140">Relationships</span></span>
<span data-ttu-id="d10f7-141">无</span><span class="sxs-lookup"><span data-stu-id="d10f7-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d10f7-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d10f7-142">JSON Representation</span></span>
<span data-ttu-id="d10f7-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d10f7-143">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchemaItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkAppConfigurationSchemaItem",
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






