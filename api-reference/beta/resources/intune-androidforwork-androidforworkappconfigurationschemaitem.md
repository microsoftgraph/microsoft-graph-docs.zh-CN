---
title: androidForWorkAppConfigurationSchemaItem 资源类型
description: Android for Work 应用程序的自定义配置架构内的单个配置项。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b3ac320b0630d7307a56b06cd07b8d4d0d7f12b9
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34993471"
---
# <a name="androidforworkappconfigurationschemaitem-resource-type"></a><span data-ttu-id="29f5b-103">androidForWorkAppConfigurationSchemaItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="29f5b-103">androidForWorkAppConfigurationSchemaItem resource type</span></span>

> <span data-ttu-id="29f5b-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="29f5b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="29f5b-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="29f5b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29f5b-106">Android for Work 应用程序的自定义配置架构内的单个配置项。</span><span class="sxs-lookup"><span data-stu-id="29f5b-106">Single configuration item inside an Android for Work application's custom configuration schema.</span></span>

## <a name="properties"></a><span data-ttu-id="29f5b-107">属性</span><span class="sxs-lookup"><span data-stu-id="29f5b-107">Properties</span></span>
|<span data-ttu-id="29f5b-108">属性</span><span class="sxs-lookup"><span data-stu-id="29f5b-108">Property</span></span>|<span data-ttu-id="29f5b-109">类型</span><span class="sxs-lookup"><span data-stu-id="29f5b-109">Type</span></span>|<span data-ttu-id="29f5b-110">说明</span><span class="sxs-lookup"><span data-stu-id="29f5b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29f5b-111">schemaItemKey</span><span class="sxs-lookup"><span data-stu-id="29f5b-111">schemaItemKey</span></span>|<span data-ttu-id="29f5b-112">String</span><span class="sxs-lookup"><span data-stu-id="29f5b-112">String</span></span>|<span data-ttu-id="29f5b-113">应用程序用于标识项的唯一键</span><span class="sxs-lookup"><span data-stu-id="29f5b-113">Unique key the application uses to identify the item</span></span>|
|<span data-ttu-id="29f5b-114">displayName</span><span class="sxs-lookup"><span data-stu-id="29f5b-114">displayName</span></span>|<span data-ttu-id="29f5b-115">字符串</span><span class="sxs-lookup"><span data-stu-id="29f5b-115">String</span></span>|<span data-ttu-id="29f5b-116">用户可读的名称</span><span class="sxs-lookup"><span data-stu-id="29f5b-116">Human readable name</span></span>|
|<span data-ttu-id="29f5b-117">说明</span><span class="sxs-lookup"><span data-stu-id="29f5b-117">description</span></span>|<span data-ttu-id="29f5b-118">String</span><span class="sxs-lookup"><span data-stu-id="29f5b-118">String</span></span>|<span data-ttu-id="29f5b-119">项在应用程序内所控制内容的说明</span><span class="sxs-lookup"><span data-stu-id="29f5b-119">Description of what the item controls within the application</span></span>|
|<span data-ttu-id="29f5b-120">defaultBoolValue</span><span class="sxs-lookup"><span data-stu-id="29f5b-120">defaultBoolValue</span></span>|<span data-ttu-id="29f5b-121">布尔值</span><span class="sxs-lookup"><span data-stu-id="29f5b-121">Boolean</span></span>|<span data-ttu-id="29f5b-122">如果由应用开发人员指定，则为布尔类型项的默认值</span><span class="sxs-lookup"><span data-stu-id="29f5b-122">Default value for boolean type items, if specified by the app developer</span></span>|
|<span data-ttu-id="29f5b-123">defaultIntValue</span><span class="sxs-lookup"><span data-stu-id="29f5b-123">defaultIntValue</span></span>|<span data-ttu-id="29f5b-124">Int32</span><span class="sxs-lookup"><span data-stu-id="29f5b-124">Int32</span></span>|<span data-ttu-id="29f5b-125">如果由应用开发人员指定，则为整数类型项的默认值</span><span class="sxs-lookup"><span data-stu-id="29f5b-125">Default value for integer type items, if specified by the app developer</span></span>|
|<span data-ttu-id="29f5b-126">defaultStringValue</span><span class="sxs-lookup"><span data-stu-id="29f5b-126">defaultStringValue</span></span>|<span data-ttu-id="29f5b-127">String</span><span class="sxs-lookup"><span data-stu-id="29f5b-127">String</span></span>|<span data-ttu-id="29f5b-128">如果由应用开发人员指定，则为字符串类型项的默认值</span><span class="sxs-lookup"><span data-stu-id="29f5b-128">Default value for string type items, if specified by the app developer</span></span>|
|<span data-ttu-id="29f5b-129">defaultStringArrayValue</span><span class="sxs-lookup"><span data-stu-id="29f5b-129">defaultStringArrayValue</span></span>|<span data-ttu-id="29f5b-130">String collection</span><span class="sxs-lookup"><span data-stu-id="29f5b-130">String collection</span></span>|<span data-ttu-id="29f5b-131">如果由应用开发人员指定，则为字符串数组类型项的默认值</span><span class="sxs-lookup"><span data-stu-id="29f5b-131">Default value for string array type items, if specified by the app developer</span></span>|
|<span data-ttu-id="29f5b-132">DataType</span><span class="sxs-lookup"><span data-stu-id="29f5b-132">dataType</span></span>|[<span data-ttu-id="29f5b-133">androidForWorkAppConfigurationSchemaItemDataType</span><span class="sxs-lookup"><span data-stu-id="29f5b-133">androidForWorkAppConfigurationSchemaItemDataType</span></span>](../resources/intune-androidforwork-androidforworkappconfigurationschemaitemdatatype.md)|<span data-ttu-id="29f5b-134">此项目描述的值的类型。</span><span class="sxs-lookup"><span data-stu-id="29f5b-134">The type of value this item describes.</span></span> <span data-ttu-id="29f5b-135">可取值为：`bool`、`integer`、`string`、`choice`、`multiselect`、`bundle`、`bundleArray`、`hidden`。</span><span class="sxs-lookup"><span data-stu-id="29f5b-135">Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span></span>|
|<span data-ttu-id="29f5b-136">选择</span><span class="sxs-lookup"><span data-stu-id="29f5b-136">selections</span></span>|<span data-ttu-id="29f5b-137">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="29f5b-137">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="29f5b-138">可为此项（仅 Choice 和 Multiselect 项）设置的有效值的用于可读名称/值对列表</span><span class="sxs-lookup"><span data-stu-id="29f5b-138">List of human readable name/value pairs for the valid values that can be set for this item (Choice and Multiselect items only)</span></span>|

## <a name="relationships"></a><span data-ttu-id="29f5b-139">关系</span><span class="sxs-lookup"><span data-stu-id="29f5b-139">Relationships</span></span>
<span data-ttu-id="29f5b-140">无</span><span class="sxs-lookup"><span data-stu-id="29f5b-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="29f5b-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="29f5b-141">JSON Representation</span></span>
<span data-ttu-id="29f5b-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="29f5b-142">Here is a JSON representation of the resource.</span></span>
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





