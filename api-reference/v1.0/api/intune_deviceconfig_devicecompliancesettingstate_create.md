# <a name="create-devicecompliancesettingstate"></a><span data-ttu-id="62f9c-101">创建 deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="62f9c-101">Create deviceComplianceSettingState</span></span>

> <span data-ttu-id="62f9c-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="62f9c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="62f9c-103">创建新的 [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="62f9c-103">Create a new [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="62f9c-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="62f9c-104">Prerequisites</span></span>
<span data-ttu-id="62f9c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="62f9c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="62f9c-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="62f9c-107">Permission type</span></span>|<span data-ttu-id="62f9c-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="62f9c-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="62f9c-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="62f9c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="62f9c-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62f9c-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="62f9c-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="62f9c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="62f9c-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="62f9c-112">Not supported.</span></span>|
|<span data-ttu-id="62f9c-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="62f9c-113">Application</span></span>|<span data-ttu-id="62f9c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="62f9c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="62f9c-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="62f9c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="62f9c-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="62f9c-116">Request headers</span></span>
|<span data-ttu-id="62f9c-117">标头</span><span class="sxs-lookup"><span data-stu-id="62f9c-117">Header</span></span>|<span data-ttu-id="62f9c-118">值</span><span class="sxs-lookup"><span data-stu-id="62f9c-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="62f9c-119">授权</span><span class="sxs-lookup"><span data-stu-id="62f9c-119">Authorization</span></span>|<span data-ttu-id="62f9c-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="62f9c-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="62f9c-121">接受</span><span class="sxs-lookup"><span data-stu-id="62f9c-121">Accept</span></span>|<span data-ttu-id="62f9c-122">application/json</span><span class="sxs-lookup"><span data-stu-id="62f9c-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="62f9c-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="62f9c-123">Request body</span></span>
<span data-ttu-id="62f9c-124">在请求正文中，提供 deviceComplianceSettingState 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="62f9c-124">In the request body, supply a JSON representation for the deviceComplianceSettingState object.</span></span>

<span data-ttu-id="62f9c-125">下表显示了创建 deviceComplianceSettingState 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="62f9c-125">The following table shows the properties that are required when you create the deviceComplianceSettingState.</span></span>

|<span data-ttu-id="62f9c-126">属性</span><span class="sxs-lookup"><span data-stu-id="62f9c-126">Property</span></span>|<span data-ttu-id="62f9c-127">类型</span><span class="sxs-lookup"><span data-stu-id="62f9c-127">Type</span></span>|<span data-ttu-id="62f9c-128">说明</span><span class="sxs-lookup"><span data-stu-id="62f9c-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62f9c-129">ID</span><span class="sxs-lookup"><span data-stu-id="62f9c-129">id</span></span>|<span data-ttu-id="62f9c-130">字符串</span><span class="sxs-lookup"><span data-stu-id="62f9c-130">String</span></span>|<span data-ttu-id="62f9c-131">实体的键</span><span class="sxs-lookup"><span data-stu-id="62f9c-131">Key of the entity</span></span>|
|<span data-ttu-id="62f9c-132">setting</span><span class="sxs-lookup"><span data-stu-id="62f9c-132">setting</span></span>|<span data-ttu-id="62f9c-133">字符串</span><span class="sxs-lookup"><span data-stu-id="62f9c-133">String</span></span>|<span data-ttu-id="62f9c-134">设置类名和属性名。</span><span class="sxs-lookup"><span data-stu-id="62f9c-134">The setting class name and property name.</span></span>|
|<span data-ttu-id="62f9c-135">settingName</span><span class="sxs-lookup"><span data-stu-id="62f9c-135">settingName</span></span>|<span data-ttu-id="62f9c-136">字符串</span><span class="sxs-lookup"><span data-stu-id="62f9c-136">String</span></span>|<span data-ttu-id="62f9c-137">报告的设置名称</span><span class="sxs-lookup"><span data-stu-id="62f9c-137">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="62f9c-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="62f9c-138">deviceId</span></span>|<span data-ttu-id="62f9c-139">字符串</span><span class="sxs-lookup"><span data-stu-id="62f9c-139">String</span></span>|<span data-ttu-id="62f9c-140">报告的设备 ID</span><span class="sxs-lookup"><span data-stu-id="62f9c-140">The Device Id that is being reported</span></span>|
|<span data-ttu-id="62f9c-141">deviceName</span><span class="sxs-lookup"><span data-stu-id="62f9c-141">deviceName</span></span>|<span data-ttu-id="62f9c-142">字符串</span><span class="sxs-lookup"><span data-stu-id="62f9c-142">String</span></span>|<span data-ttu-id="62f9c-143">报告的设备名称</span><span class="sxs-lookup"><span data-stu-id="62f9c-143">The Device Name that is being reported</span></span>|
|<span data-ttu-id="62f9c-144">userId</span><span class="sxs-lookup"><span data-stu-id="62f9c-144">userId</span></span>|<span data-ttu-id="62f9c-145">字符串</span><span class="sxs-lookup"><span data-stu-id="62f9c-145">String</span></span>|<span data-ttu-id="62f9c-146">报告的用户 ID</span><span class="sxs-lookup"><span data-stu-id="62f9c-146">The user Id that is being reported</span></span>|
|<span data-ttu-id="62f9c-147">userEmail</span><span class="sxs-lookup"><span data-stu-id="62f9c-147">userEmail</span></span>|<span data-ttu-id="62f9c-148">字符串</span><span class="sxs-lookup"><span data-stu-id="62f9c-148">String</span></span>|<span data-ttu-id="62f9c-149">报告的用户电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="62f9c-149">The User email address that is being reported</span></span>|
|<span data-ttu-id="62f9c-150">userName</span><span class="sxs-lookup"><span data-stu-id="62f9c-150">userName</span></span>|<span data-ttu-id="62f9c-151">字符串</span><span class="sxs-lookup"><span data-stu-id="62f9c-151">String</span></span>|<span data-ttu-id="62f9c-152">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="62f9c-152">The User Name that is being reported</span></span>|
|<span data-ttu-id="62f9c-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="62f9c-153">userPrincipalName</span></span>|<span data-ttu-id="62f9c-154">字符串</span><span class="sxs-lookup"><span data-stu-id="62f9c-154">String</span></span>|<span data-ttu-id="62f9c-155">报告的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="62f9c-155">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="62f9c-156">deviceModel</span><span class="sxs-lookup"><span data-stu-id="62f9c-156">deviceModel</span></span>|<span data-ttu-id="62f9c-157">字符串</span><span class="sxs-lookup"><span data-stu-id="62f9c-157">String</span></span>|<span data-ttu-id="62f9c-158">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="62f9c-158">The device model that is being reported</span></span>|
|<span data-ttu-id="62f9c-159">state</span><span class="sxs-lookup"><span data-stu-id="62f9c-159">state</span></span>|[<span data-ttu-id="62f9c-160">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="62f9c-160">complianceStatus</span></span>](../resources/intune_shared_compliancestatus.md)|<span data-ttu-id="62f9c-p102">设置的合规性状态。可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="62f9c-p102">The compliance state of the setting Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="62f9c-163">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="62f9c-163">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="62f9c-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62f9c-164">DateTimeOffset</span></span>|<span data-ttu-id="62f9c-165">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="62f9c-165">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="62f9c-166">响应</span><span class="sxs-lookup"><span data-stu-id="62f9c-166">Response</span></span>
<span data-ttu-id="62f9c-167">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="62f9c-167">If successful, this method returns a `201 Created` response code and a [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62f9c-168">示例</span><span class="sxs-lookup"><span data-stu-id="62f9c-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="62f9c-169">请求</span><span class="sxs-lookup"><span data-stu-id="62f9c-169">Request</span></span>
<span data-ttu-id="62f9c-170">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="62f9c-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="62f9c-171">响应</span><span class="sxs-lookup"><span data-stu-id="62f9c-171">Response</span></span>
<span data-ttu-id="62f9c-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="62f9c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








