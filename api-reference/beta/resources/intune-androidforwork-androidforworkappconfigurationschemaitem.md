---
title: androidForWorkAppConfigurationSchemaItem 资源类型
description: Android for Work 应用程序的自定义配置架构内的单个配置项。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 08732e31372a59216894bcb70ffd6318a0fa2f1e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42495093"
---
# <a name="androidforworkappconfigurationschemaitem-resource-type"></a><span data-ttu-id="ab7b1-103">androidForWorkAppConfigurationSchemaItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="ab7b1-103">androidForWorkAppConfigurationSchemaItem resource type</span></span>

<span data-ttu-id="ab7b1-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="ab7b1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ab7b1-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ab7b1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ab7b1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ab7b1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab7b1-107">Android for Work 应用程序的自定义配置架构内的单个配置项。</span><span class="sxs-lookup"><span data-stu-id="ab7b1-107">Single configuration item inside an Android for Work application's custom configuration schema.</span></span>

## <a name="properties"></a><span data-ttu-id="ab7b1-108">属性</span><span class="sxs-lookup"><span data-stu-id="ab7b1-108">Properties</span></span>
|<span data-ttu-id="ab7b1-109">属性</span><span class="sxs-lookup"><span data-stu-id="ab7b1-109">Property</span></span>|<span data-ttu-id="ab7b1-110">类型</span><span class="sxs-lookup"><span data-stu-id="ab7b1-110">Type</span></span>|<span data-ttu-id="ab7b1-111">说明</span><span class="sxs-lookup"><span data-stu-id="ab7b1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab7b1-112">schemaItemKey</span><span class="sxs-lookup"><span data-stu-id="ab7b1-112">schemaItemKey</span></span>|<span data-ttu-id="ab7b1-113">String</span><span class="sxs-lookup"><span data-stu-id="ab7b1-113">String</span></span>|<span data-ttu-id="ab7b1-114">应用程序用于标识项的唯一键</span><span class="sxs-lookup"><span data-stu-id="ab7b1-114">Unique key the application uses to identify the item</span></span>|
|<span data-ttu-id="ab7b1-115">displayName</span><span class="sxs-lookup"><span data-stu-id="ab7b1-115">displayName</span></span>|<span data-ttu-id="ab7b1-116">字符串</span><span class="sxs-lookup"><span data-stu-id="ab7b1-116">String</span></span>|<span data-ttu-id="ab7b1-117">用户可读的名称</span><span class="sxs-lookup"><span data-stu-id="ab7b1-117">Human readable name</span></span>|
|<span data-ttu-id="ab7b1-118">说明</span><span class="sxs-lookup"><span data-stu-id="ab7b1-118">description</span></span>|<span data-ttu-id="ab7b1-119">String</span><span class="sxs-lookup"><span data-stu-id="ab7b1-119">String</span></span>|<span data-ttu-id="ab7b1-120">项在应用程序内所控制内容的说明</span><span class="sxs-lookup"><span data-stu-id="ab7b1-120">Description of what the item controls within the application</span></span>|
|<span data-ttu-id="ab7b1-121">defaultBoolValue</span><span class="sxs-lookup"><span data-stu-id="ab7b1-121">defaultBoolValue</span></span>|<span data-ttu-id="ab7b1-122">布尔值</span><span class="sxs-lookup"><span data-stu-id="ab7b1-122">Boolean</span></span>|<span data-ttu-id="ab7b1-123">如果由应用开发人员指定，则为布尔类型项的默认值</span><span class="sxs-lookup"><span data-stu-id="ab7b1-123">Default value for boolean type items, if specified by the app developer</span></span>|
|<span data-ttu-id="ab7b1-124">defaultIntValue</span><span class="sxs-lookup"><span data-stu-id="ab7b1-124">defaultIntValue</span></span>|<span data-ttu-id="ab7b1-125">Int32</span><span class="sxs-lookup"><span data-stu-id="ab7b1-125">Int32</span></span>|<span data-ttu-id="ab7b1-126">如果由应用开发人员指定，则为整数类型项的默认值</span><span class="sxs-lookup"><span data-stu-id="ab7b1-126">Default value for integer type items, if specified by the app developer</span></span>|
|<span data-ttu-id="ab7b1-127">defaultStringValue</span><span class="sxs-lookup"><span data-stu-id="ab7b1-127">defaultStringValue</span></span>|<span data-ttu-id="ab7b1-128">String</span><span class="sxs-lookup"><span data-stu-id="ab7b1-128">String</span></span>|<span data-ttu-id="ab7b1-129">如果由应用开发人员指定，则为字符串类型项的默认值</span><span class="sxs-lookup"><span data-stu-id="ab7b1-129">Default value for string type items, if specified by the app developer</span></span>|
|<span data-ttu-id="ab7b1-130">defaultStringArrayValue</span><span class="sxs-lookup"><span data-stu-id="ab7b1-130">defaultStringArrayValue</span></span>|<span data-ttu-id="ab7b1-131">String collection</span><span class="sxs-lookup"><span data-stu-id="ab7b1-131">String collection</span></span>|<span data-ttu-id="ab7b1-132">如果由应用开发人员指定，则为字符串数组类型项的默认值</span><span class="sxs-lookup"><span data-stu-id="ab7b1-132">Default value for string array type items, if specified by the app developer</span></span>|
|<span data-ttu-id="ab7b1-133">DataType</span><span class="sxs-lookup"><span data-stu-id="ab7b1-133">dataType</span></span>|[<span data-ttu-id="ab7b1-134">androidForWorkAppConfigurationSchemaItemDataType</span><span class="sxs-lookup"><span data-stu-id="ab7b1-134">androidForWorkAppConfigurationSchemaItemDataType</span></span>](../resources/intune-androidforwork-androidforworkappconfigurationschemaitemdatatype.md)|<span data-ttu-id="ab7b1-135">此项目描述的值的类型。</span><span class="sxs-lookup"><span data-stu-id="ab7b1-135">The type of value this item describes.</span></span> <span data-ttu-id="ab7b1-136">可取值为：`bool`、`integer`、`string`、`choice`、`multiselect`、`bundle`、`bundleArray`、`hidden`。</span><span class="sxs-lookup"><span data-stu-id="ab7b1-136">Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span></span>|
|<span data-ttu-id="ab7b1-137">选择</span><span class="sxs-lookup"><span data-stu-id="ab7b1-137">selections</span></span>|<span data-ttu-id="ab7b1-138">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ab7b1-138">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="ab7b1-139">可为此项（仅 Choice 和 Multiselect 项）设置的有效值的用于可读名称/值对列表</span><span class="sxs-lookup"><span data-stu-id="ab7b1-139">List of human readable name/value pairs for the valid values that can be set for this item (Choice and Multiselect items only)</span></span>|

## <a name="relationships"></a><span data-ttu-id="ab7b1-140">关系</span><span class="sxs-lookup"><span data-stu-id="ab7b1-140">Relationships</span></span>
<span data-ttu-id="ab7b1-141">无</span><span class="sxs-lookup"><span data-stu-id="ab7b1-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ab7b1-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ab7b1-142">JSON Representation</span></span>
<span data-ttu-id="ab7b1-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ab7b1-143">Here is a JSON representation of the resource.</span></span>
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



