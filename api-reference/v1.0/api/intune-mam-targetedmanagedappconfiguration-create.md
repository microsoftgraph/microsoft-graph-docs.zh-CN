---
title: 创建 targetedManagedAppConfiguration
description: 创建新的 targetedManagedAppConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2b0745e3ed0ee59502508ef03f2bc1b6559312e2
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760340"
---
# <a name="create-targetedmanagedappconfiguration"></a><span data-ttu-id="81a84-103">创建 targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="81a84-103">Create targetedManagedAppConfiguration</span></span>

<span data-ttu-id="81a84-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81a84-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="81a84-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="81a84-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81a84-106">创建新的 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="81a84-106">Create a new [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="81a84-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="81a84-107">Prerequisites</span></span>
<span data-ttu-id="81a84-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="81a84-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81a84-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="81a84-110">Permission type</span></span>|<span data-ttu-id="81a84-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="81a84-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81a84-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="81a84-112">Delegated (work or school account)</span></span>|<span data-ttu-id="81a84-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81a84-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="81a84-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="81a84-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81a84-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="81a84-115">Not supported.</span></span>|
|<span data-ttu-id="81a84-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="81a84-116">Application</span></span>|<span data-ttu-id="81a84-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81a84-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="81a84-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="81a84-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="81a84-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="81a84-119">Request headers</span></span>
|<span data-ttu-id="81a84-120">标头</span><span class="sxs-lookup"><span data-stu-id="81a84-120">Header</span></span>|<span data-ttu-id="81a84-121">值</span><span class="sxs-lookup"><span data-stu-id="81a84-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="81a84-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="81a84-122">Authorization</span></span>|<span data-ttu-id="81a84-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="81a84-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="81a84-124">接受</span><span class="sxs-lookup"><span data-stu-id="81a84-124">Accept</span></span>|<span data-ttu-id="81a84-125">application/json</span><span class="sxs-lookup"><span data-stu-id="81a84-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="81a84-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="81a84-126">Request body</span></span>
<span data-ttu-id="81a84-127">在请求正文中，提供 targetedManagedAppConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="81a84-127">In the request body, supply a JSON representation for the targetedManagedAppConfiguration object.</span></span>

<span data-ttu-id="81a84-128">下表显示创建 targetedManagedAppConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="81a84-128">The following table shows the properties that are required when you create the targetedManagedAppConfiguration.</span></span>

|<span data-ttu-id="81a84-129">属性</span><span class="sxs-lookup"><span data-stu-id="81a84-129">Property</span></span>|<span data-ttu-id="81a84-130">类型</span><span class="sxs-lookup"><span data-stu-id="81a84-130">Type</span></span>|<span data-ttu-id="81a84-131">说明</span><span class="sxs-lookup"><span data-stu-id="81a84-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81a84-132">displayName</span><span class="sxs-lookup"><span data-stu-id="81a84-132">displayName</span></span>|<span data-ttu-id="81a84-133">String</span><span class="sxs-lookup"><span data-stu-id="81a84-133">String</span></span>|<span data-ttu-id="81a84-134">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="81a84-134">Policy display name.</span></span> <span data-ttu-id="81a84-135">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="81a84-135">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="81a84-136">description</span><span class="sxs-lookup"><span data-stu-id="81a84-136">description</span></span>|<span data-ttu-id="81a84-137">String</span><span class="sxs-lookup"><span data-stu-id="81a84-137">String</span></span>|<span data-ttu-id="81a84-138">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="81a84-138">The policy's description.</span></span> <span data-ttu-id="81a84-139">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="81a84-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="81a84-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="81a84-140">createdDateTime</span></span>|<span data-ttu-id="81a84-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81a84-141">DateTimeOffset</span></span>|<span data-ttu-id="81a84-142">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="81a84-142">The date and time the policy was created.</span></span> <span data-ttu-id="81a84-143">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="81a84-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="81a84-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="81a84-144">lastModifiedDateTime</span></span>|<span data-ttu-id="81a84-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81a84-145">DateTimeOffset</span></span>|<span data-ttu-id="81a84-146">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="81a84-146">Last time the policy was modified.</span></span> <span data-ttu-id="81a84-147">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="81a84-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="81a84-148">id</span><span class="sxs-lookup"><span data-stu-id="81a84-148">id</span></span>|<span data-ttu-id="81a84-149">String</span><span class="sxs-lookup"><span data-stu-id="81a84-149">String</span></span>|<span data-ttu-id="81a84-150">实体的键。</span><span class="sxs-lookup"><span data-stu-id="81a84-150">Key of the entity.</span></span> <span data-ttu-id="81a84-151">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="81a84-151">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="81a84-152">version</span><span class="sxs-lookup"><span data-stu-id="81a84-152">version</span></span>|<span data-ttu-id="81a84-153">String</span><span class="sxs-lookup"><span data-stu-id="81a84-153">String</span></span>|<span data-ttu-id="81a84-154">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="81a84-154">Version of the entity.</span></span> <span data-ttu-id="81a84-155">继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="81a84-155">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="81a84-156">customSettings</span><span class="sxs-lookup"><span data-stu-id="81a84-156">customSettings</span></span>|<span data-ttu-id="81a84-157">[keyValuePair](../resources/intune-mam-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="81a84-157">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="81a84-158">要发送到配置范围确定的用户应用的一组字符串键和字符串值对，不由此服务更改。继承自 [ managedAppConfiguration ](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="81a84-158">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="81a84-159">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="81a84-159">deployedAppCount</span></span>|<span data-ttu-id="81a84-160">Int32</span><span class="sxs-lookup"><span data-stu-id="81a84-160">Int32</span></span>|<span data-ttu-id="81a84-161">当前策略部署到的应用的计数。</span><span class="sxs-lookup"><span data-stu-id="81a84-161">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="81a84-162">isAssigned</span><span class="sxs-lookup"><span data-stu-id="81a84-162">isAssigned</span></span>|<span data-ttu-id="81a84-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="81a84-163">Boolean</span></span>|<span data-ttu-id="81a84-164">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="81a84-164">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="81a84-165">响应</span><span class="sxs-lookup"><span data-stu-id="81a84-165">Response</span></span>
<span data-ttu-id="81a84-166">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="81a84-166">If successful, this method returns a `201 Created` response code and a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81a84-167">示例</span><span class="sxs-lookup"><span data-stu-id="81a84-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="81a84-168">请求</span><span class="sxs-lookup"><span data-stu-id="81a84-168">Request</span></span>
<span data-ttu-id="81a84-169">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="81a84-169">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/targetedManagedAppConfigurations
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

### <a name="response"></a><span data-ttu-id="81a84-170">响应</span><span class="sxs-lookup"><span data-stu-id="81a84-170">Response</span></span>
<span data-ttu-id="81a84-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="81a84-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




