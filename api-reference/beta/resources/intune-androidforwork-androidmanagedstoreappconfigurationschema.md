---
title: androidManagedStoreAppConfigurationSchema 资源类型
description: 描述 Android 应用程序的自定义配置的模式。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9e520957ddcdba6c713b5564fdf1a85ce6ad8b08
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414947"
---
# <a name="androidmanagedstoreappconfigurationschema-resource-type"></a><span data-ttu-id="ebcc2-103">androidManagedStoreAppConfigurationSchema 资源类型</span><span class="sxs-lookup"><span data-stu-id="ebcc2-103">androidManagedStoreAppConfigurationSchema resource type</span></span>

> <span data-ttu-id="ebcc2-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="ebcc2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ebcc2-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ebcc2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ebcc2-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ebcc2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ebcc2-107">描述 Android 应用程序的自定义配置的模式。</span><span class="sxs-lookup"><span data-stu-id="ebcc2-107">Schema describing an Android application's custom configurations.</span></span>

## <a name="methods"></a><span data-ttu-id="ebcc2-108">方法</span><span class="sxs-lookup"><span data-stu-id="ebcc2-108">Methods</span></span>
|<span data-ttu-id="ebcc2-109">方法</span><span class="sxs-lookup"><span data-stu-id="ebcc2-109">Method</span></span>|<span data-ttu-id="ebcc2-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="ebcc2-110">Return Type</span></span>|<span data-ttu-id="ebcc2-111">说明</span><span class="sxs-lookup"><span data-stu-id="ebcc2-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ebcc2-112">列表 androidManagedStoreAppConfigurationSchemas</span><span class="sxs-lookup"><span data-stu-id="ebcc2-112">List androidManagedStoreAppConfigurationSchemas</span></span>](../api/intune-androidforwork-androidmanagedstoreappconfigurationschema-list.md)|<span data-ttu-id="ebcc2-113">[androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)集合</span><span class="sxs-lookup"><span data-stu-id="ebcc2-113">[androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) collection</span></span>|<span data-ttu-id="ebcc2-114">列出属性和[androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="ebcc2-114">List properties and relationships of the [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) objects.</span></span>|
|[<span data-ttu-id="ebcc2-115">获取 androidManagedStoreAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="ebcc2-115">Get androidManagedStoreAppConfigurationSchema</span></span>](../api/intune-androidforwork-androidmanagedstoreappconfigurationschema-get.md)|[<span data-ttu-id="ebcc2-116">androidManagedStoreAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="ebcc2-116">androidManagedStoreAppConfigurationSchema</span></span>](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)|<span data-ttu-id="ebcc2-117">读取属性和[androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="ebcc2-117">Read properties and relationships of the [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object.</span></span>|
|[<span data-ttu-id="ebcc2-118">创建 androidManagedStoreAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="ebcc2-118">Create androidManagedStoreAppConfigurationSchema</span></span>](../api/intune-androidforwork-androidmanagedstoreappconfigurationschema-create.md)|[<span data-ttu-id="ebcc2-119">androidManagedStoreAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="ebcc2-119">androidManagedStoreAppConfigurationSchema</span></span>](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)|<span data-ttu-id="ebcc2-120">创建新的[androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ebcc2-120">Create a new [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object.</span></span>|
|[<span data-ttu-id="ebcc2-121">删除 androidManagedStoreAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="ebcc2-121">Delete androidManagedStoreAppConfigurationSchema</span></span>](../api/intune-androidforwork-androidmanagedstoreappconfigurationschema-delete.md)|<span data-ttu-id="ebcc2-122">无</span><span class="sxs-lookup"><span data-stu-id="ebcc2-122">None</span></span>|<span data-ttu-id="ebcc2-123">删除[androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)。</span><span class="sxs-lookup"><span data-stu-id="ebcc2-123">Deletes a [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md).</span></span>|
|[<span data-ttu-id="ebcc2-124">更新 androidManagedStoreAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="ebcc2-124">Update androidManagedStoreAppConfigurationSchema</span></span>](../api/intune-androidforwork-androidmanagedstoreappconfigurationschema-update.md)|[<span data-ttu-id="ebcc2-125">androidManagedStoreAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="ebcc2-125">androidManagedStoreAppConfigurationSchema</span></span>](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)|<span data-ttu-id="ebcc2-126">更新[androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ebcc2-126">Update the properties of a [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ebcc2-127">属性</span><span class="sxs-lookup"><span data-stu-id="ebcc2-127">Properties</span></span>
|<span data-ttu-id="ebcc2-128">属性</span><span class="sxs-lookup"><span data-stu-id="ebcc2-128">Property</span></span>|<span data-ttu-id="ebcc2-129">类型</span><span class="sxs-lookup"><span data-stu-id="ebcc2-129">Type</span></span>|<span data-ttu-id="ebcc2-130">说明</span><span class="sxs-lookup"><span data-stu-id="ebcc2-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebcc2-131">id</span><span class="sxs-lookup"><span data-stu-id="ebcc2-131">id</span></span>|<span data-ttu-id="ebcc2-132">String</span><span class="sxs-lookup"><span data-stu-id="ebcc2-132">String</span></span>|<span data-ttu-id="ebcc2-133">架构对应的应用程序的 Android 包名称的实体密钥</span><span class="sxs-lookup"><span data-stu-id="ebcc2-133">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="ebcc2-134">exampleJson</span><span class="sxs-lookup"><span data-stu-id="ebcc2-134">exampleJson</span></span>|<span data-ttu-id="ebcc2-135">Binary</span><span class="sxs-lookup"><span data-stu-id="ebcc2-135">Binary</span></span>|<span data-ttu-id="ebcc2-136">包含符合此架构的示例 JSON 字符串的 UTF8 编码的字节数组，它演示如何设置此应用的配置</span><span class="sxs-lookup"><span data-stu-id="ebcc2-136">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="ebcc2-137">schemaItems</span><span class="sxs-lookup"><span data-stu-id="ebcc2-137">schemaItems</span></span>|<span data-ttu-id="ebcc2-138">[androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="ebcc2-138">[androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="ebcc2-139">项集合，每个项表示架构中命名的配置选项</span><span class="sxs-lookup"><span data-stu-id="ebcc2-139">Collection of items each representing a named configuration option in the schema</span></span>|

## <a name="relationships"></a><span data-ttu-id="ebcc2-140">关系</span><span class="sxs-lookup"><span data-stu-id="ebcc2-140">Relationships</span></span>
<span data-ttu-id="ebcc2-141">无</span><span class="sxs-lookup"><span data-stu-id="ebcc2-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ebcc2-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ebcc2-142">JSON Representation</span></span>
<span data-ttu-id="ebcc2-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ebcc2-143">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchema"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfigurationSchema",
  "id": "String (identifier)",
  "exampleJson": "binary",
  "schemaItems": [
    {
      "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem",
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




