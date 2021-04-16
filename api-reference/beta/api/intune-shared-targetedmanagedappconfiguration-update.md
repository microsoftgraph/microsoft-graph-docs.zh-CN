---
title: 更新 targetedManagedAppConfiguration
description: 更新 targetedManagedAppConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 40d96d22dc5437ce07e07f24e1c219802a674ad5
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868132"
---
# <a name="update-targetedmanagedappconfiguration"></a><span data-ttu-id="73761-103">更新 targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="73761-103">Update targetedManagedAppConfiguration</span></span>

<span data-ttu-id="73761-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73761-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="73761-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="73761-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="73761-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="73761-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73761-107">更新 [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="73761-107">Update the properties of a [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="73761-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="73761-108">Prerequisites</span></span>
<span data-ttu-id="73761-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="73761-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73761-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="73761-111">Permission type</span></span>|<span data-ttu-id="73761-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="73761-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73761-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="73761-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="73761-114">&nbsp; &nbsp; **移动应用管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="73761-114">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="73761-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73761-115">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="73761-116">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="73761-116">&nbsp; &nbsp; **Policy Set**</span></span>  | <span data-ttu-id="73761-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73761-117">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="73761-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="73761-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73761-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="73761-119">Not supported.</span></span>|
|<span data-ttu-id="73761-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="73761-120">Application</span></span>||
| <span data-ttu-id="73761-121">&nbsp; &nbsp; **移动应用管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="73761-121">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="73761-122">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73761-122">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="73761-123">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="73761-123">&nbsp; &nbsp; **Policy Set**</span></span>  | <span data-ttu-id="73761-124">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73761-124">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="73761-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="73761-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="73761-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="73761-126">Request headers</span></span>
|<span data-ttu-id="73761-127">标头</span><span class="sxs-lookup"><span data-stu-id="73761-127">Header</span></span>|<span data-ttu-id="73761-128">值</span><span class="sxs-lookup"><span data-stu-id="73761-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73761-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="73761-129">Authorization</span></span>|<span data-ttu-id="73761-130">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="73761-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73761-131">接受</span><span class="sxs-lookup"><span data-stu-id="73761-131">Accept</span></span>|<span data-ttu-id="73761-132">application/json</span><span class="sxs-lookup"><span data-stu-id="73761-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73761-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="73761-133">Request body</span></span>
<span data-ttu-id="73761-134">在请求正文中，提供 [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="73761-134">In the request body, supply a JSON representation for the [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object.</span></span>

<span data-ttu-id="73761-135">下表显示创建 [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="73761-135">The following table shows the properties that are required when you create the [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md).</span></span>

|<span data-ttu-id="73761-136">属性</span><span class="sxs-lookup"><span data-stu-id="73761-136">Property</span></span>|<span data-ttu-id="73761-137">类型</span><span class="sxs-lookup"><span data-stu-id="73761-137">Type</span></span>|<span data-ttu-id="73761-138">说明</span><span class="sxs-lookup"><span data-stu-id="73761-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73761-139">displayName</span><span class="sxs-lookup"><span data-stu-id="73761-139">displayName</span></span>|<span data-ttu-id="73761-140">String</span><span class="sxs-lookup"><span data-stu-id="73761-140">String</span></span>|<span data-ttu-id="73761-141">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="73761-141">Policy display name.</span></span> <span data-ttu-id="73761-142">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="73761-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="73761-143">说明</span><span class="sxs-lookup"><span data-stu-id="73761-143">description</span></span>|<span data-ttu-id="73761-144">String</span><span class="sxs-lookup"><span data-stu-id="73761-144">String</span></span>|<span data-ttu-id="73761-145">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="73761-145">The policy's description.</span></span> <span data-ttu-id="73761-146">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="73761-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="73761-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="73761-147">createdDateTime</span></span>|<span data-ttu-id="73761-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73761-148">DateTimeOffset</span></span>|<span data-ttu-id="73761-149">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="73761-149">The date and time the policy was created.</span></span> <span data-ttu-id="73761-150">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="73761-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="73761-151">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="73761-151">lastModifiedDateTime</span></span>|<span data-ttu-id="73761-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73761-152">DateTimeOffset</span></span>|<span data-ttu-id="73761-153">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="73761-153">Last time the policy was modified.</span></span> <span data-ttu-id="73761-154">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="73761-154">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="73761-155">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="73761-155">roleScopeTagIds</span></span>|<span data-ttu-id="73761-156">String 集合</span><span class="sxs-lookup"><span data-stu-id="73761-156">String collection</span></span>|<span data-ttu-id="73761-157">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="73761-157">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="73761-158">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="73761-158">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="73761-159">id</span><span class="sxs-lookup"><span data-stu-id="73761-159">id</span></span>|<span data-ttu-id="73761-160">String</span><span class="sxs-lookup"><span data-stu-id="73761-160">String</span></span>|<span data-ttu-id="73761-161">实体的键。</span><span class="sxs-lookup"><span data-stu-id="73761-161">Key of the entity.</span></span> <span data-ttu-id="73761-162">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="73761-162">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="73761-163">version</span><span class="sxs-lookup"><span data-stu-id="73761-163">version</span></span>|<span data-ttu-id="73761-164">String</span><span class="sxs-lookup"><span data-stu-id="73761-164">String</span></span>|<span data-ttu-id="73761-165">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="73761-165">Version of the entity.</span></span> <span data-ttu-id="73761-166">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="73761-166">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="73761-167">customSettings</span><span class="sxs-lookup"><span data-stu-id="73761-167">customSettings</span></span>|<span data-ttu-id="73761-168">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="73761-168">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="73761-169">要发送到配置范围确定的用户应用的一组字符串键和字符串值对，不由此服务更改。继承自 [ managedAppConfiguration ](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73761-169">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="73761-170">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="73761-170">deployedAppCount</span></span>|<span data-ttu-id="73761-171">Int32</span><span class="sxs-lookup"><span data-stu-id="73761-171">Int32</span></span>|<span data-ttu-id="73761-172">当前策略部署到的应用的计数。</span><span class="sxs-lookup"><span data-stu-id="73761-172">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="73761-173">isAssigned</span><span class="sxs-lookup"><span data-stu-id="73761-173">isAssigned</span></span>|<span data-ttu-id="73761-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="73761-174">Boolean</span></span>|<span data-ttu-id="73761-175">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="73761-175">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="73761-176">响应</span><span class="sxs-lookup"><span data-stu-id="73761-176">Response</span></span>
<span data-ttu-id="73761-177">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="73761-177">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73761-178">示例</span><span class="sxs-lookup"><span data-stu-id="73761-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="73761-179">请求</span><span class="sxs-lookup"><span data-stu-id="73761-179">Request</span></span>
<span data-ttu-id="73761-180">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="73761-180">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
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

### <a name="response"></a><span data-ttu-id="73761-181">响应</span><span class="sxs-lookup"><span data-stu-id="73761-181">Response</span></span>
<span data-ttu-id="73761-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="73761-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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







