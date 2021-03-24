---
title: 更新 deviceConfigurationUserStateSummary
description: 更新 deviceConfigurationUserStateSummary 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e8458c2f82562454c16dd73e584de5609a6e8393
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51130082"
---
# <a name="update-deviceconfigurationuserstatesummary"></a><span data-ttu-id="64827-103">更新 deviceConfigurationUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="64827-103">Update deviceConfigurationUserStateSummary</span></span>

<span data-ttu-id="64827-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64827-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="64827-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="64827-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64827-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="64827-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64827-107">更新 [deviceConfigurationUserStateSummary 对象](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="64827-107">Update the properties of a [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="64827-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="64827-108">Prerequisites</span></span>
<span data-ttu-id="64827-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="64827-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64827-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="64827-111">Permission type</span></span>|<span data-ttu-id="64827-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="64827-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64827-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="64827-113">Delegated (work or school account)</span></span>|<span data-ttu-id="64827-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64827-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="64827-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="64827-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64827-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="64827-116">Not supported.</span></span>|
|<span data-ttu-id="64827-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="64827-117">Application</span></span>|<span data-ttu-id="64827-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64827-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="64827-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="64827-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationUserStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="64827-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="64827-120">Request headers</span></span>
|<span data-ttu-id="64827-121">标头</span><span class="sxs-lookup"><span data-stu-id="64827-121">Header</span></span>|<span data-ttu-id="64827-122">值</span><span class="sxs-lookup"><span data-stu-id="64827-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64827-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="64827-123">Authorization</span></span>|<span data-ttu-id="64827-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="64827-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64827-125">接受</span><span class="sxs-lookup"><span data-stu-id="64827-125">Accept</span></span>|<span data-ttu-id="64827-126">application/json</span><span class="sxs-lookup"><span data-stu-id="64827-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64827-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="64827-127">Request body</span></span>
<span data-ttu-id="64827-128">在请求正文中，提供 [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="64827-128">In the request body, supply a JSON representation for the [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object.</span></span>

<span data-ttu-id="64827-129">下表显示创建 [deviceConfigurationUserStateSummary 时所需的属性](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)。</span><span class="sxs-lookup"><span data-stu-id="64827-129">The following table shows the properties that are required when you create the [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md).</span></span>

|<span data-ttu-id="64827-130">属性</span><span class="sxs-lookup"><span data-stu-id="64827-130">Property</span></span>|<span data-ttu-id="64827-131">类型</span><span class="sxs-lookup"><span data-stu-id="64827-131">Type</span></span>|<span data-ttu-id="64827-132">说明</span><span class="sxs-lookup"><span data-stu-id="64827-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64827-133">id</span><span class="sxs-lookup"><span data-stu-id="64827-133">id</span></span>|<span data-ttu-id="64827-134">String</span><span class="sxs-lookup"><span data-stu-id="64827-134">String</span></span>|<span data-ttu-id="64827-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="64827-135">Key of the entity.</span></span>|
|<span data-ttu-id="64827-136">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="64827-136">unknownUserCount</span></span>|<span data-ttu-id="64827-137">Int32</span><span class="sxs-lookup"><span data-stu-id="64827-137">Int32</span></span>|<span data-ttu-id="64827-138">未知用户数</span><span class="sxs-lookup"><span data-stu-id="64827-138">Number of unknown users</span></span>|
|<span data-ttu-id="64827-139">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="64827-139">notApplicableUserCount</span></span>|<span data-ttu-id="64827-140">Int32</span><span class="sxs-lookup"><span data-stu-id="64827-140">Int32</span></span>|<span data-ttu-id="64827-141">不适用用户的数量</span><span class="sxs-lookup"><span data-stu-id="64827-141">Number of not applicable users</span></span>|
|<span data-ttu-id="64827-142">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="64827-142">compliantUserCount</span></span>|<span data-ttu-id="64827-143">Int32</span><span class="sxs-lookup"><span data-stu-id="64827-143">Int32</span></span>|<span data-ttu-id="64827-144">兼容用户数</span><span class="sxs-lookup"><span data-stu-id="64827-144">Number of compliant users</span></span>|
|<span data-ttu-id="64827-145">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="64827-145">remediatedUserCount</span></span>|<span data-ttu-id="64827-146">Int32</span><span class="sxs-lookup"><span data-stu-id="64827-146">Int32</span></span>|<span data-ttu-id="64827-147">已修复用户数</span><span class="sxs-lookup"><span data-stu-id="64827-147">Number of remediated users</span></span>|
|<span data-ttu-id="64827-148">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="64827-148">nonCompliantUserCount</span></span>|<span data-ttu-id="64827-149">Int32</span><span class="sxs-lookup"><span data-stu-id="64827-149">Int32</span></span>|<span data-ttu-id="64827-150">不相容用户数</span><span class="sxs-lookup"><span data-stu-id="64827-150">Number of NonCompliant users</span></span>|
|<span data-ttu-id="64827-151">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="64827-151">errorUserCount</span></span>|<span data-ttu-id="64827-152">Int32</span><span class="sxs-lookup"><span data-stu-id="64827-152">Int32</span></span>|<span data-ttu-id="64827-153">错误用户数</span><span class="sxs-lookup"><span data-stu-id="64827-153">Number of error users</span></span>|
|<span data-ttu-id="64827-154">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="64827-154">conflictUserCount</span></span>|<span data-ttu-id="64827-155">Int32</span><span class="sxs-lookup"><span data-stu-id="64827-155">Int32</span></span>|<span data-ttu-id="64827-156">冲突用户数</span><span class="sxs-lookup"><span data-stu-id="64827-156">Number of conflict users</span></span>|



## <a name="response"></a><span data-ttu-id="64827-157">响应</span><span class="sxs-lookup"><span data-stu-id="64827-157">Response</span></span>
<span data-ttu-id="64827-158">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="64827-158">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64827-159">示例</span><span class="sxs-lookup"><span data-stu-id="64827-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="64827-160">请求</span><span class="sxs-lookup"><span data-stu-id="64827-160">Request</span></span>
<span data-ttu-id="64827-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="64827-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="64827-162">响应</span><span class="sxs-lookup"><span data-stu-id="64827-162">Response</span></span>
<span data-ttu-id="64827-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="64827-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




