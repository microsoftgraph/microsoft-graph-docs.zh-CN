# <a name="list-auditevents"></a><span data-ttu-id="f0462-101">列出 auditEvents</span><span class="sxs-lookup"><span data-stu-id="f0462-101">List auditEvents</span></span>

> <span data-ttu-id="f0462-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f0462-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f0462-103">列出 [auditEvent](../resources/intune_auditing_auditevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f0462-103">List properties and relationships of the [auditEvent](../resources/intune_auditing_auditevent.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f0462-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="f0462-104">Prerequisites</span></span>
<span data-ttu-id="f0462-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="f0462-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f0462-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="f0462-107">Permission type</span></span>|<span data-ttu-id="f0462-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f0462-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0462-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f0462-109">Delegated (work or school account)</span></span>|<span data-ttu-id="f0462-110">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f0462-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f0462-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f0462-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0462-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="f0462-112">Not supported.</span></span>|
|<span data-ttu-id="f0462-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="f0462-113">Application</span></span>|<span data-ttu-id="f0462-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f0462-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0462-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f0462-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents
```

## <a name="request-headers"></a><span data-ttu-id="f0462-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="f0462-116">Request headers</span></span>
|<span data-ttu-id="f0462-117">标头</span><span class="sxs-lookup"><span data-stu-id="f0462-117">Header</span></span>|<span data-ttu-id="f0462-118">值</span><span class="sxs-lookup"><span data-stu-id="f0462-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f0462-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0462-119">Authorization</span></span>|<span data-ttu-id="f0462-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f0462-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f0462-121">Accept</span><span class="sxs-lookup"><span data-stu-id="f0462-121">Accept</span></span>|<span data-ttu-id="f0462-122">application/json</span><span class="sxs-lookup"><span data-stu-id="f0462-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0462-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="f0462-123">Request body</span></span>
<span data-ttu-id="f0462-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f0462-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f0462-125">响应</span><span class="sxs-lookup"><span data-stu-id="f0462-125">Response</span></span>
<span data-ttu-id="f0462-126">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [auditEvent](../resources/intune_auditing_auditevent.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f0462-126">If successful, this method returns a `200 OK` response code and a collection of [auditEvent](../resources/intune_auditing_auditevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0462-127">示例</span><span class="sxs-lookup"><span data-stu-id="f0462-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="f0462-128">请求</span><span class="sxs-lookup"><span data-stu-id="f0462-128">Request</span></span>
<span data-ttu-id="f0462-129">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f0462-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents
```

### <a name="response"></a><span data-ttu-id="f0462-130">响应</span><span class="sxs-lookup"><span data-stu-id="f0462-130">Response</span></span>
<span data-ttu-id="f0462-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f0462-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1632

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.auditEvent",
      "id": "59653ce8-3ce8-5965-e83c-6559e83c6559",
      "displayName": "Display Name value",
      "componentName": "Component Name value",
      "actor": {
        "@odata.type": "microsoft.graph.auditActor",
        "type": "Type value",
        "userPermissions": [
          "User Permissions value"
        ],
        "applicationId": "Application Id value",
        "applicationDisplayName": "Application Display Name value",
        "userPrincipalName": "User Principal Name value",
        "servicePrincipalName": "Service Principal Name value",
        "ipAddress": "Ip Address value",
        "userId": "User Id value"
      },
      "activity": "Activity value",
      "activityDateTime": "2016-12-31T23:59:51.6363086-08:00",
      "activityType": "Activity Type value",
      "activityOperationType": "Activity Operation Type value",
      "activityResult": "Activity Result value",
      "correlationId": "52effe71-fe71-52ef-71fe-ef5271feef52",
      "resources": [
        {
          "@odata.type": "microsoft.graph.auditResource",
          "displayName": "Display Name value",
          "modifiedProperties": [
            {
              "@odata.type": "microsoft.graph.auditProperty",
              "displayName": "Display Name value",
              "oldValue": "Old Value value",
              "newValue": "New Value value"
            }
          ],
          "type": "Type value",
          "resourceId": "Resource Id value"
        }
      ],
      "category": "Category value"
    }
  ]
}
```



