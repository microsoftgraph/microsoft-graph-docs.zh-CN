---
title: 更新 androidForWorkAppConfigurationSchema
description: 更新 androidForWorkAppConfigurationSchema 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9c417c07ae2b3d4b6f3282adc4a3c66d4a849b72
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34965625"
---
# <a name="update-androidforworkappconfigurationschema"></a><span data-ttu-id="194c3-103">更新 androidForWorkAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="194c3-103">Update androidForWorkAppConfigurationSchema</span></span>

> <span data-ttu-id="194c3-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="194c3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="194c3-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="194c3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="194c3-106">更新 [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="194c3-106">Update the properties of a [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="194c3-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="194c3-107">Prerequisites</span></span>
<span data-ttu-id="194c3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="194c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="194c3-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="194c3-110">Permission type</span></span>|<span data-ttu-id="194c3-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="194c3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="194c3-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="194c3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="194c3-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="194c3-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="194c3-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="194c3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="194c3-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="194c3-115">Not supported.</span></span>|
|<span data-ttu-id="194c3-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="194c3-116">Application</span></span>|<span data-ttu-id="194c3-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="194c3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="194c3-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="194c3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkAppConfigurationSchemas/{androidForWorkAppConfigurationSchemaId}
```

## <a name="request-headers"></a><span data-ttu-id="194c3-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="194c3-119">Request headers</span></span>
|<span data-ttu-id="194c3-120">标头</span><span class="sxs-lookup"><span data-stu-id="194c3-120">Header</span></span>|<span data-ttu-id="194c3-121">值</span><span class="sxs-lookup"><span data-stu-id="194c3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="194c3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="194c3-122">Authorization</span></span>|<span data-ttu-id="194c3-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="194c3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="194c3-124">接受</span><span class="sxs-lookup"><span data-stu-id="194c3-124">Accept</span></span>|<span data-ttu-id="194c3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="194c3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="194c3-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="194c3-126">Request body</span></span>
<span data-ttu-id="194c3-127">在请求正文中，提供 [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="194c3-127">In the request body, supply a JSON representation for the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>

<span data-ttu-id="194c3-128">下表显示创建 [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="194c3-128">The following table shows the properties that are required when you create the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span></span>

|<span data-ttu-id="194c3-129">属性</span><span class="sxs-lookup"><span data-stu-id="194c3-129">Property</span></span>|<span data-ttu-id="194c3-130">类型</span><span class="sxs-lookup"><span data-stu-id="194c3-130">Type</span></span>|<span data-ttu-id="194c3-131">说明</span><span class="sxs-lookup"><span data-stu-id="194c3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="194c3-132">id</span><span class="sxs-lookup"><span data-stu-id="194c3-132">id</span></span>|<span data-ttu-id="194c3-133">String</span><span class="sxs-lookup"><span data-stu-id="194c3-133">String</span></span>|<span data-ttu-id="194c3-134">架构对应的应用程序的 Android 包名称的实体密钥</span><span class="sxs-lookup"><span data-stu-id="194c3-134">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="194c3-135">exampleJson</span><span class="sxs-lookup"><span data-stu-id="194c3-135">exampleJson</span></span>|<span data-ttu-id="194c3-136">Binary</span><span class="sxs-lookup"><span data-stu-id="194c3-136">Binary</span></span>|<span data-ttu-id="194c3-137">包含符合此架构的示例 JSON 字符串的 UTF8 编码的字节数组，它演示如何设置此应用的配置</span><span class="sxs-lookup"><span data-stu-id="194c3-137">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="194c3-138">schemaItems</span><span class="sxs-lookup"><span data-stu-id="194c3-138">schemaItems</span></span>|<span data-ttu-id="194c3-139">[androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="194c3-139">[androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="194c3-140">项集合，每个项表示架构中命名的配置选项</span><span class="sxs-lookup"><span data-stu-id="194c3-140">Collection of items each representing a named configuration option in the schema</span></span>|



## <a name="response"></a><span data-ttu-id="194c3-141">响应</span><span class="sxs-lookup"><span data-stu-id="194c3-141">Response</span></span>
<span data-ttu-id="194c3-142">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="194c3-142">If successful, this method returns a `200 OK` response code and an updated [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="194c3-143">示例</span><span class="sxs-lookup"><span data-stu-id="194c3-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="194c3-144">请求</span><span class="sxs-lookup"><span data-stu-id="194c3-144">Request</span></span>
<span data-ttu-id="194c3-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="194c3-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidForWorkAppConfigurationSchemas/{androidForWorkAppConfigurationSchemaId}
Content-type: application/json
Content-length: 795

{
  "@odata.type": "#microsoft.graph.androidForWorkAppConfigurationSchema",
  "exampleJson": "ZXhhbXBsZUpzb24=",
  "schemaItems": [
    {
      "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchemaItem",
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

### <a name="response"></a><span data-ttu-id="194c3-146">响应</span><span class="sxs-lookup"><span data-stu-id="194c3-146">Response</span></span>
<span data-ttu-id="194c3-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="194c3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 844

{
  "@odata.type": "#microsoft.graph.androidForWorkAppConfigurationSchema",
  "id": "c1230dc6-0dc6-c123-c60d-23c1c60d23c1",
  "exampleJson": "ZXhhbXBsZUpzb24=",
  "schemaItems": [
    {
      "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchemaItem",
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





