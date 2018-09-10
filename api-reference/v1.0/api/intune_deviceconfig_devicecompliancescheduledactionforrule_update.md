# <a name="update-devicecompliancescheduledactionforrule"></a><span data-ttu-id="f0a6b-101">更新 deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="f0a6b-101">Update deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="f0a6b-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f0a6b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f0a6b-103">更新 [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f0a6b-103">Update the properties of a [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f0a6b-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="f0a6b-104">Prerequisites</span></span>
<span data-ttu-id="f0a6b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="f0a6b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f0a6b-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="f0a6b-107">Permission type</span></span>|<span data-ttu-id="f0a6b-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f0a6b-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0a6b-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f0a6b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="f0a6b-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0a6b-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f0a6b-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f0a6b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0a6b-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="f0a6b-112">Not supported.</span></span>|
|<span data-ttu-id="f0a6b-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="f0a6b-113">Application</span></span>|<span data-ttu-id="f0a6b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f0a6b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0a6b-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f0a6b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
```

## <a name="request-headers"></a><span data-ttu-id="f0a6b-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="f0a6b-116">Request headers</span></span>
|<span data-ttu-id="f0a6b-117">标头</span><span class="sxs-lookup"><span data-stu-id="f0a6b-117">Header</span></span>|<span data-ttu-id="f0a6b-118">值</span><span class="sxs-lookup"><span data-stu-id="f0a6b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f0a6b-119">授权</span><span class="sxs-lookup"><span data-stu-id="f0a6b-119">Authorization</span></span>|<span data-ttu-id="f0a6b-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f0a6b-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f0a6b-121">Accept</span><span class="sxs-lookup"><span data-stu-id="f0a6b-121">Accept</span></span>|<span data-ttu-id="f0a6b-122">application/json</span><span class="sxs-lookup"><span data-stu-id="f0a6b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0a6b-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="f0a6b-123">Request body</span></span>
<span data-ttu-id="f0a6b-124">在请求正文中，提供 [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f0a6b-124">In the request body, supply a JSON representation for the [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md) object.</span></span>

<span data-ttu-id="f0a6b-125">下表显示创建 [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f0a6b-125">The following table shows the properties that are required when you create the [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md).</span></span>

|<span data-ttu-id="f0a6b-126">属性</span><span class="sxs-lookup"><span data-stu-id="f0a6b-126">Property</span></span>|<span data-ttu-id="f0a6b-127">类型</span><span class="sxs-lookup"><span data-stu-id="f0a6b-127">Type</span></span>|<span data-ttu-id="f0a6b-128">说明</span><span class="sxs-lookup"><span data-stu-id="f0a6b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0a6b-129">ID</span><span class="sxs-lookup"><span data-stu-id="f0a6b-129">id</span></span>|<span data-ttu-id="f0a6b-130">字符串</span><span class="sxs-lookup"><span data-stu-id="f0a6b-130">String</span></span>|<span data-ttu-id="f0a6b-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f0a6b-131">Key of the entity.</span></span>|
|<span data-ttu-id="f0a6b-132">ruleName</span><span class="sxs-lookup"><span data-stu-id="f0a6b-132">ruleName</span></span>|<span data-ttu-id="f0a6b-133">String</span><span class="sxs-lookup"><span data-stu-id="f0a6b-133">String</span></span>|<span data-ttu-id="f0a6b-134">此计划操作适用的规则名称。</span><span class="sxs-lookup"><span data-stu-id="f0a6b-134">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="f0a6b-135">响应</span><span class="sxs-lookup"><span data-stu-id="f0a6b-135">Response</span></span>
<span data-ttu-id="f0a6b-136">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f0a6b-136">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0a6b-137">示例</span><span class="sxs-lookup"><span data-stu-id="f0a6b-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="f0a6b-138">请求</span><span class="sxs-lookup"><span data-stu-id="f0a6b-138">Request</span></span>
<span data-ttu-id="f0a6b-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f0a6b-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
Content-type: application/json
Content-length: 37

{
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="f0a6b-140">响应</span><span class="sxs-lookup"><span data-stu-id="f0a6b-140">Response</span></span>
<span data-ttu-id="f0a6b-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f0a6b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 163

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "id": "f0075d5e-5d5e-f007-5e5d-07f05e5d07f0",
  "ruleName": "Rule Name value"
}
```








