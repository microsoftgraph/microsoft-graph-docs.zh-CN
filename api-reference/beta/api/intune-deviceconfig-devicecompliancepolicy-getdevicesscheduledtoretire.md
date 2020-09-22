---
title: getDevicesScheduledToRetire 操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f2dd6e19d93fc9132457c3888cc59a12c9bd1354
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48072704"
---
# <a name="getdevicesscheduledtoretire-action"></a><span data-ttu-id="d6d92-103">getDevicesScheduledToRetire 操作</span><span class="sxs-lookup"><span data-stu-id="d6d92-103">getDevicesScheduledToRetire action</span></span>

<span data-ttu-id="d6d92-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6d92-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d6d92-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d6d92-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6d92-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d6d92-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6d92-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d6d92-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d6d92-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d6d92-108">Prerequisites</span></span>
<span data-ttu-id="d6d92-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d6d92-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6d92-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d6d92-111">Permission type</span></span>|<span data-ttu-id="d6d92-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d6d92-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6d92-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d6d92-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d6d92-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d6d92-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d6d92-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d6d92-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6d92-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d6d92-116">Not supported.</span></span>|
|<span data-ttu-id="d6d92-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d6d92-117">Application</span></span>|<span data-ttu-id="d6d92-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d6d92-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6d92-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d6d92-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/getDevicesScheduledToRetire
```

## <a name="request-headers"></a><span data-ttu-id="d6d92-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d6d92-120">Request headers</span></span>
|<span data-ttu-id="d6d92-121">标头</span><span class="sxs-lookup"><span data-stu-id="d6d92-121">Header</span></span>|<span data-ttu-id="d6d92-122">值</span><span class="sxs-lookup"><span data-stu-id="d6d92-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6d92-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6d92-123">Authorization</span></span>|<span data-ttu-id="d6d92-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d6d92-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6d92-125">接受</span><span class="sxs-lookup"><span data-stu-id="d6d92-125">Accept</span></span>|<span data-ttu-id="d6d92-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d6d92-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6d92-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d6d92-127">Request body</span></span>
<span data-ttu-id="d6d92-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d6d92-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d6d92-129">响应</span><span class="sxs-lookup"><span data-stu-id="d6d92-129">Response</span></span>
<span data-ttu-id="d6d92-130">如果成功，此操作会 `200 OK` 在响应正文中返回响应代码和 [retireScheduledManagedDevice](../resources/intune-deviceconfig-retirescheduledmanageddevice.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="d6d92-130">If successful, this action returns a `200 OK` response code and a [retireScheduledManagedDevice](../resources/intune-deviceconfig-retirescheduledmanageddevice.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6d92-131">示例</span><span class="sxs-lookup"><span data-stu-id="d6d92-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d6d92-132">请求</span><span class="sxs-lookup"><span data-stu-id="d6d92-132">Request</span></span>
<span data-ttu-id="d6d92-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d6d92-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/getDevicesScheduledToRetire
```

### <a name="response"></a><span data-ttu-id="d6d92-134">响应</span><span class="sxs-lookup"><span data-stu-id="d6d92-134">Response</span></span>
<span data-ttu-id="d6d92-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d6d92-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 670

{
  "value": [
    {
      "@odata.type": "microsoft.graph.retireScheduledManagedDevice",
      "id": "Id value",
      "managedDeviceId": "Managed Device Id value",
      "managedDeviceName": "Managed Device Name value",
      "deviceType": "windowsRT",
      "complianceState": "notApplicable",
      "retireAfterDateTime": "2016-12-31T23:57:37.576134-08:00",
      "managementAgent": "mdm",
      "ownerType": "company",
      "deviceCompliancePolicyName": "Device Compliance Policy Name value",
      "deviceCompliancePolicyId": "Device Compliance Policy Id value",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ]
    }
  ]
}
```






