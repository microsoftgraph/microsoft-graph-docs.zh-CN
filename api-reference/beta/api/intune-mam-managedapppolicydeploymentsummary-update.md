---
title: 更新 managedAppPolicyDeploymentSummary
description: 更新 managedAppPolicyDeploymentSummary 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ad0701e5d68ed0df525a2eb584caa028e2d9255a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48701730"
---
# <a name="update-managedapppolicydeploymentsummary"></a><span data-ttu-id="51c39-103">更新 managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="51c39-103">Update managedAppPolicyDeploymentSummary</span></span>

<span data-ttu-id="51c39-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51c39-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="51c39-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="51c39-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="51c39-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="51c39-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51c39-107">更新 [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="51c39-107">Update the properties of a [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="51c39-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="51c39-108">Prerequisites</span></span>
<span data-ttu-id="51c39-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="51c39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51c39-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="51c39-111">Permission type</span></span>|<span data-ttu-id="51c39-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="51c39-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51c39-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="51c39-113">Delegated (work or school account)</span></span>|<span data-ttu-id="51c39-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51c39-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="51c39-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="51c39-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51c39-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="51c39-116">Not supported.</span></span>|
|<span data-ttu-id="51c39-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="51c39-117">Application</span></span>|<span data-ttu-id="51c39-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51c39-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="51c39-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="51c39-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
PATCH /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/deploymentSummary
PATCH /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}/deploymentSummary
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/deploymentSummary
```

## <a name="request-headers"></a><span data-ttu-id="51c39-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="51c39-120">Request headers</span></span>
|<span data-ttu-id="51c39-121">标头</span><span class="sxs-lookup"><span data-stu-id="51c39-121">Header</span></span>|<span data-ttu-id="51c39-122">值</span><span class="sxs-lookup"><span data-stu-id="51c39-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51c39-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="51c39-123">Authorization</span></span>|<span data-ttu-id="51c39-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="51c39-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51c39-125">接受</span><span class="sxs-lookup"><span data-stu-id="51c39-125">Accept</span></span>|<span data-ttu-id="51c39-126">application/json</span><span class="sxs-lookup"><span data-stu-id="51c39-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51c39-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="51c39-127">Request body</span></span>
<span data-ttu-id="51c39-128">在请求正文中，提供 [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="51c39-128">In the request body, supply a JSON representation for the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>

<span data-ttu-id="51c39-129">下表显示创建 [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="51c39-129">The following table shows the properties that are required when you create the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span></span>

|<span data-ttu-id="51c39-130">属性</span><span class="sxs-lookup"><span data-stu-id="51c39-130">Property</span></span>|<span data-ttu-id="51c39-131">类型</span><span class="sxs-lookup"><span data-stu-id="51c39-131">Type</span></span>|<span data-ttu-id="51c39-132">说明</span><span class="sxs-lookup"><span data-stu-id="51c39-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51c39-133">displayName</span><span class="sxs-lookup"><span data-stu-id="51c39-133">displayName</span></span>|<span data-ttu-id="51c39-134">String</span><span class="sxs-lookup"><span data-stu-id="51c39-134">String</span></span>|<span data-ttu-id="51c39-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="51c39-135">Not yet documented</span></span>|
|<span data-ttu-id="51c39-136">configurationDeployedUserCount</span><span class="sxs-lookup"><span data-stu-id="51c39-136">configurationDeployedUserCount</span></span>|<span data-ttu-id="51c39-137">Int32</span><span class="sxs-lookup"><span data-stu-id="51c39-137">Int32</span></span>|<span data-ttu-id="51c39-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="51c39-138">Not yet documented</span></span>|
|<span data-ttu-id="51c39-139">lastRefreshTime</span><span class="sxs-lookup"><span data-stu-id="51c39-139">lastRefreshTime</span></span>|<span data-ttu-id="51c39-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51c39-140">DateTimeOffset</span></span>|<span data-ttu-id="51c39-141">尚未记录</span><span class="sxs-lookup"><span data-stu-id="51c39-141">Not yet documented</span></span>|
|<span data-ttu-id="51c39-142">configurationDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="51c39-142">configurationDeploymentSummaryPerApp</span></span>|<span data-ttu-id="51c39-143">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="51c39-143">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md) collection</span></span>|<span data-ttu-id="51c39-144">尚未记录</span><span class="sxs-lookup"><span data-stu-id="51c39-144">Not yet documented</span></span>|
|<span data-ttu-id="51c39-145">id</span><span class="sxs-lookup"><span data-stu-id="51c39-145">id</span></span>|<span data-ttu-id="51c39-146">String</span><span class="sxs-lookup"><span data-stu-id="51c39-146">String</span></span>|<span data-ttu-id="51c39-147">实体的键。</span><span class="sxs-lookup"><span data-stu-id="51c39-147">Key of the entity.</span></span>|
|<span data-ttu-id="51c39-148">version</span><span class="sxs-lookup"><span data-stu-id="51c39-148">version</span></span>|<span data-ttu-id="51c39-149">String</span><span class="sxs-lookup"><span data-stu-id="51c39-149">String</span></span>|<span data-ttu-id="51c39-150">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="51c39-150">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="51c39-151">响应</span><span class="sxs-lookup"><span data-stu-id="51c39-151">Response</span></span>
<span data-ttu-id="51c39-152">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="51c39-152">If successful, this method returns a `200 OK` response code and an updated [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51c39-153">示例</span><span class="sxs-lookup"><span data-stu-id="51c39-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="51c39-154">请求</span><span class="sxs-lookup"><span data-stu-id="51c39-154">Request</span></span>
<span data-ttu-id="51c39-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="51c39-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
Content-type: application/json
Content-length: 588

{
  "@odata.type": "#microsoft.graph.managedAppPolicyDeploymentSummary",
  "displayName": "Display Name value",
  "configurationDeployedUserCount": 14,
  "lastRefreshTime": "2017-01-01T00:01:30.1240368-08:00",
  "configurationDeploymentSummaryPerApp": [
    {
      "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummaryPerApp",
      "mobileAppIdentifier": {
        "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
        "packageId": "Package Id value"
      },
      "configurationAppliedUserCount": 13
    }
  ],
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="51c39-156">响应</span><span class="sxs-lookup"><span data-stu-id="51c39-156">Response</span></span>
<span data-ttu-id="51c39-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="51c39-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 637

{
  "@odata.type": "#microsoft.graph.managedAppPolicyDeploymentSummary",
  "displayName": "Display Name value",
  "configurationDeployedUserCount": 14,
  "lastRefreshTime": "2017-01-01T00:01:30.1240368-08:00",
  "configurationDeploymentSummaryPerApp": [
    {
      "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummaryPerApp",
      "mobileAppIdentifier": {
        "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
        "packageId": "Package Id value"
      },
      "configurationAppliedUserCount": 13
    }
  ],
  "id": "61f2f688-f688-61f2-88f6-f26188f6f261",
  "version": "Version value"
}
```





