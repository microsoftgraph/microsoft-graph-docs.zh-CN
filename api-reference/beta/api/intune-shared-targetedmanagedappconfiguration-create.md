---
title: 创建 targetedManagedAppConfiguration
description: 创建新的 targetedManagedAppConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 42590a25bed7860136c0434c44a2cb43546e0856
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48004779"
---
# <a name="create-targetedmanagedappconfiguration"></a><span data-ttu-id="efe83-103">创建 targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="efe83-103">Create targetedManagedAppConfiguration</span></span>

<span data-ttu-id="efe83-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="efe83-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="efe83-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="efe83-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="efe83-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="efe83-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="efe83-107">创建新的 [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="efe83-107">Create a new [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="efe83-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="efe83-108">Prerequisites</span></span>
<span data-ttu-id="efe83-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="efe83-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efe83-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="efe83-111">Permission type</span></span>|<span data-ttu-id="efe83-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="efe83-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="efe83-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="efe83-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="efe83-114">&nbsp; &nbsp; **移动应用管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="efe83-114">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="efe83-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efe83-115">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="efe83-116">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="efe83-116">&nbsp; &nbsp; **Policy Set**</span></span>  | <span data-ttu-id="efe83-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efe83-117">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="efe83-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="efe83-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="efe83-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="efe83-119">Not supported.</span></span>|
|<span data-ttu-id="efe83-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="efe83-120">Application</span></span>||
| <span data-ttu-id="efe83-121">&nbsp; &nbsp; **移动应用管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="efe83-121">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="efe83-122">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efe83-122">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="efe83-123">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="efe83-123">&nbsp; &nbsp; **Policy Set**</span></span>  | <span data-ttu-id="efe83-124">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efe83-124">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="efe83-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="efe83-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="efe83-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="efe83-126">Request headers</span></span>
|<span data-ttu-id="efe83-127">标头</span><span class="sxs-lookup"><span data-stu-id="efe83-127">Header</span></span>|<span data-ttu-id="efe83-128">值</span><span class="sxs-lookup"><span data-stu-id="efe83-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="efe83-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="efe83-129">Authorization</span></span>|<span data-ttu-id="efe83-130">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="efe83-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="efe83-131">接受</span><span class="sxs-lookup"><span data-stu-id="efe83-131">Accept</span></span>|<span data-ttu-id="efe83-132">application/json</span><span class="sxs-lookup"><span data-stu-id="efe83-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="efe83-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="efe83-133">Request body</span></span>
<span data-ttu-id="efe83-134">在请求正文中，提供 targetedManagedAppConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="efe83-134">In the request body, supply a JSON representation for the targetedManagedAppConfiguration object.</span></span>

<span data-ttu-id="efe83-135">下表显示创建 targetedManagedAppConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="efe83-135">The following table shows the properties that are required when you create the targetedManagedAppConfiguration.</span></span>

|<span data-ttu-id="efe83-136">属性</span><span class="sxs-lookup"><span data-stu-id="efe83-136">Property</span></span>|<span data-ttu-id="efe83-137">类型</span><span class="sxs-lookup"><span data-stu-id="efe83-137">Type</span></span>|<span data-ttu-id="efe83-138">说明</span><span class="sxs-lookup"><span data-stu-id="efe83-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efe83-139">displayName</span><span class="sxs-lookup"><span data-stu-id="efe83-139">displayName</span></span>|<span data-ttu-id="efe83-140">String</span><span class="sxs-lookup"><span data-stu-id="efe83-140">String</span></span>|<span data-ttu-id="efe83-141">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="efe83-141">Policy display name.</span></span> <span data-ttu-id="efe83-142">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="efe83-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="efe83-143">description</span><span class="sxs-lookup"><span data-stu-id="efe83-143">description</span></span>|<span data-ttu-id="efe83-144">String</span><span class="sxs-lookup"><span data-stu-id="efe83-144">String</span></span>|<span data-ttu-id="efe83-145">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="efe83-145">The policy's description.</span></span> <span data-ttu-id="efe83-146">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="efe83-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="efe83-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="efe83-147">createdDateTime</span></span>|<span data-ttu-id="efe83-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="efe83-148">DateTimeOffset</span></span>|<span data-ttu-id="efe83-149">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="efe83-149">The date and time the policy was created.</span></span> <span data-ttu-id="efe83-150">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="efe83-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="efe83-151">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="efe83-151">lastModifiedDateTime</span></span>|<span data-ttu-id="efe83-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="efe83-152">DateTimeOffset</span></span>|<span data-ttu-id="efe83-153">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="efe83-153">Last time the policy was modified.</span></span> <span data-ttu-id="efe83-154">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="efe83-154">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="efe83-155">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="efe83-155">roleScopeTagIds</span></span>|<span data-ttu-id="efe83-156">String collection</span><span class="sxs-lookup"><span data-stu-id="efe83-156">String collection</span></span>|<span data-ttu-id="efe83-157">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="efe83-157">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="efe83-158">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="efe83-158">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="efe83-159">id</span><span class="sxs-lookup"><span data-stu-id="efe83-159">id</span></span>|<span data-ttu-id="efe83-160">String</span><span class="sxs-lookup"><span data-stu-id="efe83-160">String</span></span>|<span data-ttu-id="efe83-161">实体的键。</span><span class="sxs-lookup"><span data-stu-id="efe83-161">Key of the entity.</span></span> <span data-ttu-id="efe83-162">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="efe83-162">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="efe83-163">version</span><span class="sxs-lookup"><span data-stu-id="efe83-163">version</span></span>|<span data-ttu-id="efe83-164">String</span><span class="sxs-lookup"><span data-stu-id="efe83-164">String</span></span>|<span data-ttu-id="efe83-165">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="efe83-165">Version of the entity.</span></span> <span data-ttu-id="efe83-166">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="efe83-166">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="efe83-167">customSettings</span><span class="sxs-lookup"><span data-stu-id="efe83-167">customSettings</span></span>|<span data-ttu-id="efe83-168">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="efe83-168">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="efe83-169">要发送到配置范围确定的用户应用的一组字符串键和字符串值对，不由此服务更改。继承自 [ managedAppConfiguration ](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="efe83-169">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="efe83-170">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="efe83-170">deployedAppCount</span></span>|<span data-ttu-id="efe83-171">Int32</span><span class="sxs-lookup"><span data-stu-id="efe83-171">Int32</span></span>|<span data-ttu-id="efe83-172">当前策略部署到的应用的计数。</span><span class="sxs-lookup"><span data-stu-id="efe83-172">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="efe83-173">isAssigned</span><span class="sxs-lookup"><span data-stu-id="efe83-173">isAssigned</span></span>|<span data-ttu-id="efe83-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="efe83-174">Boolean</span></span>|<span data-ttu-id="efe83-175">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="efe83-175">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="efe83-176">响应</span><span class="sxs-lookup"><span data-stu-id="efe83-176">Response</span></span>
<span data-ttu-id="efe83-177">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="efe83-177">If successful, this method returns a `201 Created` response code and a [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="efe83-178">示例</span><span class="sxs-lookup"><span data-stu-id="efe83-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="efe83-179">请求</span><span class="sxs-lookup"><span data-stu-id="efe83-179">Request</span></span>
<span data-ttu-id="efe83-180">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="efe83-180">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="efe83-181">响应</span><span class="sxs-lookup"><span data-stu-id="efe83-181">Response</span></span>
<span data-ttu-id="efe83-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="efe83-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









