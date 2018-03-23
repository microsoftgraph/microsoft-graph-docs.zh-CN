# <a name="create-targetedmanagedappconfiguration"></a><span data-ttu-id="59de9-101">创建 targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="59de9-101">Create targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="59de9-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="59de9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="59de9-103">创建新的 [targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="59de9-103">Create a new [plannerBucket](../resources/intune_mam_targetedmanagedappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="59de9-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="59de9-104">Prerequisites</span></span>
<span data-ttu-id="59de9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="59de9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="59de9-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="59de9-107">Permission type</span></span>|<span data-ttu-id="59de9-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="59de9-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="59de9-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="59de9-109">Delegated (work or school account)</span></span>|<span data-ttu-id="59de9-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59de9-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="59de9-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="59de9-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="59de9-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="59de9-112">Not supported.</span></span>|
|<span data-ttu-id="59de9-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="59de9-113">Application</span></span>|<span data-ttu-id="59de9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="59de9-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="59de9-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="59de9-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="59de9-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="59de9-116">Request headers</span></span>
|<span data-ttu-id="59de9-117">标头</span><span class="sxs-lookup"><span data-stu-id="59de9-117">Header</span></span>|<span data-ttu-id="59de9-118">值</span><span class="sxs-lookup"><span data-stu-id="59de9-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="59de9-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="59de9-119">Authorization</span></span>|<span data-ttu-id="59de9-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="59de9-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="59de9-121">Accept</span><span class="sxs-lookup"><span data-stu-id="59de9-121">Accept</span></span>|<span data-ttu-id="59de9-122">application/json</span><span class="sxs-lookup"><span data-stu-id="59de9-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="59de9-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="59de9-123">Request body</span></span>
<span data-ttu-id="59de9-124">在请求正文中，提供 targetedManagedAppConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="59de9-124">In the request body, supply a JSON representation of user object.</span></span>

<span data-ttu-id="59de9-125">下表显示创建 targetedManagedAppConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="59de9-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="59de9-126">属性</span><span class="sxs-lookup"><span data-stu-id="59de9-126">Property</span></span>|<span data-ttu-id="59de9-127">类型</span><span class="sxs-lookup"><span data-stu-id="59de9-127">Type</span></span>|<span data-ttu-id="59de9-128">说明</span><span class="sxs-lookup"><span data-stu-id="59de9-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59de9-129">displayName</span><span class="sxs-lookup"><span data-stu-id="59de9-129">displayName</span></span>|<span data-ttu-id="59de9-130">String</span><span class="sxs-lookup"><span data-stu-id="59de9-130">String</span></span>|<span data-ttu-id="59de9-131">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="59de9-131">Policy display name.</span></span> <span data-ttu-id="59de9-132">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="59de9-132">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="59de9-133">description</span><span class="sxs-lookup"><span data-stu-id="59de9-133">description</span></span>|<span data-ttu-id="59de9-134">String</span><span class="sxs-lookup"><span data-stu-id="59de9-134">String</span></span>|<span data-ttu-id="59de9-135">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="59de9-135">The policy's description.</span></span> <span data-ttu-id="59de9-136">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="59de9-136">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="59de9-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="59de9-137">createdDateTime</span></span>|<span data-ttu-id="59de9-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59de9-138">DateTimeOffset</span></span>|<span data-ttu-id="59de9-139">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="59de9-139">The date and time when the page was created.</span></span> <span data-ttu-id="59de9-140">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="59de9-140">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="59de9-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="59de9-141">lastModifiedDateTime</span></span>|<span data-ttu-id="59de9-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59de9-142">DateTimeOffset</span></span>|<span data-ttu-id="59de9-143">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="59de9-143">Last time the policy was modified.</span></span> <span data-ttu-id="59de9-144">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="59de9-144">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="59de9-145">id</span><span class="sxs-lookup"><span data-stu-id="59de9-145">id</span></span>|<span data-ttu-id="59de9-146">String</span><span class="sxs-lookup"><span data-stu-id="59de9-146">String</span></span>|<span data-ttu-id="59de9-147">实体的键。</span><span class="sxs-lookup"><span data-stu-id="59de9-147">Key of the setting.</span></span> <span data-ttu-id="59de9-148">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="59de9-148">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="59de9-149">version</span><span class="sxs-lookup"><span data-stu-id="59de9-149">version</span></span>|<span data-ttu-id="59de9-150">String</span><span class="sxs-lookup"><span data-stu-id="59de9-150">String</span></span>|<span data-ttu-id="59de9-151">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="59de9-151">Version of the entity.</span></span> <span data-ttu-id="59de9-152">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="59de9-152">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="59de9-153">customSettings</span><span class="sxs-lookup"><span data-stu-id="59de9-153">customSettings</span></span>|<span data-ttu-id="59de9-154">[keyValuePair](../resources/intune_mam_keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="59de9-154">[keyValuePair](../resources/intune_mam_keyvaluepair.md) collection</span></span>|<span data-ttu-id="59de9-155">要发送到配置范围确定的用户应用的一组字符串键和字符串值对，不由此服务更改。继承自 [ managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="59de9-155">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md)</span></span>|
|<span data-ttu-id="59de9-156">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="59de9-156">deployedAppCount</span></span>|<span data-ttu-id="59de9-157">Int32</span><span class="sxs-lookup"><span data-stu-id="59de9-157">Int32</span></span>|<span data-ttu-id="59de9-158">当前策略部署到的应用的计数。</span><span class="sxs-lookup"><span data-stu-id="59de9-158">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="59de9-159">isAssigned</span><span class="sxs-lookup"><span data-stu-id="59de9-159">isAssigned</span></span>|<span data-ttu-id="59de9-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="59de9-160">Boolean</span></span>|<span data-ttu-id="59de9-161">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="59de9-161">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="59de9-162">响应</span><span class="sxs-lookup"><span data-stu-id="59de9-162">Response</span></span>
<span data-ttu-id="59de9-163">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="59de9-163">If successful, this method returns a `201 Created` response code and a [ListItemVersion](../resources/intune_mam_targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59de9-164">示例</span><span class="sxs-lookup"><span data-stu-id="59de9-164">Example</span></span>
### <a name="request"></a><span data-ttu-id="59de9-165">请求</span><span class="sxs-lookup"><span data-stu-id="59de9-165">Request</span></span>
<span data-ttu-id="59de9-166">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="59de9-166">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/targetedManagedAppConfigurations
Content-type: application/json
Content-length: 452

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": "Version value",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "deployedAppCount": 0,
  "isAssigned": true
}
```

### <a name="response"></a><span data-ttu-id="59de9-167">响应</span><span class="sxs-lookup"><span data-stu-id="59de9-167">Response</span></span>
<span data-ttu-id="59de9-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="59de9-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 560

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "id": "2444e029-e029-2444-29e0-442429e04424",
  "version": "Version value",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "deployedAppCount": 0,
  "isAssigned": true
}
```



