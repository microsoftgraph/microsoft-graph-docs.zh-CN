---
title: 创建 targetedManagedAppConfiguration
description: 创建新的 targetedManagedAppConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6dba486742bb93879e13a43f2967a7117bd3776d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163614"
---
# <a name="create-targetedmanagedappconfiguration"></a><span data-ttu-id="b3318-103">创建 targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="b3318-103">Create targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="b3318-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b3318-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b3318-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b3318-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3318-106">创建新的 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b3318-106">Create a new [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b3318-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="b3318-107">Prerequisites</span></span>
<span data-ttu-id="b3318-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="b3318-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b3318-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b3318-110">Permission type</span></span>|<span data-ttu-id="b3318-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b3318-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3318-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b3318-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b3318-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3318-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b3318-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b3318-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3318-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b3318-115">Not supported.</span></span>|
|<span data-ttu-id="b3318-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b3318-116">Application</span></span>|<span data-ttu-id="b3318-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b3318-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3318-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b3318-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b3318-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b3318-119">Request headers</span></span>
|<span data-ttu-id="b3318-120">标头</span><span class="sxs-lookup"><span data-stu-id="b3318-120">Header</span></span>|<span data-ttu-id="b3318-121">值</span><span class="sxs-lookup"><span data-stu-id="b3318-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3318-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3318-122">Authorization</span></span>|<span data-ttu-id="b3318-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b3318-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3318-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b3318-124">Accept</span></span>|<span data-ttu-id="b3318-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b3318-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3318-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b3318-126">Request body</span></span>
<span data-ttu-id="b3318-127">在请求正文中，提供 targetedManagedAppConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b3318-127">In the request body, supply a JSON representation for the targetedManagedAppConfiguration object.</span></span>

<span data-ttu-id="b3318-128">下表显示创建 targetedManagedAppConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b3318-128">The following table shows the properties that are required when you create the targetedManagedAppConfiguration.</span></span>

|<span data-ttu-id="b3318-129">属性</span><span class="sxs-lookup"><span data-stu-id="b3318-129">Property</span></span>|<span data-ttu-id="b3318-130">类型</span><span class="sxs-lookup"><span data-stu-id="b3318-130">Type</span></span>|<span data-ttu-id="b3318-131">说明</span><span class="sxs-lookup"><span data-stu-id="b3318-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3318-132">displayName</span><span class="sxs-lookup"><span data-stu-id="b3318-132">displayName</span></span>|<span data-ttu-id="b3318-133">String</span><span class="sxs-lookup"><span data-stu-id="b3318-133">String</span></span>|<span data-ttu-id="b3318-134">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="b3318-134">Policy display name.</span></span> <span data-ttu-id="b3318-135">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b3318-135">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b3318-136">description</span><span class="sxs-lookup"><span data-stu-id="b3318-136">description</span></span>|<span data-ttu-id="b3318-137">String</span><span class="sxs-lookup"><span data-stu-id="b3318-137">String</span></span>|<span data-ttu-id="b3318-138">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="b3318-138">The policy's description.</span></span> <span data-ttu-id="b3318-139">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b3318-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b3318-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b3318-140">createdDateTime</span></span>|<span data-ttu-id="b3318-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3318-141">DateTimeOffset</span></span>|<span data-ttu-id="b3318-142">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b3318-142">The date and time the policy was created.</span></span> <span data-ttu-id="b3318-143">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b3318-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b3318-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b3318-144">lastModifiedDateTime</span></span>|<span data-ttu-id="b3318-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3318-145">DateTimeOffset</span></span>|<span data-ttu-id="b3318-146">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="b3318-146">Last time the policy was modified.</span></span> <span data-ttu-id="b3318-147">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b3318-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b3318-148">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b3318-148">roleScopeTagIds</span></span>|<span data-ttu-id="b3318-149">String collection</span><span class="sxs-lookup"><span data-stu-id="b3318-149">String collection</span></span>|<span data-ttu-id="b3318-150">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="b3318-150">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b3318-151">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b3318-151">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b3318-152">id</span><span class="sxs-lookup"><span data-stu-id="b3318-152">id</span></span>|<span data-ttu-id="b3318-153">字符串</span><span class="sxs-lookup"><span data-stu-id="b3318-153">String</span></span>|<span data-ttu-id="b3318-154">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b3318-154">Key of the entity.</span></span> <span data-ttu-id="b3318-155">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b3318-155">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b3318-156">version</span><span class="sxs-lookup"><span data-stu-id="b3318-156">version</span></span>|<span data-ttu-id="b3318-157">String</span><span class="sxs-lookup"><span data-stu-id="b3318-157">String</span></span>|<span data-ttu-id="b3318-158">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="b3318-158">Version of the entity.</span></span> <span data-ttu-id="b3318-159">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b3318-159">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b3318-160">customSettings</span><span class="sxs-lookup"><span data-stu-id="b3318-160">customSettings</span></span>|<span data-ttu-id="b3318-161">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b3318-161">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="b3318-162">要发送到配置范围确定的用户应用的一组字符串键和字符串值对，不由此服务更改。继承自 [ managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3318-162">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="b3318-163">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="b3318-163">deployedAppCount</span></span>|<span data-ttu-id="b3318-164">Int32</span><span class="sxs-lookup"><span data-stu-id="b3318-164">Int32</span></span>|<span data-ttu-id="b3318-165">当前策略部署到的应用的计数。</span><span class="sxs-lookup"><span data-stu-id="b3318-165">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="b3318-166">isAssigned</span><span class="sxs-lookup"><span data-stu-id="b3318-166">isAssigned</span></span>|<span data-ttu-id="b3318-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3318-167">Boolean</span></span>|<span data-ttu-id="b3318-168">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="b3318-168">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="b3318-169">响应</span><span class="sxs-lookup"><span data-stu-id="b3318-169">Response</span></span>
<span data-ttu-id="b3318-170">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b3318-170">If successful, this method returns a `201 Created` response code and a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3318-171">示例</span><span class="sxs-lookup"><span data-stu-id="b3318-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="b3318-172">请求</span><span class="sxs-lookup"><span data-stu-id="b3318-172">Request</span></span>
<span data-ttu-id="b3318-173">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b3318-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b3318-174">响应</span><span class="sxs-lookup"><span data-stu-id="b3318-174">Response</span></span>
<span data-ttu-id="b3318-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b3318-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




