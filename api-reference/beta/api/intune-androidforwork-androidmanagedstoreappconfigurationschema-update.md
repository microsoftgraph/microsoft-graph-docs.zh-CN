---
title: 更新 androidManagedStoreAppConfigurationSchema
description: 更新 androidManagedStoreAppConfigurationSchema 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5a58997898c1509290eddaf93030abf15f013773
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51144562"
---
# <a name="update-androidmanagedstoreappconfigurationschema"></a><span data-ttu-id="af343-103">更新 androidManagedStoreAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="af343-103">Update androidManagedStoreAppConfigurationSchema</span></span>

<span data-ttu-id="af343-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af343-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="af343-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="af343-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="af343-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="af343-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af343-107">更新 [androidManagedStoreAppConfigurationSchema 对象](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="af343-107">Update the properties of a [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="af343-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="af343-108">Prerequisites</span></span>
<span data-ttu-id="af343-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="af343-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af343-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="af343-111">Permission type</span></span>|<span data-ttu-id="af343-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="af343-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af343-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="af343-113">Delegated (work or school account)</span></span>|<span data-ttu-id="af343-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af343-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="af343-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="af343-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af343-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="af343-116">Not supported.</span></span>|
|<span data-ttu-id="af343-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="af343-117">Application</span></span>|<span data-ttu-id="af343-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af343-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="af343-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="af343-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidManagedStoreAppConfigurationSchemas/{androidManagedStoreAppConfigurationSchemaId}
```

## <a name="request-headers"></a><span data-ttu-id="af343-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="af343-120">Request headers</span></span>
|<span data-ttu-id="af343-121">标头</span><span class="sxs-lookup"><span data-stu-id="af343-121">Header</span></span>|<span data-ttu-id="af343-122">值</span><span class="sxs-lookup"><span data-stu-id="af343-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af343-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="af343-123">Authorization</span></span>|<span data-ttu-id="af343-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="af343-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="af343-125">接受</span><span class="sxs-lookup"><span data-stu-id="af343-125">Accept</span></span>|<span data-ttu-id="af343-126">application/json</span><span class="sxs-lookup"><span data-stu-id="af343-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af343-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="af343-127">Request body</span></span>
<span data-ttu-id="af343-128">在请求正文中，提供 [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="af343-128">In the request body, supply a JSON representation for the [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object.</span></span>

<span data-ttu-id="af343-129">下表显示创建 [androidManagedStoreAppConfigurationSchema 时所需的属性](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)。</span><span class="sxs-lookup"><span data-stu-id="af343-129">The following table shows the properties that are required when you create the [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md).</span></span>

|<span data-ttu-id="af343-130">属性</span><span class="sxs-lookup"><span data-stu-id="af343-130">Property</span></span>|<span data-ttu-id="af343-131">类型</span><span class="sxs-lookup"><span data-stu-id="af343-131">Type</span></span>|<span data-ttu-id="af343-132">说明</span><span class="sxs-lookup"><span data-stu-id="af343-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af343-133">id</span><span class="sxs-lookup"><span data-stu-id="af343-133">id</span></span>|<span data-ttu-id="af343-134">String</span><span class="sxs-lookup"><span data-stu-id="af343-134">String</span></span>|<span data-ttu-id="af343-135">架构对应的应用程序的 Android 包名称的实体密钥</span><span class="sxs-lookup"><span data-stu-id="af343-135">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="af343-136">exampleJson</span><span class="sxs-lookup"><span data-stu-id="af343-136">exampleJson</span></span>|<span data-ttu-id="af343-137">Binary</span><span class="sxs-lookup"><span data-stu-id="af343-137">Binary</span></span>|<span data-ttu-id="af343-138">包含符合此架构的示例 JSON 字符串的 UTF8 编码的字节数组，它演示如何设置此应用的配置</span><span class="sxs-lookup"><span data-stu-id="af343-138">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="af343-139">schemaItems</span><span class="sxs-lookup"><span data-stu-id="af343-139">schemaItems</span></span>|<span data-ttu-id="af343-140">[androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="af343-140">[androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="af343-141">每个表示架构中命名配置选项的项的集合。</span><span class="sxs-lookup"><span data-stu-id="af343-141">Collection of items each representing a named configuration option in the schema.</span></span> <span data-ttu-id="af343-142">它仅包含根级别配置。</span><span class="sxs-lookup"><span data-stu-id="af343-142">It only contains the root-level configuration.</span></span>|
|<span data-ttu-id="af343-143">nestedSchemaItems</span><span class="sxs-lookup"><span data-stu-id="af343-143">nestedSchemaItems</span></span>|<span data-ttu-id="af343-144">[androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="af343-144">[androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="af343-145">每个表示架构中命名配置选项的项的集合。</span><span class="sxs-lookup"><span data-stu-id="af343-145">Collection of items each representing a named configuration option in the schema.</span></span> <span data-ttu-id="af343-146">它包含所有简单列表的一个列表。</span><span class="sxs-lookup"><span data-stu-id="af343-146">It contains a flat list of all configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="af343-147">响应</span><span class="sxs-lookup"><span data-stu-id="af343-147">Response</span></span>
<span data-ttu-id="af343-148">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="af343-148">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af343-149">示例</span><span class="sxs-lookup"><span data-stu-id="af343-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="af343-150">请求</span><span class="sxs-lookup"><span data-stu-id="af343-150">Request</span></span>
<span data-ttu-id="af343-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="af343-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAppConfigurationSchemas/{androidManagedStoreAppConfigurationSchemaId}
Content-type: application/json
Content-length: 1585

{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfigurationSchema",
  "exampleJson": "ZXhhbXBsZUpzb24=",
  "schemaItems": [
    {
      "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem",
      "index": 5,
      "parentIndex": 11,
      "schemaItemKey": "Schema Item Key value",
      "displayName": "Display Name value",
      "description": "Description value",
      "defaultBoolValue": true,
      "defaultIntValue": 15,
      "defaultStringValue": "Default String Value value",
      "defaultStringArrayValue": [
        "Default String Array Value value"
      ],
      "dataType": "integer",
      "selections": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ]
    }
  ],
  "nestedSchemaItems": [
    {
      "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem",
      "index": 5,
      "parentIndex": 11,
      "schemaItemKey": "Schema Item Key value",
      "displayName": "Display Name value",
      "description": "Description value",
      "defaultBoolValue": true,
      "defaultIntValue": 15,
      "defaultStringValue": "Default String Value value",
      "defaultStringArrayValue": [
        "Default String Array Value value"
      ],
      "dataType": "integer",
      "selections": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ]
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="af343-152">响应</span><span class="sxs-lookup"><span data-stu-id="af343-152">Response</span></span>
<span data-ttu-id="af343-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="af343-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1634

{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfigurationSchema",
  "id": "db86c34a-c34a-db86-4ac3-86db4ac386db",
  "exampleJson": "ZXhhbXBsZUpzb24=",
  "schemaItems": [
    {
      "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem",
      "index": 5,
      "parentIndex": 11,
      "schemaItemKey": "Schema Item Key value",
      "displayName": "Display Name value",
      "description": "Description value",
      "defaultBoolValue": true,
      "defaultIntValue": 15,
      "defaultStringValue": "Default String Value value",
      "defaultStringArrayValue": [
        "Default String Array Value value"
      ],
      "dataType": "integer",
      "selections": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ]
    }
  ],
  "nestedSchemaItems": [
    {
      "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem",
      "index": 5,
      "parentIndex": 11,
      "schemaItemKey": "Schema Item Key value",
      "displayName": "Display Name value",
      "description": "Description value",
      "defaultBoolValue": true,
      "defaultIntValue": 15,
      "defaultStringValue": "Default String Value value",
      "defaultStringArrayValue": [
        "Default String Array Value value"
      ],
      "dataType": "integer",
      "selections": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ]
    }
  ]
}
```




