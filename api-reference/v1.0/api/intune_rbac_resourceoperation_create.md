# <a name="create-resourceoperation"></a><span data-ttu-id="8ad5f-101">创建 resourceOperation</span><span class="sxs-lookup"><span data-stu-id="8ad5f-101">Create resourceOperation</span></span>

> <span data-ttu-id="8ad5f-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="8ad5f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8ad5f-103">创建新的 [resourceOperation](../resources/intune_rbac_resourceoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8ad5f-103">Create a new [plannerBucket](../resources/intune_rbac_resourceoperation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8ad5f-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="8ad5f-104">Prerequisites</span></span>
<span data-ttu-id="8ad5f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="8ad5f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8ad5f-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="8ad5f-107">Permission type</span></span>|<span data-ttu-id="8ad5f-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8ad5f-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ad5f-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8ad5f-109">Delegated (work or school account)</span></span>|<span data-ttu-id="8ad5f-110">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ad5f-110">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="8ad5f-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8ad5f-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ad5f-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="8ad5f-112">Not supported.</span></span>|
|<span data-ttu-id="8ad5f-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="8ad5f-113">Application</span></span>|<span data-ttu-id="8ad5f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8ad5f-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ad5f-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8ad5f-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/resourceOperations
```

## <a name="request-headers"></a><span data-ttu-id="8ad5f-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="8ad5f-116">Request headers</span></span>
|<span data-ttu-id="8ad5f-117">标头</span><span class="sxs-lookup"><span data-stu-id="8ad5f-117">Header</span></span>|<span data-ttu-id="8ad5f-118">值</span><span class="sxs-lookup"><span data-stu-id="8ad5f-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8ad5f-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ad5f-119">Authorization</span></span>|<span data-ttu-id="8ad5f-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8ad5f-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8ad5f-121">Accept</span><span class="sxs-lookup"><span data-stu-id="8ad5f-121">Accept</span></span>|<span data-ttu-id="8ad5f-122">application/json</span><span class="sxs-lookup"><span data-stu-id="8ad5f-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ad5f-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="8ad5f-123">Request body</span></span>
<span data-ttu-id="8ad5f-124">在请求正文中，提供 resourceOperation 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8ad5f-124">In the request body, supply a JSON representation of Table object.</span></span>

<span data-ttu-id="8ad5f-125">下表显示创建 resourceOperation 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8ad5f-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="8ad5f-126">属性</span><span class="sxs-lookup"><span data-stu-id="8ad5f-126">Property</span></span>|<span data-ttu-id="8ad5f-127">类型</span><span class="sxs-lookup"><span data-stu-id="8ad5f-127">Type</span></span>|<span data-ttu-id="8ad5f-128">说明</span><span class="sxs-lookup"><span data-stu-id="8ad5f-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ad5f-129">id</span><span class="sxs-lookup"><span data-stu-id="8ad5f-129">id</span></span>|<span data-ttu-id="8ad5f-130">String</span><span class="sxs-lookup"><span data-stu-id="8ad5f-130">String</span></span>|<span data-ttu-id="8ad5f-131">资源操作的键。</span><span class="sxs-lookup"><span data-stu-id="8ad5f-131">Key of the Resource Operation.</span></span> <span data-ttu-id="8ad5f-132">只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="8ad5f-132">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="8ad5f-133">resourceName</span><span class="sxs-lookup"><span data-stu-id="8ad5f-133">resourceName</span></span>|<span data-ttu-id="8ad5f-134">String</span><span class="sxs-lookup"><span data-stu-id="8ad5f-134">String</span></span>|<span data-ttu-id="8ad5f-135">执行此操作的资源的名称。</span><span class="sxs-lookup"><span data-stu-id="8ad5f-135">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="8ad5f-136">actionName</span><span class="sxs-lookup"><span data-stu-id="8ad5f-136">ActionName</span></span>|<span data-ttu-id="8ad5f-137">String</span><span class="sxs-lookup"><span data-stu-id="8ad5f-137">String</span></span>|<span data-ttu-id="8ad5f-138">此操作将执行的操作类型。</span><span class="sxs-lookup"><span data-stu-id="8ad5f-138">Type of action this operation is going to perform.</span></span> <span data-ttu-id="8ad5f-139">actionName 应简明，并尽可能限制在几个字以内。</span><span class="sxs-lookup"><span data-stu-id="8ad5f-139">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="8ad5f-140">description</span><span class="sxs-lookup"><span data-stu-id="8ad5f-140">description</span></span>|<span data-ttu-id="8ad5f-141">String</span><span class="sxs-lookup"><span data-stu-id="8ad5f-141">String</span></span>|<span data-ttu-id="8ad5f-142">资源操作的说明。</span><span class="sxs-lookup"><span data-stu-id="8ad5f-142">Description of the resource operation.</span></span> <span data-ttu-id="8ad5f-143">当在 Azure 门户中显示时，会在操作的鼠标悬停文本中使用说明。</span><span class="sxs-lookup"><span data-stu-id="8ad5f-143">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|



## <a name="response"></a><span data-ttu-id="8ad5f-144">响应</span><span class="sxs-lookup"><span data-stu-id="8ad5f-144">Response</span></span>
<span data-ttu-id="8ad5f-145">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [resourceOperation](../resources/intune_rbac_resourceoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8ad5f-145">If successful, this method returns a `201 Created` response code and [plannerBucketTaskBoardTaskFormat](../resources/intune_rbac_resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ad5f-146">示例</span><span class="sxs-lookup"><span data-stu-id="8ad5f-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="8ad5f-147">请求</span><span class="sxs-lookup"><span data-stu-id="8ad5f-147">Request</span></span>
<span data-ttu-id="8ad5f-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8ad5f-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/resourceOperations
Content-type: application/json
Content-length: 178

{
  "@odata.type": "#microsoft.graph.resourceOperation",
  "resourceName": "Resource Name value",
  "actionName": "Action Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="8ad5f-149">响应</span><span class="sxs-lookup"><span data-stu-id="8ad5f-149">Response</span></span>
<span data-ttu-id="8ad5f-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8ad5f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 227

{
  "@odata.type": "#microsoft.graph.resourceOperation",
  "id": "232b8fee-8fee-232b-ee8f-2b23ee8f2b23",
  "resourceName": "Resource Name value",
  "actionName": "Action Name value",
  "description": "Description value"
}
```



