---
title: 更新 androidForWorkAppConfigurationSchema
description: 更新 androidForWorkAppConfigurationSchema 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f6bcc24b93100cf8aa11bf643ac347af013ff917
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859204"
---
# <a name="update-androidforworkappconfigurationschema"></a><span data-ttu-id="c6f5a-103">更新 androidForWorkAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="c6f5a-103">Update androidForWorkAppConfigurationSchema</span></span>

> <span data-ttu-id="c6f5a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c6f5a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c6f5a-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c6f5a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c6f5a-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c6f5a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c6f5a-107">更新 [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c6f5a-107">Update the properties of a [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c6f5a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c6f5a-108">Prerequisites</span></span>
<span data-ttu-id="c6f5a-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="c6f5a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6f5a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c6f5a-111">Permission type</span></span>|<span data-ttu-id="c6f5a-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c6f5a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c6f5a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c6f5a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c6f5a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6f5a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c6f5a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c6f5a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c6f5a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c6f5a-116">Not supported.</span></span>|
|<span data-ttu-id="c6f5a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c6f5a-117">Application</span></span>|<span data-ttu-id="c6f5a-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="c6f5a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c6f5a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c6f5a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkAppConfigurationSchemas/{androidForWorkAppConfigurationSchemaId}
```

## <a name="request-headers"></a><span data-ttu-id="c6f5a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c6f5a-120">Request headers</span></span>
|<span data-ttu-id="c6f5a-121">标头</span><span class="sxs-lookup"><span data-stu-id="c6f5a-121">Header</span></span>|<span data-ttu-id="c6f5a-122">值</span><span class="sxs-lookup"><span data-stu-id="c6f5a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c6f5a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c6f5a-123">Authorization</span></span>|<span data-ttu-id="c6f5a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c6f5a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c6f5a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c6f5a-125">Accept</span></span>|<span data-ttu-id="c6f5a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c6f5a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6f5a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c6f5a-127">Request body</span></span>
<span data-ttu-id="c6f5a-128">在请求正文中，提供 [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c6f5a-128">In the request body, supply a JSON representation for the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>

<span data-ttu-id="c6f5a-129">下表显示创建 [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c6f5a-129">The following table shows the properties that are required when you create the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span></span>

|<span data-ttu-id="c6f5a-130">属性</span><span class="sxs-lookup"><span data-stu-id="c6f5a-130">Property</span></span>|<span data-ttu-id="c6f5a-131">类型</span><span class="sxs-lookup"><span data-stu-id="c6f5a-131">Type</span></span>|<span data-ttu-id="c6f5a-132">说明</span><span class="sxs-lookup"><span data-stu-id="c6f5a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6f5a-133">id</span><span class="sxs-lookup"><span data-stu-id="c6f5a-133">id</span></span>|<span data-ttu-id="c6f5a-134">String</span><span class="sxs-lookup"><span data-stu-id="c6f5a-134">String</span></span>|<span data-ttu-id="c6f5a-135">架构对应的应用程序的 Android 包名称的实体密钥</span><span class="sxs-lookup"><span data-stu-id="c6f5a-135">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="c6f5a-136">exampleJson</span><span class="sxs-lookup"><span data-stu-id="c6f5a-136">exampleJson</span></span>|<span data-ttu-id="c6f5a-137">Binary</span><span class="sxs-lookup"><span data-stu-id="c6f5a-137">Binary</span></span>|<span data-ttu-id="c6f5a-138">包含符合此架构的示例 JSON 字符串的 UTF8 编码的字节数组，它演示如何设置此应用的配置</span><span class="sxs-lookup"><span data-stu-id="c6f5a-138">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="c6f5a-139">schemaItems</span><span class="sxs-lookup"><span data-stu-id="c6f5a-139">schemaItems</span></span>|<span data-ttu-id="c6f5a-140">[androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c6f5a-140">[androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="c6f5a-141">项集合，每个项表示架构中命名的配置选项</span><span class="sxs-lookup"><span data-stu-id="c6f5a-141">Collection of items each representing a named configuration option in the schema</span></span>|



## <a name="response"></a><span data-ttu-id="c6f5a-142">响应</span><span class="sxs-lookup"><span data-stu-id="c6f5a-142">Response</span></span>
<span data-ttu-id="c6f5a-143">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c6f5a-143">If successful, this method returns a `200 OK` response code and an updated [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6f5a-144">示例</span><span class="sxs-lookup"><span data-stu-id="c6f5a-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="c6f5a-145">请求</span><span class="sxs-lookup"><span data-stu-id="c6f5a-145">Request</span></span>
<span data-ttu-id="c6f5a-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c6f5a-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidForWorkAppConfigurationSchemas/{androidForWorkAppConfigurationSchemaId}
Content-type: application/json
Content-length: 720

{
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

### <a name="response"></a><span data-ttu-id="c6f5a-147">响应</span><span class="sxs-lookup"><span data-stu-id="c6f5a-147">Response</span></span>
<span data-ttu-id="c6f5a-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c6f5a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





