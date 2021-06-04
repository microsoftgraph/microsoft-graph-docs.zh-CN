---
title: 更新 managedDeviceMobileAppConfigurationUserSummary
description: 更新 managedDeviceMobileAppConfigurationUserSummary 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8ddeb89575dda5b2250f29e75d97b238d362f30c
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754194"
---
# <a name="update-manageddevicemobileappconfigurationusersummary"></a><span data-ttu-id="54b9c-103">更新 managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="54b9c-103">Update managedDeviceMobileAppConfigurationUserSummary</span></span>

<span data-ttu-id="54b9c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54b9c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="54b9c-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="54b9c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54b9c-106">更新 [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="54b9c-106">Update the properties of a [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="54b9c-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="54b9c-107">Prerequisites</span></span>
<span data-ttu-id="54b9c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="54b9c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54b9c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="54b9c-110">Permission type</span></span>|<span data-ttu-id="54b9c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="54b9c-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54b9c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="54b9c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="54b9c-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54b9c-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="54b9c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="54b9c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54b9c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="54b9c-115">Not supported.</span></span>|
|<span data-ttu-id="54b9c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="54b9c-116">Application</span></span>|<span data-ttu-id="54b9c-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54b9c-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="54b9c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="54b9c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="54b9c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="54b9c-119">Request headers</span></span>
|<span data-ttu-id="54b9c-120">标头</span><span class="sxs-lookup"><span data-stu-id="54b9c-120">Header</span></span>|<span data-ttu-id="54b9c-121">值</span><span class="sxs-lookup"><span data-stu-id="54b9c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="54b9c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="54b9c-122">Authorization</span></span>|<span data-ttu-id="54b9c-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="54b9c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="54b9c-124">接受</span><span class="sxs-lookup"><span data-stu-id="54b9c-124">Accept</span></span>|<span data-ttu-id="54b9c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="54b9c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="54b9c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="54b9c-126">Request body</span></span>
<span data-ttu-id="54b9c-127">在请求正文中，提供 [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="54b9c-127">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>

<span data-ttu-id="54b9c-128">下表显示创建 [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="54b9c-128">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span></span>

|<span data-ttu-id="54b9c-129">属性</span><span class="sxs-lookup"><span data-stu-id="54b9c-129">Property</span></span>|<span data-ttu-id="54b9c-130">类型</span><span class="sxs-lookup"><span data-stu-id="54b9c-130">Type</span></span>|<span data-ttu-id="54b9c-131">说明</span><span class="sxs-lookup"><span data-stu-id="54b9c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54b9c-132">id</span><span class="sxs-lookup"><span data-stu-id="54b9c-132">id</span></span>|<span data-ttu-id="54b9c-133">String</span><span class="sxs-lookup"><span data-stu-id="54b9c-133">String</span></span>|<span data-ttu-id="54b9c-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="54b9c-134">Key of the entity.</span></span>|
|<span data-ttu-id="54b9c-135">pendingCount</span><span class="sxs-lookup"><span data-stu-id="54b9c-135">pendingCount</span></span>|<span data-ttu-id="54b9c-136">Int32</span><span class="sxs-lookup"><span data-stu-id="54b9c-136">Int32</span></span>|<span data-ttu-id="54b9c-137">待定用户的数量</span><span class="sxs-lookup"><span data-stu-id="54b9c-137">Number of pending Users</span></span>|
|<span data-ttu-id="54b9c-138">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="54b9c-138">notApplicableCount</span></span>|<span data-ttu-id="54b9c-139">Int32</span><span class="sxs-lookup"><span data-stu-id="54b9c-139">Int32</span></span>|<span data-ttu-id="54b9c-140">不适用用户的数量</span><span class="sxs-lookup"><span data-stu-id="54b9c-140">Number of not applicable users</span></span>|
|<span data-ttu-id="54b9c-141">successCount</span><span class="sxs-lookup"><span data-stu-id="54b9c-141">successCount</span></span>|<span data-ttu-id="54b9c-142">Int32</span><span class="sxs-lookup"><span data-stu-id="54b9c-142">Int32</span></span>|<span data-ttu-id="54b9c-143">成功用户的数量</span><span class="sxs-lookup"><span data-stu-id="54b9c-143">Number of succeeded Users</span></span>|
|<span data-ttu-id="54b9c-144">errorCount</span><span class="sxs-lookup"><span data-stu-id="54b9c-144">errorCount</span></span>|<span data-ttu-id="54b9c-145">Int32</span><span class="sxs-lookup"><span data-stu-id="54b9c-145">Int32</span></span>|<span data-ttu-id="54b9c-146">错误用户的数量</span><span class="sxs-lookup"><span data-stu-id="54b9c-146">Number of error Users</span></span>|
|<span data-ttu-id="54b9c-147">failedCount</span><span class="sxs-lookup"><span data-stu-id="54b9c-147">failedCount</span></span>|<span data-ttu-id="54b9c-148">Int32</span><span class="sxs-lookup"><span data-stu-id="54b9c-148">Int32</span></span>|<span data-ttu-id="54b9c-149">失败用户的数量</span><span class="sxs-lookup"><span data-stu-id="54b9c-149">Number of failed Users</span></span>|
|<span data-ttu-id="54b9c-150">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="54b9c-150">lastUpdateDateTime</span></span>|<span data-ttu-id="54b9c-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54b9c-151">DateTimeOffset</span></span>|<span data-ttu-id="54b9c-152">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="54b9c-152">Last update time</span></span>|
|<span data-ttu-id="54b9c-153">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="54b9c-153">configurationVersion</span></span>|<span data-ttu-id="54b9c-154">Int32</span><span class="sxs-lookup"><span data-stu-id="54b9c-154">Int32</span></span>|<span data-ttu-id="54b9c-155">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="54b9c-155">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="54b9c-156">响应</span><span class="sxs-lookup"><span data-stu-id="54b9c-156">Response</span></span>
<span data-ttu-id="54b9c-157">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="54b9c-157">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54b9c-158">示例</span><span class="sxs-lookup"><span data-stu-id="54b9c-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="54b9c-159">请求</span><span class="sxs-lookup"><span data-stu-id="54b9c-159">Request</span></span>
<span data-ttu-id="54b9c-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="54b9c-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatusSummary
Content-type: application/json
Content-length: 297

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserSummary",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="54b9c-161">响应</span><span class="sxs-lookup"><span data-stu-id="54b9c-161">Response</span></span>
<span data-ttu-id="54b9c-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="54b9c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 346

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserSummary",
  "id": "7b953742-3742-7b95-4237-957b4237957b",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```




