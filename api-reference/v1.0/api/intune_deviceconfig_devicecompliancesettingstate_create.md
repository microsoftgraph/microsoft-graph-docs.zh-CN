# <a name="create-devicecompliancesettingstate"></a><span data-ttu-id="58db2-101">创建 deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="58db2-101">Create deviceComplianceSettingState</span></span>

> <span data-ttu-id="58db2-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="58db2-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="58db2-103">创建新的 [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="58db2-103">Create a new [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="58db2-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="58db2-104">Prerequisites</span></span>
<span data-ttu-id="58db2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="58db2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="58db2-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="58db2-107">Permission type</span></span>|<span data-ttu-id="58db2-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="58db2-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58db2-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="58db2-109">Delegated (work or school account)</span></span>|<span data-ttu-id="58db2-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58db2-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="58db2-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="58db2-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58db2-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="58db2-112">Not supported.</span></span>|
|<span data-ttu-id="58db2-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="58db2-113">Application</span></span>|<span data-ttu-id="58db2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="58db2-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="58db2-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="58db2-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="58db2-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="58db2-116">Request headers</span></span>
|<span data-ttu-id="58db2-117">标头</span><span class="sxs-lookup"><span data-stu-id="58db2-117">Header</span></span>|<span data-ttu-id="58db2-118">值</span><span class="sxs-lookup"><span data-stu-id="58db2-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58db2-119">授权</span><span class="sxs-lookup"><span data-stu-id="58db2-119">Authorization</span></span>|<span data-ttu-id="58db2-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="58db2-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58db2-121">接受</span><span class="sxs-lookup"><span data-stu-id="58db2-121">Accept</span></span>|<span data-ttu-id="58db2-122">application/json</span><span class="sxs-lookup"><span data-stu-id="58db2-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58db2-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="58db2-123">Request body</span></span>
<span data-ttu-id="58db2-124">在请求正文中，提供 deviceComplianceSettingState 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="58db2-124">In the request body, supply a JSON representation for the deviceComplianceSettingState object.</span></span>

<span data-ttu-id="58db2-125">下表显示了创建 deviceComplianceSettingState 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="58db2-125">The following table shows the properties that are required when you create the deviceComplianceSettingState.</span></span>

|<span data-ttu-id="58db2-126">属性</span><span class="sxs-lookup"><span data-stu-id="58db2-126">Property</span></span>|<span data-ttu-id="58db2-127">类型</span><span class="sxs-lookup"><span data-stu-id="58db2-127">Type</span></span>|<span data-ttu-id="58db2-128">说明</span><span class="sxs-lookup"><span data-stu-id="58db2-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58db2-129">id</span><span class="sxs-lookup"><span data-stu-id="58db2-129">id</span></span>|<span data-ttu-id="58db2-130">String</span><span class="sxs-lookup"><span data-stu-id="58db2-130">String</span></span>|<span data-ttu-id="58db2-131">实体的键</span><span class="sxs-lookup"><span data-stu-id="58db2-131">Key of the entity</span></span>|
|<span data-ttu-id="58db2-132">setting</span><span class="sxs-lookup"><span data-stu-id="58db2-132">setting</span></span>|<span data-ttu-id="58db2-133">String</span><span class="sxs-lookup"><span data-stu-id="58db2-133">String</span></span>|<span data-ttu-id="58db2-134">设置类名和属性名。</span><span class="sxs-lookup"><span data-stu-id="58db2-134">The setting class name and property name.</span></span>|
|<span data-ttu-id="58db2-135">settingName</span><span class="sxs-lookup"><span data-stu-id="58db2-135">settingName</span></span>|<span data-ttu-id="58db2-136">String</span><span class="sxs-lookup"><span data-stu-id="58db2-136">String</span></span>|<span data-ttu-id="58db2-137">报告的设置名称</span><span class="sxs-lookup"><span data-stu-id="58db2-137">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="58db2-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="58db2-138">deviceId</span></span>|<span data-ttu-id="58db2-139">String</span><span class="sxs-lookup"><span data-stu-id="58db2-139">String</span></span>|<span data-ttu-id="58db2-140">报告的设备 ID</span><span class="sxs-lookup"><span data-stu-id="58db2-140">The Device Id that is being reported</span></span>|
|<span data-ttu-id="58db2-141">deviceName</span><span class="sxs-lookup"><span data-stu-id="58db2-141">deviceName</span></span>|<span data-ttu-id="58db2-142">String</span><span class="sxs-lookup"><span data-stu-id="58db2-142">String</span></span>|<span data-ttu-id="58db2-143">报告的设备名称</span><span class="sxs-lookup"><span data-stu-id="58db2-143">The Device Name that is being reported</span></span>|
|<span data-ttu-id="58db2-144">userId</span><span class="sxs-lookup"><span data-stu-id="58db2-144">userId</span></span>|<span data-ttu-id="58db2-145">String</span><span class="sxs-lookup"><span data-stu-id="58db2-145">String</span></span>|<span data-ttu-id="58db2-146">报告的用户 ID</span><span class="sxs-lookup"><span data-stu-id="58db2-146">The user Id that is being reported</span></span>|
|<span data-ttu-id="58db2-147">userEmail</span><span class="sxs-lookup"><span data-stu-id="58db2-147">userEmail</span></span>|<span data-ttu-id="58db2-148">String</span><span class="sxs-lookup"><span data-stu-id="58db2-148">String</span></span>|<span data-ttu-id="58db2-149">报告的用户电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="58db2-149">The User email address that is being reported</span></span>|
|<span data-ttu-id="58db2-150">userName</span><span class="sxs-lookup"><span data-stu-id="58db2-150">userName</span></span>|<span data-ttu-id="58db2-151">String</span><span class="sxs-lookup"><span data-stu-id="58db2-151">String</span></span>|<span data-ttu-id="58db2-152">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="58db2-152">The User Name that is being reported</span></span>|
|<span data-ttu-id="58db2-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="58db2-153">userPrincipalName</span></span>|<span data-ttu-id="58db2-154">String</span><span class="sxs-lookup"><span data-stu-id="58db2-154">String</span></span>|<span data-ttu-id="58db2-155">报告的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="58db2-155">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="58db2-156">deviceModel</span><span class="sxs-lookup"><span data-stu-id="58db2-156">deviceModel</span></span>|<span data-ttu-id="58db2-157">String</span><span class="sxs-lookup"><span data-stu-id="58db2-157">String</span></span>|<span data-ttu-id="58db2-158">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="58db2-158">The device model that is being reported</span></span>|
|<span data-ttu-id="58db2-159">state</span><span class="sxs-lookup"><span data-stu-id="58db2-159">state</span></span>|[<span data-ttu-id="58db2-160">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="58db2-160">complianceStatus</span></span>](../resources/intune_shared_compliancestatus.md)|<span data-ttu-id="58db2-161">设置合规性状态。</span><span class="sxs-lookup"><span data-stu-id="58db2-161">The compliance state of the setting Possible values are: , , , , , , .</span></span> <span data-ttu-id="58db2-162">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`。</span><span class="sxs-lookup"><span data-stu-id="58db2-162">The possible values are `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, , , , , or .</span></span>|
|<span data-ttu-id="58db2-163">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="58db2-163">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="58db2-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58db2-164">DateTimeOffset</span></span>|<span data-ttu-id="58db2-165">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="58db2-165">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="58db2-166">响应</span><span class="sxs-lookup"><span data-stu-id="58db2-166">Response</span></span>
<span data-ttu-id="58db2-167">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="58db2-167">If successful, this method returns a `201 Created` response code and a [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58db2-168">示例</span><span class="sxs-lookup"><span data-stu-id="58db2-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="58db2-169">请求</span><span class="sxs-lookup"><span data-stu-id="58db2-169">Request</span></span>
<span data-ttu-id="58db2-170">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="58db2-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
Content-type: application/json
Content-length: 517

{
  "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
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

### <a name="response"></a><span data-ttu-id="58db2-171">响应</span><span class="sxs-lookup"><span data-stu-id="58db2-171">Response</span></span>
<span data-ttu-id="58db2-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="58db2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



