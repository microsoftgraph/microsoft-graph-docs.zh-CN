---
title: 更新 managedAppPolicyDeploymentSummary
description: 更新 managedAppPolicyDeploymentSummary 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: feb753b0c881a3d5e4a91f181eba9174d1765020
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36018230"
---
# <a name="update-managedapppolicydeploymentsummary"></a><span data-ttu-id="29350-103">更新 managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="29350-103">Update managedAppPolicyDeploymentSummary</span></span>

> <span data-ttu-id="29350-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="29350-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29350-105">更新 [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="29350-105">Update the properties of a [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="29350-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="29350-106">Prerequisites</span></span>
<span data-ttu-id="29350-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="29350-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29350-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="29350-109">Permission type</span></span>|<span data-ttu-id="29350-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="29350-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="29350-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="29350-111">Delegated (work or school account)</span></span>|<span data-ttu-id="29350-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29350-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="29350-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="29350-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29350-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="29350-114">Not supported.</span></span>|
|<span data-ttu-id="29350-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="29350-115">Application</span></span>|<span data-ttu-id="29350-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="29350-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="29350-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="29350-117">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="29350-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="29350-118">Request headers</span></span>
|<span data-ttu-id="29350-119">标头</span><span class="sxs-lookup"><span data-stu-id="29350-119">Header</span></span>|<span data-ttu-id="29350-120">值</span><span class="sxs-lookup"><span data-stu-id="29350-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="29350-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="29350-121">Authorization</span></span>|<span data-ttu-id="29350-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="29350-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="29350-123">接受</span><span class="sxs-lookup"><span data-stu-id="29350-123">Accept</span></span>|<span data-ttu-id="29350-124">application/json</span><span class="sxs-lookup"><span data-stu-id="29350-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="29350-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="29350-125">Request body</span></span>
<span data-ttu-id="29350-126">在请求正文中，提供 [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="29350-126">In the request body, supply a JSON representation for the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>

<span data-ttu-id="29350-127">下表显示创建 [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="29350-127">The following table shows the properties that are required when you create the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span></span>

|<span data-ttu-id="29350-128">属性</span><span class="sxs-lookup"><span data-stu-id="29350-128">Property</span></span>|<span data-ttu-id="29350-129">类型</span><span class="sxs-lookup"><span data-stu-id="29350-129">Type</span></span>|<span data-ttu-id="29350-130">说明</span><span class="sxs-lookup"><span data-stu-id="29350-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29350-131">displayName</span><span class="sxs-lookup"><span data-stu-id="29350-131">displayName</span></span>|<span data-ttu-id="29350-132">字符串</span><span class="sxs-lookup"><span data-stu-id="29350-132">String</span></span>|<span data-ttu-id="29350-133">尚未记录</span><span class="sxs-lookup"><span data-stu-id="29350-133">Not yet documented</span></span>|
|<span data-ttu-id="29350-134">configurationDeployedUserCount</span><span class="sxs-lookup"><span data-stu-id="29350-134">configurationDeployedUserCount</span></span>|<span data-ttu-id="29350-135">Int32</span><span class="sxs-lookup"><span data-stu-id="29350-135">Int32</span></span>|<span data-ttu-id="29350-136">尚未记录</span><span class="sxs-lookup"><span data-stu-id="29350-136">Not yet documented</span></span>|
|<span data-ttu-id="29350-137">lastRefreshTime</span><span class="sxs-lookup"><span data-stu-id="29350-137">lastRefreshTime</span></span>|<span data-ttu-id="29350-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29350-138">DateTimeOffset</span></span>|<span data-ttu-id="29350-139">尚未记录</span><span class="sxs-lookup"><span data-stu-id="29350-139">Not yet documented</span></span>|
|<span data-ttu-id="29350-140">configurationDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="29350-140">configurationDeploymentSummaryPerApp</span></span>|<span data-ttu-id="29350-141">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="29350-141">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md) collection</span></span>|<span data-ttu-id="29350-142">尚未记录</span><span class="sxs-lookup"><span data-stu-id="29350-142">Not yet documented</span></span>|
|<span data-ttu-id="29350-143">id</span><span class="sxs-lookup"><span data-stu-id="29350-143">id</span></span>|<span data-ttu-id="29350-144">String</span><span class="sxs-lookup"><span data-stu-id="29350-144">String</span></span>|<span data-ttu-id="29350-145">实体的键。</span><span class="sxs-lookup"><span data-stu-id="29350-145">Key of the entity.</span></span>|
|<span data-ttu-id="29350-146">version</span><span class="sxs-lookup"><span data-stu-id="29350-146">version</span></span>|<span data-ttu-id="29350-147">String</span><span class="sxs-lookup"><span data-stu-id="29350-147">String</span></span>|<span data-ttu-id="29350-148">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="29350-148">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="29350-149">响应</span><span class="sxs-lookup"><span data-stu-id="29350-149">Response</span></span>
<span data-ttu-id="29350-150">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="29350-150">If successful, this method returns a `200 OK` response code and an updated [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29350-151">示例</span><span class="sxs-lookup"><span data-stu-id="29350-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="29350-152">请求</span><span class="sxs-lookup"><span data-stu-id="29350-152">Request</span></span>
<span data-ttu-id="29350-153">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="29350-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="29350-154">响应</span><span class="sxs-lookup"><span data-stu-id="29350-154">Response</span></span>
<span data-ttu-id="29350-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="29350-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



