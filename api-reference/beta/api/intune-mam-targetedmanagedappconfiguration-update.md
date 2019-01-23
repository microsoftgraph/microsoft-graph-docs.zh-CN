---
title: 更新 targetedManagedAppConfiguration
description: 更新 targetedManagedAppConfiguration 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: eded21015054073b6f6711faecd5c01da52fece0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403691"
---
# <a name="update-targetedmanagedappconfiguration"></a><span data-ttu-id="a2af1-103">更新 targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="a2af1-103">Update targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="a2af1-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="a2af1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a2af1-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a2af1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a2af1-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a2af1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2af1-107">更新 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a2af1-107">Update the properties of a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a2af1-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a2af1-108">Prerequisites</span></span>
<span data-ttu-id="a2af1-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a2af1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a2af1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a2af1-111">Permission type</span></span>|<span data-ttu-id="a2af1-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a2af1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2af1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a2af1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a2af1-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2af1-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a2af1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a2af1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2af1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a2af1-116">Not supported.</span></span>|
|<span data-ttu-id="a2af1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a2af1-117">Application</span></span>|<span data-ttu-id="a2af1-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="a2af1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2af1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a2af1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a2af1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a2af1-120">Request headers</span></span>
|<span data-ttu-id="a2af1-121">标头</span><span class="sxs-lookup"><span data-stu-id="a2af1-121">Header</span></span>|<span data-ttu-id="a2af1-122">值</span><span class="sxs-lookup"><span data-stu-id="a2af1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2af1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2af1-123">Authorization</span></span>|<span data-ttu-id="a2af1-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a2af1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2af1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a2af1-125">Accept</span></span>|<span data-ttu-id="a2af1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a2af1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2af1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a2af1-127">Request body</span></span>
<span data-ttu-id="a2af1-128">在请求正文中，提供 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a2af1-128">In the request body, supply a JSON representation for the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>

<span data-ttu-id="a2af1-129">下表显示创建 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a2af1-129">The following table shows the properties that are required when you create the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span></span>

|<span data-ttu-id="a2af1-130">属性</span><span class="sxs-lookup"><span data-stu-id="a2af1-130">Property</span></span>|<span data-ttu-id="a2af1-131">类型</span><span class="sxs-lookup"><span data-stu-id="a2af1-131">Type</span></span>|<span data-ttu-id="a2af1-132">说明</span><span class="sxs-lookup"><span data-stu-id="a2af1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2af1-133">displayName</span><span class="sxs-lookup"><span data-stu-id="a2af1-133">displayName</span></span>|<span data-ttu-id="a2af1-134">String</span><span class="sxs-lookup"><span data-stu-id="a2af1-134">String</span></span>|<span data-ttu-id="a2af1-135">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="a2af1-135">Policy display name.</span></span> <span data-ttu-id="a2af1-136">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a2af1-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a2af1-137">description</span><span class="sxs-lookup"><span data-stu-id="a2af1-137">description</span></span>|<span data-ttu-id="a2af1-138">String</span><span class="sxs-lookup"><span data-stu-id="a2af1-138">String</span></span>|<span data-ttu-id="a2af1-139">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="a2af1-139">The policy's description.</span></span> <span data-ttu-id="a2af1-140">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a2af1-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a2af1-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a2af1-141">createdDateTime</span></span>|<span data-ttu-id="a2af1-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2af1-142">DateTimeOffset</span></span>|<span data-ttu-id="a2af1-143">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a2af1-143">The date and time the policy was created.</span></span> <span data-ttu-id="a2af1-144">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a2af1-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a2af1-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a2af1-145">lastModifiedDateTime</span></span>|<span data-ttu-id="a2af1-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2af1-146">DateTimeOffset</span></span>|<span data-ttu-id="a2af1-147">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="a2af1-147">Last time the policy was modified.</span></span> <span data-ttu-id="a2af1-148">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a2af1-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a2af1-149">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a2af1-149">roleScopeTagIds</span></span>|<span data-ttu-id="a2af1-150">String 集合</span><span class="sxs-lookup"><span data-stu-id="a2af1-150">String collection</span></span>|<span data-ttu-id="a2af1-151">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="a2af1-151">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a2af1-152">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a2af1-152">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a2af1-153">id</span><span class="sxs-lookup"><span data-stu-id="a2af1-153">id</span></span>|<span data-ttu-id="a2af1-154">String</span><span class="sxs-lookup"><span data-stu-id="a2af1-154">String</span></span>|<span data-ttu-id="a2af1-155">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a2af1-155">Key of the entity.</span></span> <span data-ttu-id="a2af1-156">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a2af1-156">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a2af1-157">version</span><span class="sxs-lookup"><span data-stu-id="a2af1-157">version</span></span>|<span data-ttu-id="a2af1-158">String</span><span class="sxs-lookup"><span data-stu-id="a2af1-158">String</span></span>|<span data-ttu-id="a2af1-159">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="a2af1-159">Version of the entity.</span></span> <span data-ttu-id="a2af1-160">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a2af1-160">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a2af1-161">customSettings</span><span class="sxs-lookup"><span data-stu-id="a2af1-161">customSettings</span></span>|<span data-ttu-id="a2af1-162">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a2af1-162">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="a2af1-163">要发送到配置范围确定的用户应用的一组字符串键和字符串值对，不由此服务更改。继承自 [ managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a2af1-163">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="a2af1-164">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="a2af1-164">deployedAppCount</span></span>|<span data-ttu-id="a2af1-165">Int32</span><span class="sxs-lookup"><span data-stu-id="a2af1-165">Int32</span></span>|<span data-ttu-id="a2af1-166">当前策略部署到的应用的计数。</span><span class="sxs-lookup"><span data-stu-id="a2af1-166">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="a2af1-167">isAssigned</span><span class="sxs-lookup"><span data-stu-id="a2af1-167">isAssigned</span></span>|<span data-ttu-id="a2af1-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2af1-168">Boolean</span></span>|<span data-ttu-id="a2af1-169">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="a2af1-169">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="a2af1-170">响应</span><span class="sxs-lookup"><span data-stu-id="a2af1-170">Response</span></span>
<span data-ttu-id="a2af1-171">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a2af1-171">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2af1-172">示例</span><span class="sxs-lookup"><span data-stu-id="a2af1-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="a2af1-173">请求</span><span class="sxs-lookup"><span data-stu-id="a2af1-173">Request</span></span>
<span data-ttu-id="a2af1-174">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a2af1-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a2af1-175">响应</span><span class="sxs-lookup"><span data-stu-id="a2af1-175">Response</span></span>
<span data-ttu-id="a2af1-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a2af1-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




