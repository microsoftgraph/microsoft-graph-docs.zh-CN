---
title: 更新 androidManagedStoreAppConfigurationSchema
description: 更新 androidManagedStoreAppConfigurationSchema 对象的属性。
ms.openlocfilehash: e762a909db958b62d1128ff1dae178181124990c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042615"
---
# <a name="update-androidmanagedstoreappconfigurationschema"></a><span data-ttu-id="de39d-103">更新 androidManagedStoreAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="de39d-103">Update androidManagedStoreAppConfigurationSchema</span></span>

> <span data-ttu-id="de39d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="de39d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="de39d-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="de39d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="de39d-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="de39d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="de39d-107">更新[androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="de39d-107">Update the properties of a [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="de39d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="de39d-108">Prerequisites</span></span>
<span data-ttu-id="de39d-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="de39d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de39d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="de39d-111">Permission type</span></span>|<span data-ttu-id="de39d-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="de39d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de39d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="de39d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="de39d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de39d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="de39d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="de39d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de39d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="de39d-116">Not supported.</span></span>|
|<span data-ttu-id="de39d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="de39d-117">Application</span></span>|<span data-ttu-id="de39d-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="de39d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="de39d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="de39d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidManagedStoreAppConfigurationSchemas/{androidManagedStoreAppConfigurationSchemaId}
```

## <a name="request-headers"></a><span data-ttu-id="de39d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="de39d-120">Request headers</span></span>
|<span data-ttu-id="de39d-121">标头</span><span class="sxs-lookup"><span data-stu-id="de39d-121">Header</span></span>|<span data-ttu-id="de39d-122">值</span><span class="sxs-lookup"><span data-stu-id="de39d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de39d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="de39d-123">Authorization</span></span>|<span data-ttu-id="de39d-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="de39d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="de39d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="de39d-125">Accept</span></span>|<span data-ttu-id="de39d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="de39d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de39d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="de39d-127">Request body</span></span>
<span data-ttu-id="de39d-128">在请求正文中，提供[androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="de39d-128">In the request body, supply a JSON representation for the [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object.</span></span>

<span data-ttu-id="de39d-129">下表显示时创建[androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="de39d-129">The following table shows the properties that are required when you create the [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md).</span></span>

|<span data-ttu-id="de39d-130">属性</span><span class="sxs-lookup"><span data-stu-id="de39d-130">Property</span></span>|<span data-ttu-id="de39d-131">类型</span><span class="sxs-lookup"><span data-stu-id="de39d-131">Type</span></span>|<span data-ttu-id="de39d-132">说明</span><span class="sxs-lookup"><span data-stu-id="de39d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de39d-133">id</span><span class="sxs-lookup"><span data-stu-id="de39d-133">id</span></span>|<span data-ttu-id="de39d-134">String</span><span class="sxs-lookup"><span data-stu-id="de39d-134">String</span></span>|<span data-ttu-id="de39d-135">架构对应的应用程序的 Android 包名称的实体密钥</span><span class="sxs-lookup"><span data-stu-id="de39d-135">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="de39d-136">exampleJson</span><span class="sxs-lookup"><span data-stu-id="de39d-136">exampleJson</span></span>|<span data-ttu-id="de39d-137">Binary</span><span class="sxs-lookup"><span data-stu-id="de39d-137">Binary</span></span>|<span data-ttu-id="de39d-138">包含符合此架构的示例 JSON 字符串的 UTF8 编码的字节数组，它演示如何设置此应用的配置</span><span class="sxs-lookup"><span data-stu-id="de39d-138">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="de39d-139">schemaItems</span><span class="sxs-lookup"><span data-stu-id="de39d-139">schemaItems</span></span>|<span data-ttu-id="de39d-140">[androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="de39d-140">[androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="de39d-141">项集合，每个项表示架构中命名的配置选项</span><span class="sxs-lookup"><span data-stu-id="de39d-141">Collection of items each representing a named configuration option in the schema</span></span>|



## <a name="response"></a><span data-ttu-id="de39d-142">响应</span><span class="sxs-lookup"><span data-stu-id="de39d-142">Response</span></span>
<span data-ttu-id="de39d-143">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)对象。</span><span class="sxs-lookup"><span data-stu-id="de39d-143">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de39d-144">示例</span><span class="sxs-lookup"><span data-stu-id="de39d-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="de39d-145">请求</span><span class="sxs-lookup"><span data-stu-id="de39d-145">Request</span></span>
<span data-ttu-id="de39d-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="de39d-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAppConfigurationSchemas/{androidManagedStoreAppConfigurationSchemaId}
Content-type: application/json
Content-length: 725

{
  "exampleJson": "ZXhhbXBsZUpzb24=",
  "schemaItems": [
    {
      "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem",
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

### <a name="response"></a><span data-ttu-id="de39d-147">响应</span><span class="sxs-lookup"><span data-stu-id="de39d-147">Response</span></span>
<span data-ttu-id="de39d-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="de39d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 854

{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfigurationSchema",
  "id": "db86c34a-c34a-db86-4ac3-86db4ac386db",
  "exampleJson": "ZXhhbXBsZUpzb24=",
  "schemaItems": [
    {
      "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem",
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





