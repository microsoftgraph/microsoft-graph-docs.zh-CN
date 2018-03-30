# <a name="update-androidforworksettings"></a><span data-ttu-id="99b10-101">更新 androidForWorkSettings</span><span class="sxs-lookup"><span data-stu-id="99b10-101">Update androidForWorkSettings</span></span>

> <span data-ttu-id="99b10-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="99b10-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="99b10-103">更新 [androidForWorkSettings](../resources/intune_androidforwork_androidforworksettings.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="99b10-103">Update the properties of a [calendar](../resources/intune_androidforwork_androidforworksettings.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="99b10-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="99b10-104">Prerequisites</span></span>
<span data-ttu-id="99b10-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="99b10-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="99b10-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="99b10-107">Permission type</span></span>|<span data-ttu-id="99b10-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="99b10-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="99b10-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="99b10-109">Delegated (work or school account)</span></span>|<span data-ttu-id="99b10-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99b10-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="99b10-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="99b10-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="99b10-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="99b10-112">Not supported.</span></span>|
|<span data-ttu-id="99b10-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="99b10-113">Application</span></span>|<span data-ttu-id="99b10-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="99b10-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="99b10-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="99b10-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkSettings
```

## <a name="request-headers"></a><span data-ttu-id="99b10-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="99b10-116">Request headers</span></span>
|<span data-ttu-id="99b10-117">标头</span><span class="sxs-lookup"><span data-stu-id="99b10-117">Header</span></span>|<span data-ttu-id="99b10-118">值</span><span class="sxs-lookup"><span data-stu-id="99b10-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="99b10-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="99b10-119">Authorization</span></span>|<span data-ttu-id="99b10-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="99b10-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="99b10-121">Accept</span><span class="sxs-lookup"><span data-stu-id="99b10-121">Accept</span></span>|<span data-ttu-id="99b10-122">application/json</span><span class="sxs-lookup"><span data-stu-id="99b10-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="99b10-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="99b10-123">Request body</span></span>
<span data-ttu-id="99b10-124">在请求正文中，提供 [androidForWorkSettings](../resources/intune_androidforwork_androidforworksettings.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="99b10-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_androidforwork_androidforworksettings.md) object.</span></span>

<span data-ttu-id="99b10-125">下表显示了创建 [androidForWorkSettings](../resources/intune_androidforwork_androidforworksettings.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="99b10-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="99b10-126">属性</span><span class="sxs-lookup"><span data-stu-id="99b10-126">Property</span></span>|<span data-ttu-id="99b10-127">类型</span><span class="sxs-lookup"><span data-stu-id="99b10-127">Type</span></span>|<span data-ttu-id="99b10-128">说明</span><span class="sxs-lookup"><span data-stu-id="99b10-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99b10-129">id</span><span class="sxs-lookup"><span data-stu-id="99b10-129">id</span></span>|<span data-ttu-id="99b10-130">String</span><span class="sxs-lookup"><span data-stu-id="99b10-130">String</span></span>|<span data-ttu-id="99b10-131">Android for Work 设置标识符</span><span class="sxs-lookup"><span data-stu-id="99b10-131">The Android for Work settings identifier</span></span>|
|<span data-ttu-id="99b10-132">bindStatus</span><span class="sxs-lookup"><span data-stu-id="99b10-132">bindStatus</span></span>|<span data-ttu-id="99b10-133">String</span><span class="sxs-lookup"><span data-stu-id="99b10-133">String</span></span>|<span data-ttu-id="99b10-134">使用 Google EMM API 的租户的绑定状态。可取值为：`notBound`、`bound`、`boundAndValidated`、`unbinding`。</span><span class="sxs-lookup"><span data-stu-id="99b10-134">Bind status of the tenant with the Google EMM API Possible values are: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span></span>|
|<span data-ttu-id="99b10-135">lastAppSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="99b10-135">lastAppSyncDateTime</span></span>|<span data-ttu-id="99b10-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99b10-136">DateTimeOffset</span></span>|<span data-ttu-id="99b10-137">应用同步的上次完成时间</span><span class="sxs-lookup"><span data-stu-id="99b10-137">Last completion time for app sync</span></span>|
|<span data-ttu-id="99b10-138">lastAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="99b10-138">lastAppSyncStatus</span></span>|<span data-ttu-id="99b10-139">String</span><span class="sxs-lookup"><span data-stu-id="99b10-139">String</span></span>|<span data-ttu-id="99b10-140">上次应用程序同步结果。可取值为：`success`、`credentialsNotValid`、`androidForWorkApiError`、`managementServiceError`、`unknownError`、`none`。</span><span class="sxs-lookup"><span data-stu-id="99b10-140">Last application sync result Possible values are: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span></span>|
|<span data-ttu-id="99b10-141">ownerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="99b10-141">ownerUserPrincipalName</span></span>|<span data-ttu-id="99b10-142">String</span><span class="sxs-lookup"><span data-stu-id="99b10-142">String</span></span>|<span data-ttu-id="99b10-143">创建了企业的所有者 UPN</span><span class="sxs-lookup"><span data-stu-id="99b10-143">Owner UPN that created the enterprise</span></span>|
|<span data-ttu-id="99b10-144">ownerOrganizationName</span><span class="sxs-lookup"><span data-stu-id="99b10-144">ownerOrganizationName</span></span>|<span data-ttu-id="99b10-145">String</span><span class="sxs-lookup"><span data-stu-id="99b10-145">String</span></span>|<span data-ttu-id="99b10-146">载入 Android for Work 时使用的组织名称</span><span class="sxs-lookup"><span data-stu-id="99b10-146">Organization name used when onboarding Android for Work</span></span>|
|<span data-ttu-id="99b10-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="99b10-147">lastModifiedDateTime</span></span>|<span data-ttu-id="99b10-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99b10-148">DateTimeOffset</span></span>|<span data-ttu-id="99b10-149">Android for Work 设置的上次修改时间</span><span class="sxs-lookup"><span data-stu-id="99b10-149">Last modification time for Android for Work settings</span></span>|
|<span data-ttu-id="99b10-150">enrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="99b10-150">enrollmentTarget</span></span>|<span data-ttu-id="99b10-151">String</span><span class="sxs-lookup"><span data-stu-id="99b10-151">String</span></span>|<span data-ttu-id="99b10-152">指示哪些用户可以在 Android for Work 设备管理中注册设备。可取值为：`none`、`all`、`targeted`、`targetedAsEnrollmentRestrictions`。</span><span class="sxs-lookup"><span data-stu-id="99b10-152">Indicates which users can enroll devices in Android for Work device management Possible values are: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span></span>|
|<span data-ttu-id="99b10-153">targetGroupIds</span><span class="sxs-lookup"><span data-stu-id="99b10-153">targetGroupIds</span></span>|<span data-ttu-id="99b10-154">String 集合</span><span class="sxs-lookup"><span data-stu-id="99b10-154">String collection</span></span>|<span data-ttu-id="99b10-155">指定当 enrollmentTarget 设置为“定向”时可以在 Android for Work 设备管理中注册设备的 AAD 组。</span><span class="sxs-lookup"><span data-stu-id="99b10-155">Specifies which AAD groups can enroll devices in Android for Work device management if enrollmentTarget is set to 'Targeted'</span></span>|



## <a name="response"></a><span data-ttu-id="99b10-156">响应</span><span class="sxs-lookup"><span data-stu-id="99b10-156">Response</span></span>
<span data-ttu-id="99b10-157">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [androidForWorkSettings](../resources/intune_androidforwork_androidforworksettings.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="99b10-157">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_androidforwork_androidforworksettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99b10-158">示例</span><span class="sxs-lookup"><span data-stu-id="99b10-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="99b10-159">请求</span><span class="sxs-lookup"><span data-stu-id="99b10-159">Request</span></span>
<span data-ttu-id="99b10-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="99b10-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/androidForWorkSettings
Content-type: application/json
Content-length: 417

{
  "bindStatus": "bound",
  "lastAppSyncDateTime": "2016-12-31T23:57:22.8606813-08:00",
  "lastAppSyncStatus": "credentialsNotValid",
  "ownerUserPrincipalName": "Owner User Principal Name value",
  "ownerOrganizationName": "Owner Organization Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "enrollmentTarget": "all",
  "targetGroupIds": [
    "Target Group Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="99b10-161">响应</span><span class="sxs-lookup"><span data-stu-id="99b10-161">Response</span></span>
<span data-ttu-id="99b10-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="99b10-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 527

{
  "@odata.type": "#microsoft.graph.androidForWorkSettings",
  "id": "97adc169-c169-97ad-69c1-ad9769c1ad97",
  "bindStatus": "bound",
  "lastAppSyncDateTime": "2016-12-31T23:57:22.8606813-08:00",
  "lastAppSyncStatus": "credentialsNotValid",
  "ownerUserPrincipalName": "Owner User Principal Name value",
  "ownerOrganizationName": "Owner Organization Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "enrollmentTarget": "all",
  "targetGroupIds": [
    "Target Group Ids value"
  ]
}
```



