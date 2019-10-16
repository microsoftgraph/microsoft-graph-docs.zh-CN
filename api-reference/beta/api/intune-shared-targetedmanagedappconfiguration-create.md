---
title: 创建 targetedManagedAppConfiguration
description: 创建新的 targetedManagedAppConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 709112abdab171d53683176afe04970ce25844ee
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537900"
---
# <a name="create-targetedmanagedappconfiguration"></a><span data-ttu-id="c28a9-103">创建 targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="c28a9-103">Create targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="c28a9-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c28a9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c28a9-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c28a9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c28a9-106">创建新的 [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c28a9-106">Create a new [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c28a9-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="c28a9-107">Prerequisites</span></span>
<span data-ttu-id="c28a9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c28a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c28a9-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c28a9-110">Permission type</span></span>|<span data-ttu-id="c28a9-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c28a9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c28a9-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c28a9-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c28a9-113">&nbsp; &nbsp; **移动应用管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="c28a9-113">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="c28a9-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c28a9-114">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="c28a9-115">&nbsp;&nbsp; **策略集**</span><span class="sxs-lookup"><span data-stu-id="c28a9-115">&nbsp; &nbsp; **Policy Set**</span></span>  | <span data-ttu-id="c28a9-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c28a9-116">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c28a9-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c28a9-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c28a9-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="c28a9-118">Not supported.</span></span>|
|<span data-ttu-id="c28a9-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="c28a9-119">Application</span></span>||
| <span data-ttu-id="c28a9-120">&nbsp; &nbsp; **移动应用管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="c28a9-120">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="c28a9-121">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c28a9-121">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="c28a9-122">&nbsp;&nbsp; **策略集**</span><span class="sxs-lookup"><span data-stu-id="c28a9-122">&nbsp; &nbsp; **Policy Set**</span></span>  | <span data-ttu-id="c28a9-123">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c28a9-123">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c28a9-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c28a9-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c28a9-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="c28a9-125">Request headers</span></span>
|<span data-ttu-id="c28a9-126">标头</span><span class="sxs-lookup"><span data-stu-id="c28a9-126">Header</span></span>|<span data-ttu-id="c28a9-127">值</span><span class="sxs-lookup"><span data-stu-id="c28a9-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c28a9-128">授权</span><span class="sxs-lookup"><span data-stu-id="c28a9-128">Authorization</span></span>|<span data-ttu-id="c28a9-129">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c28a9-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c28a9-130">接受</span><span class="sxs-lookup"><span data-stu-id="c28a9-130">Accept</span></span>|<span data-ttu-id="c28a9-131">application/json</span><span class="sxs-lookup"><span data-stu-id="c28a9-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c28a9-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="c28a9-132">Request body</span></span>
<span data-ttu-id="c28a9-133">在请求正文中，提供 targetedManagedAppConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c28a9-133">In the request body, supply a JSON representation for the targetedManagedAppConfiguration object.</span></span>

<span data-ttu-id="c28a9-134">下表显示创建 targetedManagedAppConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c28a9-134">The following table shows the properties that are required when you create the targetedManagedAppConfiguration.</span></span>

