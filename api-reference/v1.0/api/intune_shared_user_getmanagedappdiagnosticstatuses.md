# <a name="getmanagedappdiagnosticstatuses-function"></a><span data-ttu-id="80eef-101">getManagedAppDiagnosticStatuses 函数</span><span class="sxs-lookup"><span data-stu-id="80eef-101">getManagedAppDiagnosticStatuses function</span></span>

> <span data-ttu-id="80eef-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="80eef-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="80eef-103">获取给定用户的诊断验证状态。</span><span class="sxs-lookup"><span data-stu-id="80eef-103">Gets diagnostics validation status for a given user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="80eef-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="80eef-104">Prerequisites</span></span>
<span data-ttu-id="80eef-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="80eef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="80eef-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="80eef-107">Permission type</span></span>|<span data-ttu-id="80eef-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="80eef-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80eef-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="80eef-109">Delegated (work or school account)</span></span>| <span data-ttu-id="80eef-110">_因上下文而异_</span><span class="sxs-lookup"><span data-stu-id="80eef-110">_varies by context_</span></span>|
| <span data-ttu-id="80eef-111">&nbsp; &nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="80eef-111">.mam</span></span> | <span data-ttu-id="80eef-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="80eef-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
|<span data-ttu-id="80eef-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="80eef-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80eef-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="80eef-114">Not supported.</span></span>|
|<span data-ttu-id="80eef-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="80eef-115">Application</span></span>|<span data-ttu-id="80eef-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="80eef-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="80eef-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="80eef-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppDiagnosticStatuses
```

## <a name="request-headers"></a><span data-ttu-id="80eef-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="80eef-118">Request headers</span></span>
|<span data-ttu-id="80eef-119">标头</span><span class="sxs-lookup"><span data-stu-id="80eef-119">Header</span></span>|<span data-ttu-id="80eef-120">值</span><span class="sxs-lookup"><span data-stu-id="80eef-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="80eef-121">授权</span><span class="sxs-lookup"><span data-stu-id="80eef-121">Authorization</span></span>|<span data-ttu-id="80eef-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="80eef-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="80eef-123">接受</span><span class="sxs-lookup"><span data-stu-id="80eef-123">Accept</span></span>|<span data-ttu-id="80eef-124">application/json</span><span class="sxs-lookup"><span data-stu-id="80eef-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80eef-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="80eef-125">Request body</span></span>
<span data-ttu-id="80eef-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="80eef-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="80eef-127">响应</span><span class="sxs-lookup"><span data-stu-id="80eef-127">Response</span></span>
<span data-ttu-id="80eef-128">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 [managedAppDiagnosticStatus](../resources/intune_mam_managedappdiagnosticstatus.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="80eef-128">If successful, this function returns a `200 OK` response code and a [managedAppDiagnosticStatus](../resources/intune_mam_managedappdiagnosticstatus.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80eef-129">示例</span><span class="sxs-lookup"><span data-stu-id="80eef-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="80eef-130">请求</span><span class="sxs-lookup"><span data-stu-id="80eef-130">Request</span></span>
<span data-ttu-id="80eef-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="80eef-131">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}/getManagedAppDiagnosticStatuses
```

### <a name="response"></a><span data-ttu-id="80eef-132">响应</span><span class="sxs-lookup"><span data-stu-id="80eef-132">Response</span></span>
<span data-ttu-id="80eef-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="80eef-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 249

{
  "value": [
    {
      "@odata.type": "microsoft.graph.managedAppDiagnosticStatus",
      "validationName": "Validation Name value",
      "state": "State value",
      "mitigationInstruction": "Mitigation Instruction value"
    }
  ]
}
```



