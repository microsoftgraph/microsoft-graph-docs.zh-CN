---
title: 更新 targetedManagedAppConfiguration
description: 更新 targetedManagedAppConfiguration 对象的属性。
ms.openlocfilehash: 097665b53250c90bbe553d72b2e82dabac6a11ba
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046574"
---
# <a name="update-targetedmanagedappconfiguration"></a><span data-ttu-id="3b2db-103">更新 targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="3b2db-103">Update targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="3b2db-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="3b2db-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3b2db-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3b2db-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3b2db-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="3b2db-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3b2db-107">更新 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3b2db-107">Update the properties of a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3b2db-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="3b2db-108">Prerequisites</span></span>
<span data-ttu-id="3b2db-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="3b2db-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b2db-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3b2db-111">Permission type</span></span>|<span data-ttu-id="3b2db-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3b2db-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b2db-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3b2db-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3b2db-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b2db-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3b2db-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3b2db-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b2db-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3b2db-116">Not supported.</span></span>|
|<span data-ttu-id="3b2db-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3b2db-117">Application</span></span>|<span data-ttu-id="3b2db-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="3b2db-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b2db-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3b2db-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="3b2db-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3b2db-120">Request headers</span></span>
|<span data-ttu-id="3b2db-121">标头</span><span class="sxs-lookup"><span data-stu-id="3b2db-121">Header</span></span>|<span data-ttu-id="3b2db-122">值</span><span class="sxs-lookup"><span data-stu-id="3b2db-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b2db-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b2db-123">Authorization</span></span>|<span data-ttu-id="3b2db-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3b2db-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b2db-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3b2db-125">Accept</span></span>|<span data-ttu-id="3b2db-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3b2db-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b2db-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3b2db-127">Request body</span></span>
<span data-ttu-id="3b2db-128">在请求正文中，提供 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3b2db-128">In the request body, supply a JSON representation for the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>

<span data-ttu-id="3b2db-129">下表显示创建 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3b2db-129">The following table shows the properties that are required when you create the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span></span>

|<span data-ttu-id="3b2db-130">属性</span><span class="sxs-lookup"><span data-stu-id="3b2db-130">Property</span></span>|<span data-ttu-id="3b2db-131">类型</span><span class="sxs-lookup"><span data-stu-id="3b2db-131">Type</span></span>|<span data-ttu-id="3b2db-132">说明</span><span class="sxs-lookup"><span data-stu-id="3b2db-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b2db-133">displayName</span><span class="sxs-lookup"><span data-stu-id="3b2db-133">displayName</span></span>|<span data-ttu-id="3b2db-134">String</span><span class="sxs-lookup"><span data-stu-id="3b2db-134">String</span></span>|<span data-ttu-id="3b2db-135">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="3b2db-135">Policy display name.</span></span> <span data-ttu-id="3b2db-136">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3b2db-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="3b2db-137">description</span><span class="sxs-lookup"><span data-stu-id="3b2db-137">description</span></span>|<span data-ttu-id="3b2db-138">String</span><span class="sxs-lookup"><span data-stu-id="3b2db-138">String</span></span>|<span data-ttu-id="3b2db-139">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="3b2db-139">The policy's description.</span></span> <span data-ttu-id="3b2db-140">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3b2db-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="3b2db-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3b2db-141">createdDateTime</span></span>|<span data-ttu-id="3b2db-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b2db-142">DateTimeOffset</span></span>|<span data-ttu-id="3b2db-143">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="3b2db-143">The date and time the policy was created.</span></span> <span data-ttu-id="3b2db-144">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3b2db-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="3b2db-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3b2db-145">lastModifiedDateTime</span></span>|<span data-ttu-id="3b2db-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b2db-146">DateTimeOffset</span></span>|<span data-ttu-id="3b2db-147">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="3b2db-147">Last time the policy was modified.</span></span> <span data-ttu-id="3b2db-148">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3b2db-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="3b2db-149">id</span><span class="sxs-lookup"><span data-stu-id="3b2db-149">id</span></span>|<span data-ttu-id="3b2db-150">String</span><span class="sxs-lookup"><span data-stu-id="3b2db-150">String</span></span>|<span data-ttu-id="3b2db-151">实体的键。</span><span class="sxs-lookup"><span data-stu-id="3b2db-151">Key of the entity.</span></span> <span data-ttu-id="3b2db-152">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3b2db-152">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="3b2db-153">version</span><span class="sxs-lookup"><span data-stu-id="3b2db-153">version</span></span>|<span data-ttu-id="3b2db-154">String</span><span class="sxs-lookup"><span data-stu-id="3b2db-154">String</span></span>|<span data-ttu-id="3b2db-155">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="3b2db-155">Version of the entity.</span></span> <span data-ttu-id="3b2db-156">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3b2db-156">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="3b2db-157">customSettings</span><span class="sxs-lookup"><span data-stu-id="3b2db-157">customSettings</span></span>|<span data-ttu-id="3b2db-158">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3b2db-158">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="3b2db-159">要发送到配置范围确定的用户应用的一组字符串键和字符串值对，不由此服务更改。继承自 [ managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3b2db-159">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="3b2db-160">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="3b2db-160">deployedAppCount</span></span>|<span data-ttu-id="3b2db-161">Int32</span><span class="sxs-lookup"><span data-stu-id="3b2db-161">Int32</span></span>|<span data-ttu-id="3b2db-162">当前策略部署到的应用的计数。</span><span class="sxs-lookup"><span data-stu-id="3b2db-162">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="3b2db-163">isAssigned</span><span class="sxs-lookup"><span data-stu-id="3b2db-163">isAssigned</span></span>|<span data-ttu-id="3b2db-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="3b2db-164">Boolean</span></span>|<span data-ttu-id="3b2db-165">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="3b2db-165">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="3b2db-166">响应</span><span class="sxs-lookup"><span data-stu-id="3b2db-166">Response</span></span>
<span data-ttu-id="3b2db-167">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3b2db-167">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b2db-168">示例</span><span class="sxs-lookup"><span data-stu-id="3b2db-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="3b2db-169">请求</span><span class="sxs-lookup"><span data-stu-id="3b2db-169">Request</span></span>
<span data-ttu-id="3b2db-170">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3b2db-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
Content-type: application/json
Content-length: 382

{
  "displayName": "Display Name value",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="3b2db-171">响应</span><span class="sxs-lookup"><span data-stu-id="3b2db-171">Response</span></span>
<span data-ttu-id="3b2db-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3b2db-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





