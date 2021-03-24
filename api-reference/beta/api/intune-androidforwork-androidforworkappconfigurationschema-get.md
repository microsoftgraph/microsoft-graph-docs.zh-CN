---
title: 获取 androidForWorkAppConfigurationSchema
description: 读取 androidForWorkAppConfigurationSchema 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 356b1efb85f8c17e2d91a36b36a0930b5b124dde
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51141328"
---
# <a name="get-androidforworkappconfigurationschema"></a><span data-ttu-id="a4382-103">获取 androidForWorkAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="a4382-103">Get androidForWorkAppConfigurationSchema</span></span>

<span data-ttu-id="a4382-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4382-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a4382-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a4382-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a4382-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a4382-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4382-107">读取 [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a4382-107">Read properties and relationships of the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a4382-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a4382-108">Prerequisites</span></span>
<span data-ttu-id="a4382-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a4382-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4382-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a4382-111">Permission type</span></span>|<span data-ttu-id="a4382-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a4382-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4382-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a4382-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a4382-114">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4382-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a4382-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a4382-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4382-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a4382-116">Not supported.</span></span>|
|<span data-ttu-id="a4382-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a4382-117">Application</span></span>|<span data-ttu-id="a4382-118">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4382-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4382-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a4382-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidForWorkAppConfigurationSchemas/{androidForWorkAppConfigurationSchemaId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a4382-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a4382-120">Optional query parameters</span></span>
<span data-ttu-id="a4382-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a4382-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a4382-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="a4382-122">Request headers</span></span>
|<span data-ttu-id="a4382-123">标头</span><span class="sxs-lookup"><span data-stu-id="a4382-123">Header</span></span>|<span data-ttu-id="a4382-124">值</span><span class="sxs-lookup"><span data-stu-id="a4382-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4382-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4382-125">Authorization</span></span>|<span data-ttu-id="a4382-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a4382-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4382-127">接受</span><span class="sxs-lookup"><span data-stu-id="a4382-127">Accept</span></span>|<span data-ttu-id="a4382-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a4382-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4382-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="a4382-129">Request body</span></span>
<span data-ttu-id="a4382-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a4382-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a4382-131">响应</span><span class="sxs-lookup"><span data-stu-id="a4382-131">Response</span></span>
<span data-ttu-id="a4382-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a4382-132">If successful, this method returns a `200 OK` response code and [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4382-133">示例</span><span class="sxs-lookup"><span data-stu-id="a4382-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="a4382-134">请求</span><span class="sxs-lookup"><span data-stu-id="a4382-134">Request</span></span>
<span data-ttu-id="a4382-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a4382-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidForWorkAppConfigurationSchemas/{androidForWorkAppConfigurationSchemaId}
```

### <a name="response"></a><span data-ttu-id="a4382-136">响应</span><span class="sxs-lookup"><span data-stu-id="a4382-136">Response</span></span>
<span data-ttu-id="a4382-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a4382-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




