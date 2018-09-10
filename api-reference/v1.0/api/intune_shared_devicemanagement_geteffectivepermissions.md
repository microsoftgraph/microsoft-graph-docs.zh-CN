# <a name="geteffectivepermissions-function"></a><span data-ttu-id="89664-101">getEffectivePermissions 函数</span><span class="sxs-lookup"><span data-stu-id="89664-101">getEffectivePermissions function</span></span>

> <span data-ttu-id="89664-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="89664-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="89664-103">检索当前验证的用户的有效权限</span><span class="sxs-lookup"><span data-stu-id="89664-103">Retrieves the effective permissions of the currently authenticated user</span></span>

## <a name="prerequisites"></a><span data-ttu-id="89664-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="89664-104">Prerequisites</span></span>
<span data-ttu-id="89664-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="89664-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="89664-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="89664-107">Permission type</span></span>|<span data-ttu-id="89664-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="89664-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89664-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="89664-109">Delegated (work or school account)</span></span>|<span data-ttu-id="89664-110">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="89664-110">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="89664-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="89664-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89664-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="89664-112">Not supported.</span></span>|
|<span data-ttu-id="89664-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="89664-113">Application</span></span>|<span data-ttu-id="89664-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="89664-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="89664-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="89664-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getEffectivePermissions
```

## <a name="request-headers"></a><span data-ttu-id="89664-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="89664-116">Request headers</span></span>
|<span data-ttu-id="89664-117">标头</span><span class="sxs-lookup"><span data-stu-id="89664-117">Header</span></span>|<span data-ttu-id="89664-118">值</span><span class="sxs-lookup"><span data-stu-id="89664-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89664-119">授权</span><span class="sxs-lookup"><span data-stu-id="89664-119">Authorization</span></span>|<span data-ttu-id="89664-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="89664-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89664-121">Accept</span><span class="sxs-lookup"><span data-stu-id="89664-121">Accept</span></span>|<span data-ttu-id="89664-122">application/json</span><span class="sxs-lookup"><span data-stu-id="89664-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89664-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="89664-123">Request body</span></span>
<span data-ttu-id="89664-124">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="89664-124">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="89664-125">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="89664-125">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="89664-126">属性</span><span class="sxs-lookup"><span data-stu-id="89664-126">Property</span></span>|<span data-ttu-id="89664-127">类型</span><span class="sxs-lookup"><span data-stu-id="89664-127">Type</span></span>|<span data-ttu-id="89664-128">说明</span><span class="sxs-lookup"><span data-stu-id="89664-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89664-129">scope</span><span class="sxs-lookup"><span data-stu-id="89664-129">scope</span></span>|<span data-ttu-id="89664-130">字符串</span><span class="sxs-lookup"><span data-stu-id="89664-130">String</span></span>|<span data-ttu-id="89664-131">尚未记录</span><span class="sxs-lookup"><span data-stu-id="89664-131">Not yet documented</span></span>|


## <a name="response"></a><span data-ttu-id="89664-132">响应</span><span class="sxs-lookup"><span data-stu-id="89664-132">Response</span></span>
<span data-ttu-id="89664-133">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 [rolePermission](../resources/intune_rbac_rolepermission.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="89664-133">If successful, this function returns a `200 OK` response code and a [rolePermission](../resources/intune_rbac_rolepermission.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89664-134">示例</span><span class="sxs-lookup"><span data-stu-id="89664-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="89664-135">请求</span><span class="sxs-lookup"><span data-stu-id="89664-135">Request</span></span>
<span data-ttu-id="89664-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="89664-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/getEffectivePermissions(scope='parameterValue')
```

### <a name="response"></a><span data-ttu-id="89664-137">响应</span><span class="sxs-lookup"><span data-stu-id="89664-137">Response</span></span>
<span data-ttu-id="89664-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="89664-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 471

{
  "value": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "actions": [
        "Actions value"
      ],
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "Allowed Resource Actions value"
          ],
          "notAllowedResourceActions": [
            "Not Allowed Resource Actions value"
          ]
        }
      ]
    }
  ]
}
```



