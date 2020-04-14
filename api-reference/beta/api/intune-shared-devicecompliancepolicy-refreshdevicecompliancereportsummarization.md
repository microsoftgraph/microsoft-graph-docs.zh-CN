---
title: refreshDeviceComplianceReportSummarization 操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8de8d91ebbc13ffe83bf3873fe3874bf7cfad81e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43390749"
---
# <a name="refreshdevicecompliancereportsummarization-action"></a><span data-ttu-id="dc4cc-103">refreshDeviceComplianceReportSummarization 操作</span><span class="sxs-lookup"><span data-stu-id="dc4cc-103">refreshDeviceComplianceReportSummarization action</span></span>

<span data-ttu-id="dc4cc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc4cc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dc4cc-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="dc4cc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dc4cc-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dc4cc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc4cc-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="dc4cc-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dc4cc-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="dc4cc-108">Prerequisites</span></span>
<span data-ttu-id="dc4cc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dc4cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc4cc-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="dc4cc-111">Permission type</span></span>|<span data-ttu-id="dc4cc-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="dc4cc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc4cc-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dc4cc-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="dc4cc-114">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="dc4cc-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="dc4cc-115">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="dc4cc-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="dc4cc-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dc4cc-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc4cc-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="dc4cc-117">Not supported.</span></span>|
|<span data-ttu-id="dc4cc-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="dc4cc-118">Application</span></span>||
| <span data-ttu-id="dc4cc-119">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="dc4cc-119">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="dc4cc-120">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="dc4cc-120">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc4cc-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dc4cc-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/refreshDeviceComplianceReportSummarization
```

## <a name="request-headers"></a><span data-ttu-id="dc4cc-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="dc4cc-122">Request headers</span></span>
|<span data-ttu-id="dc4cc-123">标头</span><span class="sxs-lookup"><span data-stu-id="dc4cc-123">Header</span></span>|<span data-ttu-id="dc4cc-124">值</span><span class="sxs-lookup"><span data-stu-id="dc4cc-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dc4cc-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="dc4cc-125">Authorization</span></span>|<span data-ttu-id="dc4cc-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="dc4cc-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dc4cc-127">接受</span><span class="sxs-lookup"><span data-stu-id="dc4cc-127">Accept</span></span>|<span data-ttu-id="dc4cc-128">application/json</span><span class="sxs-lookup"><span data-stu-id="dc4cc-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc4cc-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="dc4cc-129">Request body</span></span>
<span data-ttu-id="dc4cc-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="dc4cc-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dc4cc-131">响应</span><span class="sxs-lookup"><span data-stu-id="dc4cc-131">Response</span></span>
<span data-ttu-id="dc4cc-132">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="dc4cc-132">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="dc4cc-133">示例</span><span class="sxs-lookup"><span data-stu-id="dc4cc-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="dc4cc-134">请求</span><span class="sxs-lookup"><span data-stu-id="dc4cc-134">Request</span></span>
<span data-ttu-id="dc4cc-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dc4cc-135">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/refreshDeviceComplianceReportSummarization
```

### <a name="response"></a><span data-ttu-id="dc4cc-136">响应</span><span class="sxs-lookup"><span data-stu-id="dc4cc-136">Response</span></span>
<span data-ttu-id="dc4cc-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dc4cc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






