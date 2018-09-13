# <a name="update-managedapppolicydeploymentsummary"></a><span data-ttu-id="989d8-101">更新 managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="989d8-101">Update managedAppPolicyDeploymentSummary</span></span>

> <span data-ttu-id="989d8-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="989d8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="989d8-103">更新 [managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="989d8-103">Update the properties of a [managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="989d8-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="989d8-104">Prerequisites</span></span>
<span data-ttu-id="989d8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="989d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="989d8-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="989d8-107">Permission type</span></span>|<span data-ttu-id="989d8-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="989d8-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="989d8-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="989d8-109">Delegated (work or school account)</span></span>|<span data-ttu-id="989d8-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="989d8-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="989d8-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="989d8-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="989d8-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="989d8-112">Not supported.</span></span>|
|<span data-ttu-id="989d8-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="989d8-113">Application</span></span>|<span data-ttu-id="989d8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="989d8-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="989d8-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="989d8-115">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="989d8-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="989d8-116">Request headers</span></span>
|<span data-ttu-id="989d8-117">标头</span><span class="sxs-lookup"><span data-stu-id="989d8-117">Header</span></span>|<span data-ttu-id="989d8-118">值</span><span class="sxs-lookup"><span data-stu-id="989d8-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="989d8-119">授权</span><span class="sxs-lookup"><span data-stu-id="989d8-119">Authorization</span></span>|<span data-ttu-id="989d8-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="989d8-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="989d8-121">接受</span><span class="sxs-lookup"><span data-stu-id="989d8-121">Accept</span></span>|<span data-ttu-id="989d8-122">application/json</span><span class="sxs-lookup"><span data-stu-id="989d8-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="989d8-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="989d8-123">Request body</span></span>
<span data-ttu-id="989d8-124">在请求正文中，提供 [managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="989d8-124">In the request body, supply a JSON representation for the [managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md) object.</span></span>

<span data-ttu-id="989d8-125">下表显示创建 [managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="989d8-125">The following table shows the properties that are required when you create the [managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md).</span></span>

|<span data-ttu-id="989d8-126">属性</span><span class="sxs-lookup"><span data-stu-id="989d8-126">Property</span></span>|<span data-ttu-id="989d8-127">类型</span><span class="sxs-lookup"><span data-stu-id="989d8-127">Type</span></span>|<span data-ttu-id="989d8-128">说明</span><span class="sxs-lookup"><span data-stu-id="989d8-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="989d8-129">displayName</span><span class="sxs-lookup"><span data-stu-id="989d8-129">displayName</span></span>|<span data-ttu-id="989d8-130">字符串</span><span class="sxs-lookup"><span data-stu-id="989d8-130">String</span></span>|<span data-ttu-id="989d8-131">尚未记录</span><span class="sxs-lookup"><span data-stu-id="989d8-131">Not yet documented</span></span>|
|<span data-ttu-id="989d8-132">configurationDeployedUserCount</span><span class="sxs-lookup"><span data-stu-id="989d8-132">configurationDeployedUserCount</span></span>|<span data-ttu-id="989d8-133">Int32</span><span class="sxs-lookup"><span data-stu-id="989d8-133">Int32</span></span>|<span data-ttu-id="989d8-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="989d8-134">Not yet documented</span></span>|
|<span data-ttu-id="989d8-135">lastRefreshTime</span><span class="sxs-lookup"><span data-stu-id="989d8-135">lastRefreshTime</span></span>|<span data-ttu-id="989d8-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="989d8-136">DateTimeOffset</span></span>|<span data-ttu-id="989d8-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="989d8-137">Not yet documented</span></span>|
|<span data-ttu-id="989d8-138">configurationDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="989d8-138">configurationDeploymentSummaryPerApp</span></span>|<span data-ttu-id="989d8-139">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune_mam_managedapppolicydeploymentsummaryperapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="989d8-139">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune_mam_managedapppolicydeploymentsummaryperapp.md) collection</span></span>|<span data-ttu-id="989d8-140">尚未记录</span><span class="sxs-lookup"><span data-stu-id="989d8-140">Not yet documented</span></span>|
|<span data-ttu-id="989d8-141">id</span><span class="sxs-lookup"><span data-stu-id="989d8-141">id</span></span>|<span data-ttu-id="989d8-142">字符串</span><span class="sxs-lookup"><span data-stu-id="989d8-142">String</span></span>|<span data-ttu-id="989d8-143">实体的键。</span><span class="sxs-lookup"><span data-stu-id="989d8-143">Key of the entity.</span></span>|
|<span data-ttu-id="989d8-144">version</span><span class="sxs-lookup"><span data-stu-id="989d8-144">version</span></span>|<span data-ttu-id="989d8-145">字符串</span><span class="sxs-lookup"><span data-stu-id="989d8-145">String</span></span>|<span data-ttu-id="989d8-146">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="989d8-146">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="989d8-147">响应</span><span class="sxs-lookup"><span data-stu-id="989d8-147">Response</span></span>
<span data-ttu-id="989d8-148">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="989d8-148">If successful, this method returns a `200 OK` response code and an updated [managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="989d8-149">示例</span><span class="sxs-lookup"><span data-stu-id="989d8-149">Example</span></span>
### <a name="request"></a><span data-ttu-id="989d8-150">请求</span><span class="sxs-lookup"><span data-stu-id="989d8-150">Request</span></span>
<span data-ttu-id="989d8-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="989d8-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
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

### <a name="response"></a><span data-ttu-id="989d8-152">响应</span><span class="sxs-lookup"><span data-stu-id="989d8-152">Response</span></span>
<span data-ttu-id="989d8-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="989d8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








