---
title: 更新 managedAppPolicyDeploymentSummary
description: 更新 managedAppPolicyDeploymentSummary 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 220443e5c75121083fb23758e42d7ec331bbee18
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877420"
---
# <a name="update-managedapppolicydeploymentsummary"></a><span data-ttu-id="69834-103">更新 managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="69834-103">Update managedAppPolicyDeploymentSummary</span></span>

> <span data-ttu-id="69834-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="69834-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="69834-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="69834-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="69834-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="69834-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="69834-107">更新 [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="69834-107">Update the properties of a [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="69834-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="69834-108">Prerequisites</span></span>
<span data-ttu-id="69834-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="69834-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69834-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="69834-111">Permission type</span></span>|<span data-ttu-id="69834-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="69834-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69834-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="69834-113">Delegated (work or school account)</span></span>|<span data-ttu-id="69834-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69834-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="69834-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="69834-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69834-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="69834-116">Not supported.</span></span>|
|<span data-ttu-id="69834-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="69834-117">Application</span></span>|<span data-ttu-id="69834-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="69834-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="69834-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="69834-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="69834-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="69834-120">Request headers</span></span>
|<span data-ttu-id="69834-121">标头</span><span class="sxs-lookup"><span data-stu-id="69834-121">Header</span></span>|<span data-ttu-id="69834-122">值</span><span class="sxs-lookup"><span data-stu-id="69834-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69834-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="69834-123">Authorization</span></span>|<span data-ttu-id="69834-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="69834-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69834-125">Accept</span><span class="sxs-lookup"><span data-stu-id="69834-125">Accept</span></span>|<span data-ttu-id="69834-126">application/json</span><span class="sxs-lookup"><span data-stu-id="69834-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69834-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="69834-127">Request body</span></span>
<span data-ttu-id="69834-128">在请求正文中，提供 [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="69834-128">In the request body, supply a JSON representation for the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>

<span data-ttu-id="69834-129">下表显示创建 [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="69834-129">The following table shows the properties that are required when you create the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span></span>

|<span data-ttu-id="69834-130">属性</span><span class="sxs-lookup"><span data-stu-id="69834-130">Property</span></span>|<span data-ttu-id="69834-131">类型</span><span class="sxs-lookup"><span data-stu-id="69834-131">Type</span></span>|<span data-ttu-id="69834-132">说明</span><span class="sxs-lookup"><span data-stu-id="69834-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69834-133">displayName</span><span class="sxs-lookup"><span data-stu-id="69834-133">displayName</span></span>|<span data-ttu-id="69834-134">字符串</span><span class="sxs-lookup"><span data-stu-id="69834-134">String</span></span>|<span data-ttu-id="69834-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="69834-135">Not yet documented</span></span>|
|<span data-ttu-id="69834-136">configurationDeployedUserCount</span><span class="sxs-lookup"><span data-stu-id="69834-136">configurationDeployedUserCount</span></span>|<span data-ttu-id="69834-137">Int32</span><span class="sxs-lookup"><span data-stu-id="69834-137">Int32</span></span>|<span data-ttu-id="69834-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="69834-138">Not yet documented</span></span>|
|<span data-ttu-id="69834-139">lastRefreshTime</span><span class="sxs-lookup"><span data-stu-id="69834-139">lastRefreshTime</span></span>|<span data-ttu-id="69834-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69834-140">DateTimeOffset</span></span>|<span data-ttu-id="69834-141">尚未记录</span><span class="sxs-lookup"><span data-stu-id="69834-141">Not yet documented</span></span>|
|<span data-ttu-id="69834-142">configurationDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="69834-142">configurationDeploymentSummaryPerApp</span></span>|<span data-ttu-id="69834-143">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="69834-143">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md) collection</span></span>|<span data-ttu-id="69834-144">尚未记录</span><span class="sxs-lookup"><span data-stu-id="69834-144">Not yet documented</span></span>|
|<span data-ttu-id="69834-145">id</span><span class="sxs-lookup"><span data-stu-id="69834-145">id</span></span>|<span data-ttu-id="69834-146">String</span><span class="sxs-lookup"><span data-stu-id="69834-146">String</span></span>|<span data-ttu-id="69834-147">实体的键。</span><span class="sxs-lookup"><span data-stu-id="69834-147">Key of the entity.</span></span>|
|<span data-ttu-id="69834-148">version</span><span class="sxs-lookup"><span data-stu-id="69834-148">version</span></span>|<span data-ttu-id="69834-149">String</span><span class="sxs-lookup"><span data-stu-id="69834-149">String</span></span>|<span data-ttu-id="69834-150">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="69834-150">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="69834-151">响应</span><span class="sxs-lookup"><span data-stu-id="69834-151">Response</span></span>
<span data-ttu-id="69834-152">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="69834-152">If successful, this method returns a `200 OK` response code and an updated [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69834-153">示例</span><span class="sxs-lookup"><span data-stu-id="69834-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="69834-154">请求</span><span class="sxs-lookup"><span data-stu-id="69834-154">Request</span></span>
<span data-ttu-id="69834-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="69834-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
Content-type: application/json
Content-length: 516

{
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

### <a name="response"></a><span data-ttu-id="69834-156">响应</span><span class="sxs-lookup"><span data-stu-id="69834-156">Response</span></span>
<span data-ttu-id="69834-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="69834-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





