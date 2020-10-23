---
title: 更新 deviceConfigurationUserStateSummary
description: 更新 deviceConfigurationUserStateSummary 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: aadb068c2511192cc341404a43dc60b957b0210b
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731286"
---
# <a name="update-deviceconfigurationuserstatesummary"></a><span data-ttu-id="9ea2b-103">更新 deviceConfigurationUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="9ea2b-103">Update deviceConfigurationUserStateSummary</span></span>

<span data-ttu-id="9ea2b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ea2b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9ea2b-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9ea2b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9ea2b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9ea2b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ea2b-107">更新 [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9ea2b-107">Update the properties of a [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9ea2b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9ea2b-108">Prerequisites</span></span>
<span data-ttu-id="9ea2b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9ea2b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ea2b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9ea2b-111">Permission type</span></span>|<span data-ttu-id="9ea2b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9ea2b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ea2b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9ea2b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9ea2b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ea2b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9ea2b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9ea2b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ea2b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9ea2b-116">Not supported.</span></span>|
|<span data-ttu-id="9ea2b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9ea2b-117">Application</span></span>|<span data-ttu-id="9ea2b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ea2b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ea2b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9ea2b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationUserStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="9ea2b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9ea2b-120">Request headers</span></span>
|<span data-ttu-id="9ea2b-121">标头</span><span class="sxs-lookup"><span data-stu-id="9ea2b-121">Header</span></span>|<span data-ttu-id="9ea2b-122">值</span><span class="sxs-lookup"><span data-stu-id="9ea2b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9ea2b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ea2b-123">Authorization</span></span>|<span data-ttu-id="9ea2b-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9ea2b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9ea2b-125">接受</span><span class="sxs-lookup"><span data-stu-id="9ea2b-125">Accept</span></span>|<span data-ttu-id="9ea2b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9ea2b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ea2b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9ea2b-127">Request body</span></span>
<span data-ttu-id="9ea2b-128">在请求正文中，提供 [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9ea2b-128">In the request body, supply a JSON representation for the [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object.</span></span>

<span data-ttu-id="9ea2b-129">下表显示创建 [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9ea2b-129">The following table shows the properties that are required when you create the [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md).</span></span>

|<span data-ttu-id="9ea2b-130">属性</span><span class="sxs-lookup"><span data-stu-id="9ea2b-130">Property</span></span>|<span data-ttu-id="9ea2b-131">类型</span><span class="sxs-lookup"><span data-stu-id="9ea2b-131">Type</span></span>|<span data-ttu-id="9ea2b-132">说明</span><span class="sxs-lookup"><span data-stu-id="9ea2b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ea2b-133">id</span><span class="sxs-lookup"><span data-stu-id="9ea2b-133">id</span></span>|<span data-ttu-id="9ea2b-134">String</span><span class="sxs-lookup"><span data-stu-id="9ea2b-134">String</span></span>|<span data-ttu-id="9ea2b-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9ea2b-135">Key of the entity.</span></span>|
|<span data-ttu-id="9ea2b-136">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="9ea2b-136">unknownUserCount</span></span>|<span data-ttu-id="9ea2b-137">Int32</span><span class="sxs-lookup"><span data-stu-id="9ea2b-137">Int32</span></span>|<span data-ttu-id="9ea2b-138">未知用户的数量</span><span class="sxs-lookup"><span data-stu-id="9ea2b-138">Number of unknown users</span></span>|
|<span data-ttu-id="9ea2b-139">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="9ea2b-139">notApplicableUserCount</span></span>|<span data-ttu-id="9ea2b-140">Int32</span><span class="sxs-lookup"><span data-stu-id="9ea2b-140">Int32</span></span>|<span data-ttu-id="9ea2b-141">不适用的用户数</span><span class="sxs-lookup"><span data-stu-id="9ea2b-141">Number of not applicable users</span></span>|
|<span data-ttu-id="9ea2b-142">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="9ea2b-142">compliantUserCount</span></span>|<span data-ttu-id="9ea2b-143">Int32</span><span class="sxs-lookup"><span data-stu-id="9ea2b-143">Int32</span></span>|<span data-ttu-id="9ea2b-144">合规用户数</span><span class="sxs-lookup"><span data-stu-id="9ea2b-144">Number of compliant users</span></span>|
|<span data-ttu-id="9ea2b-145">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="9ea2b-145">remediatedUserCount</span></span>|<span data-ttu-id="9ea2b-146">Int32</span><span class="sxs-lookup"><span data-stu-id="9ea2b-146">Int32</span></span>|<span data-ttu-id="9ea2b-147">已修正用户的数量</span><span class="sxs-lookup"><span data-stu-id="9ea2b-147">Number of remediated users</span></span>|
|<span data-ttu-id="9ea2b-148">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="9ea2b-148">nonCompliantUserCount</span></span>|<span data-ttu-id="9ea2b-149">Int32</span><span class="sxs-lookup"><span data-stu-id="9ea2b-149">Int32</span></span>|<span data-ttu-id="9ea2b-150">不符合的用户数</span><span class="sxs-lookup"><span data-stu-id="9ea2b-150">Number of NonCompliant users</span></span>|
|<span data-ttu-id="9ea2b-151">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="9ea2b-151">errorUserCount</span></span>|<span data-ttu-id="9ea2b-152">Int32</span><span class="sxs-lookup"><span data-stu-id="9ea2b-152">Int32</span></span>|<span data-ttu-id="9ea2b-153">错误用户数</span><span class="sxs-lookup"><span data-stu-id="9ea2b-153">Number of error users</span></span>|
|<span data-ttu-id="9ea2b-154">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="9ea2b-154">conflictUserCount</span></span>|<span data-ttu-id="9ea2b-155">Int32</span><span class="sxs-lookup"><span data-stu-id="9ea2b-155">Int32</span></span>|<span data-ttu-id="9ea2b-156">冲突用户数</span><span class="sxs-lookup"><span data-stu-id="9ea2b-156">Number of conflict users</span></span>|



## <a name="response"></a><span data-ttu-id="9ea2b-157">响应</span><span class="sxs-lookup"><span data-stu-id="9ea2b-157">Response</span></span>
<span data-ttu-id="9ea2b-158">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9ea2b-158">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ea2b-159">示例</span><span class="sxs-lookup"><span data-stu-id="9ea2b-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="9ea2b-160">请求</span><span class="sxs-lookup"><span data-stu-id="9ea2b-160">Request</span></span>
<span data-ttu-id="9ea2b-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9ea2b-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9ea2b-162">响应</span><span class="sxs-lookup"><span data-stu-id="9ea2b-162">Response</span></span>
<span data-ttu-id="9ea2b-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9ea2b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





