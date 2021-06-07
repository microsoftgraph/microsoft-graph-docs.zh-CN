---
title: getConfigurationSettingNonComplianceReport 操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ca0190ee065dedc858edaf85417e280db00e4162
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52748913"
---
# <a name="getconfigurationsettingnoncompliancereport-action"></a><span data-ttu-id="8e022-103">getConfigurationSettingNonComplianceReport 操作</span><span class="sxs-lookup"><span data-stu-id="8e022-103">getConfigurationSettingNonComplianceReport action</span></span>

<span data-ttu-id="8e022-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e022-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8e022-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8e022-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e022-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8e022-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8e022-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="8e022-107">Prerequisites</span></span>
<span data-ttu-id="8e022-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8e022-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e022-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8e022-110">Permission type</span></span>|<span data-ttu-id="8e022-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8e022-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e022-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8e022-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8e022-113">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All、DeviceManagementApps.Read.All、DeviceManagementApps.ReadWrite.All、DeviceManagementManagedDevices.Read.All、DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e022-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8e022-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8e022-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e022-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8e022-115">Not supported.</span></span>|
|<span data-ttu-id="8e022-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8e022-116">Application</span></span>|<span data-ttu-id="8e022-117">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All、DeviceManagementApps.Read.All、DeviceManagementApps.ReadWrite.All、DeviceManagementManagedDevices.Read.All、DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e022-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e022-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8e022-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/getConfigurationSettingNonComplianceReport
```

## <a name="request-headers"></a><span data-ttu-id="8e022-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8e022-119">Request headers</span></span>
|<span data-ttu-id="8e022-120">标头</span><span class="sxs-lookup"><span data-stu-id="8e022-120">Header</span></span>|<span data-ttu-id="8e022-121">值</span><span class="sxs-lookup"><span data-stu-id="8e022-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e022-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e022-122">Authorization</span></span>|<span data-ttu-id="8e022-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8e022-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e022-124">接受</span><span class="sxs-lookup"><span data-stu-id="8e022-124">Accept</span></span>|<span data-ttu-id="8e022-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8e022-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e022-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="8e022-126">Request body</span></span>
<span data-ttu-id="8e022-127">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8e022-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="8e022-128">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="8e022-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="8e022-129">属性</span><span class="sxs-lookup"><span data-stu-id="8e022-129">Property</span></span>|<span data-ttu-id="8e022-130">类型</span><span class="sxs-lookup"><span data-stu-id="8e022-130">Type</span></span>|<span data-ttu-id="8e022-131">说明</span><span class="sxs-lookup"><span data-stu-id="8e022-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e022-132">name</span><span class="sxs-lookup"><span data-stu-id="8e022-132">name</span></span>|<span data-ttu-id="8e022-133">String</span><span class="sxs-lookup"><span data-stu-id="8e022-133">String</span></span>|<span data-ttu-id="8e022-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8e022-134">Not yet documented</span></span>|
|<span data-ttu-id="8e022-135">select</span><span class="sxs-lookup"><span data-stu-id="8e022-135">select</span></span>|<span data-ttu-id="8e022-136">String collection</span><span class="sxs-lookup"><span data-stu-id="8e022-136">String collection</span></span>|<span data-ttu-id="8e022-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8e022-137">Not yet documented</span></span>|
|<span data-ttu-id="8e022-138">search</span><span class="sxs-lookup"><span data-stu-id="8e022-138">search</span></span>|<span data-ttu-id="8e022-139">String</span><span class="sxs-lookup"><span data-stu-id="8e022-139">String</span></span>|<span data-ttu-id="8e022-140">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8e022-140">Not yet documented</span></span>|
|<span data-ttu-id="8e022-141">groupBy</span><span class="sxs-lookup"><span data-stu-id="8e022-141">groupBy</span></span>|<span data-ttu-id="8e022-142">String collection</span><span class="sxs-lookup"><span data-stu-id="8e022-142">String collection</span></span>|<span data-ttu-id="8e022-143">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8e022-143">Not yet documented</span></span>|
|<span data-ttu-id="8e022-144">orderBy</span><span class="sxs-lookup"><span data-stu-id="8e022-144">orderBy</span></span>|<span data-ttu-id="8e022-145">String collection</span><span class="sxs-lookup"><span data-stu-id="8e022-145">String collection</span></span>|<span data-ttu-id="8e022-146">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8e022-146">Not yet documented</span></span>|
|<span data-ttu-id="8e022-147">skip</span><span class="sxs-lookup"><span data-stu-id="8e022-147">skip</span></span>|<span data-ttu-id="8e022-148">Int32</span><span class="sxs-lookup"><span data-stu-id="8e022-148">Int32</span></span>|<span data-ttu-id="8e022-149">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8e022-149">Not yet documented</span></span>|
|<span data-ttu-id="8e022-150">top</span><span class="sxs-lookup"><span data-stu-id="8e022-150">top</span></span>|<span data-ttu-id="8e022-151">Int32</span><span class="sxs-lookup"><span data-stu-id="8e022-151">Int32</span></span>|<span data-ttu-id="8e022-152">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8e022-152">Not yet documented</span></span>|
|<span data-ttu-id="8e022-153">sessionId</span><span class="sxs-lookup"><span data-stu-id="8e022-153">sessionId</span></span>|<span data-ttu-id="8e022-154">String</span><span class="sxs-lookup"><span data-stu-id="8e022-154">String</span></span>|<span data-ttu-id="8e022-155">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8e022-155">Not yet documented</span></span>|
|<span data-ttu-id="8e022-156">filter</span><span class="sxs-lookup"><span data-stu-id="8e022-156">filter</span></span>|<span data-ttu-id="8e022-157">String</span><span class="sxs-lookup"><span data-stu-id="8e022-157">String</span></span>|<span data-ttu-id="8e022-158">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8e022-158">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="8e022-159">响应</span><span class="sxs-lookup"><span data-stu-id="8e022-159">Response</span></span>
<span data-ttu-id="8e022-160">如果成功，此操作在响应 `200 OK` 正文中返回 响应代码和 Stream。</span><span class="sxs-lookup"><span data-stu-id="8e022-160">If successful, this action returns a `200 OK` response code and a Stream in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e022-161">示例</span><span class="sxs-lookup"><span data-stu-id="8e022-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="8e022-162">请求</span><span class="sxs-lookup"><span data-stu-id="8e022-162">Request</span></span>
<span data-ttu-id="8e022-163">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8e022-163">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/reports/getConfigurationSettingNonComplianceReport

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

### <a name="response"></a><span data-ttu-id="8e022-164">响应</span><span class="sxs-lookup"><span data-stu-id="8e022-164">Response</span></span>
<span data-ttu-id="8e022-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8e022-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 115

{
  "value": "Z2V0Q29uZmlndXJhdGlvblNldHRpbmdOb25Db21wbGlhbmNlUmVwb3J0IEludHVuZSBEb2MgU2FtcGxlIDIxMDczMDYzMzQ="
}
```




