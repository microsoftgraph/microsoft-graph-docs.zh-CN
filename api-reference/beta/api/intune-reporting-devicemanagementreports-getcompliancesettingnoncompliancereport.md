---
title: getComplianceSettingNonComplianceReport 操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f0412c297209e004a99cb43af02955a0f43848fd
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160512"
---
# <a name="getcompliancesettingnoncompliancereport-action"></a><span data-ttu-id="f830f-103">getComplianceSettingNonComplianceReport 操作</span><span class="sxs-lookup"><span data-stu-id="f830f-103">getComplianceSettingNonComplianceReport action</span></span>

<span data-ttu-id="f830f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f830f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f830f-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f830f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f830f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f830f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f830f-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f830f-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f830f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f830f-108">Prerequisites</span></span>
<span data-ttu-id="f830f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f830f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f830f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f830f-111">Permission type</span></span>|<span data-ttu-id="f830f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f830f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f830f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f830f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f830f-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All、DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All、DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="f830f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="f830f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f830f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f830f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f830f-116">Not supported.</span></span>|
|<span data-ttu-id="f830f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f830f-117">Application</span></span>|<span data-ttu-id="f830f-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All、DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All、DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="f830f-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f830f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f830f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/getComplianceSettingNonComplianceReport
```

## <a name="request-headers"></a><span data-ttu-id="f830f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f830f-120">Request headers</span></span>
|<span data-ttu-id="f830f-121">标头</span><span class="sxs-lookup"><span data-stu-id="f830f-121">Header</span></span>|<span data-ttu-id="f830f-122">值</span><span class="sxs-lookup"><span data-stu-id="f830f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f830f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f830f-123">Authorization</span></span>|<span data-ttu-id="f830f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f830f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f830f-125">接受</span><span class="sxs-lookup"><span data-stu-id="f830f-125">Accept</span></span>|<span data-ttu-id="f830f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f830f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f830f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f830f-127">Request body</span></span>
<span data-ttu-id="f830f-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f830f-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="f830f-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="f830f-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f830f-130">属性</span><span class="sxs-lookup"><span data-stu-id="f830f-130">Property</span></span>|<span data-ttu-id="f830f-131">类型</span><span class="sxs-lookup"><span data-stu-id="f830f-131">Type</span></span>|<span data-ttu-id="f830f-132">说明</span><span class="sxs-lookup"><span data-stu-id="f830f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f830f-133">名称</span><span class="sxs-lookup"><span data-stu-id="f830f-133">name</span></span>|<span data-ttu-id="f830f-134">String</span><span class="sxs-lookup"><span data-stu-id="f830f-134">String</span></span>|<span data-ttu-id="f830f-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f830f-135">Not yet documented</span></span>|
|<span data-ttu-id="f830f-136">select</span><span class="sxs-lookup"><span data-stu-id="f830f-136">select</span></span>|<span data-ttu-id="f830f-137">String collection</span><span class="sxs-lookup"><span data-stu-id="f830f-137">String collection</span></span>|<span data-ttu-id="f830f-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f830f-138">Not yet documented</span></span>|
|<span data-ttu-id="f830f-139">search</span><span class="sxs-lookup"><span data-stu-id="f830f-139">search</span></span>|<span data-ttu-id="f830f-140">String</span><span class="sxs-lookup"><span data-stu-id="f830f-140">String</span></span>|<span data-ttu-id="f830f-141">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f830f-141">Not yet documented</span></span>|
|<span data-ttu-id="f830f-142">groupBy</span><span class="sxs-lookup"><span data-stu-id="f830f-142">groupBy</span></span>|<span data-ttu-id="f830f-143">String collection</span><span class="sxs-lookup"><span data-stu-id="f830f-143">String collection</span></span>|<span data-ttu-id="f830f-144">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f830f-144">Not yet documented</span></span>|
|<span data-ttu-id="f830f-145">orderBy</span><span class="sxs-lookup"><span data-stu-id="f830f-145">orderBy</span></span>|<span data-ttu-id="f830f-146">String collection</span><span class="sxs-lookup"><span data-stu-id="f830f-146">String collection</span></span>|<span data-ttu-id="f830f-147">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f830f-147">Not yet documented</span></span>|
|<span data-ttu-id="f830f-148">skip</span><span class="sxs-lookup"><span data-stu-id="f830f-148">skip</span></span>|<span data-ttu-id="f830f-149">Int32</span><span class="sxs-lookup"><span data-stu-id="f830f-149">Int32</span></span>|<span data-ttu-id="f830f-150">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f830f-150">Not yet documented</span></span>|
|<span data-ttu-id="f830f-151">top</span><span class="sxs-lookup"><span data-stu-id="f830f-151">top</span></span>|<span data-ttu-id="f830f-152">Int32</span><span class="sxs-lookup"><span data-stu-id="f830f-152">Int32</span></span>|<span data-ttu-id="f830f-153">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f830f-153">Not yet documented</span></span>|
|<span data-ttu-id="f830f-154">sessionId</span><span class="sxs-lookup"><span data-stu-id="f830f-154">sessionId</span></span>|<span data-ttu-id="f830f-155">String</span><span class="sxs-lookup"><span data-stu-id="f830f-155">String</span></span>|<span data-ttu-id="f830f-156">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f830f-156">Not yet documented</span></span>|
|<span data-ttu-id="f830f-157">filter</span><span class="sxs-lookup"><span data-stu-id="f830f-157">filter</span></span>|<span data-ttu-id="f830f-158">String</span><span class="sxs-lookup"><span data-stu-id="f830f-158">String</span></span>|<span data-ttu-id="f830f-159">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f830f-159">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f830f-160">响应</span><span class="sxs-lookup"><span data-stu-id="f830f-160">Response</span></span>
<span data-ttu-id="f830f-161">如果成功，此操作在响应 `200 OK` 正文中返回响应代码和 Stream。</span><span class="sxs-lookup"><span data-stu-id="f830f-161">If successful, this action returns a `200 OK` response code and a Stream in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f830f-162">示例</span><span class="sxs-lookup"><span data-stu-id="f830f-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="f830f-163">请求</span><span class="sxs-lookup"><span data-stu-id="f830f-163">Request</span></span>
<span data-ttu-id="f830f-164">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f830f-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reports/getComplianceSettingNonComplianceReport

Content-type: application/json
Content-length: 278

{
  "name": "Name value",
  "select": [
    "Select value"
  ],
  "search": "Search value",
  "groupBy": [
    "Group By value"
  ],
  "orderBy": [
    "Order By value"
  ],
  "skip": 4,
  "top": 3,
  "sessionId": "Session Id value",
  "filter": "Filter value"
}
```

### <a name="response"></a><span data-ttu-id="f830f-165">响应</span><span class="sxs-lookup"><span data-stu-id="f830f-165">Response</span></span>
<span data-ttu-id="f830f-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f830f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 111

{
  "value": "Z2V0Q29tcGxpYW5jZVNldHRpbmdOb25Db21wbGlhbmNlUmVwb3J0IEludHVuZSBEb2MgU2FtcGxlIDU0NDgzMTA0NQ=="
}
```




