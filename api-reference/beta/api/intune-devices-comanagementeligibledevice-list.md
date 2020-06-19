---
title: 列出 comanagementEligibleDevices
description: 列出 comanagementEligibleDevice 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2aba5e3294162a6584a0f7b2f133f9fa78f6e80a
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792525"
---
# <a name="list-comanagementeligibledevices"></a><span data-ttu-id="af9ee-103">列出 comanagementEligibleDevices</span><span class="sxs-lookup"><span data-stu-id="af9ee-103">List comanagementEligibleDevices</span></span>

<span data-ttu-id="af9ee-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af9ee-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="af9ee-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="af9ee-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="af9ee-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="af9ee-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af9ee-107">列出[comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="af9ee-107">List properties and relationships of the [comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="af9ee-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="af9ee-108">Prerequisites</span></span>
<span data-ttu-id="af9ee-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="af9ee-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="af9ee-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af9ee-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af9ee-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="af9ee-111">Permission type</span></span>|<span data-ttu-id="af9ee-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="af9ee-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af9ee-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="af9ee-113">Delegated (work or school account)</span></span>|<span data-ttu-id="af9ee-114">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="af9ee-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="af9ee-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="af9ee-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af9ee-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="af9ee-116">Not supported.</span></span>|
|<span data-ttu-id="af9ee-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="af9ee-117">Application</span></span>|<span data-ttu-id="af9ee-118">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="af9ee-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="af9ee-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="af9ee-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/comanagementEligibleDevices
```

## <a name="request-headers"></a><span data-ttu-id="af9ee-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="af9ee-120">Request headers</span></span>
|<span data-ttu-id="af9ee-121">标头</span><span class="sxs-lookup"><span data-stu-id="af9ee-121">Header</span></span>|<span data-ttu-id="af9ee-122">值</span><span class="sxs-lookup"><span data-stu-id="af9ee-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af9ee-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="af9ee-123">Authorization</span></span>|<span data-ttu-id="af9ee-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="af9ee-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="af9ee-125">接受</span><span class="sxs-lookup"><span data-stu-id="af9ee-125">Accept</span></span>|<span data-ttu-id="af9ee-126">application/json</span><span class="sxs-lookup"><span data-stu-id="af9ee-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af9ee-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="af9ee-127">Request body</span></span>
<span data-ttu-id="af9ee-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="af9ee-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="af9ee-129">响应</span><span class="sxs-lookup"><span data-stu-id="af9ee-129">Response</span></span>
<span data-ttu-id="af9ee-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="af9ee-130">If successful, this method returns a `200 OK` response code and a collection of [comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af9ee-131">示例</span><span class="sxs-lookup"><span data-stu-id="af9ee-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="af9ee-132">请求</span><span class="sxs-lookup"><span data-stu-id="af9ee-132">Request</span></span>
<span data-ttu-id="af9ee-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="af9ee-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/comanagementEligibleDevices
```

### <a name="response"></a><span data-ttu-id="af9ee-134">响应</span><span class="sxs-lookup"><span data-stu-id="af9ee-134">Response</span></span>
<span data-ttu-id="af9ee-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="af9ee-135">Here is an example of the response.</span></span> <span data-ttu-id="af9ee-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="af9ee-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="af9ee-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="af9ee-137">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 880

{
  "value": [
    {
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
  ]
}
```



