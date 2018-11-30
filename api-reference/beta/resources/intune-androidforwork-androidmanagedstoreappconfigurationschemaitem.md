---
title: androidManagedStoreAppConfigurationSchemaItem 资源类型
description: 在 Android 应用程序的自定义配置架构的单个配置项。
ms.openlocfilehash: 94ae8735800e4f79be2e7c61f8b971bafd8c394f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047561"
---
# <a name="androidmanagedstoreappconfigurationschemaitem-resource-type"></a><span data-ttu-id="22dad-103">androidManagedStoreAppConfigurationSchemaItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="22dad-103">androidManagedStoreAppConfigurationSchemaItem resource type</span></span>

> <span data-ttu-id="22dad-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="22dad-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="22dad-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="22dad-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="22dad-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="22dad-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="22dad-107">在 Android 应用程序的自定义配置架构的单个配置项。</span><span class="sxs-lookup"><span data-stu-id="22dad-107">Single configuration item inside an Android application's custom configuration schema.</span></span>
## <a name="properties"></a><span data-ttu-id="22dad-108">属性</span><span class="sxs-lookup"><span data-stu-id="22dad-108">Properties</span></span>
|<span data-ttu-id="22dad-109">属性</span><span class="sxs-lookup"><span data-stu-id="22dad-109">Property</span></span>|<span data-ttu-id="22dad-110">类型</span><span class="sxs-lookup"><span data-stu-id="22dad-110">Type</span></span>|<span data-ttu-id="22dad-111">说明</span><span class="sxs-lookup"><span data-stu-id="22dad-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22dad-112">schemaItemKey</span><span class="sxs-lookup"><span data-stu-id="22dad-112">schemaItemKey</span></span>|<span data-ttu-id="22dad-113">String</span><span class="sxs-lookup"><span data-stu-id="22dad-113">String</span></span>|<span data-ttu-id="22dad-114">应用程序用于标识项的唯一键</span><span class="sxs-lookup"><span data-stu-id="22dad-114">Unique key the application uses to identify the item</span></span>|
|<span data-ttu-id="22dad-115">displayName</span><span class="sxs-lookup"><span data-stu-id="22dad-115">displayName</span></span>|<span data-ttu-id="22dad-116">String</span><span class="sxs-lookup"><span data-stu-id="22dad-116">String</span></span>|<span data-ttu-id="22dad-117">用户可读的名称</span><span class="sxs-lookup"><span data-stu-id="22dad-117">Human readable name</span></span>|
|<span data-ttu-id="22dad-118">说明</span><span class="sxs-lookup"><span data-stu-id="22dad-118">description</span></span>|<span data-ttu-id="22dad-119">String</span><span class="sxs-lookup"><span data-stu-id="22dad-119">String</span></span>|<span data-ttu-id="22dad-120">项在应用程序内所控制内容的说明</span><span class="sxs-lookup"><span data-stu-id="22dad-120">Description of what the item controls within the application</span></span>|
|<span data-ttu-id="22dad-121">defaultBoolValue</span><span class="sxs-lookup"><span data-stu-id="22dad-121">defaultBoolValue</span></span>|<span data-ttu-id="22dad-122">布尔值</span><span class="sxs-lookup"><span data-stu-id="22dad-122">Boolean</span></span>|<span data-ttu-id="22dad-123">如果由应用开发人员指定，则为布尔类型项的默认值</span><span class="sxs-lookup"><span data-stu-id="22dad-123">Default value for boolean type items, if specified by the app developer</span></span>|
|<span data-ttu-id="22dad-124">defaultIntValue</span><span class="sxs-lookup"><span data-stu-id="22dad-124">defaultIntValue</span></span>|<span data-ttu-id="22dad-125">Int32</span><span class="sxs-lookup"><span data-stu-id="22dad-125">Int32</span></span>|<span data-ttu-id="22dad-126">如果由应用开发人员指定，则为整数类型项的默认值</span><span class="sxs-lookup"><span data-stu-id="22dad-126">Default value for integer type items, if specified by the app developer</span></span>|
|<span data-ttu-id="22dad-127">defaultStringValue</span><span class="sxs-lookup"><span data-stu-id="22dad-127">defaultStringValue</span></span>|<span data-ttu-id="22dad-128">String</span><span class="sxs-lookup"><span data-stu-id="22dad-128">String</span></span>|<span data-ttu-id="22dad-129">如果由应用开发人员指定，则为字符串类型项的默认值</span><span class="sxs-lookup"><span data-stu-id="22dad-129">Default value for string type items, if specified by the app developer</span></span>|
|<span data-ttu-id="22dad-130">defaultStringArrayValue</span><span class="sxs-lookup"><span data-stu-id="22dad-130">defaultStringArrayValue</span></span>|<span data-ttu-id="22dad-131">String collection</span><span class="sxs-lookup"><span data-stu-id="22dad-131">String collection</span></span>|<span data-ttu-id="22dad-132">如果由应用开发人员指定，则为字符串数组类型项的默认值</span><span class="sxs-lookup"><span data-stu-id="22dad-132">Default value for string array type items, if specified by the app developer</span></span>|
|<span data-ttu-id="22dad-133">DataType</span><span class="sxs-lookup"><span data-stu-id="22dad-133">dataType</span></span>|[<span data-ttu-id="22dad-134">androidManagedStoreAppConfigurationSchemaItemDataType</span><span class="sxs-lookup"><span data-stu-id="22dad-134">androidManagedStoreAppConfigurationSchemaItemDataType</span></span>](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitemdatatype.md)|<span data-ttu-id="22dad-135">描述此项的值的类型。</span><span class="sxs-lookup"><span data-stu-id="22dad-135">The type of value this item describes.</span></span> <span data-ttu-id="22dad-136">可取值为：`bool`、`integer`、`string`、`choice`、`multiselect`、`bundle`、`bundleArray`、`hidden`。</span><span class="sxs-lookup"><span data-stu-id="22dad-136">Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span></span>|
|<span data-ttu-id="22dad-137">选择</span><span class="sxs-lookup"><span data-stu-id="22dad-137">selections</span></span>|<span data-ttu-id="22dad-138">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="22dad-138">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="22dad-139">可为此项（仅 Choice 和 Multiselect 项）设置的有效值的用于可读名称/值对列表</span><span class="sxs-lookup"><span data-stu-id="22dad-139">List of human readable name/value pairs for the valid values that can be set for this item (Choice and Multiselect items only)</span></span>|

## <a name="relationships"></a><span data-ttu-id="22dad-140">关系</span><span class="sxs-lookup"><span data-stu-id="22dad-140">Relationships</span></span>
<span data-ttu-id="22dad-141">无</span><span class="sxs-lookup"><span data-stu-id="22dad-141">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="22dad-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="22dad-142">JSON Representation</span></span>
<span data-ttu-id="22dad-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="22dad-143">Here is a JSON representation of the resource.</span></span>
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





