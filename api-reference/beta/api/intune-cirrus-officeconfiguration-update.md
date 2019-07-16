---
title: 更新 officeConfiguration
description: 更新 officeConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e452a3743148b4767c1259d68746924d3b0675c4
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35725882"
---
# <a name="update-officeconfiguration"></a><span data-ttu-id="d7a0e-103">更新 officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="d7a0e-103">Update officeConfiguration</span></span>

> <span data-ttu-id="d7a0e-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d7a0e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d7a0e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d7a0e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7a0e-106">更新[officeConfiguration](../resources/intune-cirrus-officeconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d7a0e-106">Update the properties of a [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d7a0e-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="d7a0e-107">Prerequisites</span></span>
<span data-ttu-id="d7a0e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d7a0e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7a0e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d7a0e-110">Permission type</span></span>|<span data-ttu-id="d7a0e-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d7a0e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d7a0e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d7a0e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d7a0e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7a0e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d7a0e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d7a0e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d7a0e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d7a0e-115">Not supported.</span></span>|
|<span data-ttu-id="d7a0e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d7a0e-116">Application</span></span>|<span data-ttu-id="d7a0e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d7a0e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d7a0e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d7a0e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /officeConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="d7a0e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d7a0e-119">Request headers</span></span>
|<span data-ttu-id="d7a0e-120">标头</span><span class="sxs-lookup"><span data-stu-id="d7a0e-120">Header</span></span>|<span data-ttu-id="d7a0e-121">值</span><span class="sxs-lookup"><span data-stu-id="d7a0e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d7a0e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7a0e-122">Authorization</span></span>|<span data-ttu-id="d7a0e-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d7a0e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d7a0e-124">接受</span><span class="sxs-lookup"><span data-stu-id="d7a0e-124">Accept</span></span>|<span data-ttu-id="d7a0e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d7a0e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7a0e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d7a0e-126">Request body</span></span>
<span data-ttu-id="d7a0e-127">在请求正文中, 提供[officeConfiguration](../resources/intune-cirrus-officeconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d7a0e-127">In the request body, supply a JSON representation for the [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>

<span data-ttu-id="d7a0e-128">下表显示创建[officeConfiguration](../resources/intune-cirrus-officeconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d7a0e-128">The following table shows the properties that are required when you create the [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md).</span></span>

|<span data-ttu-id="d7a0e-129">属性</span><span class="sxs-lookup"><span data-stu-id="d7a0e-129">Property</span></span>|<span data-ttu-id="d7a0e-130">类型</span><span class="sxs-lookup"><span data-stu-id="d7a0e-130">Type</span></span>|<span data-ttu-id="d7a0e-131">说明</span><span class="sxs-lookup"><span data-stu-id="d7a0e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7a0e-132">id</span><span class="sxs-lookup"><span data-stu-id="d7a0e-132">id</span></span>|<span data-ttu-id="d7a0e-133">String</span><span class="sxs-lookup"><span data-stu-id="d7a0e-133">String</span></span>|<span data-ttu-id="d7a0e-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d7a0e-134">Not yet documented</span></span>|
|<span data-ttu-id="d7a0e-135">tenantCheckinStatuses</span><span class="sxs-lookup"><span data-stu-id="d7a0e-135">tenantCheckinStatuses</span></span>|<span data-ttu-id="d7a0e-136">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)集合</span><span class="sxs-lookup"><span data-stu-id="d7a0e-136">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="d7a0e-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d7a0e-137">Not yet documented</span></span>|
|<span data-ttu-id="d7a0e-138">tenantUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="d7a0e-138">tenantUserCheckinSummary</span></span>|[<span data-ttu-id="d7a0e-139">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="d7a0e-139">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="d7a0e-140">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d7a0e-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d7a0e-141">响应</span><span class="sxs-lookup"><span data-stu-id="d7a0e-141">Response</span></span>
<span data-ttu-id="d7a0e-142">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[officeConfiguration](../resources/intune-cirrus-officeconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d7a0e-142">If successful, this method returns a `200 OK` response code and an updated [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7a0e-143">示例</span><span class="sxs-lookup"><span data-stu-id="d7a0e-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="d7a0e-144">请求</span><span class="sxs-lookup"><span data-stu-id="d7a0e-144">Request</span></span>
<span data-ttu-id="d7a0e-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d7a0e-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/officeConfiguration
Content-type: application/json
Content-length: 843

{
  "@odata.type": "#microsoft.graph.officeConfiguration",
  "tenantCheckinStatuses": [
    {
      "@odata.type": "microsoft.graph.officeClientCheckinStatus",
      "userId": "User Id value",
      "userPrincipalName": "User Principal Name value",
      "deviceName": "Device Name value",
      "devicePlatform": "Device Platform value",
      "devicePlatformVersion": "Device Platform Version value",
      "wasSuccessful": true,
      "checkinDateTime": "2016-12-31T23:56:33.9571764-08:00",
      "errorMessage": "Error Message value",
      "appliedPolicies": [
        "Applied Policies value"
      ],
      "lastTaskName": "Last Task Name value"
    }
  ],
  "tenantUserCheckinSummary": {
    "@odata.type": "microsoft.graph.officeUserCheckinSummary",
    "succeededUserCount": 2,
    "failedUserCount": 15
  }
}
```

### <a name="response"></a><span data-ttu-id="d7a0e-146">响应</span><span class="sxs-lookup"><span data-stu-id="d7a0e-146">Response</span></span>
<span data-ttu-id="d7a0e-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d7a0e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 892

{
  "@odata.type": "#microsoft.graph.officeConfiguration",
  "id": "4b5f7085-7085-4b5f-8570-5f4b85705f4b",
  "tenantCheckinStatuses": [
    {
      "@odata.type": "microsoft.graph.officeClientCheckinStatus",
      "userId": "User Id value",
      "userPrincipalName": "User Principal Name value",
      "deviceName": "Device Name value",
      "devicePlatform": "Device Platform value",
      "devicePlatformVersion": "Device Platform Version value",
      "wasSuccessful": true,
      "checkinDateTime": "2016-12-31T23:56:33.9571764-08:00",
      "errorMessage": "Error Message value",
      "appliedPolicies": [
        "Applied Policies value"
      ],
      "lastTaskName": "Last Task Name value"
    }
  ],
  "tenantUserCheckinSummary": {
    "@odata.type": "microsoft.graph.officeUserCheckinSummary",
    "succeededUserCount": 2,
    "failedUserCount": 15
  }
}
```





