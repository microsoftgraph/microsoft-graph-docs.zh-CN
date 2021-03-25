---
title: 创建 defaultDeviceCompliancePolicy
description: 创建新的 defaultDeviceCompliancePolicy 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8d529fe57fafe65355219750f8bd73ff764b7c3d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51155769"
---
# <a name="create-defaultdevicecompliancepolicy"></a><span data-ttu-id="0ecad-103">创建 defaultDeviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="0ecad-103">Create defaultDeviceCompliancePolicy</span></span>

<span data-ttu-id="0ecad-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ecad-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0ecad-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0ecad-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0ecad-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0ecad-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ecad-107">创建新的 [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0ecad-107">Create a new [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0ecad-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="0ecad-108">Prerequisites</span></span>
<span data-ttu-id="0ecad-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0ecad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ecad-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0ecad-111">Permission type</span></span>|<span data-ttu-id="0ecad-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0ecad-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ecad-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0ecad-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0ecad-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ecad-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0ecad-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0ecad-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ecad-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0ecad-116">Not supported.</span></span>|
|<span data-ttu-id="0ecad-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0ecad-117">Application</span></span>|<span data-ttu-id="0ecad-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ecad-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ecad-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0ecad-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="0ecad-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0ecad-120">Request headers</span></span>
|<span data-ttu-id="0ecad-121">标头</span><span class="sxs-lookup"><span data-stu-id="0ecad-121">Header</span></span>|<span data-ttu-id="0ecad-122">值</span><span class="sxs-lookup"><span data-stu-id="0ecad-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ecad-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ecad-123">Authorization</span></span>|<span data-ttu-id="0ecad-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0ecad-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ecad-125">接受</span><span class="sxs-lookup"><span data-stu-id="0ecad-125">Accept</span></span>|<span data-ttu-id="0ecad-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0ecad-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ecad-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0ecad-127">Request body</span></span>
<span data-ttu-id="0ecad-128">在请求正文中，提供 defaultDeviceCompliancePolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0ecad-128">In the request body, supply a JSON representation for the defaultDeviceCompliancePolicy object.</span></span>

<span data-ttu-id="0ecad-129">下表显示创建 defaultDeviceCompliancePolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0ecad-129">The following table shows the properties that are required when you create the defaultDeviceCompliancePolicy.</span></span>

|<span data-ttu-id="0ecad-130">属性</span><span class="sxs-lookup"><span data-stu-id="0ecad-130">Property</span></span>|<span data-ttu-id="0ecad-131">类型</span><span class="sxs-lookup"><span data-stu-id="0ecad-131">Type</span></span>|<span data-ttu-id="0ecad-132">说明</span><span class="sxs-lookup"><span data-stu-id="0ecad-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ecad-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0ecad-133">roleScopeTagIds</span></span>|<span data-ttu-id="0ecad-134">String collection</span><span class="sxs-lookup"><span data-stu-id="0ecad-134">String collection</span></span>|<span data-ttu-id="0ecad-135">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="0ecad-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0ecad-136">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0ecad-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0ecad-137">id</span><span class="sxs-lookup"><span data-stu-id="0ecad-137">id</span></span>|<span data-ttu-id="0ecad-138">String</span><span class="sxs-lookup"><span data-stu-id="0ecad-138">String</span></span>|<span data-ttu-id="0ecad-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0ecad-139">Key of the entity.</span></span> <span data-ttu-id="0ecad-140">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0ecad-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0ecad-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0ecad-141">createdDateTime</span></span>|<span data-ttu-id="0ecad-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ecad-142">DateTimeOffset</span></span>|<span data-ttu-id="0ecad-143">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0ecad-143">DateTime the object was created.</span></span> <span data-ttu-id="0ecad-144">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0ecad-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0ecad-145">说明</span><span class="sxs-lookup"><span data-stu-id="0ecad-145">description</span></span>|<span data-ttu-id="0ecad-146">String</span><span class="sxs-lookup"><span data-stu-id="0ecad-146">String</span></span>|<span data-ttu-id="0ecad-147">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="0ecad-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0ecad-148">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0ecad-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0ecad-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0ecad-149">lastModifiedDateTime</span></span>|<span data-ttu-id="0ecad-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ecad-150">DateTimeOffset</span></span>|<span data-ttu-id="0ecad-151">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0ecad-151">DateTime the object was last modified.</span></span> <span data-ttu-id="0ecad-152">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0ecad-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0ecad-153">displayName</span><span class="sxs-lookup"><span data-stu-id="0ecad-153">displayName</span></span>|<span data-ttu-id="0ecad-154">String</span><span class="sxs-lookup"><span data-stu-id="0ecad-154">String</span></span>|<span data-ttu-id="0ecad-155">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="0ecad-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0ecad-156">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0ecad-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0ecad-157">version</span><span class="sxs-lookup"><span data-stu-id="0ecad-157">version</span></span>|<span data-ttu-id="0ecad-158">Int32</span><span class="sxs-lookup"><span data-stu-id="0ecad-158">Int32</span></span>|<span data-ttu-id="0ecad-159">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="0ecad-159">Version of the device configuration.</span></span> <span data-ttu-id="0ecad-160">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0ecad-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|



## <a name="response"></a><span data-ttu-id="0ecad-161">响应</span><span class="sxs-lookup"><span data-stu-id="0ecad-161">Response</span></span>
<span data-ttu-id="0ecad-162">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0ecad-162">If successful, this method returns a `201 Created` response code and a [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ecad-163">示例</span><span class="sxs-lookup"><span data-stu-id="0ecad-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="0ecad-164">请求</span><span class="sxs-lookup"><span data-stu-id="0ecad-164">Request</span></span>
<span data-ttu-id="0ecad-165">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0ecad-165">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 229

{
  "@odata.type": "#microsoft.graph.defaultDeviceCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="0ecad-166">响应</span><span class="sxs-lookup"><span data-stu-id="0ecad-166">Response</span></span>
<span data-ttu-id="0ecad-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0ecad-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 401

{
  "@odata.type": "#microsoft.graph.defaultDeviceCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "a285f027-f027-a285-27f0-85a227f085a2",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7
}
```




