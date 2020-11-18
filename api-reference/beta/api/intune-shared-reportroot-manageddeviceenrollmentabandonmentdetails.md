---
title: managedDeviceEnrollmentAbandonmentDetails 函数
description: 注册 abandonment 详细信息报告的元数据
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d55d2c8bc6b18760b3cbc5327a8e955ddcd89408
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49200602"
---
# <a name="manageddeviceenrollmentabandonmentdetails-function"></a><span data-ttu-id="9b15c-103">managedDeviceEnrollmentAbandonmentDetails 函数</span><span class="sxs-lookup"><span data-stu-id="9b15c-103">managedDeviceEnrollmentAbandonmentDetails function</span></span>

<span data-ttu-id="9b15c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b15c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9b15c-105">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9b15c-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9b15c-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9b15c-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9b15c-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9b15c-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b15c-108">注册 abandonment 详细信息报告的元数据</span><span class="sxs-lookup"><span data-stu-id="9b15c-108">Metadata for Enrollment abandonment details report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9b15c-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="9b15c-109">Prerequisites</span></span>
<span data-ttu-id="9b15c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9b15c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b15c-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="9b15c-112">Permission type</span></span>|<span data-ttu-id="9b15c-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9b15c-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b15c-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9b15c-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="9b15c-115">&nbsp;&nbsp; **Troublshooting**</span><span class="sxs-lookup"><span data-stu-id="9b15c-115">&nbsp; &nbsp; **Troublshooting**</span></span> | <span data-ttu-id="9b15c-116">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="9b15c-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="9b15c-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9b15c-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b15c-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="9b15c-118">Not supported.</span></span>|
|<span data-ttu-id="9b15c-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="9b15c-119">Application</span></span>||
| <span data-ttu-id="9b15c-120">&nbsp;&nbsp; **Troublshooting**</span><span class="sxs-lookup"><span data-stu-id="9b15c-120">&nbsp; &nbsp; **Troublshooting**</span></span> | <span data-ttu-id="9b15c-121">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="9b15c-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b15c-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9b15c-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentAbandonmentDetails
```

## <a name="request-headers"></a><span data-ttu-id="9b15c-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="9b15c-123">Request headers</span></span>
|<span data-ttu-id="9b15c-124">标头</span><span class="sxs-lookup"><span data-stu-id="9b15c-124">Header</span></span>|<span data-ttu-id="9b15c-125">值</span><span class="sxs-lookup"><span data-stu-id="9b15c-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9b15c-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b15c-126">Authorization</span></span>|<span data-ttu-id="9b15c-127">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9b15c-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9b15c-128">接受</span><span class="sxs-lookup"><span data-stu-id="9b15c-128">Accept</span></span>|<span data-ttu-id="9b15c-129">application/json</span><span class="sxs-lookup"><span data-stu-id="9b15c-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b15c-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="9b15c-130">Request body</span></span>
<span data-ttu-id="9b15c-131">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="9b15c-131">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="9b15c-132">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="9b15c-132">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="9b15c-133">属性</span><span class="sxs-lookup"><span data-stu-id="9b15c-133">Property</span></span>|<span data-ttu-id="9b15c-134">类型</span><span class="sxs-lookup"><span data-stu-id="9b15c-134">Type</span></span>|<span data-ttu-id="9b15c-135">说明</span><span class="sxs-lookup"><span data-stu-id="9b15c-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b15c-136">skip</span><span class="sxs-lookup"><span data-stu-id="9b15c-136">skip</span></span>|<span data-ttu-id="9b15c-137">Int32</span><span class="sxs-lookup"><span data-stu-id="9b15c-137">Int32</span></span>|<span data-ttu-id="9b15c-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9b15c-138">Not yet documented</span></span>|
|<span data-ttu-id="9b15c-139">top</span><span class="sxs-lookup"><span data-stu-id="9b15c-139">top</span></span>|<span data-ttu-id="9b15c-140">Int32</span><span class="sxs-lookup"><span data-stu-id="9b15c-140">Int32</span></span>|<span data-ttu-id="9b15c-141">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9b15c-141">Not yet documented</span></span>|
|<span data-ttu-id="9b15c-142">filter</span><span class="sxs-lookup"><span data-stu-id="9b15c-142">filter</span></span>|<span data-ttu-id="9b15c-143">String</span><span class="sxs-lookup"><span data-stu-id="9b15c-143">String</span></span>|<span data-ttu-id="9b15c-144">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9b15c-144">Not yet documented</span></span>|
|<span data-ttu-id="9b15c-145">skipToken</span><span class="sxs-lookup"><span data-stu-id="9b15c-145">skipToken</span></span>|<span data-ttu-id="9b15c-146">String</span><span class="sxs-lookup"><span data-stu-id="9b15c-146">String</span></span>|<span data-ttu-id="9b15c-147">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9b15c-147">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9b15c-148">响应</span><span class="sxs-lookup"><span data-stu-id="9b15c-148">Response</span></span>
<span data-ttu-id="9b15c-149">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 [report](../resources/intune-shared-report.md)。</span><span class="sxs-lookup"><span data-stu-id="9b15c-149">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b15c-150">示例</span><span class="sxs-lookup"><span data-stu-id="9b15c-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="9b15c-151">请求</span><span class="sxs-lookup"><span data-stu-id="9b15c-151">Request</span></span>
<span data-ttu-id="9b15c-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9b15c-152">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentAbandonmentDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="9b15c-153">响应</span><span class="sxs-lookup"><span data-stu-id="9b15c-153">Response</span></span>
<span data-ttu-id="9b15c-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9b15c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 123

{
  "value": {
    "@odata.type": "microsoft.graph.report",
    "content": "<Unknown Primitive Type Edm.Stream>"
  }
}
```












