# <a name="create-devicecompliancescheduledactionforrule"></a><span data-ttu-id="801d9-101">创建 deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="801d9-101">Create deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="801d9-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="801d9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="801d9-103">创建新的 [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="801d9-103">Create a new [plannerBucket](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="801d9-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="801d9-104">Prerequisites</span></span>
<span data-ttu-id="801d9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="801d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="801d9-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="801d9-107">Permission type</span></span>|<span data-ttu-id="801d9-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="801d9-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="801d9-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="801d9-109">Delegated (work or school account)</span></span>|<span data-ttu-id="801d9-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="801d9-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="801d9-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="801d9-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="801d9-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="801d9-112">Not supported.</span></span>|
|<span data-ttu-id="801d9-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="801d9-113">Application</span></span>|<span data-ttu-id="801d9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="801d9-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="801d9-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="801d9-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
```

## <a name="request-headers"></a><span data-ttu-id="801d9-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="801d9-116">Request headers</span></span>
|<span data-ttu-id="801d9-117">标头</span><span class="sxs-lookup"><span data-stu-id="801d9-117">Header</span></span>|<span data-ttu-id="801d9-118">值</span><span class="sxs-lookup"><span data-stu-id="801d9-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="801d9-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="801d9-119">Authorization</span></span>|<span data-ttu-id="801d9-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="801d9-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="801d9-121">Accept</span><span class="sxs-lookup"><span data-stu-id="801d9-121">Accept</span></span>|<span data-ttu-id="801d9-122">application/json</span><span class="sxs-lookup"><span data-stu-id="801d9-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="801d9-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="801d9-123">Request body</span></span>
<span data-ttu-id="801d9-124">在请求正文中，提供 deviceComplianceScheduledActionForRule 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="801d9-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="801d9-125">下表显示创建 deviceComplianceScheduledActionForRule 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="801d9-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="801d9-126">属性</span><span class="sxs-lookup"><span data-stu-id="801d9-126">Property</span></span>|<span data-ttu-id="801d9-127">类型</span><span class="sxs-lookup"><span data-stu-id="801d9-127">Type</span></span>|<span data-ttu-id="801d9-128">说明</span><span class="sxs-lookup"><span data-stu-id="801d9-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="801d9-129">id</span><span class="sxs-lookup"><span data-stu-id="801d9-129">id</span></span>|<span data-ttu-id="801d9-130">String</span><span class="sxs-lookup"><span data-stu-id="801d9-130">String</span></span>|<span data-ttu-id="801d9-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="801d9-131">Key of the setting.</span></span>|
|<span data-ttu-id="801d9-132">ruleName</span><span class="sxs-lookup"><span data-stu-id="801d9-132">ruleName</span></span>|<span data-ttu-id="801d9-133">String</span><span class="sxs-lookup"><span data-stu-id="801d9-133">String</span></span>|<span data-ttu-id="801d9-134">此计划操作适用的规则名称。</span><span class="sxs-lookup"><span data-stu-id="801d9-134">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="801d9-135">响应</span><span class="sxs-lookup"><span data-stu-id="801d9-135">Response</span></span>
<span data-ttu-id="801d9-136">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="801d9-136">If successful, this method returns a `201 Created` response code and a [directoryObject](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="801d9-137">示例</span><span class="sxs-lookup"><span data-stu-id="801d9-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="801d9-138">请求</span><span class="sxs-lookup"><span data-stu-id="801d9-138">Request</span></span>
<span data-ttu-id="801d9-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="801d9-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="801d9-140">响应</span><span class="sxs-lookup"><span data-stu-id="801d9-140">Response</span></span>
<span data-ttu-id="801d9-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="801d9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 163

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "id": "f0075d5e-5d5e-f007-5e5d-07f05e5d07f0",
  "ruleName": "Rule Name value"
}
```



