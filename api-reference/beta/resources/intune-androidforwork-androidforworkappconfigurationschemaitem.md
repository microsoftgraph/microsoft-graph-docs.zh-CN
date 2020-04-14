---
title: androidForWorkAppConfigurationSchemaItem 资源类型
description: Android for Work 应用程序的自定义配置架构内的单个配置项。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d8ed09ee79b8a5607f4aec0647ed7d221ee407e5
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43459273"
---
# <a name="androidforworkappconfigurationschemaitem-resource-type"></a><span data-ttu-id="e6907-103">androidForWorkAppConfigurationSchemaItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="e6907-103">androidForWorkAppConfigurationSchemaItem resource type</span></span>

<span data-ttu-id="e6907-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6907-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e6907-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e6907-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e6907-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e6907-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6907-107">Android for Work 应用程序的自定义配置架构内的单个配置项。</span><span class="sxs-lookup"><span data-stu-id="e6907-107">Single configuration item inside an Android for Work application's custom configuration schema.</span></span>

## <a name="properties"></a><span data-ttu-id="e6907-108">属性</span><span class="sxs-lookup"><span data-stu-id="e6907-108">Properties</span></span>
|<span data-ttu-id="e6907-109">属性</span><span class="sxs-lookup"><span data-stu-id="e6907-109">Property</span></span>|<span data-ttu-id="e6907-110">类型</span><span class="sxs-lookup"><span data-stu-id="e6907-110">Type</span></span>|<span data-ttu-id="e6907-111">说明</span><span class="sxs-lookup"><span data-stu-id="e6907-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6907-112">schemaItemKey</span><span class="sxs-lookup"><span data-stu-id="e6907-112">schemaItemKey</span></span>|<span data-ttu-id="e6907-113">String</span><span class="sxs-lookup"><span data-stu-id="e6907-113">String</span></span>|<span data-ttu-id="e6907-114">应用程序用于标识项的唯一键</span><span class="sxs-lookup"><span data-stu-id="e6907-114">Unique key the application uses to identify the item</span></span>|
|<span data-ttu-id="e6907-115">displayName</span><span class="sxs-lookup"><span data-stu-id="e6907-115">displayName</span></span>|<span data-ttu-id="e6907-116">字符串</span><span class="sxs-lookup"><span data-stu-id="e6907-116">String</span></span>|<span data-ttu-id="e6907-117">用户可读的名称</span><span class="sxs-lookup"><span data-stu-id="e6907-117">Human readable name</span></span>|
|<span data-ttu-id="e6907-118">description</span><span class="sxs-lookup"><span data-stu-id="e6907-118">description</span></span>|<span data-ttu-id="e6907-119">String</span><span class="sxs-lookup"><span data-stu-id="e6907-119">String</span></span>|<span data-ttu-id="e6907-120">项在应用程序内所控制内容的说明</span><span class="sxs-lookup"><span data-stu-id="e6907-120">Description of what the item controls within the application</span></span>|
|<span data-ttu-id="e6907-121">defaultBoolValue</span><span class="sxs-lookup"><span data-stu-id="e6907-121">defaultBoolValue</span></span>|<span data-ttu-id="e6907-122">布尔值</span><span class="sxs-lookup"><span data-stu-id="e6907-122">Boolean</span></span>|<span data-ttu-id="e6907-123">如果由应用开发人员指定，则为布尔类型项的默认值</span><span class="sxs-lookup"><span data-stu-id="e6907-123">Default value for boolean type items, if specified by the app developer</span></span>|
|<span data-ttu-id="e6907-124">defaultIntValue</span><span class="sxs-lookup"><span data-stu-id="e6907-124">defaultIntValue</span></span>|<span data-ttu-id="e6907-125">Int32</span><span class="sxs-lookup"><span data-stu-id="e6907-125">Int32</span></span>|<span data-ttu-id="e6907-126">如果由应用开发人员指定，则为整数类型项的默认值</span><span class="sxs-lookup"><span data-stu-id="e6907-126">Default value for integer type items, if specified by the app developer</span></span>|
|<span data-ttu-id="e6907-127">defaultStringValue</span><span class="sxs-lookup"><span data-stu-id="e6907-127">defaultStringValue</span></span>|<span data-ttu-id="e6907-128">String</span><span class="sxs-lookup"><span data-stu-id="e6907-128">String</span></span>|<span data-ttu-id="e6907-129">如果由应用开发人员指定，则为字符串类型项的默认值</span><span class="sxs-lookup"><span data-stu-id="e6907-129">Default value for string type items, if specified by the app developer</span></span>|
|<span data-ttu-id="e6907-130">defaultStringArrayValue</span><span class="sxs-lookup"><span data-stu-id="e6907-130">defaultStringArrayValue</span></span>|<span data-ttu-id="e6907-131">String collection</span><span class="sxs-lookup"><span data-stu-id="e6907-131">String collection</span></span>|<span data-ttu-id="e6907-132">如果由应用开发人员指定，则为字符串数组类型项的默认值</span><span class="sxs-lookup"><span data-stu-id="e6907-132">Default value for string array type items, if specified by the app developer</span></span>|
|<span data-ttu-id="e6907-133">DataType</span><span class="sxs-lookup"><span data-stu-id="e6907-133">dataType</span></span>|[<span data-ttu-id="e6907-134">androidForWorkAppConfigurationSchemaItemDataType</span><span class="sxs-lookup"><span data-stu-id="e6907-134">androidForWorkAppConfigurationSchemaItemDataType</span></span>](../resources/intune-androidforwork-androidforworkappconfigurationschemaitemdatatype.md)|<span data-ttu-id="e6907-135">此项目描述的值的类型。</span><span class="sxs-lookup"><span data-stu-id="e6907-135">The type of value this item describes.</span></span> <span data-ttu-id="e6907-136">可取值为：`bool`、`integer`、`string`、`choice`、`multiselect`、`bundle`、`bundleArray`、`hidden`。</span><span class="sxs-lookup"><span data-stu-id="e6907-136">Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span></span>|
|<span data-ttu-id="e6907-137">选择</span><span class="sxs-lookup"><span data-stu-id="e6907-137">selections</span></span>|<span data-ttu-id="e6907-138">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e6907-138">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="e6907-139">可为此项（仅 Choice 和 Multiselect 项）设置的有效值的用于可读名称/值对列表</span><span class="sxs-lookup"><span data-stu-id="e6907-139">List of human readable name/value pairs for the valid values that can be set for this item (Choice and Multiselect items only)</span></span>|

## <a name="relationships"></a><span data-ttu-id="e6907-140">关系</span><span class="sxs-lookup"><span data-stu-id="e6907-140">Relationships</span></span>
<span data-ttu-id="e6907-141">无</span><span class="sxs-lookup"><span data-stu-id="e6907-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e6907-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e6907-142">JSON Representation</span></span>
<span data-ttu-id="e6907-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e6907-143">Here is a JSON representation of the resource.</span></span>
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



