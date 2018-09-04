# <a name="update-devicecomplianceactionitem"></a><span data-ttu-id="ef434-101">更新 deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="ef434-101">Update deviceComplianceActionItem</span></span>

> <span data-ttu-id="ef434-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ef434-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ef434-103">更新 [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ef434-103">Update the properties of a [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ef434-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="ef434-104">Prerequisites</span></span>
<span data-ttu-id="ef434-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="ef434-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ef434-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="ef434-107">Permission type</span></span>|<span data-ttu-id="ef434-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ef434-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef434-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ef434-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ef434-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef434-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ef434-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ef434-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef434-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="ef434-112">Not supported.</span></span>|
|<span data-ttu-id="ef434-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="ef434-113">Application</span></span>|<span data-ttu-id="ef434-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ef434-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef434-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ef434-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## <a name="request-headers"></a><span data-ttu-id="ef434-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="ef434-116">Request headers</span></span>
|<span data-ttu-id="ef434-117">标头</span><span class="sxs-lookup"><span data-stu-id="ef434-117">Header</span></span>|<span data-ttu-id="ef434-118">值</span><span class="sxs-lookup"><span data-stu-id="ef434-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef434-119">授权</span><span class="sxs-lookup"><span data-stu-id="ef434-119">Authorization</span></span>|<span data-ttu-id="ef434-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ef434-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef434-121">接受</span><span class="sxs-lookup"><span data-stu-id="ef434-121">Accept</span></span>|<span data-ttu-id="ef434-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ef434-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef434-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="ef434-123">Request body</span></span>
<span data-ttu-id="ef434-124">在请求正文中，提供 [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ef434-124">In the request body, supply a JSON representation for the [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md) object.</span></span>

<span data-ttu-id="ef434-125">下表显示了创建 [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ef434-125">The following table shows the properties that are required when you create the [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md).</span></span>

|<span data-ttu-id="ef434-126">属性</span><span class="sxs-lookup"><span data-stu-id="ef434-126">Property</span></span>|<span data-ttu-id="ef434-127">类型</span><span class="sxs-lookup"><span data-stu-id="ef434-127">Type</span></span>|<span data-ttu-id="ef434-128">说明</span><span class="sxs-lookup"><span data-stu-id="ef434-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef434-129">id</span><span class="sxs-lookup"><span data-stu-id="ef434-129">id</span></span>|<span data-ttu-id="ef434-130">字符串</span><span class="sxs-lookup"><span data-stu-id="ef434-130">String</span></span>|<span data-ttu-id="ef434-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ef434-131">Key of the entity.</span></span>|
|<span data-ttu-id="ef434-132">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="ef434-132">gracePeriodHours</span></span>|<span data-ttu-id="ef434-133">Int32</span><span class="sxs-lookup"><span data-stu-id="ef434-133">Int32</span></span>|<span data-ttu-id="ef434-134">强制执行操作前要等待的小时数。</span><span class="sxs-lookup"><span data-stu-id="ef434-134">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="ef434-135">有效值为 0 至 8760</span><span class="sxs-lookup"><span data-stu-id="ef434-135">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="ef434-136">actionType</span><span class="sxs-lookup"><span data-stu-id="ef434-136">actionType</span></span>|[<span data-ttu-id="ef434-137">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="ef434-137">deviceComplianceActionType</span></span>](../resources/intune_deviceconfig_devicecomplianceactiontype.md)|<span data-ttu-id="ef434-138">采取什么操作。</span><span class="sxs-lookup"><span data-stu-id="ef434-138">What action to take.</span></span> <span data-ttu-id="ef434-139">可取值为：`noAction`、`notification`、`block`、`retire`、`wipe`、`removeResourceAccessProfiles`。</span><span class="sxs-lookup"><span data-stu-id="ef434-139">The possible values are `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, , , , , , or .</span></span>|
|<span data-ttu-id="ef434-140">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="ef434-140">notificationTemplateId</span></span>|<span data-ttu-id="ef434-141">String</span><span class="sxs-lookup"><span data-stu-id="ef434-141">String</span></span>|<span data-ttu-id="ef434-142">要使用的通知消息模板</span><span class="sxs-lookup"><span data-stu-id="ef434-142">What notification Message template to use</span></span>|
|<span data-ttu-id="ef434-143">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="ef434-143">notificationMessageCCList</span></span>|<span data-ttu-id="ef434-144">String 集合</span><span class="sxs-lookup"><span data-stu-id="ef434-144">String collection</span></span>|<span data-ttu-id="ef434-145">指定此通知邮件抄送对象的组 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="ef434-145">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="ef434-146">响应</span><span class="sxs-lookup"><span data-stu-id="ef434-146">Response</span></span>
<span data-ttu-id="ef434-147">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ef434-147">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef434-148">示例</span><span class="sxs-lookup"><span data-stu-id="ef434-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="ef434-149">请求</span><span class="sxs-lookup"><span data-stu-id="ef434-149">Request</span></span>
<span data-ttu-id="ef434-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ef434-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
Content-type: application/json
Content-length: 206

{
  "gracePeriodHours": 0,
  "actionType": "notification",
  "notificationTemplateId": "Notification Template Id value",
  "notificationMessageCCList": [
    "Notification Message CCList value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="ef434-151">响应</span><span class="sxs-lookup"><span data-stu-id="ef434-151">Response</span></span>
<span data-ttu-id="ef434-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ef434-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 320

{
  "@odata.type": "#microsoft.graph.deviceComplianceActionItem",
  "id": "e01a1893-1893-e01a-9318-1ae093181ae0",
  "gracePeriodHours": 0,
  "actionType": "notification",
  "notificationTemplateId": "Notification Template Id value",
  "notificationMessageCCList": [
    "Notification Message CCList value"
  ]
}
```



