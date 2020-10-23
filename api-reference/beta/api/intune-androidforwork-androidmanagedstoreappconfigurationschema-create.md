---
title: 创建 androidManagedStoreAppConfigurationSchema
description: 创建新的 androidManagedStoreAppConfigurationSchema 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d0f743d03e9ce915e5d8bd0f31d94593da01c9ed
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48700960"
---
# <a name="create-androidmanagedstoreappconfigurationschema"></a><span data-ttu-id="c8d50-103">创建 androidManagedStoreAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="c8d50-103">Create androidManagedStoreAppConfigurationSchema</span></span>

<span data-ttu-id="c8d50-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8d50-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c8d50-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c8d50-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c8d50-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c8d50-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8d50-107">创建新的 [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c8d50-107">Create a new [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c8d50-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c8d50-108">Prerequisites</span></span>
<span data-ttu-id="c8d50-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c8d50-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8d50-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c8d50-111">Permission type</span></span>|<span data-ttu-id="c8d50-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c8d50-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8d50-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c8d50-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c8d50-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8d50-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c8d50-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c8d50-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8d50-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c8d50-116">Not supported.</span></span>|
|<span data-ttu-id="c8d50-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c8d50-117">Application</span></span>|<span data-ttu-id="c8d50-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8d50-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8d50-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c8d50-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidManagedStoreAppConfigurationSchemas
```

## <a name="request-headers"></a><span data-ttu-id="c8d50-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c8d50-120">Request headers</span></span>
|<span data-ttu-id="c8d50-121">标头</span><span class="sxs-lookup"><span data-stu-id="c8d50-121">Header</span></span>|<span data-ttu-id="c8d50-122">值</span><span class="sxs-lookup"><span data-stu-id="c8d50-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8d50-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8d50-123">Authorization</span></span>|<span data-ttu-id="c8d50-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c8d50-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8d50-125">接受</span><span class="sxs-lookup"><span data-stu-id="c8d50-125">Accept</span></span>|<span data-ttu-id="c8d50-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c8d50-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8d50-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c8d50-127">Request body</span></span>
<span data-ttu-id="c8d50-128">在请求正文中，提供 androidManagedStoreAppConfigurationSchema 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c8d50-128">In the request body, supply a JSON representation for the androidManagedStoreAppConfigurationSchema object.</span></span>

<span data-ttu-id="c8d50-129">下表显示创建 androidManagedStoreAppConfigurationSchema 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c8d50-129">The following table shows the properties that are required when you create the androidManagedStoreAppConfigurationSchema.</span></span>

|<span data-ttu-id="c8d50-130">属性</span><span class="sxs-lookup"><span data-stu-id="c8d50-130">Property</span></span>|<span data-ttu-id="c8d50-131">类型</span><span class="sxs-lookup"><span data-stu-id="c8d50-131">Type</span></span>|<span data-ttu-id="c8d50-132">说明</span><span class="sxs-lookup"><span data-stu-id="c8d50-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8d50-133">id</span><span class="sxs-lookup"><span data-stu-id="c8d50-133">id</span></span>|<span data-ttu-id="c8d50-134">String</span><span class="sxs-lookup"><span data-stu-id="c8d50-134">String</span></span>|<span data-ttu-id="c8d50-135">架构对应的应用程序的 Android 包名称的实体密钥</span><span class="sxs-lookup"><span data-stu-id="c8d50-135">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="c8d50-136">exampleJson</span><span class="sxs-lookup"><span data-stu-id="c8d50-136">exampleJson</span></span>|<span data-ttu-id="c8d50-137">Binary</span><span class="sxs-lookup"><span data-stu-id="c8d50-137">Binary</span></span>|<span data-ttu-id="c8d50-138">包含符合此架构的示例 JSON 字符串的 UTF8 编码的字节数组，它演示如何设置此应用的配置</span><span class="sxs-lookup"><span data-stu-id="c8d50-138">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="c8d50-139">schemaItems</span><span class="sxs-lookup"><span data-stu-id="c8d50-139">schemaItems</span></span>|<span data-ttu-id="c8d50-140">[androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c8d50-140">[androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="c8d50-141">项集合，每个项表示架构中的命名配置选项。</span><span class="sxs-lookup"><span data-stu-id="c8d50-141">Collection of items each representing a named configuration option in the schema.</span></span> <span data-ttu-id="c8d50-142">它仅包含根级别的配置。</span><span class="sxs-lookup"><span data-stu-id="c8d50-142">It only contains the root-level configuration.</span></span>|
|<span data-ttu-id="c8d50-143">nestedSchemaItems</span><span class="sxs-lookup"><span data-stu-id="c8d50-143">nestedSchemaItems</span></span>|<span data-ttu-id="c8d50-144">[androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c8d50-144">[androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="c8d50-145">项集合，每个项表示架构中的命名配置选项。</span><span class="sxs-lookup"><span data-stu-id="c8d50-145">Collection of items each representing a named configuration option in the schema.</span></span> <span data-ttu-id="c8d50-146">它包含所有配置的简单列表。</span><span class="sxs-lookup"><span data-stu-id="c8d50-146">It contains a flat list of all configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="c8d50-147">响应</span><span class="sxs-lookup"><span data-stu-id="c8d50-147">Response</span></span>
<span data-ttu-id="c8d50-148">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c8d50-148">If successful, this method returns a `201 Created` response code and a [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8d50-149">示例</span><span class="sxs-lookup"><span data-stu-id="c8d50-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="c8d50-150">请求</span><span class="sxs-lookup"><span data-stu-id="c8d50-150">Request</span></span>
<span data-ttu-id="c8d50-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c8d50-151">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAppConfigurationSchemas
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

### <a name="response"></a><span data-ttu-id="c8d50-152">响应</span><span class="sxs-lookup"><span data-stu-id="c8d50-152">Response</span></span>
<span data-ttu-id="c8d50-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c8d50-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





