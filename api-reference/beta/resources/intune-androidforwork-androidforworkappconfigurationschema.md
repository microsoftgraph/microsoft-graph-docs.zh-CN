---
title: androidForWorkAppConfigurationSchema 资源类型
description: 描述 Android for Work 应用程序的自定义配置的架构。
localization_priority: Normal
ms.openlocfilehash: fecb4c3983254643704e6c5966212272f8f1d65e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882892"
---
# <a name="androidforworkappconfigurationschema-resource-type"></a><span data-ttu-id="5b52b-103">androidForWorkAppConfigurationSchema 资源类型</span><span class="sxs-lookup"><span data-stu-id="5b52b-103">androidForWorkAppConfigurationSchema resource type</span></span>

> <span data-ttu-id="5b52b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5b52b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5b52b-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5b52b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5b52b-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5b52b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5b52b-107">描述 Android for Work 应用程序的自定义配置的架构。</span><span class="sxs-lookup"><span data-stu-id="5b52b-107">Schema describing an Android for Work application's custom configurations.</span></span>
## <a name="methods"></a><span data-ttu-id="5b52b-108">方法</span><span class="sxs-lookup"><span data-stu-id="5b52b-108">Methods</span></span>
|<span data-ttu-id="5b52b-109">方法</span><span class="sxs-lookup"><span data-stu-id="5b52b-109">Method</span></span>|<span data-ttu-id="5b52b-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="5b52b-110">Return Type</span></span>|<span data-ttu-id="5b52b-111">说明</span><span class="sxs-lookup"><span data-stu-id="5b52b-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5b52b-112">列出 androidForWorkAppConfigurationSchemas</span><span class="sxs-lookup"><span data-stu-id="5b52b-112">List androidForWorkAppConfigurationSchemas</span></span>](../api/intune-androidforwork-androidforworkappconfigurationschema-list.md)|<span data-ttu-id="5b52b-113">[androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5b52b-113">[androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) collection</span></span>|<span data-ttu-id="5b52b-114">列出 [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5b52b-114">List properties and relationships of the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) objects.</span></span>|
|[<span data-ttu-id="5b52b-115">获取 androidForWorkAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="5b52b-115">Get androidForWorkAppConfigurationSchema</span></span>](../api/intune-androidforwork-androidforworkappconfigurationschema-get.md)|[<span data-ttu-id="5b52b-116">androidForWorkAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="5b52b-116">androidForWorkAppConfigurationSchema</span></span>](../resources/intune-androidforwork-androidforworkappconfigurationschema.md)|<span data-ttu-id="5b52b-117">读取 [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5b52b-117">Read properties and relationships of the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>|
|[<span data-ttu-id="5b52b-118">创建 androidForWorkAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="5b52b-118">Create androidForWorkAppConfigurationSchema</span></span>](../api/intune-androidforwork-androidforworkappconfigurationschema-create.md)|[<span data-ttu-id="5b52b-119">androidForWorkAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="5b52b-119">androidForWorkAppConfigurationSchema</span></span>](../resources/intune-androidforwork-androidforworkappconfigurationschema.md)|<span data-ttu-id="5b52b-120">创建新的 [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5b52b-120">Create a new [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>|
|[<span data-ttu-id="5b52b-121">删除 androidForWorkAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="5b52b-121">Delete androidForWorkAppConfigurationSchema</span></span>](../api/intune-androidforwork-androidforworkappconfigurationschema-delete.md)|<span data-ttu-id="5b52b-122">无</span><span class="sxs-lookup"><span data-stu-id="5b52b-122">None</span></span>|<span data-ttu-id="5b52b-123">删除 [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md)。</span><span class="sxs-lookup"><span data-stu-id="5b52b-123">Deletes a [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span></span>|
|[<span data-ttu-id="5b52b-124">更新 androidForWorkAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="5b52b-124">Update androidForWorkAppConfigurationSchema</span></span>](../api/intune-androidforwork-androidforworkappconfigurationschema-update.md)|[<span data-ttu-id="5b52b-125">androidForWorkAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="5b52b-125">androidForWorkAppConfigurationSchema</span></span>](../resources/intune-androidforwork-androidforworkappconfigurationschema.md)|<span data-ttu-id="5b52b-126">更新 [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5b52b-126">Update the properties of a [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5b52b-127">属性</span><span class="sxs-lookup"><span data-stu-id="5b52b-127">Properties</span></span>
|<span data-ttu-id="5b52b-128">属性</span><span class="sxs-lookup"><span data-stu-id="5b52b-128">Property</span></span>|<span data-ttu-id="5b52b-129">类型</span><span class="sxs-lookup"><span data-stu-id="5b52b-129">Type</span></span>|<span data-ttu-id="5b52b-130">说明</span><span class="sxs-lookup"><span data-stu-id="5b52b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b52b-131">id</span><span class="sxs-lookup"><span data-stu-id="5b52b-131">id</span></span>|<span data-ttu-id="5b52b-132">String</span><span class="sxs-lookup"><span data-stu-id="5b52b-132">String</span></span>|<span data-ttu-id="5b52b-133">架构对应的应用程序的 Android 包名称的实体密钥</span><span class="sxs-lookup"><span data-stu-id="5b52b-133">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="5b52b-134">exampleJson</span><span class="sxs-lookup"><span data-stu-id="5b52b-134">exampleJson</span></span>|<span data-ttu-id="5b52b-135">Binary</span><span class="sxs-lookup"><span data-stu-id="5b52b-135">Binary</span></span>|<span data-ttu-id="5b52b-136">包含符合此架构的示例 JSON 字符串的 UTF8 编码的字节数组，它演示如何设置此应用的配置</span><span class="sxs-lookup"><span data-stu-id="5b52b-136">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="5b52b-137">schemaItems</span><span class="sxs-lookup"><span data-stu-id="5b52b-137">schemaItems</span></span>|<span data-ttu-id="5b52b-138">[androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5b52b-138">[androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="5b52b-139">项集合，每个项表示架构中命名的配置选项</span><span class="sxs-lookup"><span data-stu-id="5b52b-139">Collection of items each representing a named configuration option in the schema</span></span>|

## <a name="relationships"></a><span data-ttu-id="5b52b-140">关系</span><span class="sxs-lookup"><span data-stu-id="5b52b-140">Relationships</span></span>
<span data-ttu-id="5b52b-141">无</span><span class="sxs-lookup"><span data-stu-id="5b52b-141">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5b52b-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5b52b-142">JSON Representation</span></span>
<span data-ttu-id="5b52b-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5b52b-143">Here is a JSON representation of the resource.</span></span>
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





