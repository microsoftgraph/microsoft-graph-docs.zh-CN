---
title: 更新 deviceManagementIntentUserStateSummary
description: 更新 deviceManagementIntentUserStateSummary 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7eb98c9c77c5bc8cecef7994fd2913111bd913fb
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33915759"
---
# <a name="update-devicemanagementintentuserstatesummary"></a><span data-ttu-id="d8d71-103">更新 deviceManagementIntentUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="d8d71-103">Update deviceManagementIntentUserStateSummary</span></span>

> <span data-ttu-id="d8d71-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d8d71-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d8d71-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d8d71-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8d71-106">更新[deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d8d71-106">Update the properties of a [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d8d71-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="d8d71-107">Prerequisites</span></span>
<span data-ttu-id="d8d71-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d8d71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8d71-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d8d71-110">Permission type</span></span>|<span data-ttu-id="d8d71-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d8d71-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8d71-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d8d71-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d8d71-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8d71-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d8d71-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d8d71-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8d71-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d8d71-115">Not supported.</span></span>|
|<span data-ttu-id="d8d71-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d8d71-116">Application</span></span>|<span data-ttu-id="d8d71-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d8d71-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8d71-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d8d71-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="d8d71-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d8d71-119">Request headers</span></span>
|<span data-ttu-id="d8d71-120">标头</span><span class="sxs-lookup"><span data-stu-id="d8d71-120">Header</span></span>|<span data-ttu-id="d8d71-121">值</span><span class="sxs-lookup"><span data-stu-id="d8d71-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8d71-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8d71-122">Authorization</span></span>|<span data-ttu-id="d8d71-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d8d71-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8d71-124">接受</span><span class="sxs-lookup"><span data-stu-id="d8d71-124">Accept</span></span>|<span data-ttu-id="d8d71-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d8d71-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8d71-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d8d71-126">Request body</span></span>
<span data-ttu-id="d8d71-127">在请求正文中, 提供[deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d8d71-127">In the request body, supply a JSON representation for the [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object.</span></span>

<span data-ttu-id="d8d71-128">下表显示创建[deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d8d71-128">The following table shows the properties that are required when you create the [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md).</span></span>

|<span data-ttu-id="d8d71-129">属性</span><span class="sxs-lookup"><span data-stu-id="d8d71-129">Property</span></span>|<span data-ttu-id="d8d71-130">类型</span><span class="sxs-lookup"><span data-stu-id="d8d71-130">Type</span></span>|<span data-ttu-id="d8d71-131">说明</span><span class="sxs-lookup"><span data-stu-id="d8d71-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8d71-132">id</span><span class="sxs-lookup"><span data-stu-id="d8d71-132">id</span></span>|<span data-ttu-id="d8d71-133">String</span><span class="sxs-lookup"><span data-stu-id="d8d71-133">String</span></span>|<span data-ttu-id="d8d71-134">ID</span><span class="sxs-lookup"><span data-stu-id="d8d71-134">The ID</span></span>|
|<span data-ttu-id="d8d71-135">conflictCount</span><span class="sxs-lookup"><span data-stu-id="d8d71-135">conflictCount</span></span>|<span data-ttu-id="d8d71-136">Int32</span><span class="sxs-lookup"><span data-stu-id="d8d71-136">Int32</span></span>|<span data-ttu-id="d8d71-137">发生冲突的用户数</span><span class="sxs-lookup"><span data-stu-id="d8d71-137">Number of users in conflict</span></span>|
|<span data-ttu-id="d8d71-138">errorCount</span><span class="sxs-lookup"><span data-stu-id="d8d71-138">errorCount</span></span>|<span data-ttu-id="d8d71-139">Int32</span><span class="sxs-lookup"><span data-stu-id="d8d71-139">Int32</span></span>|<span data-ttu-id="d8d71-140">错误用户数</span><span class="sxs-lookup"><span data-stu-id="d8d71-140">Number of error users</span></span>|
|<span data-ttu-id="d8d71-141">failedCount</span><span class="sxs-lookup"><span data-stu-id="d8d71-141">failedCount</span></span>|<span data-ttu-id="d8d71-142">Int32</span><span class="sxs-lookup"><span data-stu-id="d8d71-142">Int32</span></span>|<span data-ttu-id="d8d71-143">失败的用户数</span><span class="sxs-lookup"><span data-stu-id="d8d71-143">Number of failed users</span></span>|
|<span data-ttu-id="d8d71-144">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="d8d71-144">notApplicableCount</span></span>|<span data-ttu-id="d8d71-145">Int32</span><span class="sxs-lookup"><span data-stu-id="d8d71-145">Int32</span></span>|<span data-ttu-id="d8d71-146">不适用的用户数</span><span class="sxs-lookup"><span data-stu-id="d8d71-146">Number of not applicable users</span></span>|
|<span data-ttu-id="d8d71-147">successCount</span><span class="sxs-lookup"><span data-stu-id="d8d71-147">successCount</span></span>|<span data-ttu-id="d8d71-148">Int32</span><span class="sxs-lookup"><span data-stu-id="d8d71-148">Int32</span></span>|<span data-ttu-id="d8d71-149">成功的用户数</span><span class="sxs-lookup"><span data-stu-id="d8d71-149">Number of succeeded users</span></span>|



## <a name="response"></a><span data-ttu-id="d8d71-150">响应</span><span class="sxs-lookup"><span data-stu-id="d8d71-150">Response</span></span>
<span data-ttu-id="d8d71-151">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d8d71-151">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8d71-152">示例</span><span class="sxs-lookup"><span data-stu-id="d8d71-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="d8d71-153">请求</span><span class="sxs-lookup"><span data-stu-id="d8d71-153">Request</span></span>
<span data-ttu-id="d8d71-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d8d71-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/userStateSummary
Content-type: application/json
Content-length: 198

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentUserStateSummary",
  "conflictCount": 13,
  "errorCount": 10,
  "failedCount": 11,
  "notApplicableCount": 2,
  "successCount": 12
}
```

### <a name="response"></a><span data-ttu-id="d8d71-155">响应</span><span class="sxs-lookup"><span data-stu-id="d8d71-155">Response</span></span>
<span data-ttu-id="d8d71-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d8d71-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 247

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentUserStateSummary",
  "id": "be567e02-7e02-be56-027e-56be027e56be",
  "conflictCount": 13,
  "errorCount": 10,
  "failedCount": 11,
  "notApplicableCount": 2,
  "successCount": 12
}
```




