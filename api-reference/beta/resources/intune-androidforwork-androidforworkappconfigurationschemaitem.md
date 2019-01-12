---
title: androidForWorkAppConfigurationSchemaItem 资源类型
description: Android for Work 应用程序的自定义配置架构内的单个配置项。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 7e8500df3065c68ae8ddc2ad85413aa4d31f8980
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923451"
---
# <a name="androidforworkappconfigurationschemaitem-resource-type"></a><span data-ttu-id="8a055-103">androidForWorkAppConfigurationSchemaItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="8a055-103">androidForWorkAppConfigurationSchemaItem resource type</span></span>

> <span data-ttu-id="8a055-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8a055-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8a055-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8a055-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8a055-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="8a055-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8a055-107">Android for Work 应用程序的自定义配置架构内的单个配置项。</span><span class="sxs-lookup"><span data-stu-id="8a055-107">Single configuration item inside an Android for Work application's custom configuration schema.</span></span>
## <a name="properties"></a><span data-ttu-id="8a055-108">属性</span><span class="sxs-lookup"><span data-stu-id="8a055-108">Properties</span></span>
|<span data-ttu-id="8a055-109">属性</span><span class="sxs-lookup"><span data-stu-id="8a055-109">Property</span></span>|<span data-ttu-id="8a055-110">类型</span><span class="sxs-lookup"><span data-stu-id="8a055-110">Type</span></span>|<span data-ttu-id="8a055-111">说明</span><span class="sxs-lookup"><span data-stu-id="8a055-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a055-112">schemaItemKey</span><span class="sxs-lookup"><span data-stu-id="8a055-112">schemaItemKey</span></span>|<span data-ttu-id="8a055-113">String</span><span class="sxs-lookup"><span data-stu-id="8a055-113">String</span></span>|<span data-ttu-id="8a055-114">应用程序用于标识项的唯一键</span><span class="sxs-lookup"><span data-stu-id="8a055-114">Unique key the application uses to identify the item</span></span>|
|<span data-ttu-id="8a055-115">displayName</span><span class="sxs-lookup"><span data-stu-id="8a055-115">displayName</span></span>|<span data-ttu-id="8a055-116">String</span><span class="sxs-lookup"><span data-stu-id="8a055-116">String</span></span>|<span data-ttu-id="8a055-117">用户可读的名称</span><span class="sxs-lookup"><span data-stu-id="8a055-117">Human readable name</span></span>|
|<span data-ttu-id="8a055-118">说明</span><span class="sxs-lookup"><span data-stu-id="8a055-118">description</span></span>|<span data-ttu-id="8a055-119">String</span><span class="sxs-lookup"><span data-stu-id="8a055-119">String</span></span>|<span data-ttu-id="8a055-120">项在应用程序内所控制内容的说明</span><span class="sxs-lookup"><span data-stu-id="8a055-120">Description of what the item controls within the application</span></span>|
|<span data-ttu-id="8a055-121">defaultBoolValue</span><span class="sxs-lookup"><span data-stu-id="8a055-121">defaultBoolValue</span></span>|<span data-ttu-id="8a055-122">布尔值</span><span class="sxs-lookup"><span data-stu-id="8a055-122">Boolean</span></span>|<span data-ttu-id="8a055-123">如果由应用开发人员指定，则为布尔类型项的默认值</span><span class="sxs-lookup"><span data-stu-id="8a055-123">Default value for boolean type items, if specified by the app developer</span></span>|
|<span data-ttu-id="8a055-124">defaultIntValue</span><span class="sxs-lookup"><span data-stu-id="8a055-124">defaultIntValue</span></span>|<span data-ttu-id="8a055-125">Int32</span><span class="sxs-lookup"><span data-stu-id="8a055-125">Int32</span></span>|<span data-ttu-id="8a055-126">如果由应用开发人员指定，则为整数类型项的默认值</span><span class="sxs-lookup"><span data-stu-id="8a055-126">Default value for integer type items, if specified by the app developer</span></span>|
|<span data-ttu-id="8a055-127">defaultStringValue</span><span class="sxs-lookup"><span data-stu-id="8a055-127">defaultStringValue</span></span>|<span data-ttu-id="8a055-128">String</span><span class="sxs-lookup"><span data-stu-id="8a055-128">String</span></span>|<span data-ttu-id="8a055-129">如果由应用开发人员指定，则为字符串类型项的默认值</span><span class="sxs-lookup"><span data-stu-id="8a055-129">Default value for string type items, if specified by the app developer</span></span>|
|<span data-ttu-id="8a055-130">defaultStringArrayValue</span><span class="sxs-lookup"><span data-stu-id="8a055-130">defaultStringArrayValue</span></span>|<span data-ttu-id="8a055-131">String collection</span><span class="sxs-lookup"><span data-stu-id="8a055-131">String collection</span></span>|<span data-ttu-id="8a055-132">如果由应用开发人员指定，则为字符串数组类型项的默认值</span><span class="sxs-lookup"><span data-stu-id="8a055-132">Default value for string array type items, if specified by the app developer</span></span>|
|<span data-ttu-id="8a055-133">DataType</span><span class="sxs-lookup"><span data-stu-id="8a055-133">dataType</span></span>|[<span data-ttu-id="8a055-134">androidForWorkAppConfigurationSchemaItemDataType</span><span class="sxs-lookup"><span data-stu-id="8a055-134">androidForWorkAppConfigurationSchemaItemDataType</span></span>](../resources/intune-androidforwork-androidforworkappconfigurationschemaitemdatatype.md)|<span data-ttu-id="8a055-135">描述此项的值的类型。</span><span class="sxs-lookup"><span data-stu-id="8a055-135">The type of value this item describes.</span></span> <span data-ttu-id="8a055-136">可取值为：`bool`、`integer`、`string`、`choice`、`multiselect`、`bundle`、`bundleArray`、`hidden`。</span><span class="sxs-lookup"><span data-stu-id="8a055-136">Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span></span>|
|<span data-ttu-id="8a055-137">选择</span><span class="sxs-lookup"><span data-stu-id="8a055-137">selections</span></span>|<span data-ttu-id="8a055-138">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8a055-138">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="8a055-139">可为此项（仅 Choice 和 Multiselect 项）设置的有效值的用于可读名称/值对列表</span><span class="sxs-lookup"><span data-stu-id="8a055-139">List of human readable name/value pairs for the valid values that can be set for this item (Choice and Multiselect items only)</span></span>|

## <a name="relationships"></a><span data-ttu-id="8a055-140">关系</span><span class="sxs-lookup"><span data-stu-id="8a055-140">Relationships</span></span>
<span data-ttu-id="8a055-141">无</span><span class="sxs-lookup"><span data-stu-id="8a055-141">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8a055-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8a055-142">JSON Representation</span></span>
<span data-ttu-id="8a055-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8a055-143">Here is a JSON representation of the resource.</span></span>
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





