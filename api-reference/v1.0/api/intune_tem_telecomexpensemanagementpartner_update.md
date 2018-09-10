# <a name="update-telecomexpensemanagementpartner"></a><span data-ttu-id="5f181-101">更新 telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="5f181-101">Update telecomExpenseManagementPartner</span></span>

> <span data-ttu-id="5f181-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5f181-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5f181-103">更新 [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5f181-103">Update the properties of a [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5f181-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="5f181-104">Prerequisites</span></span>
<span data-ttu-id="5f181-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="5f181-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5f181-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="5f181-107">Permission type</span></span>|<span data-ttu-id="5f181-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5f181-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5f181-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5f181-109">Delegated (work or school account)</span></span>|<span data-ttu-id="5f181-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f181-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5f181-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5f181-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f181-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="5f181-112">Not supported.</span></span>|
|<span data-ttu-id="5f181-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="5f181-113">Application</span></span>|<span data-ttu-id="5f181-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5f181-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5f181-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5f181-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="5f181-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="5f181-116">Request headers</span></span>
|<span data-ttu-id="5f181-117">标头</span><span class="sxs-lookup"><span data-stu-id="5f181-117">Header</span></span>|<span data-ttu-id="5f181-118">值</span><span class="sxs-lookup"><span data-stu-id="5f181-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5f181-119">授权</span><span class="sxs-lookup"><span data-stu-id="5f181-119">Authorization</span></span>|<span data-ttu-id="5f181-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5f181-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5f181-121">Accept</span><span class="sxs-lookup"><span data-stu-id="5f181-121">Accept</span></span>|<span data-ttu-id="5f181-122">application/json</span><span class="sxs-lookup"><span data-stu-id="5f181-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f181-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="5f181-123">Request body</span></span>
<span data-ttu-id="5f181-124">在请求正文中，提供 [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5f181-124">In the request body, supply a JSON representation for the [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) object.</span></span>

<span data-ttu-id="5f181-125">下表显示创建 [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5f181-125">The following table shows the properties that are required when you create the [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md).</span></span>

|<span data-ttu-id="5f181-126">属性</span><span class="sxs-lookup"><span data-stu-id="5f181-126">Property</span></span>|<span data-ttu-id="5f181-127">类型</span><span class="sxs-lookup"><span data-stu-id="5f181-127">Type</span></span>|<span data-ttu-id="5f181-128">说明</span><span class="sxs-lookup"><span data-stu-id="5f181-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f181-129">ID</span><span class="sxs-lookup"><span data-stu-id="5f181-129">id</span></span>|<span data-ttu-id="5f181-130">字符串</span><span class="sxs-lookup"><span data-stu-id="5f181-130">String</span></span>|<span data-ttu-id="5f181-131">TEM 合作伙伴的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="5f181-131">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="5f181-132">displayName</span><span class="sxs-lookup"><span data-stu-id="5f181-132">displayName</span></span>|<span data-ttu-id="5f181-133">字符串</span><span class="sxs-lookup"><span data-stu-id="5f181-133">String</span></span>|<span data-ttu-id="5f181-134">TEM 合作伙伴的显示名称。</span><span class="sxs-lookup"><span data-stu-id="5f181-134">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="5f181-135">url</span><span class="sxs-lookup"><span data-stu-id="5f181-135">url</span></span>|<span data-ttu-id="5f181-136">字符串</span><span class="sxs-lookup"><span data-stu-id="5f181-136">String</span></span>|<span data-ttu-id="5f181-137">TEM 合作伙伴的管理控制面板的 URL，管理员可以在其中配置其 TEM 服务。</span><span class="sxs-lookup"><span data-stu-id="5f181-137">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="5f181-138">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="5f181-138">appAuthorized</span></span>|<span data-ttu-id="5f181-139">布尔值</span><span class="sxs-lookup"><span data-stu-id="5f181-139">Boolean</span></span>|<span data-ttu-id="5f181-140">是否已授权合作伙伴的 AAD 应用访问 Intune。</span><span class="sxs-lookup"><span data-stu-id="5f181-140">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="5f181-141">enabled</span><span class="sxs-lookup"><span data-stu-id="5f181-141">enabled</span></span>|<span data-ttu-id="5f181-142">布尔值</span><span class="sxs-lookup"><span data-stu-id="5f181-142">Boolean</span></span>|<span data-ttu-id="5f181-143">当前是启用还是禁用了 Intune 的 TEM 服务连接。</span><span class="sxs-lookup"><span data-stu-id="5f181-143">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="5f181-144">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="5f181-144">lastConnectionDateTime</span></span>|<span data-ttu-id="5f181-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f181-145">DateTimeOffset</span></span>|<span data-ttu-id="5f181-146">TEM 合作伙伴发送到 Intune 的上一个请求的时间戳。</span><span class="sxs-lookup"><span data-stu-id="5f181-146">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="5f181-147">响应</span><span class="sxs-lookup"><span data-stu-id="5f181-147">Response</span></span>
<span data-ttu-id="5f181-148">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5f181-148">If successful, this method returns a `200 OK` response code and an updated [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f181-149">示例</span><span class="sxs-lookup"><span data-stu-id="5f181-149">Example</span></span>
### <a name="request"></a><span data-ttu-id="5f181-150">请求</span><span class="sxs-lookup"><span data-stu-id="5f181-150">Request</span></span>
<span data-ttu-id="5f181-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5f181-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
Content-type: application/json
Content-length: 178

{
  "displayName": "Display Name value",
  "url": "Url value",
  "appAuthorized": true,
  "enabled": true,
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```

### <a name="response"></a><span data-ttu-id="5f181-152">响应</span><span class="sxs-lookup"><span data-stu-id="5f181-152">Response</span></span>
<span data-ttu-id="5f181-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5f181-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 297

{
  "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
  "id": "47a3b399-b399-47a3-99b3-a34799b3a347",
  "displayName": "Display Name value",
  "url": "Url value",
  "appAuthorized": true,
  "enabled": true,
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```








