---
title: getComanagedDevicesSummary 函数
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 10bc2573d2bec17f0faf8532237e7a3ebda03cce
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792378"
---
# <a name="getcomanageddevicessummary-function"></a><span data-ttu-id="525e9-103">getComanagedDevicesSummary 函数</span><span class="sxs-lookup"><span data-stu-id="525e9-103">getComanagedDevicesSummary function</span></span>

<span data-ttu-id="525e9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="525e9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="525e9-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="525e9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="525e9-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="525e9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="525e9-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="525e9-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="525e9-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="525e9-108">Prerequisites</span></span>
<span data-ttu-id="525e9-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="525e9-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="525e9-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="525e9-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="525e9-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="525e9-111">Permission type</span></span>|<span data-ttu-id="525e9-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="525e9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="525e9-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="525e9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="525e9-114">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="525e9-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="525e9-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="525e9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="525e9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="525e9-116">Not supported.</span></span>|
|<span data-ttu-id="525e9-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="525e9-117">Application</span></span>|<span data-ttu-id="525e9-118">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="525e9-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="525e9-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="525e9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getComanagedDevicesSummary
```

## <a name="request-headers"></a><span data-ttu-id="525e9-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="525e9-120">Request headers</span></span>
|<span data-ttu-id="525e9-121">标头</span><span class="sxs-lookup"><span data-stu-id="525e9-121">Header</span></span>|<span data-ttu-id="525e9-122">值</span><span class="sxs-lookup"><span data-stu-id="525e9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="525e9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="525e9-123">Authorization</span></span>|<span data-ttu-id="525e9-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="525e9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="525e9-125">接受</span><span class="sxs-lookup"><span data-stu-id="525e9-125">Accept</span></span>|<span data-ttu-id="525e9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="525e9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="525e9-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="525e9-127">Request body</span></span>
<span data-ttu-id="525e9-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="525e9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="525e9-129">响应</span><span class="sxs-lookup"><span data-stu-id="525e9-129">Response</span></span>
<span data-ttu-id="525e9-130">如果成功，此函数会 `200 OK` 在响应正文中返回响应代码和[comanagedDevicesSummary](../resources/intune-devices-comanageddevicessummary.md) 。</span><span class="sxs-lookup"><span data-stu-id="525e9-130">If successful, this function returns a `200 OK` response code and a [comanagedDevicesSummary](../resources/intune-devices-comanageddevicessummary.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="525e9-131">示例</span><span class="sxs-lookup"><span data-stu-id="525e9-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="525e9-132">请求</span><span class="sxs-lookup"><span data-stu-id="525e9-132">Request</span></span>
<span data-ttu-id="525e9-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="525e9-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getComanagedDevicesSummary
```

### <a name="response"></a><span data-ttu-id="525e9-134">响应</span><span class="sxs-lookup"><span data-stu-id="525e9-134">Response</span></span>
<span data-ttu-id="525e9-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="525e9-135">Here is an example of the response.</span></span> <span data-ttu-id="525e9-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="525e9-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="525e9-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="525e9-137">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 348

{
  "value": {
    "@odata.type": "microsoft.graph.comanagedDevicesSummary",
    "inventoryCount": 14,
    "compliancePolicyCount": 5,
    "resourceAccessCount": 3,
    "configurationSettingsCount": 10,
    "windowsUpdateForBusinessCount": 13,
    "endpointProtectionCount": 7,
    "modernAppsCount": 15,
    "officeAppsCount": 15
  }
}
```



