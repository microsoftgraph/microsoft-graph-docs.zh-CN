---
title: 更新 managedAppPolicyDeploymentSummary
description: 更新 managedAppPolicyDeploymentSummary 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: af97bda63cbcdf8f5373faa1f064f8f201b8ef36
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756966"
---
# <a name="update-managedapppolicydeploymentsummary"></a><span data-ttu-id="b93a9-103">更新 managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="b93a9-103">Update managedAppPolicyDeploymentSummary</span></span>

<span data-ttu-id="b93a9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b93a9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b93a9-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b93a9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b93a9-106">更新 [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b93a9-106">Update the properties of a [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b93a9-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="b93a9-107">Prerequisites</span></span>
<span data-ttu-id="b93a9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b93a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b93a9-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b93a9-110">Permission type</span></span>|<span data-ttu-id="b93a9-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b93a9-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b93a9-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b93a9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b93a9-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b93a9-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b93a9-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b93a9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b93a9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b93a9-115">Not supported.</span></span>|
|<span data-ttu-id="b93a9-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b93a9-116">Application</span></span>|<span data-ttu-id="b93a9-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b93a9-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b93a9-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b93a9-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="b93a9-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b93a9-119">Request headers</span></span>
|<span data-ttu-id="b93a9-120">标头</span><span class="sxs-lookup"><span data-stu-id="b93a9-120">Header</span></span>|<span data-ttu-id="b93a9-121">值</span><span class="sxs-lookup"><span data-stu-id="b93a9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b93a9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b93a9-122">Authorization</span></span>|<span data-ttu-id="b93a9-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b93a9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b93a9-124">接受</span><span class="sxs-lookup"><span data-stu-id="b93a9-124">Accept</span></span>|<span data-ttu-id="b93a9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b93a9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b93a9-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b93a9-126">Request body</span></span>
<span data-ttu-id="b93a9-127">在请求正文中，提供 [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b93a9-127">In the request body, supply a JSON representation for the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>

<span data-ttu-id="b93a9-128">下表显示创建 [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b93a9-128">The following table shows the properties that are required when you create the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span></span>

|<span data-ttu-id="b93a9-129">属性</span><span class="sxs-lookup"><span data-stu-id="b93a9-129">Property</span></span>|<span data-ttu-id="b93a9-130">类型</span><span class="sxs-lookup"><span data-stu-id="b93a9-130">Type</span></span>|<span data-ttu-id="b93a9-131">说明</span><span class="sxs-lookup"><span data-stu-id="b93a9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b93a9-132">displayName</span><span class="sxs-lookup"><span data-stu-id="b93a9-132">displayName</span></span>|<span data-ttu-id="b93a9-133">String</span><span class="sxs-lookup"><span data-stu-id="b93a9-133">String</span></span>|<span data-ttu-id="b93a9-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b93a9-134">Not yet documented</span></span>|
|<span data-ttu-id="b93a9-135">configurationDeployedUserCount</span><span class="sxs-lookup"><span data-stu-id="b93a9-135">configurationDeployedUserCount</span></span>|<span data-ttu-id="b93a9-136">Int32</span><span class="sxs-lookup"><span data-stu-id="b93a9-136">Int32</span></span>|<span data-ttu-id="b93a9-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b93a9-137">Not yet documented</span></span>|
|<span data-ttu-id="b93a9-138">lastRefreshTime</span><span class="sxs-lookup"><span data-stu-id="b93a9-138">lastRefreshTime</span></span>|<span data-ttu-id="b93a9-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b93a9-139">DateTimeOffset</span></span>|<span data-ttu-id="b93a9-140">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b93a9-140">Not yet documented</span></span>|
|<span data-ttu-id="b93a9-141">configurationDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="b93a9-141">configurationDeploymentSummaryPerApp</span></span>|<span data-ttu-id="b93a9-142">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b93a9-142">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md) collection</span></span>|<span data-ttu-id="b93a9-143">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b93a9-143">Not yet documented</span></span>|
|<span data-ttu-id="b93a9-144">id</span><span class="sxs-lookup"><span data-stu-id="b93a9-144">id</span></span>|<span data-ttu-id="b93a9-145">String</span><span class="sxs-lookup"><span data-stu-id="b93a9-145">String</span></span>|<span data-ttu-id="b93a9-146">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b93a9-146">Key of the entity.</span></span>|
|<span data-ttu-id="b93a9-147">version</span><span class="sxs-lookup"><span data-stu-id="b93a9-147">version</span></span>|<span data-ttu-id="b93a9-148">String</span><span class="sxs-lookup"><span data-stu-id="b93a9-148">String</span></span>|<span data-ttu-id="b93a9-149">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="b93a9-149">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="b93a9-150">响应</span><span class="sxs-lookup"><span data-stu-id="b93a9-150">Response</span></span>
<span data-ttu-id="b93a9-151">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b93a9-151">If successful, this method returns a `200 OK` response code and an updated [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b93a9-152">示例</span><span class="sxs-lookup"><span data-stu-id="b93a9-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="b93a9-153">请求</span><span class="sxs-lookup"><span data-stu-id="b93a9-153">Request</span></span>
<span data-ttu-id="b93a9-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b93a9-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
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

### <a name="response"></a><span data-ttu-id="b93a9-155">响应</span><span class="sxs-lookup"><span data-stu-id="b93a9-155">Response</span></span>
<span data-ttu-id="b93a9-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b93a9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




