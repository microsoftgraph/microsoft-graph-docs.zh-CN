# <a name="update-onpremisesconditionalaccesssettings"></a><span data-ttu-id="a935c-101">更新 onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="a935c-101">Update onPremisesConditionalAccessSettings</span></span>

> <span data-ttu-id="a935c-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a935c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a935c-103">更新 [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a935c-103">Update the properties of a [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a935c-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="a935c-104">Prerequisites</span></span>
<span data-ttu-id="a935c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a935c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a935c-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="a935c-107">Permission type</span></span>|<span data-ttu-id="a935c-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a935c-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a935c-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a935c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="a935c-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a935c-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a935c-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a935c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a935c-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="a935c-112">Not supported.</span></span>|
|<span data-ttu-id="a935c-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="a935c-113">Application</span></span>|<span data-ttu-id="a935c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a935c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a935c-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a935c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/conditionalAccessSettings
```

## <a name="request-headers"></a><span data-ttu-id="a935c-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="a935c-116">Request headers</span></span>
|<span data-ttu-id="a935c-117">标头</span><span class="sxs-lookup"><span data-stu-id="a935c-117">Header</span></span>|<span data-ttu-id="a935c-118">值</span><span class="sxs-lookup"><span data-stu-id="a935c-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a935c-119">授权</span><span class="sxs-lookup"><span data-stu-id="a935c-119">Authorization</span></span>|<span data-ttu-id="a935c-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a935c-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a935c-121">接受</span><span class="sxs-lookup"><span data-stu-id="a935c-121">Accept</span></span>|<span data-ttu-id="a935c-122">application/json</span><span class="sxs-lookup"><span data-stu-id="a935c-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a935c-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="a935c-123">Request body</span></span>
<span data-ttu-id="a935c-124">在请求正文中，提供 [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a935c-124">In the request body, supply a JSON representation for the [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) object.</span></span>

<span data-ttu-id="a935c-125">下表显示创建 [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a935c-125">The following table shows the properties that are required when you create the [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md).</span></span>

|<span data-ttu-id="a935c-126">属性</span><span class="sxs-lookup"><span data-stu-id="a935c-126">Property</span></span>|<span data-ttu-id="a935c-127">类型</span><span class="sxs-lookup"><span data-stu-id="a935c-127">Type</span></span>|<span data-ttu-id="a935c-128">说明</span><span class="sxs-lookup"><span data-stu-id="a935c-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a935c-129">id</span><span class="sxs-lookup"><span data-stu-id="a935c-129">id</span></span>|<span data-ttu-id="a935c-130">字符串</span><span class="sxs-lookup"><span data-stu-id="a935c-130">String</span></span>|<span data-ttu-id="a935c-131">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a935c-131">Not yet documented</span></span>|
|<span data-ttu-id="a935c-132">enabled</span><span class="sxs-lookup"><span data-stu-id="a935c-132">enabled</span></span>|<span data-ttu-id="a935c-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="a935c-133">Boolean</span></span>|<span data-ttu-id="a935c-134">指示是否为该组织启用了本地条件访问</span><span class="sxs-lookup"><span data-stu-id="a935c-134">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="a935c-135">includedGroups</span><span class="sxs-lookup"><span data-stu-id="a935c-135">includedGroups</span></span>|<span data-ttu-id="a935c-136">Guid 集合</span><span class="sxs-lookup"><span data-stu-id="a935c-136">Guid collection</span></span>|<span data-ttu-id="a935c-137">本地条件访问将面向的用户组。</span><span class="sxs-lookup"><span data-stu-id="a935c-137">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="a935c-138">这些组中的所有用户都需要托管移动设备并符合邮件访问的要求。</span><span class="sxs-lookup"><span data-stu-id="a935c-138">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="a935c-139">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="a935c-139">excludedGroups</span></span>|<span data-ttu-id="a935c-140">Guid 集合</span><span class="sxs-lookup"><span data-stu-id="a935c-140">Guid collection</span></span>|<span data-ttu-id="a935c-141">将由本地条件访问豁免的用户组。</span><span class="sxs-lookup"><span data-stu-id="a935c-141">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="a935c-142">这些组中的所有用户都将从条件访问策略中豁免。</span><span class="sxs-lookup"><span data-stu-id="a935c-142">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="a935c-143">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="a935c-143">overrideDefaultRule</span></span>|<span data-ttu-id="a935c-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="a935c-144">Boolean</span></span>|<span data-ttu-id="a935c-145">允许设备时重写默认访问规则以确保授予访问。</span><span class="sxs-lookup"><span data-stu-id="a935c-145">Override the default access rule when allowing a device to ensure access is granted.</span></span>|



## <a name="response"></a><span data-ttu-id="a935c-146">响应</span><span class="sxs-lookup"><span data-stu-id="a935c-146">Response</span></span>
<span data-ttu-id="a935c-147">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a935c-147">If successful, this method returns a `200 OK` response code and an updated [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a935c-148">示例</span><span class="sxs-lookup"><span data-stu-id="a935c-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="a935c-149">请求</span><span class="sxs-lookup"><span data-stu-id="a935c-149">Request</span></span>
<span data-ttu-id="a935c-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a935c-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/conditionalAccessSettings
Content-type: application/json
Content-length: 195

{
  "enabled": true,
  "includedGroups": [
    "79199ed9-e50b-4257-8de4-70b9c8685061"
  ],
  "excludedGroups": [
    "79199ed9-e50b-4257-8de4-70b9c8685061"
  ],
  "overrideDefaultRule": true
}
```

### <a name="response"></a><span data-ttu-id="a935c-151">响应</span><span class="sxs-lookup"><span data-stu-id="a935c-151">Response</span></span>
<span data-ttu-id="a935c-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a935c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 318

{
  "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
  "id": "a0efde21-de21-a0ef-21de-efa021deefa0",
  "enabled": true,
  "includedGroups": [
    "79199ed9-e50b-4257-8de4-70b9c8685061"
  ],
  "excludedGroups": [
    "79199ed9-e50b-4257-8de4-70b9c8685061"
  ],
  "overrideDefaultRule": true
}
```



