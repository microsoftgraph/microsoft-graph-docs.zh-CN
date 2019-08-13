---
title: getTargetedUsersAndDevices 操作
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f6fbed2f2dce6da3637b4a4921b84834d04dfb60
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36346035"
---
# <a name="gettargetedusersanddevices-action"></a><span data-ttu-id="38ef3-103">getTargetedUsersAndDevices 操作</span><span class="sxs-lookup"><span data-stu-id="38ef3-103">getTargetedUsersAndDevices action</span></span>

> <span data-ttu-id="38ef3-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="38ef3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="38ef3-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="38ef3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38ef3-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="38ef3-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="38ef3-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="38ef3-107">Prerequisites</span></span>
<span data-ttu-id="38ef3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="38ef3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38ef3-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="38ef3-110">Permission type</span></span>|<span data-ttu-id="38ef3-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="38ef3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38ef3-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="38ef3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="38ef3-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="38ef3-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="38ef3-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="38ef3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38ef3-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="38ef3-115">Not supported.</span></span>|
|<span data-ttu-id="38ef3-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="38ef3-116">Application</span></span>|<span data-ttu-id="38ef3-117">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="38ef3-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="38ef3-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="38ef3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/getTargetedUsersAndDevices
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/getTargetedUsersAndDevices
```

## <a name="request-headers"></a><span data-ttu-id="38ef3-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="38ef3-119">Request headers</span></span>
|<span data-ttu-id="38ef3-120">标头</span><span class="sxs-lookup"><span data-stu-id="38ef3-120">Header</span></span>|<span data-ttu-id="38ef3-121">值</span><span class="sxs-lookup"><span data-stu-id="38ef3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="38ef3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="38ef3-122">Authorization</span></span>|<span data-ttu-id="38ef3-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="38ef3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="38ef3-124">接受</span><span class="sxs-lookup"><span data-stu-id="38ef3-124">Accept</span></span>|<span data-ttu-id="38ef3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="38ef3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="38ef3-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="38ef3-126">Request body</span></span>
<span data-ttu-id="38ef3-127">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="38ef3-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="38ef3-128">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="38ef3-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="38ef3-129">属性</span><span class="sxs-lookup"><span data-stu-id="38ef3-129">Property</span></span>|<span data-ttu-id="38ef3-130">类型</span><span class="sxs-lookup"><span data-stu-id="38ef3-130">Type</span></span>|<span data-ttu-id="38ef3-131">说明</span><span class="sxs-lookup"><span data-stu-id="38ef3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38ef3-132">deviceConfigurationIds</span><span class="sxs-lookup"><span data-stu-id="38ef3-132">deviceConfigurationIds</span></span>|<span data-ttu-id="38ef3-133">String collection</span><span class="sxs-lookup"><span data-stu-id="38ef3-133">String collection</span></span>|<span data-ttu-id="38ef3-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="38ef3-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="38ef3-135">响应</span><span class="sxs-lookup"><span data-stu-id="38ef3-135">Response</span></span>
<span data-ttu-id="38ef3-136">如果成功, 此操作会在`200 OK`响应正文中返回响应代码和[deviceConfigurationTargetedUserAndDevice](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md)集合。</span><span class="sxs-lookup"><span data-stu-id="38ef3-136">If successful, this action returns a `200 OK` response code and a [deviceConfigurationTargetedUserAndDevice](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38ef3-137">示例</span><span class="sxs-lookup"><span data-stu-id="38ef3-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="38ef3-138">请求</span><span class="sxs-lookup"><span data-stu-id="38ef3-138">Request</span></span>
<span data-ttu-id="38ef3-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="38ef3-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/getTargetedUsersAndDevices

Content-type: application/json
Content-length: 78

{
  "deviceConfigurationIds": [
    "Device Configuration Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="38ef3-140">响应</span><span class="sxs-lookup"><span data-stu-id="38ef3-140">Response</span></span>
<span data-ttu-id="38ef3-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="38ef3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 409

{
  "value": [
    {
      "@odata.type": "microsoft.graph.deviceConfigurationTargetedUserAndDevice",
      "deviceId": "Device Id value",
      "deviceName": "Device Name value",
      "userId": "User Id value",
      "userDisplayName": "User Display Name value",
      "userPrincipalName": "User Principal Name value",
      "lastCheckinDateTime": "2017-01-01T00:02:46.0431416-08:00"
    }
  ]
}
```