|<span data-ttu-id="c28a9-135">属性</span><span class="sxs-lookup"><span data-stu-id="c28a9-135">Property</span></span>|<span data-ttu-id="c28a9-136">类型</span><span class="sxs-lookup"><span data-stu-id="c28a9-136">Type</span></span>|<span data-ttu-id="c28a9-137">说明</span><span class="sxs-lookup"><span data-stu-id="c28a9-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c28a9-138">displayName</span><span class="sxs-lookup"><span data-stu-id="c28a9-138">displayName</span></span>|<span data-ttu-id="c28a9-139">字符串</span><span class="sxs-lookup"><span data-stu-id="c28a9-139">String</span></span>|<span data-ttu-id="c28a9-140">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="c28a9-140">Policy display name.</span></span> <span data-ttu-id="c28a9-141">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c28a9-141">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c28a9-142">说明</span><span class="sxs-lookup"><span data-stu-id="c28a9-142">description</span></span>|<span data-ttu-id="c28a9-143">String</span><span class="sxs-lookup"><span data-stu-id="c28a9-143">String</span></span>|<span data-ttu-id="c28a9-144">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="c28a9-144">The policy's description.</span></span> <span data-ttu-id="c28a9-145">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c28a9-145">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c28a9-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c28a9-146">createdDateTime</span></span>|<span data-ttu-id="c28a9-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c28a9-147">DateTimeOffset</span></span>|<span data-ttu-id="c28a9-148">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c28a9-148">The date and time the policy was created.</span></span> <span data-ttu-id="c28a9-149">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c28a9-149">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c28a9-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c28a9-150">lastModifiedDateTime</span></span>|<span data-ttu-id="c28a9-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c28a9-151">DateTimeOffset</span></span>|<span data-ttu-id="c28a9-152">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="c28a9-152">Last time the policy was modified.</span></span> <span data-ttu-id="c28a9-153">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c28a9-153">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c28a9-154">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c28a9-154">roleScopeTagIds</span></span>|<span data-ttu-id="c28a9-155">String 集合</span><span class="sxs-lookup"><span data-stu-id="c28a9-155">String collection</span></span>|<span data-ttu-id="c28a9-156">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="c28a9-156">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c28a9-157">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c28a9-157">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c28a9-158">id</span><span class="sxs-lookup"><span data-stu-id="c28a9-158">id</span></span>|<span data-ttu-id="c28a9-159">字符串</span><span class="sxs-lookup"><span data-stu-id="c28a9-159">String</span></span>|<span data-ttu-id="c28a9-160">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c28a9-160">Key of the entity.</span></span> <span data-ttu-id="c28a9-161">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c28a9-161">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c28a9-162">version</span><span class="sxs-lookup"><span data-stu-id="c28a9-162">version</span></span>|<span data-ttu-id="c28a9-163">String</span><span class="sxs-lookup"><span data-stu-id="c28a9-163">String</span></span>|<span data-ttu-id="c28a9-164">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="c28a9-164">Version of the entity.</span></span> <span data-ttu-id="c28a9-165">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c28a9-165">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c28a9-166">customSettings</span><span class="sxs-lookup"><span data-stu-id="c28a9-166">customSettings</span></span>|<span data-ttu-id="c28a9-167">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c28a9-167">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="c28a9-168">要发送到配置范围确定的用户应用的一组字符串键和字符串值对，不由此服务更改。继承自 [ managedAppConfiguration ](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c28a9-168">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="c28a9-169">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="c28a9-169">deployedAppCount</span></span>|<span data-ttu-id="c28a9-170">Int32</span><span class="sxs-lookup"><span data-stu-id="c28a9-170">Int32</span></span>|<span data-ttu-id="c28a9-171">当前策略部署到的应用的计数。</span><span class="sxs-lookup"><span data-stu-id="c28a9-171">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="c28a9-172">isAssigned</span><span class="sxs-lookup"><span data-stu-id="c28a9-172">isAssigned</span></span>|<span data-ttu-id="c28a9-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="c28a9-173">Boolean</span></span>|<span data-ttu-id="c28a9-174">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="c28a9-174">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="c28a9-175">响应</span><span class="sxs-lookup"><span data-stu-id="c28a9-175">Response</span></span>
<span data-ttu-id="c28a9-176">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c28a9-176">If successful, this method returns a `201 Created` response code and a [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c28a9-177">示例</span><span class="sxs-lookup"><span data-stu-id="c28a9-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="c28a9-178">请求</span><span class="sxs-lookup"><span data-stu-id="c28a9-178">Request</span></span>
<span data-ttu-id="c28a9-179">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c28a9-179">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations
Content-type: application/json
Content-length: 450

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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

### <a name="response"></a><span data-ttu-id="c28a9-180">响应</span><span class="sxs-lookup"><span data-stu-id="c28a9-180">Response</span></span>
<span data-ttu-id="c28a9-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c28a9-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 622

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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






