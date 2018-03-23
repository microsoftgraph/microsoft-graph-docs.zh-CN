# <a name="create-deviceconfigurationstate"></a><span data-ttu-id="bf299-101">创建 deviceConfigurationState</span><span class="sxs-lookup"><span data-stu-id="bf299-101">Create deviceConfigurationState</span></span>

> <span data-ttu-id="bf299-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="bf299-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bf299-103">创建新的 [deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bf299-103">Create a new [plannerBucket](../resources/intune_deviceconfig_deviceconfigurationstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bf299-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="bf299-104">Prerequisites</span></span>
<span data-ttu-id="bf299-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="bf299-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="bf299-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="bf299-107">Permission type</span></span>|<span data-ttu-id="bf299-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bf299-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bf299-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bf299-109">Delegated (work or school account)</span></span>|<span data-ttu-id="bf299-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf299-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bf299-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bf299-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bf299-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="bf299-112">Not supported.</span></span>|
|<span data-ttu-id="bf299-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="bf299-113">Application</span></span>|<span data-ttu-id="bf299-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="bf299-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bf299-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bf299-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /managedDevices/{managedDevicesId}/deviceConfigurationStates
```

## <a name="request-headers"></a><span data-ttu-id="bf299-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="bf299-116">Request headers</span></span>
|<span data-ttu-id="bf299-117">标头</span><span class="sxs-lookup"><span data-stu-id="bf299-117">Header</span></span>|<span data-ttu-id="bf299-118">值</span><span class="sxs-lookup"><span data-stu-id="bf299-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bf299-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="bf299-119">Authorization</span></span>|<span data-ttu-id="bf299-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bf299-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="bf299-121">Accept</span><span class="sxs-lookup"><span data-stu-id="bf299-121">Accept</span></span>|<span data-ttu-id="bf299-122">application/json</span><span class="sxs-lookup"><span data-stu-id="bf299-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf299-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="bf299-123">Request body</span></span>
<span data-ttu-id="bf299-124">在请求正文中，提供 deviceConfigurationState 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bf299-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="bf299-125">下表显示创建 deviceConfigurationState 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="bf299-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="bf299-126">属性</span><span class="sxs-lookup"><span data-stu-id="bf299-126">Property</span></span>|<span data-ttu-id="bf299-127">类型</span><span class="sxs-lookup"><span data-stu-id="bf299-127">Type</span></span>|<span data-ttu-id="bf299-128">说明</span><span class="sxs-lookup"><span data-stu-id="bf299-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf299-129">id</span><span class="sxs-lookup"><span data-stu-id="bf299-129">id</span></span>|<span data-ttu-id="bf299-130">String</span><span class="sxs-lookup"><span data-stu-id="bf299-130">String</span></span>|<span data-ttu-id="bf299-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="bf299-131">Key of the setting.</span></span>|
|<span data-ttu-id="bf299-132">settingStates</span><span class="sxs-lookup"><span data-stu-id="bf299-132">settingStates</span></span>|<span data-ttu-id="bf299-133">[deviceConfigurationSettingState](../resources/intune_deviceconfig_deviceconfigurationsettingstate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bf299-133">[deviceConfigurationSettingState](../resources/intune_deviceconfig_deviceconfigurationsettingstate.md) collection</span></span>|<span data-ttu-id="bf299-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="bf299-134">Not yet documented</span></span>|
|<span data-ttu-id="bf299-135">displayName</span><span class="sxs-lookup"><span data-stu-id="bf299-135">displayName</span></span>|<span data-ttu-id="bf299-136">String</span><span class="sxs-lookup"><span data-stu-id="bf299-136">String</span></span>|<span data-ttu-id="bf299-137">此 policyBase 的策略名称</span><span class="sxs-lookup"><span data-stu-id="bf299-137">The name of the policy for this policyBase</span></span>|
|<span data-ttu-id="bf299-138">version</span><span class="sxs-lookup"><span data-stu-id="bf299-138">version</span></span>|<span data-ttu-id="bf299-139">Int32</span><span class="sxs-lookup"><span data-stu-id="bf299-139">Int32</span></span>|<span data-ttu-id="bf299-140">策略版本</span><span class="sxs-lookup"><span data-stu-id="bf299-140">The version of the message.</span></span>|
|<span data-ttu-id="bf299-141">platformType</span><span class="sxs-lookup"><span data-stu-id="bf299-141">PlatformType</span></span>|<span data-ttu-id="bf299-142">String</span><span class="sxs-lookup"><span data-stu-id="bf299-142">String</span></span>|<span data-ttu-id="bf299-143">策略适用的平台类型。可取值为：`android`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`all`。</span><span class="sxs-lookup"><span data-stu-id="bf299-143">Platform type that the policy applies to Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `all`.</span></span>|
|<span data-ttu-id="bf299-144">state</span><span class="sxs-lookup"><span data-stu-id="bf299-144">state</span></span>|<span data-ttu-id="bf299-145">String</span><span class="sxs-lookup"><span data-stu-id="bf299-145">String</span></span>|<span data-ttu-id="bf299-146">策略符合性状态。可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`。</span><span class="sxs-lookup"><span data-stu-id="bf299-146">The compliance state of the policy Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="bf299-147">settingCount</span><span class="sxs-lookup"><span data-stu-id="bf299-147">settingCount</span></span>|<span data-ttu-id="bf299-148">Int32</span><span class="sxs-lookup"><span data-stu-id="bf299-148">Int32</span></span>|<span data-ttu-id="bf299-149">策略保留的设置计数</span><span class="sxs-lookup"><span data-stu-id="bf299-149">Count of how many setting a policy holds</span></span>|



## <a name="response"></a><span data-ttu-id="bf299-150">响应</span><span class="sxs-lookup"><span data-stu-id="bf299-150">Response</span></span>
<span data-ttu-id="bf299-151">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bf299-151">If successful, this method returns a `201 Created` response code and a [ListItemVersion](../resources/intune_deviceconfig_deviceconfigurationstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf299-152">示例</span><span class="sxs-lookup"><span data-stu-id="bf299-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="bf299-153">请求</span><span class="sxs-lookup"><span data-stu-id="bf299-153">Request</span></span>
<span data-ttu-id="bf299-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bf299-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/managedDevices/{managedDevicesId}/deviceConfigurationStates
Content-type: application/json
Content-length: 967

{
  "@odata.type": "#microsoft.graph.deviceConfigurationState",
  "settingStates": [
    {
      "@odata.type": "microsoft.graph.deviceConfigurationSettingState",
      "setting": "Setting value",
      "settingName": "Setting Name value",
      "instanceDisplayName": "Instance Display Name value",
      "state": "notApplicable",
      "errorCode": 9,
      "errorDescription": "Error Description value",
      "userId": "User Id value",
      "userName": "User Name value",
      "userEmail": "User Email value",
      "userPrincipalName": "User Principal Name value",
      "sources": [
        {
          "@odata.type": "microsoft.graph.settingSource",
          "id": "Id value",
          "displayName": "Display Name value"
        }
      ],
      "currentValue": "Current Value value"
    }
  ],
  "displayName": "Display Name value",
  "version": 7,
  "platformType": "iOS",
  "state": "notApplicable",
  "settingCount": 12
}
```

### <a name="response"></a><span data-ttu-id="bf299-155">响应</span><span class="sxs-lookup"><span data-stu-id="bf299-155">Response</span></span>
<span data-ttu-id="bf299-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bf299-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1016

{
  "@odata.type": "#microsoft.graph.deviceConfigurationState",
  "id": "11692784-2784-1169-8427-691184276911",
  "settingStates": [
    {
      "@odata.type": "microsoft.graph.deviceConfigurationSettingState",
      "setting": "Setting value",
      "settingName": "Setting Name value",
      "instanceDisplayName": "Instance Display Name value",
      "state": "notApplicable",
      "errorCode": 9,
      "errorDescription": "Error Description value",
      "userId": "User Id value",
      "userName": "User Name value",
      "userEmail": "User Email value",
      "userPrincipalName": "User Principal Name value",
      "sources": [
        {
          "@odata.type": "microsoft.graph.settingSource",
          "id": "Id value",
          "displayName": "Display Name value"
        }
      ],
      "currentValue": "Current Value value"
    }
  ],
  "displayName": "Display Name value",
  "version": 7,
  "platformType": "iOS",
  "state": "notApplicable",
  "settingCount": 12
}
```



