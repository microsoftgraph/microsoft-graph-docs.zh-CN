---
title: 更新 defaultDeviceCompliancePolicy
description: 更新 defaultDeviceCompliancePolicy 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 161bbba9dccd8a7e554c8a377f2befed0070585d
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42756552"
---
# <a name="update-defaultdevicecompliancepolicy"></a><span data-ttu-id="93852-103">更新 defaultDeviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="93852-103">Update defaultDeviceCompliancePolicy</span></span>

> <span data-ttu-id="93852-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="93852-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="93852-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="93852-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93852-106">更新[defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="93852-106">Update the properties of a [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="93852-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="93852-107">Prerequisites</span></span>
<span data-ttu-id="93852-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="93852-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93852-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="93852-110">Permission type</span></span>|<span data-ttu-id="93852-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="93852-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="93852-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="93852-112">Delegated (work or school account)</span></span>|<span data-ttu-id="93852-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93852-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="93852-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="93852-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="93852-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="93852-115">Not supported.</span></span>|
|<span data-ttu-id="93852-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="93852-116">Application</span></span>|<span data-ttu-id="93852-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93852-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="93852-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="93852-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="93852-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="93852-119">Request headers</span></span>
|<span data-ttu-id="93852-120">标头</span><span class="sxs-lookup"><span data-stu-id="93852-120">Header</span></span>|<span data-ttu-id="93852-121">值</span><span class="sxs-lookup"><span data-stu-id="93852-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="93852-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="93852-122">Authorization</span></span>|<span data-ttu-id="93852-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="93852-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="93852-124">接受</span><span class="sxs-lookup"><span data-stu-id="93852-124">Accept</span></span>|<span data-ttu-id="93852-125">application/json</span><span class="sxs-lookup"><span data-stu-id="93852-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="93852-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="93852-126">Request body</span></span>
<span data-ttu-id="93852-127">在请求正文中，提供[defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="93852-127">In the request body, supply a JSON representation for the [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>

<span data-ttu-id="93852-128">下表显示创建[defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="93852-128">The following table shows the properties that are required when you create the [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md).</span></span>

|<span data-ttu-id="93852-129">属性</span><span class="sxs-lookup"><span data-stu-id="93852-129">Property</span></span>|<span data-ttu-id="93852-130">类型</span><span class="sxs-lookup"><span data-stu-id="93852-130">Type</span></span>|<span data-ttu-id="93852-131">说明</span><span class="sxs-lookup"><span data-stu-id="93852-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93852-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="93852-132">roleScopeTagIds</span></span>|<span data-ttu-id="93852-133">String collection</span><span class="sxs-lookup"><span data-stu-id="93852-133">String collection</span></span>|<span data-ttu-id="93852-134">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="93852-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="93852-135">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="93852-135">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="93852-136">id</span><span class="sxs-lookup"><span data-stu-id="93852-136">id</span></span>|<span data-ttu-id="93852-137">字符串</span><span class="sxs-lookup"><span data-stu-id="93852-137">String</span></span>|<span data-ttu-id="93852-138">实体的键。</span><span class="sxs-lookup"><span data-stu-id="93852-138">Key of the entity.</span></span> <span data-ttu-id="93852-139">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="93852-139">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="93852-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="93852-140">createdDateTime</span></span>|<span data-ttu-id="93852-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93852-141">DateTimeOffset</span></span>|<span data-ttu-id="93852-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="93852-142">DateTime the object was created.</span></span> <span data-ttu-id="93852-143">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="93852-143">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="93852-144">说明</span><span class="sxs-lookup"><span data-stu-id="93852-144">description</span></span>|<span data-ttu-id="93852-145">String</span><span class="sxs-lookup"><span data-stu-id="93852-145">String</span></span>|<span data-ttu-id="93852-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="93852-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="93852-147">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="93852-147">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="93852-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="93852-148">lastModifiedDateTime</span></span>|<span data-ttu-id="93852-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93852-149">DateTimeOffset</span></span>|<span data-ttu-id="93852-150">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="93852-150">DateTime the object was last modified.</span></span> <span data-ttu-id="93852-151">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="93852-151">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="93852-152">displayName</span><span class="sxs-lookup"><span data-stu-id="93852-152">displayName</span></span>|<span data-ttu-id="93852-153">String</span><span class="sxs-lookup"><span data-stu-id="93852-153">String</span></span>|<span data-ttu-id="93852-154">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="93852-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="93852-155">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="93852-155">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="93852-156">version</span><span class="sxs-lookup"><span data-stu-id="93852-156">version</span></span>|<span data-ttu-id="93852-157">Int32</span><span class="sxs-lookup"><span data-stu-id="93852-157">Int32</span></span>|<span data-ttu-id="93852-158">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="93852-158">Version of the device configuration.</span></span> <span data-ttu-id="93852-159">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="93852-159">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|



## <a name="response"></a><span data-ttu-id="93852-160">响应</span><span class="sxs-lookup"><span data-stu-id="93852-160">Response</span></span>
<span data-ttu-id="93852-161">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="93852-161">If successful, this method returns a `200 OK` response code and an updated [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93852-162">示例</span><span class="sxs-lookup"><span data-stu-id="93852-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="93852-163">请求</span><span class="sxs-lookup"><span data-stu-id="93852-163">Request</span></span>
<span data-ttu-id="93852-164">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="93852-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
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

### <a name="response"></a><span data-ttu-id="93852-165">响应</span><span class="sxs-lookup"><span data-stu-id="93852-165">Response</span></span>
<span data-ttu-id="93852-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="93852-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




