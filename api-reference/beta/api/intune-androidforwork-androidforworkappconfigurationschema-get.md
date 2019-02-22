---
title: 获取 androidForWorkAppConfigurationSchema
description: 读取 androidForWorkAppConfigurationSchema 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3cef7dfe59d5c7b99fa433ac216703425ca551b8
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30171685"
---
# <a name="get-androidforworkappconfigurationschema"></a><span data-ttu-id="50944-103">获取 androidForWorkAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="50944-103">Get androidForWorkAppConfigurationSchema</span></span>

> <span data-ttu-id="50944-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="50944-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50944-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="50944-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50944-106">读取 [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="50944-106">Read properties and relationships of the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="50944-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="50944-107">Prerequisites</span></span>
<span data-ttu-id="50944-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="50944-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="50944-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="50944-110">Permission type</span></span>|<span data-ttu-id="50944-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="50944-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50944-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="50944-112">Delegated (work or school account)</span></span>|<span data-ttu-id="50944-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="50944-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="50944-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="50944-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50944-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="50944-115">Not supported.</span></span>|
|<span data-ttu-id="50944-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="50944-116">Application</span></span>|<span data-ttu-id="50944-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="50944-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="50944-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="50944-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidForWorkAppConfigurationSchemas/{androidForWorkAppConfigurationSchemaId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="50944-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="50944-119">Optional query parameters</span></span>
<span data-ttu-id="50944-120">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="50944-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="50944-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="50944-121">Request headers</span></span>
|<span data-ttu-id="50944-122">标头</span><span class="sxs-lookup"><span data-stu-id="50944-122">Header</span></span>|<span data-ttu-id="50944-123">值</span><span class="sxs-lookup"><span data-stu-id="50944-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50944-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="50944-124">Authorization</span></span>|<span data-ttu-id="50944-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="50944-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50944-126">Accept</span><span class="sxs-lookup"><span data-stu-id="50944-126">Accept</span></span>|<span data-ttu-id="50944-127">application/json</span><span class="sxs-lookup"><span data-stu-id="50944-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50944-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="50944-128">Request body</span></span>
<span data-ttu-id="50944-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="50944-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="50944-130">响应</span><span class="sxs-lookup"><span data-stu-id="50944-130">Response</span></span>
<span data-ttu-id="50944-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="50944-131">If successful, this method returns a `200 OK` response code and [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50944-132">示例</span><span class="sxs-lookup"><span data-stu-id="50944-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="50944-133">请求</span><span class="sxs-lookup"><span data-stu-id="50944-133">Request</span></span>
<span data-ttu-id="50944-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="50944-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidForWorkAppConfigurationSchemas/{androidForWorkAppConfigurationSchemaId}
```

### <a name="response"></a><span data-ttu-id="50944-135">响应</span><span class="sxs-lookup"><span data-stu-id="50944-135">Response</span></span>
<span data-ttu-id="50944-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="50944-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 913

{
  "value": {
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
}
```




