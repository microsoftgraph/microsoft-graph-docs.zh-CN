---
title: 更新 androidManagedStoreAppConfigurationSchema
description: 更新 androidManagedStoreAppConfigurationSchema 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 95d4da95613f33682d56df2c91a5e3a149d39a08
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42762404"
---
# <a name="update-androidmanagedstoreappconfigurationschema"></a><span data-ttu-id="faa16-103">更新 androidManagedStoreAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="faa16-103">Update androidManagedStoreAppConfigurationSchema</span></span>

> <span data-ttu-id="faa16-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="faa16-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="faa16-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="faa16-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="faa16-106">更新[androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="faa16-106">Update the properties of a [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="faa16-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="faa16-107">Prerequisites</span></span>
<span data-ttu-id="faa16-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="faa16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="faa16-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="faa16-110">Permission type</span></span>|<span data-ttu-id="faa16-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="faa16-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="faa16-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="faa16-112">Delegated (work or school account)</span></span>|<span data-ttu-id="faa16-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="faa16-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="faa16-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="faa16-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="faa16-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="faa16-115">Not supported.</span></span>|
|<span data-ttu-id="faa16-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="faa16-116">Application</span></span>|<span data-ttu-id="faa16-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="faa16-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="faa16-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="faa16-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidManagedStoreAppConfigurationSchemas/{androidManagedStoreAppConfigurationSchemaId}
```

## <a name="request-headers"></a><span data-ttu-id="faa16-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="faa16-119">Request headers</span></span>
|<span data-ttu-id="faa16-120">标头</span><span class="sxs-lookup"><span data-stu-id="faa16-120">Header</span></span>|<span data-ttu-id="faa16-121">值</span><span class="sxs-lookup"><span data-stu-id="faa16-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="faa16-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="faa16-122">Authorization</span></span>|<span data-ttu-id="faa16-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="faa16-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="faa16-124">接受</span><span class="sxs-lookup"><span data-stu-id="faa16-124">Accept</span></span>|<span data-ttu-id="faa16-125">application/json</span><span class="sxs-lookup"><span data-stu-id="faa16-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="faa16-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="faa16-126">Request body</span></span>
<span data-ttu-id="faa16-127">在请求正文中，提供[androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="faa16-127">In the request body, supply a JSON representation for the [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object.</span></span>

<span data-ttu-id="faa16-128">下表显示创建[androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="faa16-128">The following table shows the properties that are required when you create the [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md).</span></span>

|<span data-ttu-id="faa16-129">属性</span><span class="sxs-lookup"><span data-stu-id="faa16-129">Property</span></span>|<span data-ttu-id="faa16-130">类型</span><span class="sxs-lookup"><span data-stu-id="faa16-130">Type</span></span>|<span data-ttu-id="faa16-131">说明</span><span class="sxs-lookup"><span data-stu-id="faa16-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="faa16-132">id</span><span class="sxs-lookup"><span data-stu-id="faa16-132">id</span></span>|<span data-ttu-id="faa16-133">String</span><span class="sxs-lookup"><span data-stu-id="faa16-133">String</span></span>|<span data-ttu-id="faa16-134">架构对应的应用程序的 Android 包名称的实体密钥</span><span class="sxs-lookup"><span data-stu-id="faa16-134">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="faa16-135">exampleJson</span><span class="sxs-lookup"><span data-stu-id="faa16-135">exampleJson</span></span>|<span data-ttu-id="faa16-136">Binary</span><span class="sxs-lookup"><span data-stu-id="faa16-136">Binary</span></span>|<span data-ttu-id="faa16-137">包含符合此架构的示例 JSON 字符串的 UTF8 编码的字节数组，它演示如何设置此应用的配置</span><span class="sxs-lookup"><span data-stu-id="faa16-137">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="faa16-138">schemaItems</span><span class="sxs-lookup"><span data-stu-id="faa16-138">schemaItems</span></span>|<span data-ttu-id="faa16-139">[androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="faa16-139">[androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="faa16-140">项集合，每个项表示架构中的命名配置选项。</span><span class="sxs-lookup"><span data-stu-id="faa16-140">Collection of items each representing a named configuration option in the schema.</span></span> <span data-ttu-id="faa16-141">它仅包含根级别的配置。</span><span class="sxs-lookup"><span data-stu-id="faa16-141">It only contains the root-level configuration.</span></span>|
|<span data-ttu-id="faa16-142">nestedSchemaItems</span><span class="sxs-lookup"><span data-stu-id="faa16-142">nestedSchemaItems</span></span>|<span data-ttu-id="faa16-143">[androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="faa16-143">[androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="faa16-144">项集合，每个项表示架构中的命名配置选项。</span><span class="sxs-lookup"><span data-stu-id="faa16-144">Collection of items each representing a named configuration option in the schema.</span></span> <span data-ttu-id="faa16-145">它包含所有配置的简单列表。</span><span class="sxs-lookup"><span data-stu-id="faa16-145">It contains a flat list of all configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="faa16-146">响应</span><span class="sxs-lookup"><span data-stu-id="faa16-146">Response</span></span>
<span data-ttu-id="faa16-147">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)对象。</span><span class="sxs-lookup"><span data-stu-id="faa16-147">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="faa16-148">示例</span><span class="sxs-lookup"><span data-stu-id="faa16-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="faa16-149">请求</span><span class="sxs-lookup"><span data-stu-id="faa16-149">Request</span></span>
<span data-ttu-id="faa16-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="faa16-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="faa16-151">响应</span><span class="sxs-lookup"><span data-stu-id="faa16-151">Response</span></span>
<span data-ttu-id="faa16-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="faa16-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




