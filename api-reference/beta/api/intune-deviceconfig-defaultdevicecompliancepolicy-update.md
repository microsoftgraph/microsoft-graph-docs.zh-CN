---
title: 更新 defaultDeviceCompliancePolicy
description: 更新 defaultDeviceCompliancePolicy 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0f4f6a28704fd31cad93a48321100e1e286d8c22
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37534209"
---
# <a name="update-defaultdevicecompliancepolicy"></a><span data-ttu-id="c36f0-103">更新 defaultDeviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="c36f0-103">Update defaultDeviceCompliancePolicy</span></span>

> <span data-ttu-id="c36f0-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c36f0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c36f0-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c36f0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c36f0-106">更新[defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c36f0-106">Update the properties of a [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c36f0-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="c36f0-107">Prerequisites</span></span>
<span data-ttu-id="c36f0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c36f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c36f0-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c36f0-110">Permission type</span></span>|<span data-ttu-id="c36f0-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c36f0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c36f0-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c36f0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c36f0-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c36f0-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c36f0-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c36f0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c36f0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c36f0-115">Not supported.</span></span>|
|<span data-ttu-id="c36f0-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c36f0-116">Application</span></span>|<span data-ttu-id="c36f0-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c36f0-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c36f0-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c36f0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="c36f0-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c36f0-119">Request headers</span></span>
|<span data-ttu-id="c36f0-120">标头</span><span class="sxs-lookup"><span data-stu-id="c36f0-120">Header</span></span>|<span data-ttu-id="c36f0-121">值</span><span class="sxs-lookup"><span data-stu-id="c36f0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c36f0-122">授权</span><span class="sxs-lookup"><span data-stu-id="c36f0-122">Authorization</span></span>|<span data-ttu-id="c36f0-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c36f0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c36f0-124">接受</span><span class="sxs-lookup"><span data-stu-id="c36f0-124">Accept</span></span>|<span data-ttu-id="c36f0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c36f0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c36f0-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c36f0-126">Request body</span></span>
<span data-ttu-id="c36f0-127">在请求正文中，提供[defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c36f0-127">In the request body, supply a JSON representation for the [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>

<span data-ttu-id="c36f0-128">下表显示创建[defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c36f0-128">The following table shows the properties that are required when you create the [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md).</span></span>

|<span data-ttu-id="c36f0-129">属性</span><span class="sxs-lookup"><span data-stu-id="c36f0-129">Property</span></span>|<span data-ttu-id="c36f0-130">类型</span><span class="sxs-lookup"><span data-stu-id="c36f0-130">Type</span></span>|<span data-ttu-id="c36f0-131">说明</span><span class="sxs-lookup"><span data-stu-id="c36f0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c36f0-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c36f0-132">roleScopeTagIds</span></span>|<span data-ttu-id="c36f0-133">String 集合</span><span class="sxs-lookup"><span data-stu-id="c36f0-133">String collection</span></span>|<span data-ttu-id="c36f0-134">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="c36f0-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c36f0-135">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c36f0-135">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c36f0-136">id</span><span class="sxs-lookup"><span data-stu-id="c36f0-136">id</span></span>|<span data-ttu-id="c36f0-137">字符串</span><span class="sxs-lookup"><span data-stu-id="c36f0-137">String</span></span>|<span data-ttu-id="c36f0-138">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c36f0-138">Key of the entity.</span></span> <span data-ttu-id="c36f0-139">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c36f0-139">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c36f0-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c36f0-140">createdDateTime</span></span>|<span data-ttu-id="c36f0-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c36f0-141">DateTimeOffset</span></span>|<span data-ttu-id="c36f0-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c36f0-142">DateTime the object was created.</span></span> <span data-ttu-id="c36f0-143">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c36f0-143">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c36f0-144">说明</span><span class="sxs-lookup"><span data-stu-id="c36f0-144">description</span></span>|<span data-ttu-id="c36f0-145">String</span><span class="sxs-lookup"><span data-stu-id="c36f0-145">String</span></span>|<span data-ttu-id="c36f0-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="c36f0-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c36f0-147">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c36f0-147">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c36f0-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c36f0-148">lastModifiedDateTime</span></span>|<span data-ttu-id="c36f0-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c36f0-149">DateTimeOffset</span></span>|<span data-ttu-id="c36f0-150">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c36f0-150">DateTime the object was last modified.</span></span> <span data-ttu-id="c36f0-151">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c36f0-151">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c36f0-152">displayName</span><span class="sxs-lookup"><span data-stu-id="c36f0-152">displayName</span></span>|<span data-ttu-id="c36f0-153">String</span><span class="sxs-lookup"><span data-stu-id="c36f0-153">String</span></span>|<span data-ttu-id="c36f0-154">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="c36f0-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c36f0-155">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c36f0-155">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c36f0-156">version</span><span class="sxs-lookup"><span data-stu-id="c36f0-156">version</span></span>|<span data-ttu-id="c36f0-157">Int32</span><span class="sxs-lookup"><span data-stu-id="c36f0-157">Int32</span></span>|<span data-ttu-id="c36f0-158">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="c36f0-158">Version of the device configuration.</span></span> <span data-ttu-id="c36f0-159">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c36f0-159">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|



## <a name="response"></a><span data-ttu-id="c36f0-160">响应</span><span class="sxs-lookup"><span data-stu-id="c36f0-160">Response</span></span>
<span data-ttu-id="c36f0-161">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c36f0-161">If successful, this method returns a `200 OK` response code and an updated [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c36f0-162">示例</span><span class="sxs-lookup"><span data-stu-id="c36f0-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="c36f0-163">请求</span><span class="sxs-lookup"><span data-stu-id="c36f0-163">Request</span></span>
<span data-ttu-id="c36f0-164">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c36f0-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c36f0-165">响应</span><span class="sxs-lookup"><span data-stu-id="c36f0-165">Response</span></span>
<span data-ttu-id="c36f0-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c36f0-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






