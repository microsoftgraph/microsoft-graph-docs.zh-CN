# <a name="list-devicecomplianceactionitems"></a><span data-ttu-id="03d88-101">列出 deviceComplianceActionItems</span><span class="sxs-lookup"><span data-stu-id="03d88-101">List deviceComplianceActionItems</span></span>

> <span data-ttu-id="03d88-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="03d88-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="03d88-103">列出 [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="03d88-103">List properties and relationships of the [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="03d88-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="03d88-104">Prerequisites</span></span>
<span data-ttu-id="03d88-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="03d88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="03d88-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="03d88-107">Permission type</span></span>|<span data-ttu-id="03d88-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="03d88-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03d88-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="03d88-109">Delegated (work or school account)</span></span>|<span data-ttu-id="03d88-110">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="03d88-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="03d88-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="03d88-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03d88-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="03d88-112">Not supported.</span></span>|
|<span data-ttu-id="03d88-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="03d88-113">Application</span></span>|<span data-ttu-id="03d88-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="03d88-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="03d88-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="03d88-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="03d88-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="03d88-116">Request headers</span></span>
|<span data-ttu-id="03d88-117">标头</span><span class="sxs-lookup"><span data-stu-id="03d88-117">Header</span></span>|<span data-ttu-id="03d88-118">值</span><span class="sxs-lookup"><span data-stu-id="03d88-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03d88-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="03d88-119">Authorization</span></span>|<span data-ttu-id="03d88-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="03d88-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03d88-121">Accept</span><span class="sxs-lookup"><span data-stu-id="03d88-121">Accept</span></span>|<span data-ttu-id="03d88-122">application/json</span><span class="sxs-lookup"><span data-stu-id="03d88-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03d88-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="03d88-123">Request body</span></span>
<span data-ttu-id="03d88-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="03d88-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="03d88-125">响应</span><span class="sxs-lookup"><span data-stu-id="03d88-125">Response</span></span>
<span data-ttu-id="03d88-126">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="03d88-126">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03d88-127">示例</span><span class="sxs-lookup"><span data-stu-id="03d88-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="03d88-128">请求</span><span class="sxs-lookup"><span data-stu-id="03d88-128">Request</span></span>
<span data-ttu-id="03d88-129">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="03d88-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

### <a name="response"></a><span data-ttu-id="03d88-130">响应</span><span class="sxs-lookup"><span data-stu-id="03d88-130">Response</span></span>
<span data-ttu-id="03d88-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="03d88-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 385

{
  "value": [
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
  ]
}
```



