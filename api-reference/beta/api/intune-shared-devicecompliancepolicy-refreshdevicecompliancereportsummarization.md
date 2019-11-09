---
title: refreshDeviceComplianceReportSummarization 操作
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f2e2b39afbfd80148a730995e654aed67f4fb136
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/09/2019
ms.locfileid: "38086177"
---
# <a name="refreshdevicecompliancereportsummarization-action"></a><span data-ttu-id="09756-103">refreshDeviceComplianceReportSummarization 操作</span><span class="sxs-lookup"><span data-stu-id="09756-103">refreshDeviceComplianceReportSummarization action</span></span>

> <span data-ttu-id="09756-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="09756-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="09756-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="09756-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09756-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="09756-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="09756-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="09756-107">Prerequisites</span></span>
<span data-ttu-id="09756-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="09756-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09756-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="09756-110">Permission type</span></span>|<span data-ttu-id="09756-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="09756-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="09756-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="09756-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="09756-113">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="09756-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="09756-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="09756-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="09756-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="09756-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="09756-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="09756-116">Not supported.</span></span>|
|<span data-ttu-id="09756-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="09756-117">Application</span></span>||
| <span data-ttu-id="09756-118">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="09756-118">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="09756-119">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="09756-119">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="09756-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="09756-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/refreshDeviceComplianceReportSummarization
```

## <a name="request-headers"></a><span data-ttu-id="09756-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="09756-121">Request headers</span></span>
|<span data-ttu-id="09756-122">标头</span><span class="sxs-lookup"><span data-stu-id="09756-122">Header</span></span>|<span data-ttu-id="09756-123">值</span><span class="sxs-lookup"><span data-stu-id="09756-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="09756-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="09756-124">Authorization</span></span>|<span data-ttu-id="09756-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="09756-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="09756-126">接受</span><span class="sxs-lookup"><span data-stu-id="09756-126">Accept</span></span>|<span data-ttu-id="09756-127">application/json</span><span class="sxs-lookup"><span data-stu-id="09756-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="09756-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="09756-128">Request body</span></span>
<span data-ttu-id="09756-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="09756-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="09756-130">响应</span><span class="sxs-lookup"><span data-stu-id="09756-130">Response</span></span>
<span data-ttu-id="09756-131">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="09756-131">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="09756-132">示例</span><span class="sxs-lookup"><span data-stu-id="09756-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="09756-133">请求</span><span class="sxs-lookup"><span data-stu-id="09756-133">Request</span></span>
<span data-ttu-id="09756-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="09756-134">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/refreshDeviceComplianceReportSummarization
```

### <a name="response"></a><span data-ttu-id="09756-135">响应</span><span class="sxs-lookup"><span data-stu-id="09756-135">Response</span></span>
<span data-ttu-id="09756-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="09756-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```









