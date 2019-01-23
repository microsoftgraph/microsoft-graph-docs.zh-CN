---
title: androidForWorkAppConfigurationSchemaItem 资源类型
description: Android for Work 应用程序的自定义配置架构内的单个配置项。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 45370a7c5bec72e63d25e2c8242ac8b07c4cc4e4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29392729"
---
# <a name="androidforworkappconfigurationschemaitem-resource-type"></a><span data-ttu-id="c3929-103">androidForWorkAppConfigurationSchemaItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="c3929-103">androidForWorkAppConfigurationSchemaItem resource type</span></span>

> <span data-ttu-id="c3929-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="c3929-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c3929-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c3929-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c3929-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c3929-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3929-107">Android for Work 应用程序的自定义配置架构内的单个配置项。</span><span class="sxs-lookup"><span data-stu-id="c3929-107">Single configuration item inside an Android for Work application's custom configuration schema.</span></span>

## <a name="properties"></a><span data-ttu-id="c3929-108">属性</span><span class="sxs-lookup"><span data-stu-id="c3929-108">Properties</span></span>
|<span data-ttu-id="c3929-109">属性</span><span class="sxs-lookup"><span data-stu-id="c3929-109">Property</span></span>|<span data-ttu-id="c3929-110">类型</span><span class="sxs-lookup"><span data-stu-id="c3929-110">Type</span></span>|<span data-ttu-id="c3929-111">说明</span><span class="sxs-lookup"><span data-stu-id="c3929-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3929-112">schemaItemKey</span><span class="sxs-lookup"><span data-stu-id="c3929-112">schemaItemKey</span></span>|<span data-ttu-id="c3929-113">String</span><span class="sxs-lookup"><span data-stu-id="c3929-113">String</span></span>|<span data-ttu-id="c3929-114">应用程序用于标识项的唯一键</span><span class="sxs-lookup"><span data-stu-id="c3929-114">Unique key the application uses to identify the item</span></span>|
|<span data-ttu-id="c3929-115">displayName</span><span class="sxs-lookup"><span data-stu-id="c3929-115">displayName</span></span>|<span data-ttu-id="c3929-116">String</span><span class="sxs-lookup"><span data-stu-id="c3929-116">String</span></span>|<span data-ttu-id="c3929-117">用户可读的名称</span><span class="sxs-lookup"><span data-stu-id="c3929-117">Human readable name</span></span>|
|<span data-ttu-id="c3929-118">说明</span><span class="sxs-lookup"><span data-stu-id="c3929-118">description</span></span>|<span data-ttu-id="c3929-119">String</span><span class="sxs-lookup"><span data-stu-id="c3929-119">String</span></span>|<span data-ttu-id="c3929-120">项在应用程序内所控制内容的说明</span><span class="sxs-lookup"><span data-stu-id="c3929-120">Description of what the item controls within the application</span></span>|
|<span data-ttu-id="c3929-121">defaultBoolValue</span><span class="sxs-lookup"><span data-stu-id="c3929-121">defaultBoolValue</span></span>|<span data-ttu-id="c3929-122">布尔值</span><span class="sxs-lookup"><span data-stu-id="c3929-122">Boolean</span></span>|<span data-ttu-id="c3929-123">如果由应用开发人员指定，则为布尔类型项的默认值</span><span class="sxs-lookup"><span data-stu-id="c3929-123">Default value for boolean type items, if specified by the app developer</span></span>|
|<span data-ttu-id="c3929-124">defaultIntValue</span><span class="sxs-lookup"><span data-stu-id="c3929-124">defaultIntValue</span></span>|<span data-ttu-id="c3929-125">Int32</span><span class="sxs-lookup"><span data-stu-id="c3929-125">Int32</span></span>|<span data-ttu-id="c3929-126">如果由应用开发人员指定，则为整数类型项的默认值</span><span class="sxs-lookup"><span data-stu-id="c3929-126">Default value for integer type items, if specified by the app developer</span></span>|
|<span data-ttu-id="c3929-127">defaultStringValue</span><span class="sxs-lookup"><span data-stu-id="c3929-127">defaultStringValue</span></span>|<span data-ttu-id="c3929-128">String</span><span class="sxs-lookup"><span data-stu-id="c3929-128">String</span></span>|<span data-ttu-id="c3929-129">如果由应用开发人员指定，则为字符串类型项的默认值</span><span class="sxs-lookup"><span data-stu-id="c3929-129">Default value for string type items, if specified by the app developer</span></span>|
|<span data-ttu-id="c3929-130">defaultStringArrayValue</span><span class="sxs-lookup"><span data-stu-id="c3929-130">defaultStringArrayValue</span></span>|<span data-ttu-id="c3929-131">String collection</span><span class="sxs-lookup"><span data-stu-id="c3929-131">String collection</span></span>|<span data-ttu-id="c3929-132">如果由应用开发人员指定，则为字符串数组类型项的默认值</span><span class="sxs-lookup"><span data-stu-id="c3929-132">Default value for string array type items, if specified by the app developer</span></span>|
|<span data-ttu-id="c3929-133">DataType</span><span class="sxs-lookup"><span data-stu-id="c3929-133">dataType</span></span>|[<span data-ttu-id="c3929-134">androidForWorkAppConfigurationSchemaItemDataType</span><span class="sxs-lookup"><span data-stu-id="c3929-134">androidForWorkAppConfigurationSchemaItemDataType</span></span>](../resources/intune-androidforwork-androidforworkappconfigurationschemaitemdatatype.md)|<span data-ttu-id="c3929-135">描述此项的值的类型。</span><span class="sxs-lookup"><span data-stu-id="c3929-135">The type of value this item describes.</span></span> <span data-ttu-id="c3929-136">可取值为：`bool`、`integer`、`string`、`choice`、`multiselect`、`bundle`、`bundleArray`、`hidden`。</span><span class="sxs-lookup"><span data-stu-id="c3929-136">Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span></span>|
|<span data-ttu-id="c3929-137">选择</span><span class="sxs-lookup"><span data-stu-id="c3929-137">selections</span></span>|<span data-ttu-id="c3929-138">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c3929-138">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="c3929-139">可为此项（仅 Choice 和 Multiselect 项）设置的有效值的用于可读名称/值对列表</span><span class="sxs-lookup"><span data-stu-id="c3929-139">List of human readable name/value pairs for the valid values that can be set for this item (Choice and Multiselect items only)</span></span>|

## <a name="relationships"></a><span data-ttu-id="c3929-140">关系</span><span class="sxs-lookup"><span data-stu-id="c3929-140">Relationships</span></span>
<span data-ttu-id="c3929-141">无</span><span class="sxs-lookup"><span data-stu-id="c3929-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c3929-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c3929-142">JSON Representation</span></span>
<span data-ttu-id="c3929-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c3929-143">Here is a JSON representation of the resource.</span></span>
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




