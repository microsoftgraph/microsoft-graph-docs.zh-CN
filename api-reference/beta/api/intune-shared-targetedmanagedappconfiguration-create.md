---
title: 创建 targetedManagedAppConfiguration
description: 创建新的 targetedManagedAppConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7b3117e5122004c01bcb3d94c6d59ac337a9b362
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43465342"
---
# <a name="create-targetedmanagedappconfiguration"></a><span data-ttu-id="79109-103">创建 targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="79109-103">Create targetedManagedAppConfiguration</span></span>

<span data-ttu-id="79109-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79109-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="79109-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="79109-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79109-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="79109-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79109-107">创建新的 [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="79109-107">Create a new [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="79109-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="79109-108">Prerequisites</span></span>
<span data-ttu-id="79109-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="79109-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79109-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="79109-111">Permission type</span></span>|<span data-ttu-id="79109-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="79109-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79109-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="79109-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="79109-114">&nbsp; &nbsp; **移动应用管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="79109-114">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="79109-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79109-115">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="79109-116">&nbsp;&nbsp; **策略集**</span><span class="sxs-lookup"><span data-stu-id="79109-116">&nbsp; &nbsp; **Policy Set**</span></span>  | <span data-ttu-id="79109-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79109-117">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="79109-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="79109-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79109-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="79109-119">Not supported.</span></span>|
|<span data-ttu-id="79109-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="79109-120">Application</span></span>||
| <span data-ttu-id="79109-121">&nbsp; &nbsp; **移动应用管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="79109-121">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="79109-122">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79109-122">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="79109-123">&nbsp;&nbsp; **策略集**</span><span class="sxs-lookup"><span data-stu-id="79109-123">&nbsp; &nbsp; **Policy Set**</span></span>  | <span data-ttu-id="79109-124">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79109-124">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="79109-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="79109-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="79109-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="79109-126">Request headers</span></span>
|<span data-ttu-id="79109-127">标头</span><span class="sxs-lookup"><span data-stu-id="79109-127">Header</span></span>|<span data-ttu-id="79109-128">值</span><span class="sxs-lookup"><span data-stu-id="79109-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79109-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="79109-129">Authorization</span></span>|<span data-ttu-id="79109-130">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="79109-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79109-131">接受</span><span class="sxs-lookup"><span data-stu-id="79109-131">Accept</span></span>|<span data-ttu-id="79109-132">application/json</span><span class="sxs-lookup"><span data-stu-id="79109-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79109-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="79109-133">Request body</span></span>
<span data-ttu-id="79109-134">在请求正文中，提供 targetedManagedAppConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="79109-134">In the request body, supply a JSON representation for the targetedManagedAppConfiguration object.</span></span>

<span data-ttu-id="79109-135">下表显示创建 targetedManagedAppConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="79109-135">The following table shows the properties that are required when you create the targetedManagedAppConfiguration.</span></span>

|<span data-ttu-id="79109-136">属性</span><span class="sxs-lookup"><span data-stu-id="79109-136">Property</span></span>|<span data-ttu-id="79109-137">类型</span><span class="sxs-lookup"><span data-stu-id="79109-137">Type</span></span>|<span data-ttu-id="79109-138">说明</span><span class="sxs-lookup"><span data-stu-id="79109-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79109-139">displayName</span><span class="sxs-lookup"><span data-stu-id="79109-139">displayName</span></span>|<span data-ttu-id="79109-140">字符串</span><span class="sxs-lookup"><span data-stu-id="79109-140">String</span></span>|<span data-ttu-id="79109-141">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="79109-141">Policy display name.</span></span> <span data-ttu-id="79109-142">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="79109-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="79109-143">description</span><span class="sxs-lookup"><span data-stu-id="79109-143">description</span></span>|<span data-ttu-id="79109-144">String</span><span class="sxs-lookup"><span data-stu-id="79109-144">String</span></span>|<span data-ttu-id="79109-145">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="79109-145">The policy's description.</span></span> <span data-ttu-id="79109-146">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="79109-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="79109-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="79109-147">createdDateTime</span></span>|<span data-ttu-id="79109-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79109-148">DateTimeOffset</span></span>|<span data-ttu-id="79109-149">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="79109-149">The date and time the policy was created.</span></span> <span data-ttu-id="79109-150">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="79109-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="79109-151">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="79109-151">lastModifiedDateTime</span></span>|<span data-ttu-id="79109-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79109-152">DateTimeOffset</span></span>|<span data-ttu-id="79109-153">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="79109-153">Last time the policy was modified.</span></span> <span data-ttu-id="79109-154">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="79109-154">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="79109-155">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="79109-155">roleScopeTagIds</span></span>|<span data-ttu-id="79109-156">String collection</span><span class="sxs-lookup"><span data-stu-id="79109-156">String collection</span></span>|<span data-ttu-id="79109-157">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="79109-157">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="79109-158">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="79109-158">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="79109-159">id</span><span class="sxs-lookup"><span data-stu-id="79109-159">id</span></span>|<span data-ttu-id="79109-160">字符串</span><span class="sxs-lookup"><span data-stu-id="79109-160">String</span></span>|<span data-ttu-id="79109-161">实体的键。</span><span class="sxs-lookup"><span data-stu-id="79109-161">Key of the entity.</span></span> <span data-ttu-id="79109-162">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="79109-162">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="79109-163">version</span><span class="sxs-lookup"><span data-stu-id="79109-163">version</span></span>|<span data-ttu-id="79109-164">String</span><span class="sxs-lookup"><span data-stu-id="79109-164">String</span></span>|<span data-ttu-id="79109-165">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="79109-165">Version of the entity.</span></span> <span data-ttu-id="79109-166">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="79109-166">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="79109-167">customSettings</span><span class="sxs-lookup"><span data-stu-id="79109-167">customSettings</span></span>|<span data-ttu-id="79109-168">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="79109-168">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="79109-169">要发送到配置范围确定的用户应用的一组字符串键和字符串值对，不由此服务更改。继承自 [ managedAppConfiguration ](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="79109-169">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="79109-170">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="79109-170">deployedAppCount</span></span>|<span data-ttu-id="79109-171">Int32</span><span class="sxs-lookup"><span data-stu-id="79109-171">Int32</span></span>|<span data-ttu-id="79109-172">当前策略部署到的应用的计数。</span><span class="sxs-lookup"><span data-stu-id="79109-172">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="79109-173">isAssigned</span><span class="sxs-lookup"><span data-stu-id="79109-173">isAssigned</span></span>|<span data-ttu-id="79109-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="79109-174">Boolean</span></span>|<span data-ttu-id="79109-175">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="79109-175">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="79109-176">响应</span><span class="sxs-lookup"><span data-stu-id="79109-176">Response</span></span>
<span data-ttu-id="79109-177">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="79109-177">If successful, this method returns a `201 Created` response code and a [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79109-178">示例</span><span class="sxs-lookup"><span data-stu-id="79109-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="79109-179">请求</span><span class="sxs-lookup"><span data-stu-id="79109-179">Request</span></span>
<span data-ttu-id="79109-180">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="79109-180">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="79109-181">响应</span><span class="sxs-lookup"><span data-stu-id="79109-181">Response</span></span>
<span data-ttu-id="79109-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="79109-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






