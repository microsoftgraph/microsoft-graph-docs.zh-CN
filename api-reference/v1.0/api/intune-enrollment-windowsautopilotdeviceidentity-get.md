---
title: 获取 windowsAutopilotDeviceIdentity
description: 读取 windowsAutopilotDeviceIdentity 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f8039791e1371d50cf38c69dd6026bfeffc7463e
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752991"
---
# <a name="get-windowsautopilotdeviceidentity"></a><span data-ttu-id="69ad4-103">获取 windowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="69ad4-103">Get windowsAutopilotDeviceIdentity</span></span>

<span data-ttu-id="69ad4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69ad4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="69ad4-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="69ad4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69ad4-106">读取 [windowsAutopilotDeviceIdentity 对象的属性和](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="69ad4-106">Read properties and relationships of the [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="69ad4-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="69ad4-107">Prerequisites</span></span>
<span data-ttu-id="69ad4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="69ad4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69ad4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="69ad4-110">Permission type</span></span>|<span data-ttu-id="69ad4-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="69ad4-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69ad4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="69ad4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="69ad4-113">DeviceManagementServiceConfig.Read.All、DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69ad4-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="69ad4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="69ad4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69ad4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="69ad4-115">Not supported.</span></span>|
|<span data-ttu-id="69ad4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="69ad4-116">Application</span></span>|<span data-ttu-id="69ad4-117">DeviceManagementServiceConfig.Read.All、DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69ad4-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="69ad4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="69ad4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="69ad4-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="69ad4-119">Optional query parameters</span></span>
<span data-ttu-id="69ad4-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="69ad4-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="69ad4-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="69ad4-121">Request headers</span></span>
|<span data-ttu-id="69ad4-122">标头</span><span class="sxs-lookup"><span data-stu-id="69ad4-122">Header</span></span>|<span data-ttu-id="69ad4-123">值</span><span class="sxs-lookup"><span data-stu-id="69ad4-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69ad4-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="69ad4-124">Authorization</span></span>|<span data-ttu-id="69ad4-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="69ad4-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69ad4-126">接受</span><span class="sxs-lookup"><span data-stu-id="69ad4-126">Accept</span></span>|<span data-ttu-id="69ad4-127">application/json</span><span class="sxs-lookup"><span data-stu-id="69ad4-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69ad4-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="69ad4-128">Request body</span></span>
<span data-ttu-id="69ad4-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="69ad4-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="69ad4-130">响应</span><span class="sxs-lookup"><span data-stu-id="69ad4-130">Response</span></span>
<span data-ttu-id="69ad4-131">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="69ad4-131">If successful, this method returns a `200 OK` response code and [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69ad4-132">示例</span><span class="sxs-lookup"><span data-stu-id="69ad4-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="69ad4-133">请求</span><span class="sxs-lookup"><span data-stu-id="69ad4-133">Request</span></span>
<span data-ttu-id="69ad4-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="69ad4-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}
```

### <a name="response"></a><span data-ttu-id="69ad4-135">响应</span><span class="sxs-lookup"><span data-stu-id="69ad4-135">Response</span></span>
<span data-ttu-id="69ad4-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="69ad4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 918

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
    "id": "fac6f0b1-f0b1-fac6-b1f0-c6fab1f0c6fa",
    "groupTag": "Group Tag value",
    "purchaseOrderIdentifier": "Purchase Order Identifier value",
    "serialNumber": "Serial Number value",
    "productKey": "Product Key value",
    "manufacturer": "Manufacturer value",
    "model": "Model value",
    "enrollmentState": "enrolled",
    "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
    "addressableUserName": "Addressable User Name value",
    "userPrincipalName": "User Principal Name value",
    "resourceName": "Resource Name value",
    "skuNumber": "Sku Number value",
    "systemFamily": "System Family value",
    "azureActiveDirectoryDeviceId": "Azure Active Directory Device Id value",
    "managedDeviceId": "Managed Device Id value",
    "displayName": "Display Name value"
  }
}
```




