---
title: 更新 deviceManagementIntentUserStateSummary
description: 更新 deviceManagementIntentUserStateSummary 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1661770f444fe7479d47858ce6e8ad394d3ed98e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507740"
---
# <a name="update-devicemanagementintentuserstatesummary"></a><span data-ttu-id="6d0ff-103">更新 deviceManagementIntentUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="6d0ff-103">Update deviceManagementIntentUserStateSummary</span></span>

> <span data-ttu-id="6d0ff-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6d0ff-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6d0ff-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6d0ff-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d0ff-106">更新[deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6d0ff-106">Update the properties of a [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6d0ff-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="6d0ff-107">Prerequisites</span></span>
<span data-ttu-id="6d0ff-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6d0ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d0ff-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6d0ff-110">Permission type</span></span>|<span data-ttu-id="6d0ff-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6d0ff-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6d0ff-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6d0ff-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6d0ff-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d0ff-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6d0ff-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6d0ff-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6d0ff-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6d0ff-115">Not supported.</span></span>|
|<span data-ttu-id="6d0ff-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6d0ff-116">Application</span></span>|<span data-ttu-id="6d0ff-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="6d0ff-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6d0ff-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6d0ff-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="6d0ff-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6d0ff-119">Request headers</span></span>
|<span data-ttu-id="6d0ff-120">标头</span><span class="sxs-lookup"><span data-stu-id="6d0ff-120">Header</span></span>|<span data-ttu-id="6d0ff-121">值</span><span class="sxs-lookup"><span data-stu-id="6d0ff-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6d0ff-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d0ff-122">Authorization</span></span>|<span data-ttu-id="6d0ff-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6d0ff-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6d0ff-124">接受</span><span class="sxs-lookup"><span data-stu-id="6d0ff-124">Accept</span></span>|<span data-ttu-id="6d0ff-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6d0ff-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d0ff-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6d0ff-126">Request body</span></span>
<span data-ttu-id="6d0ff-127">在请求正文中, 提供[deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6d0ff-127">In the request body, supply a JSON representation for the [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object.</span></span>

<span data-ttu-id="6d0ff-128">下表显示创建[deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6d0ff-128">The following table shows the properties that are required when you create the [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md).</span></span>

|<span data-ttu-id="6d0ff-129">属性</span><span class="sxs-lookup"><span data-stu-id="6d0ff-129">Property</span></span>|<span data-ttu-id="6d0ff-130">类型</span><span class="sxs-lookup"><span data-stu-id="6d0ff-130">Type</span></span>|<span data-ttu-id="6d0ff-131">说明</span><span class="sxs-lookup"><span data-stu-id="6d0ff-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d0ff-132">id</span><span class="sxs-lookup"><span data-stu-id="6d0ff-132">id</span></span>|<span data-ttu-id="6d0ff-133">String</span><span class="sxs-lookup"><span data-stu-id="6d0ff-133">String</span></span>|<span data-ttu-id="6d0ff-134">ID</span><span class="sxs-lookup"><span data-stu-id="6d0ff-134">The ID</span></span>|
|<span data-ttu-id="6d0ff-135">conflictCount</span><span class="sxs-lookup"><span data-stu-id="6d0ff-135">conflictCount</span></span>|<span data-ttu-id="6d0ff-136">Int32</span><span class="sxs-lookup"><span data-stu-id="6d0ff-136">Int32</span></span>|<span data-ttu-id="6d0ff-137">发生冲突的用户数</span><span class="sxs-lookup"><span data-stu-id="6d0ff-137">Number of users in conflict</span></span>|
|<span data-ttu-id="6d0ff-138">errorCount</span><span class="sxs-lookup"><span data-stu-id="6d0ff-138">errorCount</span></span>|<span data-ttu-id="6d0ff-139">Int32</span><span class="sxs-lookup"><span data-stu-id="6d0ff-139">Int32</span></span>|<span data-ttu-id="6d0ff-140">错误用户数</span><span class="sxs-lookup"><span data-stu-id="6d0ff-140">Number of error users</span></span>|
|<span data-ttu-id="6d0ff-141">failedCount</span><span class="sxs-lookup"><span data-stu-id="6d0ff-141">failedCount</span></span>|<span data-ttu-id="6d0ff-142">Int32</span><span class="sxs-lookup"><span data-stu-id="6d0ff-142">Int32</span></span>|<span data-ttu-id="6d0ff-143">失败的用户数</span><span class="sxs-lookup"><span data-stu-id="6d0ff-143">Number of failed users</span></span>|
|<span data-ttu-id="6d0ff-144">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="6d0ff-144">notApplicableCount</span></span>|<span data-ttu-id="6d0ff-145">Int32</span><span class="sxs-lookup"><span data-stu-id="6d0ff-145">Int32</span></span>|<span data-ttu-id="6d0ff-146">不适用的用户数</span><span class="sxs-lookup"><span data-stu-id="6d0ff-146">Number of not applicable users</span></span>|
|<span data-ttu-id="6d0ff-147">successCount</span><span class="sxs-lookup"><span data-stu-id="6d0ff-147">successCount</span></span>|<span data-ttu-id="6d0ff-148">Int32</span><span class="sxs-lookup"><span data-stu-id="6d0ff-148">Int32</span></span>|<span data-ttu-id="6d0ff-149">成功的用户数</span><span class="sxs-lookup"><span data-stu-id="6d0ff-149">Number of succeeded users</span></span>|



## <a name="response"></a><span data-ttu-id="6d0ff-150">响应</span><span class="sxs-lookup"><span data-stu-id="6d0ff-150">Response</span></span>
<span data-ttu-id="6d0ff-151">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6d0ff-151">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d0ff-152">示例</span><span class="sxs-lookup"><span data-stu-id="6d0ff-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="6d0ff-153">请求</span><span class="sxs-lookup"><span data-stu-id="6d0ff-153">Request</span></span>
<span data-ttu-id="6d0ff-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6d0ff-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6d0ff-155">响应</span><span class="sxs-lookup"><span data-stu-id="6d0ff-155">Response</span></span>
<span data-ttu-id="6d0ff-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6d0ff-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





