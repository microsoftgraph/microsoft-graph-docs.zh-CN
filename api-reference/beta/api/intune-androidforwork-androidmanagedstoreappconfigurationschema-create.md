---
title: 创建 androidManagedStoreAppConfigurationSchema
description: 创建新的 androidManagedStoreAppConfigurationSchema 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fe65543c01607196fbc0da17563848c7ae6a6738
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405945"
---
# <a name="create-androidmanagedstoreappconfigurationschema"></a><span data-ttu-id="2c5b7-103">创建 androidManagedStoreAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="2c5b7-103">Create androidManagedStoreAppConfigurationSchema</span></span>

> <span data-ttu-id="2c5b7-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="2c5b7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2c5b7-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2c5b7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2c5b7-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2c5b7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c5b7-107">创建新的[androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2c5b7-107">Create a new [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2c5b7-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="2c5b7-108">Prerequisites</span></span>
<span data-ttu-id="2c5b7-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="2c5b7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2c5b7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2c5b7-111">Permission type</span></span>|<span data-ttu-id="2c5b7-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2c5b7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2c5b7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2c5b7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2c5b7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c5b7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2c5b7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2c5b7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2c5b7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2c5b7-116">Not supported.</span></span>|
|<span data-ttu-id="2c5b7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2c5b7-117">Application</span></span>|<span data-ttu-id="2c5b7-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="2c5b7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2c5b7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2c5b7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidManagedStoreAppConfigurationSchemas
```

## <a name="request-headers"></a><span data-ttu-id="2c5b7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2c5b7-120">Request headers</span></span>
|<span data-ttu-id="2c5b7-121">标头</span><span class="sxs-lookup"><span data-stu-id="2c5b7-121">Header</span></span>|<span data-ttu-id="2c5b7-122">值</span><span class="sxs-lookup"><span data-stu-id="2c5b7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2c5b7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2c5b7-123">Authorization</span></span>|<span data-ttu-id="2c5b7-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2c5b7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2c5b7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2c5b7-125">Accept</span></span>|<span data-ttu-id="2c5b7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2c5b7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2c5b7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2c5b7-127">Request body</span></span>
<span data-ttu-id="2c5b7-128">在请求正文中，提供 androidManagedStoreAppConfigurationSchema 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2c5b7-128">In the request body, supply a JSON representation for the androidManagedStoreAppConfigurationSchema object.</span></span>

<span data-ttu-id="2c5b7-129">下表显示时创建 androidManagedStoreAppConfigurationSchema 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2c5b7-129">The following table shows the properties that are required when you create the androidManagedStoreAppConfigurationSchema.</span></span>

|<span data-ttu-id="2c5b7-130">属性</span><span class="sxs-lookup"><span data-stu-id="2c5b7-130">Property</span></span>|<span data-ttu-id="2c5b7-131">类型</span><span class="sxs-lookup"><span data-stu-id="2c5b7-131">Type</span></span>|<span data-ttu-id="2c5b7-132">说明</span><span class="sxs-lookup"><span data-stu-id="2c5b7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c5b7-133">id</span><span class="sxs-lookup"><span data-stu-id="2c5b7-133">id</span></span>|<span data-ttu-id="2c5b7-134">String</span><span class="sxs-lookup"><span data-stu-id="2c5b7-134">String</span></span>|<span data-ttu-id="2c5b7-135">架构对应的应用程序的 Android 包名称的实体密钥</span><span class="sxs-lookup"><span data-stu-id="2c5b7-135">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="2c5b7-136">exampleJson</span><span class="sxs-lookup"><span data-stu-id="2c5b7-136">exampleJson</span></span>|<span data-ttu-id="2c5b7-137">Binary</span><span class="sxs-lookup"><span data-stu-id="2c5b7-137">Binary</span></span>|<span data-ttu-id="2c5b7-138">包含符合此架构的示例 JSON 字符串的 UTF8 编码的字节数组，它演示如何设置此应用的配置</span><span class="sxs-lookup"><span data-stu-id="2c5b7-138">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="2c5b7-139">schemaItems</span><span class="sxs-lookup"><span data-stu-id="2c5b7-139">schemaItems</span></span>|<span data-ttu-id="2c5b7-140">[androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="2c5b7-140">[androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="2c5b7-141">项集合，每个项表示架构中命名的配置选项</span><span class="sxs-lookup"><span data-stu-id="2c5b7-141">Collection of items each representing a named configuration option in the schema</span></span>|



## <a name="response"></a><span data-ttu-id="2c5b7-142">响应</span><span class="sxs-lookup"><span data-stu-id="2c5b7-142">Response</span></span>
<span data-ttu-id="2c5b7-143">如果成功，此方法返回`201 Created`响应代码和响应正文中的[androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2c5b7-143">If successful, this method returns a `201 Created` response code and a [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2c5b7-144">示例</span><span class="sxs-lookup"><span data-stu-id="2c5b7-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="2c5b7-145">请求</span><span class="sxs-lookup"><span data-stu-id="2c5b7-145">Request</span></span>
<span data-ttu-id="2c5b7-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2c5b7-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAppConfigurationSchemas
Content-type: application/json
Content-length: 805

{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfigurationSchema",
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

### <a name="response"></a><span data-ttu-id="2c5b7-147">响应</span><span class="sxs-lookup"><span data-stu-id="2c5b7-147">Response</span></span>
<span data-ttu-id="2c5b7-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2c5b7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




