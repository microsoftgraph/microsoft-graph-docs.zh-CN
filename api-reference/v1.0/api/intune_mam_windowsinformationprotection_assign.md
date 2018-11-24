# <a name="assign-action"></a><span data-ttu-id="ea7cb-101">assign 操作</span><span class="sxs-lookup"><span data-stu-id="ea7cb-101">assign action</span></span>

> <span data-ttu-id="ea7cb-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ea7cb-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ea7cb-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ea7cb-103">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ea7cb-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="ea7cb-104">Prerequisites</span></span>
<span data-ttu-id="ea7cb-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](../../../concepts/permissions_reference.md)。
</span><span class="sxs-lookup"><span data-stu-id="ea7cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ea7cb-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="ea7cb-107">Permission type</span></span>|<span data-ttu-id="ea7cb-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ea7cb-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea7cb-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ea7cb-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ea7cb-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea7cb-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ea7cb-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ea7cb-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea7cb-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="ea7cb-112">Not supported.</span></span>|
|<span data-ttu-id="ea7cb-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="ea7cb-113">Application</span></span>|<span data-ttu-id="ea7cb-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ea7cb-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea7cb-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ea7cb-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/assign
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}/assign
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="ea7cb-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="ea7cb-116">Request headers</span></span>
|<span data-ttu-id="ea7cb-117">标头</span><span class="sxs-lookup"><span data-stu-id="ea7cb-117">Header</span></span>|<span data-ttu-id="ea7cb-118">值</span><span class="sxs-lookup"><span data-stu-id="ea7cb-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea7cb-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea7cb-119">Authorization</span></span>|<span data-ttu-id="ea7cb-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ea7cb-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea7cb-121">Accept</span><span class="sxs-lookup"><span data-stu-id="ea7cb-121">Accept</span></span>|<span data-ttu-id="ea7cb-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ea7cb-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea7cb-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="ea7cb-123">Request body</span></span>
<span data-ttu-id="ea7cb-124">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ea7cb-124">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ea7cb-125">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="ea7cb-125">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ea7cb-126">属性</span><span class="sxs-lookup"><span data-stu-id="ea7cb-126">Property</span></span>|<span data-ttu-id="ea7cb-127">类型</span><span class="sxs-lookup"><span data-stu-id="ea7cb-127">Type</span></span>|<span data-ttu-id="ea7cb-128">说明</span><span class="sxs-lookup"><span data-stu-id="ea7cb-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea7cb-129">assignments</span><span class="sxs-lookup"><span data-stu-id="ea7cb-129">assignments</span></span>|<span data-ttu-id="ea7cb-130">[targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ea7cb-130">[targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="ea7cb-131">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ea7cb-131">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ea7cb-132">响应</span><span class="sxs-lookup"><span data-stu-id="ea7cb-132">Response</span></span>
<span data-ttu-id="ea7cb-133">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="ea7cb-133">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ea7cb-134">示例</span><span class="sxs-lookup"><span data-stu-id="ea7cb-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="ea7cb-135">请求</span><span class="sxs-lookup"><span data-stu-id="ea7cb-135">Request</span></span>
<span data-ttu-id="ea7cb-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ea7cb-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/assign

Content-type: application/json
Content-length: 282

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
      "id": "8b68c4a6-c4a6-8b68-a6c4-688ba6c4688b",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="ea7cb-137">响应</span><span class="sxs-lookup"><span data-stu-id="ea7cb-137">Response</span></span>
<span data-ttu-id="ea7cb-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ea7cb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



