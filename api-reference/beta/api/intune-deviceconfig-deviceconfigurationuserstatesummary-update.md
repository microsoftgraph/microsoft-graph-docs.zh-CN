---
title: 更新 deviceConfigurationUserStateSummary
description: 更新 deviceConfigurationUserStateSummary 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b03f366ba494e351e5dab898ec10e259db250521
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31776316"
---
# <a name="update-deviceconfigurationuserstatesummary"></a><span data-ttu-id="4d568-103">更新 deviceConfigurationUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="4d568-103">Update deviceConfigurationUserStateSummary</span></span>

> <span data-ttu-id="4d568-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4d568-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4d568-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4d568-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d568-106">更新[deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4d568-106">Update the properties of a [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4d568-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="4d568-107">Prerequisites</span></span>
<span data-ttu-id="4d568-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4d568-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d568-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4d568-110">Permission type</span></span>|<span data-ttu-id="4d568-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4d568-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d568-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4d568-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4d568-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d568-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4d568-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4d568-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d568-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4d568-115">Not supported.</span></span>|
|<span data-ttu-id="4d568-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4d568-116">Application</span></span>|<span data-ttu-id="4d568-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="4d568-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d568-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4d568-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationUserStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="4d568-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4d568-119">Request headers</span></span>
|<span data-ttu-id="4d568-120">标头</span><span class="sxs-lookup"><span data-stu-id="4d568-120">Header</span></span>|<span data-ttu-id="4d568-121">值</span><span class="sxs-lookup"><span data-stu-id="4d568-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4d568-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d568-122">Authorization</span></span>|<span data-ttu-id="4d568-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4d568-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4d568-124">接受</span><span class="sxs-lookup"><span data-stu-id="4d568-124">Accept</span></span>|<span data-ttu-id="4d568-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4d568-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d568-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4d568-126">Request body</span></span>
<span data-ttu-id="4d568-127">在请求正文中, 提供[deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4d568-127">In the request body, supply a JSON representation for the [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object.</span></span>

<span data-ttu-id="4d568-128">下表显示创建[deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4d568-128">The following table shows the properties that are required when you create the [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md).</span></span>

|<span data-ttu-id="4d568-129">属性</span><span class="sxs-lookup"><span data-stu-id="4d568-129">Property</span></span>|<span data-ttu-id="4d568-130">类型</span><span class="sxs-lookup"><span data-stu-id="4d568-130">Type</span></span>|<span data-ttu-id="4d568-131">说明</span><span class="sxs-lookup"><span data-stu-id="4d568-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d568-132">id</span><span class="sxs-lookup"><span data-stu-id="4d568-132">id</span></span>|<span data-ttu-id="4d568-133">String</span><span class="sxs-lookup"><span data-stu-id="4d568-133">String</span></span>|<span data-ttu-id="4d568-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="4d568-134">Key of the entity.</span></span>|
|<span data-ttu-id="4d568-135">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="4d568-135">unknownUserCount</span></span>|<span data-ttu-id="4d568-136">Int32</span><span class="sxs-lookup"><span data-stu-id="4d568-136">Int32</span></span>|<span data-ttu-id="4d568-137">未知用户的数量</span><span class="sxs-lookup"><span data-stu-id="4d568-137">Number of unknown users</span></span>|
|<span data-ttu-id="4d568-138">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="4d568-138">notApplicableUserCount</span></span>|<span data-ttu-id="4d568-139">Int32</span><span class="sxs-lookup"><span data-stu-id="4d568-139">Int32</span></span>|<span data-ttu-id="4d568-140">不适用的用户数</span><span class="sxs-lookup"><span data-stu-id="4d568-140">Number of not applicable users</span></span>|
|<span data-ttu-id="4d568-141">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="4d568-141">compliantUserCount</span></span>|<span data-ttu-id="4d568-142">Int32</span><span class="sxs-lookup"><span data-stu-id="4d568-142">Int32</span></span>|<span data-ttu-id="4d568-143">合规用户数</span><span class="sxs-lookup"><span data-stu-id="4d568-143">Number of compliant users</span></span>|
|<span data-ttu-id="4d568-144">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="4d568-144">remediatedUserCount</span></span>|<span data-ttu-id="4d568-145">Int32</span><span class="sxs-lookup"><span data-stu-id="4d568-145">Int32</span></span>|<span data-ttu-id="4d568-146">已修正用户的数量</span><span class="sxs-lookup"><span data-stu-id="4d568-146">Number of remediated users</span></span>|
|<span data-ttu-id="4d568-147">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="4d568-147">nonCompliantUserCount</span></span>|<span data-ttu-id="4d568-148">Int32</span><span class="sxs-lookup"><span data-stu-id="4d568-148">Int32</span></span>|<span data-ttu-id="4d568-149">不符合的用户数</span><span class="sxs-lookup"><span data-stu-id="4d568-149">Number of NonCompliant users</span></span>|
|<span data-ttu-id="4d568-150">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="4d568-150">errorUserCount</span></span>|<span data-ttu-id="4d568-151">Int32</span><span class="sxs-lookup"><span data-stu-id="4d568-151">Int32</span></span>|<span data-ttu-id="4d568-152">错误用户数</span><span class="sxs-lookup"><span data-stu-id="4d568-152">Number of error users</span></span>|
|<span data-ttu-id="4d568-153">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="4d568-153">conflictUserCount</span></span>|<span data-ttu-id="4d568-154">Int32</span><span class="sxs-lookup"><span data-stu-id="4d568-154">Int32</span></span>|<span data-ttu-id="4d568-155">冲突用户数</span><span class="sxs-lookup"><span data-stu-id="4d568-155">Number of conflict users</span></span>|



## <a name="response"></a><span data-ttu-id="4d568-156">响应</span><span class="sxs-lookup"><span data-stu-id="4d568-156">Response</span></span>
<span data-ttu-id="4d568-157">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4d568-157">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d568-158">示例</span><span class="sxs-lookup"><span data-stu-id="4d568-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="4d568-159">请求</span><span class="sxs-lookup"><span data-stu-id="4d568-159">Request</span></span>
<span data-ttu-id="4d568-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4d568-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationUserStateSummaries
Content-type: application/json
Content-length: 275

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStateSummary",
  "unknownUserCount": 0,
  "notApplicableUserCount": 6,
  "compliantUserCount": 2,
  "remediatedUserCount": 3,
  "nonCompliantUserCount": 5,
  "errorUserCount": 14,
  "conflictUserCount": 1
}
```

### <a name="response"></a><span data-ttu-id="4d568-161">响应</span><span class="sxs-lookup"><span data-stu-id="4d568-161">Response</span></span>
<span data-ttu-id="4d568-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4d568-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 324

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStateSummary",
  "id": "e8957887-7887-e895-8778-95e8877895e8",
  "unknownUserCount": 0,
  "notApplicableUserCount": 6,
  "compliantUserCount": 2,
  "remediatedUserCount": 3,
  "nonCompliantUserCount": 5,
  "errorUserCount": 14,
  "conflictUserCount": 1
}
```





