---
title: 列出 androidForWorkAppConfigurationSchemas
description: 列出 androidForWorkAppConfigurationSchema 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8e11d11e1e5af7f52eb37e5b1fc6c60181b728d4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32499822"
---
# <a name="list-androidforworkappconfigurationschemas"></a><span data-ttu-id="ba151-103">列出 androidForWorkAppConfigurationSchemas</span><span class="sxs-lookup"><span data-stu-id="ba151-103">List androidForWorkAppConfigurationSchemas</span></span>

> <span data-ttu-id="ba151-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ba151-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba151-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ba151-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba151-106">列出 [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ba151-106">List properties and relationships of the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ba151-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="ba151-107">Prerequisites</span></span>
<span data-ttu-id="ba151-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ba151-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba151-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ba151-110">Permission type</span></span>|<span data-ttu-id="ba151-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ba151-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ba151-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ba151-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ba151-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ba151-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ba151-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ba151-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba151-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ba151-115">Not supported.</span></span>|
|<span data-ttu-id="ba151-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ba151-116">Application</span></span>|<span data-ttu-id="ba151-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ba151-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba151-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ba151-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidForWorkAppConfigurationSchemas
```

## <a name="request-headers"></a><span data-ttu-id="ba151-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ba151-119">Request headers</span></span>
|<span data-ttu-id="ba151-120">标头</span><span class="sxs-lookup"><span data-stu-id="ba151-120">Header</span></span>|<span data-ttu-id="ba151-121">值</span><span class="sxs-lookup"><span data-stu-id="ba151-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ba151-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba151-122">Authorization</span></span>|<span data-ttu-id="ba151-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ba151-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ba151-124">接受</span><span class="sxs-lookup"><span data-stu-id="ba151-124">Accept</span></span>|<span data-ttu-id="ba151-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ba151-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba151-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ba151-126">Request body</span></span>
<span data-ttu-id="ba151-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ba151-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba151-128">响应</span><span class="sxs-lookup"><span data-stu-id="ba151-128">Response</span></span>
<span data-ttu-id="ba151-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ba151-129">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba151-130">示例</span><span class="sxs-lookup"><span data-stu-id="ba151-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="ba151-131">请求</span><span class="sxs-lookup"><span data-stu-id="ba151-131">Request</span></span>
<span data-ttu-id="ba151-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ba151-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidForWorkAppConfigurationSchemas
```

### <a name="response"></a><span data-ttu-id="ba151-133">响应</span><span class="sxs-lookup"><span data-stu-id="ba151-133">Response</span></span>
<span data-ttu-id="ba151-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ba151-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 977

{
  "value": [
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
  ]
}
```





