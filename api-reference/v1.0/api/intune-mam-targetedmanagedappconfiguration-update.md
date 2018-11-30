---
title: 更新 targetedManagedAppConfiguration
description: 更新 targetedManagedAppConfiguration 对象的属性。
ms.openlocfilehash: 2157c6bb07562ca3aaff1a15737ec5dc6a7f19bd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011337"
---
# <a name="update-targetedmanagedappconfiguration"></a><span data-ttu-id="fa3a7-103">更新 targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="fa3a7-103">Update targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="fa3a7-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="fa3a7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fa3a7-105">更新 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="fa3a7-105">Update the properties of a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fa3a7-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="fa3a7-106">Prerequisites</span></span>
<span data-ttu-id="fa3a7-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="fa3a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa3a7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="fa3a7-109">Permission type</span></span>|<span data-ttu-id="fa3a7-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fa3a7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa3a7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fa3a7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fa3a7-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa3a7-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fa3a7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fa3a7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa3a7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="fa3a7-114">Not supported.</span></span>|
|<span data-ttu-id="fa3a7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="fa3a7-115">Application</span></span>|<span data-ttu-id="fa3a7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fa3a7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa3a7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fa3a7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="fa3a7-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="fa3a7-118">Request headers</span></span>
|<span data-ttu-id="fa3a7-119">标头</span><span class="sxs-lookup"><span data-stu-id="fa3a7-119">Header</span></span>|<span data-ttu-id="fa3a7-120">值</span><span class="sxs-lookup"><span data-stu-id="fa3a7-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa3a7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa3a7-121">Authorization</span></span>|<span data-ttu-id="fa3a7-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fa3a7-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa3a7-123">Accept</span><span class="sxs-lookup"><span data-stu-id="fa3a7-123">Accept</span></span>|<span data-ttu-id="fa3a7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fa3a7-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa3a7-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="fa3a7-125">Request body</span></span>
<span data-ttu-id="fa3a7-126">在请求正文中，提供 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fa3a7-126">In the request body, supply a JSON representation for the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>

<span data-ttu-id="fa3a7-127">下表显示创建 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="fa3a7-127">The following table shows the properties that are required when you create the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span></span>

|<span data-ttu-id="fa3a7-128">属性</span><span class="sxs-lookup"><span data-stu-id="fa3a7-128">Property</span></span>|<span data-ttu-id="fa3a7-129">类型</span><span class="sxs-lookup"><span data-stu-id="fa3a7-129">Type</span></span>|<span data-ttu-id="fa3a7-130">说明</span><span class="sxs-lookup"><span data-stu-id="fa3a7-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa3a7-131">displayName</span><span class="sxs-lookup"><span data-stu-id="fa3a7-131">displayName</span></span>|<span data-ttu-id="fa3a7-132">String</span><span class="sxs-lookup"><span data-stu-id="fa3a7-132">String</span></span>|<span data-ttu-id="fa3a7-133">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="fa3a7-133">Policy display name.</span></span> <span data-ttu-id="fa3a7-134">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fa3a7-134">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="fa3a7-135">description</span><span class="sxs-lookup"><span data-stu-id="fa3a7-135">description</span></span>|<span data-ttu-id="fa3a7-136">String</span><span class="sxs-lookup"><span data-stu-id="fa3a7-136">String</span></span>|<span data-ttu-id="fa3a7-137">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="fa3a7-137">The policy's description.</span></span> <span data-ttu-id="fa3a7-138">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fa3a7-138">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="fa3a7-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fa3a7-139">createdDateTime</span></span>|<span data-ttu-id="fa3a7-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa3a7-140">DateTimeOffset</span></span>|<span data-ttu-id="fa3a7-141">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="fa3a7-141">The date and time the policy was created.</span></span> <span data-ttu-id="fa3a7-142">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fa3a7-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="fa3a7-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fa3a7-143">lastModifiedDateTime</span></span>|<span data-ttu-id="fa3a7-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa3a7-144">DateTimeOffset</span></span>|<span data-ttu-id="fa3a7-145">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="fa3a7-145">Last time the policy was modified.</span></span> <span data-ttu-id="fa3a7-146">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fa3a7-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="fa3a7-147">id</span><span class="sxs-lookup"><span data-stu-id="fa3a7-147">id</span></span>|<span data-ttu-id="fa3a7-148">String</span><span class="sxs-lookup"><span data-stu-id="fa3a7-148">String</span></span>|<span data-ttu-id="fa3a7-149">实体的键。</span><span class="sxs-lookup"><span data-stu-id="fa3a7-149">Key of the entity.</span></span> <span data-ttu-id="fa3a7-150">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fa3a7-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="fa3a7-151">version</span><span class="sxs-lookup"><span data-stu-id="fa3a7-151">version</span></span>|<span data-ttu-id="fa3a7-152">String</span><span class="sxs-lookup"><span data-stu-id="fa3a7-152">String</span></span>|<span data-ttu-id="fa3a7-153">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="fa3a7-153">Version of the entity.</span></span> <span data-ttu-id="fa3a7-154">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fa3a7-154">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="fa3a7-155">customSettings</span><span class="sxs-lookup"><span data-stu-id="fa3a7-155">customSettings</span></span>|<span data-ttu-id="fa3a7-156">[keyValuePair](../resources/intune-mam-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fa3a7-156">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="fa3a7-157">要发送到配置范围确定的用户应用的一组字符串键和字符串值对，不由此服务更改。继承自 [ managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fa3a7-157">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="fa3a7-158">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="fa3a7-158">deployedAppCount</span></span>|<span data-ttu-id="fa3a7-159">Int32</span><span class="sxs-lookup"><span data-stu-id="fa3a7-159">Int32</span></span>|<span data-ttu-id="fa3a7-160">当前策略部署到的应用的计数。</span><span class="sxs-lookup"><span data-stu-id="fa3a7-160">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="fa3a7-161">isAssigned</span><span class="sxs-lookup"><span data-stu-id="fa3a7-161">isAssigned</span></span>|<span data-ttu-id="fa3a7-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="fa3a7-162">Boolean</span></span>|<span data-ttu-id="fa3a7-163">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="fa3a7-163">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="fa3a7-164">响应</span><span class="sxs-lookup"><span data-stu-id="fa3a7-164">Response</span></span>
<span data-ttu-id="fa3a7-165">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fa3a7-165">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa3a7-166">示例</span><span class="sxs-lookup"><span data-stu-id="fa3a7-166">Example</span></span>
### <a name="request"></a><span data-ttu-id="fa3a7-167">请求</span><span class="sxs-lookup"><span data-stu-id="fa3a7-167">Request</span></span>
<span data-ttu-id="fa3a7-168">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fa3a7-168">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
Content-type: application/json
Content-length: 388

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "version": "Version value",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "deployedAppCount": 0,
  "isAssigned": true
}
```

### <a name="response"></a><span data-ttu-id="fa3a7-169">响应</span><span class="sxs-lookup"><span data-stu-id="fa3a7-169">Response</span></span>
<span data-ttu-id="fa3a7-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fa3a7-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 560

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "id": "2444e029-e029-2444-29e0-442429e04424",
  "version": "Version value",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "deployedAppCount": 0,
  "isAssigned": true
}
```



