# <a name="update-organization"></a><span data-ttu-id="50bcc-101">更新 organization</span><span class="sxs-lookup"><span data-stu-id="50bcc-101">Update organization</span></span>

> <span data-ttu-id="50bcc-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="50bcc-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="50bcc-103">更新 [organization](../resources/intune_onboarding_organization.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="50bcc-103">Update the properties of a [organization](../resources/intune_onboarding_organization.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="50bcc-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="50bcc-104">Prerequisites</span></span>
<span data-ttu-id="50bcc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="50bcc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="50bcc-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="50bcc-107">Permission type</span></span>|<span data-ttu-id="50bcc-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="50bcc-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50bcc-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="50bcc-109">Delegated (work or school account)</span></span>|<span data-ttu-id="50bcc-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50bcc-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="50bcc-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="50bcc-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50bcc-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="50bcc-112">Not supported.</span></span>|
|<span data-ttu-id="50bcc-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="50bcc-113">Application</span></span>|<span data-ttu-id="50bcc-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="50bcc-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="50bcc-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="50bcc-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /organization/{organizationId}
```

## <a name="request-headers"></a><span data-ttu-id="50bcc-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="50bcc-116">Request headers</span></span>
|<span data-ttu-id="50bcc-117">标头</span><span class="sxs-lookup"><span data-stu-id="50bcc-117">Header</span></span>|<span data-ttu-id="50bcc-118">值</span><span class="sxs-lookup"><span data-stu-id="50bcc-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50bcc-119">授权</span><span class="sxs-lookup"><span data-stu-id="50bcc-119">Authorization</span></span>|<span data-ttu-id="50bcc-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="50bcc-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50bcc-121">接受</span><span class="sxs-lookup"><span data-stu-id="50bcc-121">Accept</span></span>|<span data-ttu-id="50bcc-122">application/json</span><span class="sxs-lookup"><span data-stu-id="50bcc-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50bcc-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="50bcc-123">Request body</span></span>
<span data-ttu-id="50bcc-124">在请求正文中，提供 [organization](../resources/intune_onboarding_organization.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="50bcc-124">In the request body, supply a JSON representation for the [organization](../resources/intune_onboarding_organization.md) object.</span></span>

<span data-ttu-id="50bcc-125">下表显示创建 [organization](../resources/intune_onboarding_organization.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="50bcc-125">The following table shows the properties that are required when you create the [organization](../resources/intune_onboarding_organization.md).</span></span>

|<span data-ttu-id="50bcc-126">属性</span><span class="sxs-lookup"><span data-stu-id="50bcc-126">Property</span></span>|<span data-ttu-id="50bcc-127">类型</span><span class="sxs-lookup"><span data-stu-id="50bcc-127">Type</span></span>|<span data-ttu-id="50bcc-128">说明</span><span class="sxs-lookup"><span data-stu-id="50bcc-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50bcc-129">ID</span><span class="sxs-lookup"><span data-stu-id="50bcc-129">id</span></span>|<span data-ttu-id="50bcc-130">字符串</span><span class="sxs-lookup"><span data-stu-id="50bcc-130">String</span></span>|<span data-ttu-id="50bcc-131">对象的 GUID。</span><span class="sxs-lookup"><span data-stu-id="50bcc-131">The GUID for the object.</span></span>|
|<span data-ttu-id="50bcc-132">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="50bcc-132">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="50bcc-133">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="50bcc-133">mdmAuthority</span></span>](../resources/intune_onboarding_mdmauthority.md)|<span data-ttu-id="50bcc-p102">移动设备管理机构。 可取值为：`unknown`、`intune`、`sccm`、`office365`。</span><span class="sxs-lookup"><span data-stu-id="50bcc-p102">Mobile device management authority. The possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|



## <a name="response"></a><span data-ttu-id="50bcc-136">响应</span><span class="sxs-lookup"><span data-stu-id="50bcc-136">Response</span></span>
<span data-ttu-id="50bcc-137">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [organization](../resources/intune_onboarding_organization.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="50bcc-137">If successful, this method returns a `200 OK` response code and an updated [organization](../resources/intune_onboarding_organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50bcc-138">示例</span><span class="sxs-lookup"><span data-stu-id="50bcc-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="50bcc-139">请求</span><span class="sxs-lookup"><span data-stu-id="50bcc-139">Request</span></span>
<span data-ttu-id="50bcc-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="50bcc-140">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/organization/{organizationId}
Content-type: application/json
Content-length: 51

{
  "mobileDeviceManagementAuthority": "intune"
}
```

### <a name="response"></a><span data-ttu-id="50bcc-141">响应</span><span class="sxs-lookup"><span data-stu-id="50bcc-141">Response</span></span>
<span data-ttu-id="50bcc-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="50bcc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 151

{
  "@odata.type": "#microsoft.graph.organization",
  "id": "9efe224a-224a-9efe-4a22-fe9e4a22fe9e",
  "mobileDeviceManagementAuthority": "intune"
}
```








