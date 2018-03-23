# <a name="update-devicecompliancesettingstate"></a><span data-ttu-id="2474f-101">更新 deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="2474f-101">Update deviceComplianceSettingState</span></span>

> <span data-ttu-id="2474f-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="2474f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2474f-103">更新 [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2474f-103">Update the properties of a [calendar](../resources/intune_deviceconfig_devicecompliancesettingstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2474f-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="2474f-104">Prerequisites</span></span>
<span data-ttu-id="2474f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="2474f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2474f-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="2474f-107">Permission type</span></span>|<span data-ttu-id="2474f-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2474f-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2474f-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2474f-109">Delegated (work or school account)</span></span>|<span data-ttu-id="2474f-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2474f-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2474f-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2474f-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2474f-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="2474f-112">Not supported.</span></span>|
|<span data-ttu-id="2474f-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="2474f-113">Application</span></span>|<span data-ttu-id="2474f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2474f-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2474f-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2474f-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="2474f-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="2474f-116">Request headers</span></span>
|<span data-ttu-id="2474f-117">标头</span><span class="sxs-lookup"><span data-stu-id="2474f-117">Header</span></span>|<span data-ttu-id="2474f-118">值</span><span class="sxs-lookup"><span data-stu-id="2474f-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2474f-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="2474f-119">Authorization</span></span>|<span data-ttu-id="2474f-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2474f-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="2474f-121">Accept</span><span class="sxs-lookup"><span data-stu-id="2474f-121">Accept</span></span>|<span data-ttu-id="2474f-122">application/json</span><span class="sxs-lookup"><span data-stu-id="2474f-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2474f-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="2474f-123">Request body</span></span>
<span data-ttu-id="2474f-124">在请求正文中，提供 [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2474f-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_devicecompliancesettingstate.md) object.</span></span>

<span data-ttu-id="2474f-125">下表显示了创建 [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2474f-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="2474f-126">属性</span><span class="sxs-lookup"><span data-stu-id="2474f-126">Property</span></span>|<span data-ttu-id="2474f-127">类型</span><span class="sxs-lookup"><span data-stu-id="2474f-127">Type</span></span>|<span data-ttu-id="2474f-128">说明</span><span class="sxs-lookup"><span data-stu-id="2474f-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2474f-129">id</span><span class="sxs-lookup"><span data-stu-id="2474f-129">id</span></span>|<span data-ttu-id="2474f-130">String</span><span class="sxs-lookup"><span data-stu-id="2474f-130">String</span></span>|<span data-ttu-id="2474f-131">实体的键</span><span class="sxs-lookup"><span data-stu-id="2474f-131">Key of the setting.</span></span>|
|<span data-ttu-id="2474f-132">setting</span><span class="sxs-lookup"><span data-stu-id="2474f-132">setting</span></span>|<span data-ttu-id="2474f-133">String</span><span class="sxs-lookup"><span data-stu-id="2474f-133">String</span></span>|<span data-ttu-id="2474f-134">设置类名和属性名。</span><span class="sxs-lookup"><span data-stu-id="2474f-134">The setting class name and property name.</span></span>|
|<span data-ttu-id="2474f-135">settingName</span><span class="sxs-lookup"><span data-stu-id="2474f-135">settingName</span></span>|<span data-ttu-id="2474f-136">String</span><span class="sxs-lookup"><span data-stu-id="2474f-136">String</span></span>|<span data-ttu-id="2474f-137">报告的设置名称</span><span class="sxs-lookup"><span data-stu-id="2474f-137">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="2474f-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="2474f-138">deviceId</span></span>|<span data-ttu-id="2474f-139">String</span><span class="sxs-lookup"><span data-stu-id="2474f-139">String</span></span>|<span data-ttu-id="2474f-140">报告的设备 ID</span><span class="sxs-lookup"><span data-stu-id="2474f-140">The Device Id that is being reported</span></span>|
|<span data-ttu-id="2474f-141">deviceName</span><span class="sxs-lookup"><span data-stu-id="2474f-141">deviceName</span></span>|<span data-ttu-id="2474f-142">String</span><span class="sxs-lookup"><span data-stu-id="2474f-142">String</span></span>|<span data-ttu-id="2474f-143">报告的设备名称</span><span class="sxs-lookup"><span data-stu-id="2474f-143">The Device Name that is being reported</span></span>|
|<span data-ttu-id="2474f-144">userId</span><span class="sxs-lookup"><span data-stu-id="2474f-144">userID</span></span>|<span data-ttu-id="2474f-145">String</span><span class="sxs-lookup"><span data-stu-id="2474f-145">String</span></span>|<span data-ttu-id="2474f-146">报告的用户 ID</span><span class="sxs-lookup"><span data-stu-id="2474f-146">The user Id that is being reported</span></span>|
|<span data-ttu-id="2474f-147">userEmail</span><span class="sxs-lookup"><span data-stu-id="2474f-147">userEmail</span></span>|<span data-ttu-id="2474f-148">String</span><span class="sxs-lookup"><span data-stu-id="2474f-148">String</span></span>|<span data-ttu-id="2474f-149">报告的用户电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="2474f-149">The User email address that is being reported</span></span>|
|<span data-ttu-id="2474f-150">userName</span><span class="sxs-lookup"><span data-stu-id="2474f-150">UserName</span></span>|<span data-ttu-id="2474f-151">String</span><span class="sxs-lookup"><span data-stu-id="2474f-151">String</span></span>|<span data-ttu-id="2474f-152">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="2474f-152">The User Name that is being reported</span></span>|
|<span data-ttu-id="2474f-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2474f-153">userPrincipalName</span></span>|<span data-ttu-id="2474f-154">String</span><span class="sxs-lookup"><span data-stu-id="2474f-154">String</span></span>|<span data-ttu-id="2474f-155">报告的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="2474f-155">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="2474f-156">deviceModel</span><span class="sxs-lookup"><span data-stu-id="2474f-156">deviceModel</span></span>|<span data-ttu-id="2474f-157">String</span><span class="sxs-lookup"><span data-stu-id="2474f-157">String</span></span>|<span data-ttu-id="2474f-158">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="2474f-158">The device model that is being reported</span></span>|
|<span data-ttu-id="2474f-159">state</span><span class="sxs-lookup"><span data-stu-id="2474f-159">state</span></span>|<span data-ttu-id="2474f-160">String</span><span class="sxs-lookup"><span data-stu-id="2474f-160">String</span></span>|<span data-ttu-id="2474f-161">设置的符合性状态。可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`。</span><span class="sxs-lookup"><span data-stu-id="2474f-161">The compliance state of the setting Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="2474f-162">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="2474f-162">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="2474f-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2474f-163">DateTimeOffset</span></span>|<span data-ttu-id="2474f-164">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="2474f-164">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="2474f-165">响应</span><span class="sxs-lookup"><span data-stu-id="2474f-165">Response</span></span>
<span data-ttu-id="2474f-166">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2474f-166">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2474f-167">示例</span><span class="sxs-lookup"><span data-stu-id="2474f-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="2474f-168">请求</span><span class="sxs-lookup"><span data-stu-id="2474f-168">Request</span></span>
<span data-ttu-id="2474f-169">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2474f-169">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
Content-type: application/json
Content-length: 450

{
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "deviceId": "Device Id value",
  "deviceName": "Device Name value",
  "userId": "User Id value",
  "userEmail": "User Email value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "deviceModel": "Device Model value",
  "state": "notApplicable",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00"
}
```

### <a name="response"></a><span data-ttu-id="2474f-170">响应</span><span class="sxs-lookup"><span data-stu-id="2474f-170">Response</span></span>
<span data-ttu-id="2474f-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2474f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 566

{
  "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
  "id": "9905f955-f955-9905-55f9-059955f90599",
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "deviceId": "Device Id value",
  "deviceName": "Device Name value",
  "userId": "User Id value",
  "userEmail": "User Email value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "deviceModel": "Device Model value",
  "state": "notApplicable",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00"
}
```



