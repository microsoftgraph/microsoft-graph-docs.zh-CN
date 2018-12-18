---
title: managedDeviceEnrollmentAbandonmentDetails 函数
description: 注册放弃的元数据的详细信息报表
author: tfitzmac
ms.openlocfilehash: 187f5389bbea761555f4067081d4e0557f2ce5bd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317953"
---
# <a name="manageddeviceenrollmentabandonmentdetails-function"></a><span data-ttu-id="26941-103">managedDeviceEnrollmentAbandonmentDetails 函数</span><span class="sxs-lookup"><span data-stu-id="26941-103">managedDeviceEnrollmentAbandonmentDetails function</span></span>

> <span data-ttu-id="26941-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="26941-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="26941-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="26941-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="26941-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="26941-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="26941-107">注册放弃的元数据的详细信息报表</span><span class="sxs-lookup"><span data-stu-id="26941-107">Metadata for Enrollment abandonment details report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="26941-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="26941-108">Prerequisites</span></span>
<span data-ttu-id="26941-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="26941-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26941-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="26941-111">Permission type</span></span>|<span data-ttu-id="26941-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="26941-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26941-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="26941-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="26941-114">&nbsp;&nbsp; **故障诊断**</span><span class="sxs-lookup"><span data-stu-id="26941-114">&nbsp; &nbsp; **Troublshooting**</span></span> | <span data-ttu-id="26941-115">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="26941-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="26941-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="26941-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26941-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="26941-117">Not supported.</span></span>|
|<span data-ttu-id="26941-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="26941-118">Application</span></span>|<span data-ttu-id="26941-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="26941-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="26941-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="26941-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentAbandonmentDetails
```

## <a name="request-headers"></a><span data-ttu-id="26941-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="26941-121">Request headers</span></span>
|<span data-ttu-id="26941-122">标头</span><span class="sxs-lookup"><span data-stu-id="26941-122">Header</span></span>|<span data-ttu-id="26941-123">值</span><span class="sxs-lookup"><span data-stu-id="26941-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="26941-124">授权</span><span class="sxs-lookup"><span data-stu-id="26941-124">Authorization</span></span>|<span data-ttu-id="26941-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="26941-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="26941-126">Accept</span><span class="sxs-lookup"><span data-stu-id="26941-126">Accept</span></span>|<span data-ttu-id="26941-127">application/json</span><span class="sxs-lookup"><span data-stu-id="26941-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="26941-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="26941-128">Request body</span></span>
<span data-ttu-id="26941-129">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="26941-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="26941-130">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="26941-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="26941-131">属性</span><span class="sxs-lookup"><span data-stu-id="26941-131">Property</span></span>|<span data-ttu-id="26941-132">类型</span><span class="sxs-lookup"><span data-stu-id="26941-132">Type</span></span>|<span data-ttu-id="26941-133">说明</span><span class="sxs-lookup"><span data-stu-id="26941-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26941-134">skip</span><span class="sxs-lookup"><span data-stu-id="26941-134">skip</span></span>|<span data-ttu-id="26941-135">Int32</span><span class="sxs-lookup"><span data-stu-id="26941-135">Int32</span></span>|<span data-ttu-id="26941-136">尚未记录</span><span class="sxs-lookup"><span data-stu-id="26941-136">Not yet documented</span></span>|
|<span data-ttu-id="26941-137">top</span><span class="sxs-lookup"><span data-stu-id="26941-137">top</span></span>|<span data-ttu-id="26941-138">Int32</span><span class="sxs-lookup"><span data-stu-id="26941-138">Int32</span></span>|<span data-ttu-id="26941-139">尚未记录</span><span class="sxs-lookup"><span data-stu-id="26941-139">Not yet documented</span></span>|
|<span data-ttu-id="26941-140">filter</span><span class="sxs-lookup"><span data-stu-id="26941-140">filter</span></span>|<span data-ttu-id="26941-141">字符串</span><span class="sxs-lookup"><span data-stu-id="26941-141">String</span></span>|<span data-ttu-id="26941-142">尚未记录</span><span class="sxs-lookup"><span data-stu-id="26941-142">Not yet documented</span></span>|
|<span data-ttu-id="26941-143">skipToken</span><span class="sxs-lookup"><span data-stu-id="26941-143">skipToken</span></span>|<span data-ttu-id="26941-144">字符串</span><span class="sxs-lookup"><span data-stu-id="26941-144">String</span></span>|<span data-ttu-id="26941-145">尚未记录</span><span class="sxs-lookup"><span data-stu-id="26941-145">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="26941-146">响应</span><span class="sxs-lookup"><span data-stu-id="26941-146">Response</span></span>
<span data-ttu-id="26941-147">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 [report](../resources/intune-shared-report.md)。</span><span class="sxs-lookup"><span data-stu-id="26941-147">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26941-148">示例</span><span class="sxs-lookup"><span data-stu-id="26941-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="26941-149">请求</span><span class="sxs-lookup"><span data-stu-id="26941-149">Request</span></span>
<span data-ttu-id="26941-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="26941-150">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentAbandonmentDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="26941-151">响应</span><span class="sxs-lookup"><span data-stu-id="26941-151">Response</span></span>
<span data-ttu-id="26941-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="26941-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





