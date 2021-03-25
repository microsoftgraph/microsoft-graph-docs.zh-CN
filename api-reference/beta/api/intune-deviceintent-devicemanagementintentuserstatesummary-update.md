---
title: 更新 deviceManagementIntentUserStateSummary
description: 更新 deviceManagementIntentUserStateSummary 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 23de4af33eacac6e4eeffe92fff53243fdf63f36
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51150799"
---
# <a name="update-devicemanagementintentuserstatesummary"></a><span data-ttu-id="a40b2-103">更新 deviceManagementIntentUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="a40b2-103">Update deviceManagementIntentUserStateSummary</span></span>

<span data-ttu-id="a40b2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a40b2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a40b2-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a40b2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a40b2-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a40b2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a40b2-107">更新 [deviceManagementIntentUserStateSummary 对象](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="a40b2-107">Update the properties of a [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a40b2-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a40b2-108">Prerequisites</span></span>
<span data-ttu-id="a40b2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a40b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a40b2-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a40b2-111">Permission type</span></span>|<span data-ttu-id="a40b2-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a40b2-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a40b2-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a40b2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a40b2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a40b2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a40b2-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a40b2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a40b2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a40b2-116">Not supported.</span></span>|
|<span data-ttu-id="a40b2-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a40b2-117">Application</span></span>|<span data-ttu-id="a40b2-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a40b2-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a40b2-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a40b2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="a40b2-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a40b2-120">Request headers</span></span>
|<span data-ttu-id="a40b2-121">标头</span><span class="sxs-lookup"><span data-stu-id="a40b2-121">Header</span></span>|<span data-ttu-id="a40b2-122">值</span><span class="sxs-lookup"><span data-stu-id="a40b2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a40b2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a40b2-123">Authorization</span></span>|<span data-ttu-id="a40b2-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a40b2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a40b2-125">接受</span><span class="sxs-lookup"><span data-stu-id="a40b2-125">Accept</span></span>|<span data-ttu-id="a40b2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a40b2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a40b2-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a40b2-127">Request body</span></span>
<span data-ttu-id="a40b2-128">在请求正文中，提供 [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a40b2-128">In the request body, supply a JSON representation for the [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object.</span></span>

<span data-ttu-id="a40b2-129">下表显示创建 [deviceManagementIntentUserStateSummary 时所需的属性](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)。</span><span class="sxs-lookup"><span data-stu-id="a40b2-129">The following table shows the properties that are required when you create the [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md).</span></span>

|<span data-ttu-id="a40b2-130">属性</span><span class="sxs-lookup"><span data-stu-id="a40b2-130">Property</span></span>|<span data-ttu-id="a40b2-131">类型</span><span class="sxs-lookup"><span data-stu-id="a40b2-131">Type</span></span>|<span data-ttu-id="a40b2-132">说明</span><span class="sxs-lookup"><span data-stu-id="a40b2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a40b2-133">id</span><span class="sxs-lookup"><span data-stu-id="a40b2-133">id</span></span>|<span data-ttu-id="a40b2-134">String</span><span class="sxs-lookup"><span data-stu-id="a40b2-134">String</span></span>|<span data-ttu-id="a40b2-135">The ID</span><span class="sxs-lookup"><span data-stu-id="a40b2-135">The ID</span></span>|
|<span data-ttu-id="a40b2-136">conflictCount</span><span class="sxs-lookup"><span data-stu-id="a40b2-136">conflictCount</span></span>|<span data-ttu-id="a40b2-137">Int32</span><span class="sxs-lookup"><span data-stu-id="a40b2-137">Int32</span></span>|<span data-ttu-id="a40b2-138">发生冲突的用户数</span><span class="sxs-lookup"><span data-stu-id="a40b2-138">Number of users in conflict</span></span>|
|<span data-ttu-id="a40b2-139">errorCount</span><span class="sxs-lookup"><span data-stu-id="a40b2-139">errorCount</span></span>|<span data-ttu-id="a40b2-140">Int32</span><span class="sxs-lookup"><span data-stu-id="a40b2-140">Int32</span></span>|<span data-ttu-id="a40b2-141">错误用户数</span><span class="sxs-lookup"><span data-stu-id="a40b2-141">Number of error users</span></span>|
|<span data-ttu-id="a40b2-142">failedCount</span><span class="sxs-lookup"><span data-stu-id="a40b2-142">failedCount</span></span>|<span data-ttu-id="a40b2-143">Int32</span><span class="sxs-lookup"><span data-stu-id="a40b2-143">Int32</span></span>|<span data-ttu-id="a40b2-144">失败用户数</span><span class="sxs-lookup"><span data-stu-id="a40b2-144">Number of failed users</span></span>|
|<span data-ttu-id="a40b2-145">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="a40b2-145">notApplicableCount</span></span>|<span data-ttu-id="a40b2-146">Int32</span><span class="sxs-lookup"><span data-stu-id="a40b2-146">Int32</span></span>|<span data-ttu-id="a40b2-147">不适用用户的数量</span><span class="sxs-lookup"><span data-stu-id="a40b2-147">Number of not applicable users</span></span>|
|<span data-ttu-id="a40b2-148">successCount</span><span class="sxs-lookup"><span data-stu-id="a40b2-148">successCount</span></span>|<span data-ttu-id="a40b2-149">Int32</span><span class="sxs-lookup"><span data-stu-id="a40b2-149">Int32</span></span>|<span data-ttu-id="a40b2-150">成功用户数</span><span class="sxs-lookup"><span data-stu-id="a40b2-150">Number of succeeded users</span></span>|



## <a name="response"></a><span data-ttu-id="a40b2-151">响应</span><span class="sxs-lookup"><span data-stu-id="a40b2-151">Response</span></span>
<span data-ttu-id="a40b2-152">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a40b2-152">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a40b2-153">示例</span><span class="sxs-lookup"><span data-stu-id="a40b2-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="a40b2-154">请求</span><span class="sxs-lookup"><span data-stu-id="a40b2-154">Request</span></span>
<span data-ttu-id="a40b2-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a40b2-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a40b2-156">响应</span><span class="sxs-lookup"><span data-stu-id="a40b2-156">Response</span></span>
<span data-ttu-id="a40b2-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a40b2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




