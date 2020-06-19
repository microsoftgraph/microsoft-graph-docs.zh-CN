---
title: 获取 comanagementEligibleDevice
description: 读取 comanagementEligibleDevice 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d78aafaa045fe61956dda9f41e4d4b728bf05b5f
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792532"
---
# <a name="get-comanagementeligibledevice"></a><span data-ttu-id="56ca9-103">获取 comanagementEligibleDevice</span><span class="sxs-lookup"><span data-stu-id="56ca9-103">Get comanagementEligibleDevice</span></span>

<span data-ttu-id="56ca9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56ca9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="56ca9-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="56ca9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="56ca9-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="56ca9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56ca9-107">读取[comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="56ca9-107">Read properties and relationships of the [comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="56ca9-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="56ca9-108">Prerequisites</span></span>
<span data-ttu-id="56ca9-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="56ca9-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="56ca9-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56ca9-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56ca9-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="56ca9-111">Permission type</span></span>|<span data-ttu-id="56ca9-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="56ca9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56ca9-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="56ca9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="56ca9-114">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="56ca9-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="56ca9-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="56ca9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56ca9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="56ca9-116">Not supported.</span></span>|
|<span data-ttu-id="56ca9-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="56ca9-117">Application</span></span>|<span data-ttu-id="56ca9-118">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="56ca9-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="56ca9-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="56ca9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/comanagementEligibleDevices/{comanagementEligibleDeviceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="56ca9-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="56ca9-120">Optional query parameters</span></span>
<span data-ttu-id="56ca9-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="56ca9-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="56ca9-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="56ca9-122">Request headers</span></span>
|<span data-ttu-id="56ca9-123">标头</span><span class="sxs-lookup"><span data-stu-id="56ca9-123">Header</span></span>|<span data-ttu-id="56ca9-124">值</span><span class="sxs-lookup"><span data-stu-id="56ca9-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="56ca9-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="56ca9-125">Authorization</span></span>|<span data-ttu-id="56ca9-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="56ca9-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="56ca9-127">接受</span><span class="sxs-lookup"><span data-stu-id="56ca9-127">Accept</span></span>|<span data-ttu-id="56ca9-128">application/json</span><span class="sxs-lookup"><span data-stu-id="56ca9-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="56ca9-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="56ca9-129">Request body</span></span>
<span data-ttu-id="56ca9-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="56ca9-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="56ca9-131">响应</span><span class="sxs-lookup"><span data-stu-id="56ca9-131">Response</span></span>
<span data-ttu-id="56ca9-132">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md)对象。</span><span class="sxs-lookup"><span data-stu-id="56ca9-132">If successful, this method returns a `200 OK` response code and [comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56ca9-133">示例</span><span class="sxs-lookup"><span data-stu-id="56ca9-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="56ca9-134">请求</span><span class="sxs-lookup"><span data-stu-id="56ca9-134">Request</span></span>
<span data-ttu-id="56ca9-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="56ca9-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/comanagementEligibleDevices/{comanagementEligibleDeviceId}
```

### <a name="response"></a><span data-ttu-id="56ca9-136">响应</span><span class="sxs-lookup"><span data-stu-id="56ca9-136">Response</span></span>
<span data-ttu-id="56ca9-137">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="56ca9-137">Here is an example of the response.</span></span> <span data-ttu-id="56ca9-138">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="56ca9-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="56ca9-139">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="56ca9-139">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 824

{
  "value": {
    "@odata.type": "#microsoft.graph.comanagementEligibleDevice",
    "id": "ac20683b-683b-ac20-3b68-20ac3b6820ac",
    "deviceName": "Device Name value",
    "deviceType": "windowsRT",
    "clientRegistrationStatus": "registered",
    "ownerType": "company",
    "managementAgents": "mdm",
    "managementState": "retirePending",
    "referenceId": "Reference Id value",
    "mdmStatus": "Mdm Status value",
    "osVersion": "Os Version value",
    "serialNumber": "Serial Number value",
    "manufacturer": "Manufacturer value",
    "model": "Model value",
    "osDescription": "Os Description value",
    "entitySource": 12,
    "userId": "User Id value",
    "upn": "Upn value",
    "userEmail": "User Email value",
    "userName": "User Name value",
    "status": "eligible"
  }
}
```



