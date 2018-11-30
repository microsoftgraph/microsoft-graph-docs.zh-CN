---
title: 创建 targetedManagedAppConfiguration
description: 创建新的 targetedManagedAppConfiguration 对象。
ms.openlocfilehash: d65fed3c202e418133a0d657ac1496ad97b32c07
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047598"
---
# <a name="create-targetedmanagedappconfiguration"></a><span data-ttu-id="74ca4-103">创建 targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="74ca4-103">Create targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="74ca4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="74ca4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="74ca4-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="74ca4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="74ca4-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="74ca4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="74ca4-107">创建新的 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="74ca4-107">Create a new [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="74ca4-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="74ca4-108">Prerequisites</span></span>
<span data-ttu-id="74ca4-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="74ca4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74ca4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="74ca4-111">Permission type</span></span>|<span data-ttu-id="74ca4-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="74ca4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="74ca4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="74ca4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="74ca4-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74ca4-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="74ca4-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="74ca4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="74ca4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="74ca4-116">Not supported.</span></span>|
|<span data-ttu-id="74ca4-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="74ca4-117">Application</span></span>|<span data-ttu-id="74ca4-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="74ca4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="74ca4-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="74ca4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="74ca4-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="74ca4-120">Request headers</span></span>
|<span data-ttu-id="74ca4-121">标头</span><span class="sxs-lookup"><span data-stu-id="74ca4-121">Header</span></span>|<span data-ttu-id="74ca4-122">值</span><span class="sxs-lookup"><span data-stu-id="74ca4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="74ca4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="74ca4-123">Authorization</span></span>|<span data-ttu-id="74ca4-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="74ca4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="74ca4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="74ca4-125">Accept</span></span>|<span data-ttu-id="74ca4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="74ca4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="74ca4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="74ca4-127">Request body</span></span>
<span data-ttu-id="74ca4-128">在请求正文中，提供 targetedManagedAppConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="74ca4-128">In the request body, supply a JSON representation for the targetedManagedAppConfiguration object.</span></span>

<span data-ttu-id="74ca4-129">下表显示创建 targetedManagedAppConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="74ca4-129">The following table shows the properties that are required when you create the targetedManagedAppConfiguration.</span></span>

|<span data-ttu-id="74ca4-130">属性</span><span class="sxs-lookup"><span data-stu-id="74ca4-130">Property</span></span>|<span data-ttu-id="74ca4-131">类型</span><span class="sxs-lookup"><span data-stu-id="74ca4-131">Type</span></span>|<span data-ttu-id="74ca4-132">说明</span><span class="sxs-lookup"><span data-stu-id="74ca4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74ca4-133">displayName</span><span class="sxs-lookup"><span data-stu-id="74ca4-133">displayName</span></span>|<span data-ttu-id="74ca4-134">String</span><span class="sxs-lookup"><span data-stu-id="74ca4-134">String</span></span>|<span data-ttu-id="74ca4-135">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="74ca4-135">Policy display name.</span></span> <span data-ttu-id="74ca4-136">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="74ca4-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="74ca4-137">description</span><span class="sxs-lookup"><span data-stu-id="74ca4-137">description</span></span>|<span data-ttu-id="74ca4-138">String</span><span class="sxs-lookup"><span data-stu-id="74ca4-138">String</span></span>|<span data-ttu-id="74ca4-139">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="74ca4-139">The policy's description.</span></span> <span data-ttu-id="74ca4-140">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="74ca4-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="74ca4-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="74ca4-141">createdDateTime</span></span>|<span data-ttu-id="74ca4-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74ca4-142">DateTimeOffset</span></span>|<span data-ttu-id="74ca4-143">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="74ca4-143">The date and time the policy was created.</span></span> <span data-ttu-id="74ca4-144">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="74ca4-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="74ca4-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="74ca4-145">lastModifiedDateTime</span></span>|<span data-ttu-id="74ca4-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74ca4-146">DateTimeOffset</span></span>|<span data-ttu-id="74ca4-147">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="74ca4-147">Last time the policy was modified.</span></span> <span data-ttu-id="74ca4-148">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="74ca4-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="74ca4-149">id</span><span class="sxs-lookup"><span data-stu-id="74ca4-149">id</span></span>|<span data-ttu-id="74ca4-150">String</span><span class="sxs-lookup"><span data-stu-id="74ca4-150">String</span></span>|<span data-ttu-id="74ca4-151">实体的键。</span><span class="sxs-lookup"><span data-stu-id="74ca4-151">Key of the entity.</span></span> <span data-ttu-id="74ca4-152">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="74ca4-152">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="74ca4-153">version</span><span class="sxs-lookup"><span data-stu-id="74ca4-153">version</span></span>|<span data-ttu-id="74ca4-154">String</span><span class="sxs-lookup"><span data-stu-id="74ca4-154">String</span></span>|<span data-ttu-id="74ca4-155">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="74ca4-155">Version of the entity.</span></span> <span data-ttu-id="74ca4-156">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="74ca4-156">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="74ca4-157">customSettings</span><span class="sxs-lookup"><span data-stu-id="74ca4-157">customSettings</span></span>|<span data-ttu-id="74ca4-158">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="74ca4-158">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="74ca4-159">要发送到配置范围确定的用户应用的一组字符串键和字符串值对，不由此服务更改。继承自 [ managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="74ca4-159">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="74ca4-160">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="74ca4-160">deployedAppCount</span></span>|<span data-ttu-id="74ca4-161">Int32</span><span class="sxs-lookup"><span data-stu-id="74ca4-161">Int32</span></span>|<span data-ttu-id="74ca4-162">当前策略部署到的应用的计数。</span><span class="sxs-lookup"><span data-stu-id="74ca4-162">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="74ca4-163">isAssigned</span><span class="sxs-lookup"><span data-stu-id="74ca4-163">isAssigned</span></span>|<span data-ttu-id="74ca4-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="74ca4-164">Boolean</span></span>|<span data-ttu-id="74ca4-165">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="74ca4-165">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="74ca4-166">响应</span><span class="sxs-lookup"><span data-stu-id="74ca4-166">Response</span></span>
<span data-ttu-id="74ca4-167">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="74ca4-167">If successful, this method returns a `201 Created` response code and a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74ca4-168">示例</span><span class="sxs-lookup"><span data-stu-id="74ca4-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="74ca4-169">请求</span><span class="sxs-lookup"><span data-stu-id="74ca4-169">Request</span></span>
<span data-ttu-id="74ca4-170">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="74ca4-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations
Content-type: application/json
Content-length: 452

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
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

### <a name="response"></a><span data-ttu-id="74ca4-171">响应</span><span class="sxs-lookup"><span data-stu-id="74ca4-171">Response</span></span>
<span data-ttu-id="74ca4-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="74ca4-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





