---
title: androidForWorkAppConfigurationSchema 资源类型
description: 描述 Android for Work 应用程序的自定义配置的架构。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 69df29143a3c30f4096108143510f802c815add1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415045"
---
# <a name="androidforworkappconfigurationschema-resource-type"></a><span data-ttu-id="3d13d-103">androidForWorkAppConfigurationSchema 资源类型</span><span class="sxs-lookup"><span data-stu-id="3d13d-103">androidForWorkAppConfigurationSchema resource type</span></span>

> <span data-ttu-id="3d13d-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="3d13d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3d13d-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3d13d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3d13d-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3d13d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d13d-107">描述 Android for Work 应用程序的自定义配置的架构。</span><span class="sxs-lookup"><span data-stu-id="3d13d-107">Schema describing an Android for Work application's custom configurations.</span></span>

## <a name="methods"></a><span data-ttu-id="3d13d-108">方法</span><span class="sxs-lookup"><span data-stu-id="3d13d-108">Methods</span></span>
|<span data-ttu-id="3d13d-109">方法</span><span class="sxs-lookup"><span data-stu-id="3d13d-109">Method</span></span>|<span data-ttu-id="3d13d-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="3d13d-110">Return Type</span></span>|<span data-ttu-id="3d13d-111">说明</span><span class="sxs-lookup"><span data-stu-id="3d13d-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3d13d-112">列出 androidForWorkAppConfigurationSchemas</span><span class="sxs-lookup"><span data-stu-id="3d13d-112">List androidForWorkAppConfigurationSchemas</span></span>](../api/intune-androidforwork-androidforworkappconfigurationschema-list.md)|<span data-ttu-id="3d13d-113">[androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3d13d-113">[androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) collection</span></span>|<span data-ttu-id="3d13d-114">列出 [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3d13d-114">List properties and relationships of the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) objects.</span></span>|
|[<span data-ttu-id="3d13d-115">获取 androidForWorkAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="3d13d-115">Get androidForWorkAppConfigurationSchema</span></span>](../api/intune-androidforwork-androidforworkappconfigurationschema-get.md)|[<span data-ttu-id="3d13d-116">androidForWorkAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="3d13d-116">androidForWorkAppConfigurationSchema</span></span>](../resources/intune-androidforwork-androidforworkappconfigurationschema.md)|<span data-ttu-id="3d13d-117">读取 [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3d13d-117">Read properties and relationships of the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>|
|[<span data-ttu-id="3d13d-118">创建 androidForWorkAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="3d13d-118">Create androidForWorkAppConfigurationSchema</span></span>](../api/intune-androidforwork-androidforworkappconfigurationschema-create.md)|[<span data-ttu-id="3d13d-119">androidForWorkAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="3d13d-119">androidForWorkAppConfigurationSchema</span></span>](../resources/intune-androidforwork-androidforworkappconfigurationschema.md)|<span data-ttu-id="3d13d-120">创建新的 [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3d13d-120">Create a new [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>|
|[<span data-ttu-id="3d13d-121">删除 androidForWorkAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="3d13d-121">Delete androidForWorkAppConfigurationSchema</span></span>](../api/intune-androidforwork-androidforworkappconfigurationschema-delete.md)|<span data-ttu-id="3d13d-122">无</span><span class="sxs-lookup"><span data-stu-id="3d13d-122">None</span></span>|<span data-ttu-id="3d13d-123">删除 [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md)。</span><span class="sxs-lookup"><span data-stu-id="3d13d-123">Deletes a [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span></span>|
|[<span data-ttu-id="3d13d-124">更新 androidForWorkAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="3d13d-124">Update androidForWorkAppConfigurationSchema</span></span>](../api/intune-androidforwork-androidforworkappconfigurationschema-update.md)|[<span data-ttu-id="3d13d-125">androidForWorkAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="3d13d-125">androidForWorkAppConfigurationSchema</span></span>](../resources/intune-androidforwork-androidforworkappconfigurationschema.md)|<span data-ttu-id="3d13d-126">更新 [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3d13d-126">Update the properties of a [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3d13d-127">属性</span><span class="sxs-lookup"><span data-stu-id="3d13d-127">Properties</span></span>
|<span data-ttu-id="3d13d-128">属性</span><span class="sxs-lookup"><span data-stu-id="3d13d-128">Property</span></span>|<span data-ttu-id="3d13d-129">类型</span><span class="sxs-lookup"><span data-stu-id="3d13d-129">Type</span></span>|<span data-ttu-id="3d13d-130">说明</span><span class="sxs-lookup"><span data-stu-id="3d13d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d13d-131">id</span><span class="sxs-lookup"><span data-stu-id="3d13d-131">id</span></span>|<span data-ttu-id="3d13d-132">String</span><span class="sxs-lookup"><span data-stu-id="3d13d-132">String</span></span>|<span data-ttu-id="3d13d-133">架构对应的应用程序的 Android 包名称的实体密钥</span><span class="sxs-lookup"><span data-stu-id="3d13d-133">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="3d13d-134">exampleJson</span><span class="sxs-lookup"><span data-stu-id="3d13d-134">exampleJson</span></span>|<span data-ttu-id="3d13d-135">Binary</span><span class="sxs-lookup"><span data-stu-id="3d13d-135">Binary</span></span>|<span data-ttu-id="3d13d-136">包含符合此架构的示例 JSON 字符串的 UTF8 编码的字节数组，它演示如何设置此应用的配置</span><span class="sxs-lookup"><span data-stu-id="3d13d-136">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="3d13d-137">schemaItems</span><span class="sxs-lookup"><span data-stu-id="3d13d-137">schemaItems</span></span>|<span data-ttu-id="3d13d-138">[androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3d13d-138">[androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="3d13d-139">项集合，每个项表示架构中命名的配置选项</span><span class="sxs-lookup"><span data-stu-id="3d13d-139">Collection of items each representing a named configuration option in the schema</span></span>|

## <a name="relationships"></a><span data-ttu-id="3d13d-140">关系</span><span class="sxs-lookup"><span data-stu-id="3d13d-140">Relationships</span></span>
<span data-ttu-id="3d13d-141">无</span><span class="sxs-lookup"><span data-stu-id="3d13d-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3d13d-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3d13d-142">JSON Representation</span></span>
<span data-ttu-id="3d13d-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3d13d-143">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchema"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkAppConfigurationSchema",
  "id": "String (identifier)",
  "exampleJson": "binary",
  "schemaItems": [
    {
      "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchemaItem",
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
  ]
}
```




