---
title: 更新 androidForWorkAppConfigurationSchema
description: 更新 androidForWorkAppConfigurationSchema 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dac55baada3bc4e2254aea9b2279588a137ac172
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51141307"
---
# <a name="update-androidforworkappconfigurationschema"></a><span data-ttu-id="525ee-103">更新 androidForWorkAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="525ee-103">Update androidForWorkAppConfigurationSchema</span></span>

<span data-ttu-id="525ee-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="525ee-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="525ee-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="525ee-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="525ee-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="525ee-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="525ee-107">更新 [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="525ee-107">Update the properties of a [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="525ee-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="525ee-108">Prerequisites</span></span>
<span data-ttu-id="525ee-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="525ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="525ee-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="525ee-111">Permission type</span></span>|<span data-ttu-id="525ee-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="525ee-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="525ee-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="525ee-113">Delegated (work or school account)</span></span>|<span data-ttu-id="525ee-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="525ee-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="525ee-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="525ee-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="525ee-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="525ee-116">Not supported.</span></span>|
|<span data-ttu-id="525ee-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="525ee-117">Application</span></span>|<span data-ttu-id="525ee-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="525ee-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="525ee-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="525ee-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkAppConfigurationSchemas/{androidForWorkAppConfigurationSchemaId}
```

## <a name="request-headers"></a><span data-ttu-id="525ee-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="525ee-120">Request headers</span></span>
|<span data-ttu-id="525ee-121">标头</span><span class="sxs-lookup"><span data-stu-id="525ee-121">Header</span></span>|<span data-ttu-id="525ee-122">值</span><span class="sxs-lookup"><span data-stu-id="525ee-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="525ee-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="525ee-123">Authorization</span></span>|<span data-ttu-id="525ee-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="525ee-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="525ee-125">接受</span><span class="sxs-lookup"><span data-stu-id="525ee-125">Accept</span></span>|<span data-ttu-id="525ee-126">application/json</span><span class="sxs-lookup"><span data-stu-id="525ee-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="525ee-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="525ee-127">Request body</span></span>
<span data-ttu-id="525ee-128">在请求正文中，提供 [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="525ee-128">In the request body, supply a JSON representation for the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>

<span data-ttu-id="525ee-129">下表显示创建 [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="525ee-129">The following table shows the properties that are required when you create the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span></span>

|<span data-ttu-id="525ee-130">属性</span><span class="sxs-lookup"><span data-stu-id="525ee-130">Property</span></span>|<span data-ttu-id="525ee-131">类型</span><span class="sxs-lookup"><span data-stu-id="525ee-131">Type</span></span>|<span data-ttu-id="525ee-132">说明</span><span class="sxs-lookup"><span data-stu-id="525ee-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="525ee-133">id</span><span class="sxs-lookup"><span data-stu-id="525ee-133">id</span></span>|<span data-ttu-id="525ee-134">String</span><span class="sxs-lookup"><span data-stu-id="525ee-134">String</span></span>|<span data-ttu-id="525ee-135">架构对应的应用程序的 Android 包名称的实体密钥</span><span class="sxs-lookup"><span data-stu-id="525ee-135">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="525ee-136">exampleJson</span><span class="sxs-lookup"><span data-stu-id="525ee-136">exampleJson</span></span>|<span data-ttu-id="525ee-137">Binary</span><span class="sxs-lookup"><span data-stu-id="525ee-137">Binary</span></span>|<span data-ttu-id="525ee-138">包含符合此架构的示例 JSON 字符串的 UTF8 编码的字节数组，它演示如何设置此应用的配置</span><span class="sxs-lookup"><span data-stu-id="525ee-138">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="525ee-139">schemaItems</span><span class="sxs-lookup"><span data-stu-id="525ee-139">schemaItems</span></span>|<span data-ttu-id="525ee-140">[androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="525ee-140">[androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="525ee-141">项集合，每个项表示架构中命名的配置选项</span><span class="sxs-lookup"><span data-stu-id="525ee-141">Collection of items each representing a named configuration option in the schema</span></span>|



## <a name="response"></a><span data-ttu-id="525ee-142">响应</span><span class="sxs-lookup"><span data-stu-id="525ee-142">Response</span></span>
<span data-ttu-id="525ee-143">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="525ee-143">If successful, this method returns a `200 OK` response code and an updated [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="525ee-144">示例</span><span class="sxs-lookup"><span data-stu-id="525ee-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="525ee-145">请求</span><span class="sxs-lookup"><span data-stu-id="525ee-145">Request</span></span>
<span data-ttu-id="525ee-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="525ee-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="525ee-147">响应</span><span class="sxs-lookup"><span data-stu-id="525ee-147">Response</span></span>
<span data-ttu-id="525ee-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="525ee-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




