---
title: 更新 managedAppPolicyDeploymentSummary
description: 更新 managedAppPolicyDeploymentSummary 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 92985407748d06a8f68c987fceb3c1fda2c7f643
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51149210"
---
# <a name="update-managedapppolicydeploymentsummary"></a><span data-ttu-id="ecef4-103">更新 managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="ecef4-103">Update managedAppPolicyDeploymentSummary</span></span>

<span data-ttu-id="ecef4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ecef4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ecef4-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ecef4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ecef4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ecef4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ecef4-107">更新 [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ecef4-107">Update the properties of a [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ecef4-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ecef4-108">Prerequisites</span></span>
<span data-ttu-id="ecef4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ecef4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ecef4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ecef4-111">Permission type</span></span>|<span data-ttu-id="ecef4-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ecef4-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ecef4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ecef4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ecef4-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ecef4-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ecef4-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ecef4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ecef4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ecef4-116">Not supported.</span></span>|
|<span data-ttu-id="ecef4-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ecef4-117">Application</span></span>|<span data-ttu-id="ecef4-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ecef4-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ecef4-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ecef4-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="ecef4-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ecef4-120">Request headers</span></span>
|<span data-ttu-id="ecef4-121">标头</span><span class="sxs-lookup"><span data-stu-id="ecef4-121">Header</span></span>|<span data-ttu-id="ecef4-122">值</span><span class="sxs-lookup"><span data-stu-id="ecef4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ecef4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ecef4-123">Authorization</span></span>|<span data-ttu-id="ecef4-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ecef4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ecef4-125">接受</span><span class="sxs-lookup"><span data-stu-id="ecef4-125">Accept</span></span>|<span data-ttu-id="ecef4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ecef4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ecef4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ecef4-127">Request body</span></span>
<span data-ttu-id="ecef4-128">在请求正文中，提供 [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ecef4-128">In the request body, supply a JSON representation for the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>

<span data-ttu-id="ecef4-129">下表显示创建 [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ecef4-129">The following table shows the properties that are required when you create the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span></span>

|<span data-ttu-id="ecef4-130">属性</span><span class="sxs-lookup"><span data-stu-id="ecef4-130">Property</span></span>|<span data-ttu-id="ecef4-131">类型</span><span class="sxs-lookup"><span data-stu-id="ecef4-131">Type</span></span>|<span data-ttu-id="ecef4-132">说明</span><span class="sxs-lookup"><span data-stu-id="ecef4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ecef4-133">displayName</span><span class="sxs-lookup"><span data-stu-id="ecef4-133">displayName</span></span>|<span data-ttu-id="ecef4-134">String</span><span class="sxs-lookup"><span data-stu-id="ecef4-134">String</span></span>|<span data-ttu-id="ecef4-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ecef4-135">Not yet documented</span></span>|
|<span data-ttu-id="ecef4-136">configurationDeployedUserCount</span><span class="sxs-lookup"><span data-stu-id="ecef4-136">configurationDeployedUserCount</span></span>|<span data-ttu-id="ecef4-137">Int32</span><span class="sxs-lookup"><span data-stu-id="ecef4-137">Int32</span></span>|<span data-ttu-id="ecef4-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ecef4-138">Not yet documented</span></span>|
|<span data-ttu-id="ecef4-139">lastRefreshTime</span><span class="sxs-lookup"><span data-stu-id="ecef4-139">lastRefreshTime</span></span>|<span data-ttu-id="ecef4-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ecef4-140">DateTimeOffset</span></span>|<span data-ttu-id="ecef4-141">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ecef4-141">Not yet documented</span></span>|
|<span data-ttu-id="ecef4-142">configurationDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="ecef4-142">configurationDeploymentSummaryPerApp</span></span>|<span data-ttu-id="ecef4-143">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ecef4-143">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md) collection</span></span>|<span data-ttu-id="ecef4-144">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ecef4-144">Not yet documented</span></span>|
|<span data-ttu-id="ecef4-145">id</span><span class="sxs-lookup"><span data-stu-id="ecef4-145">id</span></span>|<span data-ttu-id="ecef4-146">String</span><span class="sxs-lookup"><span data-stu-id="ecef4-146">String</span></span>|<span data-ttu-id="ecef4-147">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ecef4-147">Key of the entity.</span></span>|
|<span data-ttu-id="ecef4-148">version</span><span class="sxs-lookup"><span data-stu-id="ecef4-148">version</span></span>|<span data-ttu-id="ecef4-149">String</span><span class="sxs-lookup"><span data-stu-id="ecef4-149">String</span></span>|<span data-ttu-id="ecef4-150">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="ecef4-150">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="ecef4-151">响应</span><span class="sxs-lookup"><span data-stu-id="ecef4-151">Response</span></span>
<span data-ttu-id="ecef4-152">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ecef4-152">If successful, this method returns a `200 OK` response code and an updated [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ecef4-153">示例</span><span class="sxs-lookup"><span data-stu-id="ecef4-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="ecef4-154">请求</span><span class="sxs-lookup"><span data-stu-id="ecef4-154">Request</span></span>
<span data-ttu-id="ecef4-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ecef4-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
Content-type: application/json
Content-length: 589

{
  "@odata.type": "#microsoft.graph.managedAppPolicyDeploymentSummary",
  "displayName": "Display Name value",
  "configurationDeployedUserCount": 14,
  "lastRefreshTime": "2017-01-01T00:01:30.1240368-08:00",
  "configurationDeploymentSummaryPerApp": [
    {
      "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummaryPerApp",
      "mobileAppIdentifier": {
        "@odata.type": "microsoft.graph.windowsAppIdentifier",
        "windowsAppId": "Windows App Id value"
      },
      "configurationAppliedUserCount": 13
    }
  ],
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="ecef4-156">响应</span><span class="sxs-lookup"><span data-stu-id="ecef4-156">Response</span></span>
<span data-ttu-id="ecef4-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ecef4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 638

{
  "@odata.type": "#microsoft.graph.managedAppPolicyDeploymentSummary",
  "displayName": "Display Name value",
  "configurationDeployedUserCount": 14,
  "lastRefreshTime": "2017-01-01T00:01:30.1240368-08:00",
  "configurationDeploymentSummaryPerApp": [
    {
      "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummaryPerApp",
      "mobileAppIdentifier": {
        "@odata.type": "microsoft.graph.windowsAppIdentifier",
        "windowsAppId": "Windows App Id value"
      },
      "configurationAppliedUserCount": 13
    }
  ],
  "id": "61f2f688-f688-61f2-88f6-f26188f6f261",
  "version": "Version value"
}
```




