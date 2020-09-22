---
title: 更新 androidForWorkAppConfigurationSchema
description: 更新 androidForWorkAppConfigurationSchema 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c5e29e3d061f136c6917e23d56052333b869978a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48001391"
---
# <a name="update-androidforworkappconfigurationschema"></a><span data-ttu-id="6fe47-103">更新 androidForWorkAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="6fe47-103">Update androidForWorkAppConfigurationSchema</span></span>

<span data-ttu-id="6fe47-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6fe47-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6fe47-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6fe47-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6fe47-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6fe47-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6fe47-107">更新 [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6fe47-107">Update the properties of a [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6fe47-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6fe47-108">Prerequisites</span></span>
<span data-ttu-id="6fe47-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6fe47-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6fe47-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6fe47-111">Permission type</span></span>|<span data-ttu-id="6fe47-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6fe47-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6fe47-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6fe47-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6fe47-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fe47-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6fe47-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6fe47-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6fe47-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6fe47-116">Not supported.</span></span>|
|<span data-ttu-id="6fe47-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6fe47-117">Application</span></span>|<span data-ttu-id="6fe47-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fe47-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6fe47-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6fe47-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkAppConfigurationSchemas/{androidForWorkAppConfigurationSchemaId}
```

## <a name="request-headers"></a><span data-ttu-id="6fe47-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6fe47-120">Request headers</span></span>
|<span data-ttu-id="6fe47-121">标头</span><span class="sxs-lookup"><span data-stu-id="6fe47-121">Header</span></span>|<span data-ttu-id="6fe47-122">值</span><span class="sxs-lookup"><span data-stu-id="6fe47-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6fe47-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6fe47-123">Authorization</span></span>|<span data-ttu-id="6fe47-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6fe47-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6fe47-125">接受</span><span class="sxs-lookup"><span data-stu-id="6fe47-125">Accept</span></span>|<span data-ttu-id="6fe47-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6fe47-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6fe47-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6fe47-127">Request body</span></span>
<span data-ttu-id="6fe47-128">在请求正文中，提供 [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6fe47-128">In the request body, supply a JSON representation for the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>

<span data-ttu-id="6fe47-129">下表显示创建 [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6fe47-129">The following table shows the properties that are required when you create the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span></span>

|<span data-ttu-id="6fe47-130">属性</span><span class="sxs-lookup"><span data-stu-id="6fe47-130">Property</span></span>|<span data-ttu-id="6fe47-131">类型</span><span class="sxs-lookup"><span data-stu-id="6fe47-131">Type</span></span>|<span data-ttu-id="6fe47-132">说明</span><span class="sxs-lookup"><span data-stu-id="6fe47-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fe47-133">id</span><span class="sxs-lookup"><span data-stu-id="6fe47-133">id</span></span>|<span data-ttu-id="6fe47-134">String</span><span class="sxs-lookup"><span data-stu-id="6fe47-134">String</span></span>|<span data-ttu-id="6fe47-135">架构对应的应用程序的 Android 包名称的实体密钥</span><span class="sxs-lookup"><span data-stu-id="6fe47-135">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="6fe47-136">exampleJson</span><span class="sxs-lookup"><span data-stu-id="6fe47-136">exampleJson</span></span>|<span data-ttu-id="6fe47-137">Binary</span><span class="sxs-lookup"><span data-stu-id="6fe47-137">Binary</span></span>|<span data-ttu-id="6fe47-138">包含符合此架构的示例 JSON 字符串的 UTF8 编码的字节数组，它演示如何设置此应用的配置</span><span class="sxs-lookup"><span data-stu-id="6fe47-138">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="6fe47-139">schemaItems</span><span class="sxs-lookup"><span data-stu-id="6fe47-139">schemaItems</span></span>|<span data-ttu-id="6fe47-140">[androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6fe47-140">[androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="6fe47-141">项集合，每个项表示架构中命名的配置选项</span><span class="sxs-lookup"><span data-stu-id="6fe47-141">Collection of items each representing a named configuration option in the schema</span></span>|



## <a name="response"></a><span data-ttu-id="6fe47-142">响应</span><span class="sxs-lookup"><span data-stu-id="6fe47-142">Response</span></span>
<span data-ttu-id="6fe47-143">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6fe47-143">If successful, this method returns a `200 OK` response code and an updated [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6fe47-144">示例</span><span class="sxs-lookup"><span data-stu-id="6fe47-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="6fe47-145">请求</span><span class="sxs-lookup"><span data-stu-id="6fe47-145">Request</span></span>
<span data-ttu-id="6fe47-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6fe47-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6fe47-147">响应</span><span class="sxs-lookup"><span data-stu-id="6fe47-147">Response</span></span>
<span data-ttu-id="6fe47-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6fe47-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






