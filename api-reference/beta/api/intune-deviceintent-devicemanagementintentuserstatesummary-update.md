---
title: 更新 deviceManagementIntentUserStateSummary
description: 更新 deviceManagementIntentUserStateSummary 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f43e8499b341b30b475ed3ccc9a1954056c6bb21
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43325608"
---
# <a name="update-devicemanagementintentuserstatesummary"></a><span data-ttu-id="d671e-103">更新 deviceManagementIntentUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="d671e-103">Update deviceManagementIntentUserStateSummary</span></span>

<span data-ttu-id="d671e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d671e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d671e-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d671e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d671e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d671e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d671e-107">更新[deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d671e-107">Update the properties of a [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d671e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d671e-108">Prerequisites</span></span>
<span data-ttu-id="d671e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d671e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d671e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d671e-111">Permission type</span></span>|<span data-ttu-id="d671e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d671e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d671e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d671e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d671e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d671e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d671e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d671e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d671e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d671e-116">Not supported.</span></span>|
|<span data-ttu-id="d671e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d671e-117">Application</span></span>|<span data-ttu-id="d671e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d671e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d671e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d671e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="d671e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d671e-120">Request headers</span></span>
|<span data-ttu-id="d671e-121">标头</span><span class="sxs-lookup"><span data-stu-id="d671e-121">Header</span></span>|<span data-ttu-id="d671e-122">值</span><span class="sxs-lookup"><span data-stu-id="d671e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d671e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d671e-123">Authorization</span></span>|<span data-ttu-id="d671e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d671e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d671e-125">接受</span><span class="sxs-lookup"><span data-stu-id="d671e-125">Accept</span></span>|<span data-ttu-id="d671e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d671e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d671e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d671e-127">Request body</span></span>
<span data-ttu-id="d671e-128">在请求正文中，提供[deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d671e-128">In the request body, supply a JSON representation for the [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object.</span></span>

<span data-ttu-id="d671e-129">下表显示创建[deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d671e-129">The following table shows the properties that are required when you create the [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md).</span></span>

|<span data-ttu-id="d671e-130">属性</span><span class="sxs-lookup"><span data-stu-id="d671e-130">Property</span></span>|<span data-ttu-id="d671e-131">类型</span><span class="sxs-lookup"><span data-stu-id="d671e-131">Type</span></span>|<span data-ttu-id="d671e-132">说明</span><span class="sxs-lookup"><span data-stu-id="d671e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d671e-133">id</span><span class="sxs-lookup"><span data-stu-id="d671e-133">id</span></span>|<span data-ttu-id="d671e-134">字符串</span><span class="sxs-lookup"><span data-stu-id="d671e-134">String</span></span>|<span data-ttu-id="d671e-135">ID</span><span class="sxs-lookup"><span data-stu-id="d671e-135">The ID</span></span>|
|<span data-ttu-id="d671e-136">conflictCount</span><span class="sxs-lookup"><span data-stu-id="d671e-136">conflictCount</span></span>|<span data-ttu-id="d671e-137">Int32</span><span class="sxs-lookup"><span data-stu-id="d671e-137">Int32</span></span>|<span data-ttu-id="d671e-138">发生冲突的用户数</span><span class="sxs-lookup"><span data-stu-id="d671e-138">Number of users in conflict</span></span>|
|<span data-ttu-id="d671e-139">errorCount</span><span class="sxs-lookup"><span data-stu-id="d671e-139">errorCount</span></span>|<span data-ttu-id="d671e-140">Int32</span><span class="sxs-lookup"><span data-stu-id="d671e-140">Int32</span></span>|<span data-ttu-id="d671e-141">错误用户数</span><span class="sxs-lookup"><span data-stu-id="d671e-141">Number of error users</span></span>|
|<span data-ttu-id="d671e-142">failedCount</span><span class="sxs-lookup"><span data-stu-id="d671e-142">failedCount</span></span>|<span data-ttu-id="d671e-143">Int32</span><span class="sxs-lookup"><span data-stu-id="d671e-143">Int32</span></span>|<span data-ttu-id="d671e-144">失败的用户数</span><span class="sxs-lookup"><span data-stu-id="d671e-144">Number of failed users</span></span>|
|<span data-ttu-id="d671e-145">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="d671e-145">notApplicableCount</span></span>|<span data-ttu-id="d671e-146">Int32</span><span class="sxs-lookup"><span data-stu-id="d671e-146">Int32</span></span>|<span data-ttu-id="d671e-147">不适用的用户数</span><span class="sxs-lookup"><span data-stu-id="d671e-147">Number of not applicable users</span></span>|
|<span data-ttu-id="d671e-148">successCount</span><span class="sxs-lookup"><span data-stu-id="d671e-148">successCount</span></span>|<span data-ttu-id="d671e-149">Int32</span><span class="sxs-lookup"><span data-stu-id="d671e-149">Int32</span></span>|<span data-ttu-id="d671e-150">成功的用户数</span><span class="sxs-lookup"><span data-stu-id="d671e-150">Number of succeeded users</span></span>|



## <a name="response"></a><span data-ttu-id="d671e-151">响应</span><span class="sxs-lookup"><span data-stu-id="d671e-151">Response</span></span>
<span data-ttu-id="d671e-152">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d671e-152">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d671e-153">示例</span><span class="sxs-lookup"><span data-stu-id="d671e-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="d671e-154">请求</span><span class="sxs-lookup"><span data-stu-id="d671e-154">Request</span></span>
<span data-ttu-id="d671e-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d671e-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d671e-156">响应</span><span class="sxs-lookup"><span data-stu-id="d671e-156">Response</span></span>
<span data-ttu-id="d671e-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d671e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



