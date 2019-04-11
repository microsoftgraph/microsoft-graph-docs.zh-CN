---
title: 更新 defaultDeviceCompliancePolicy
description: 更新 defaultDeviceCompliancePolicy 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d69ebb9b07f5544f88e01980ca5684c2ce3dda8a
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31781965"
---
# <a name="update-defaultdevicecompliancepolicy"></a><span data-ttu-id="5dcb5-103">更新 defaultDeviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="5dcb5-103">Update defaultDeviceCompliancePolicy</span></span>

> <span data-ttu-id="5dcb5-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5dcb5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5dcb5-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5dcb5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5dcb5-106">更新[defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5dcb5-106">Update the properties of a [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5dcb5-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="5dcb5-107">Prerequisites</span></span>
<span data-ttu-id="5dcb5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5dcb5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5dcb5-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5dcb5-110">Permission type</span></span>|<span data-ttu-id="5dcb5-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5dcb5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5dcb5-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5dcb5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5dcb5-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5dcb5-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5dcb5-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5dcb5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5dcb5-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5dcb5-115">Not supported.</span></span>|
|<span data-ttu-id="5dcb5-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="5dcb5-116">Application</span></span>|<span data-ttu-id="5dcb5-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="5dcb5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5dcb5-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5dcb5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="5dcb5-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="5dcb5-119">Request headers</span></span>
|<span data-ttu-id="5dcb5-120">标头</span><span class="sxs-lookup"><span data-stu-id="5dcb5-120">Header</span></span>|<span data-ttu-id="5dcb5-121">值</span><span class="sxs-lookup"><span data-stu-id="5dcb5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5dcb5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5dcb5-122">Authorization</span></span>|<span data-ttu-id="5dcb5-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5dcb5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5dcb5-124">接受</span><span class="sxs-lookup"><span data-stu-id="5dcb5-124">Accept</span></span>|<span data-ttu-id="5dcb5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5dcb5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5dcb5-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="5dcb5-126">Request body</span></span>
<span data-ttu-id="5dcb5-127">在请求正文中, 提供[defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5dcb5-127">In the request body, supply a JSON representation for the [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>

<span data-ttu-id="5dcb5-128">下表显示创建[defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5dcb5-128">The following table shows the properties that are required when you create the [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md).</span></span>

|<span data-ttu-id="5dcb5-129">属性</span><span class="sxs-lookup"><span data-stu-id="5dcb5-129">Property</span></span>|<span data-ttu-id="5dcb5-130">类型</span><span class="sxs-lookup"><span data-stu-id="5dcb5-130">Type</span></span>|<span data-ttu-id="5dcb5-131">说明</span><span class="sxs-lookup"><span data-stu-id="5dcb5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5dcb5-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5dcb5-132">roleScopeTagIds</span></span>|<span data-ttu-id="5dcb5-133">String 集合</span><span class="sxs-lookup"><span data-stu-id="5dcb5-133">String collection</span></span>|<span data-ttu-id="5dcb5-134">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="5dcb5-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5dcb5-135">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5dcb5-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5dcb5-136">id</span><span class="sxs-lookup"><span data-stu-id="5dcb5-136">id</span></span>|<span data-ttu-id="5dcb5-137">String</span><span class="sxs-lookup"><span data-stu-id="5dcb5-137">String</span></span>|<span data-ttu-id="5dcb5-138">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5dcb5-138">Key of the entity.</span></span> <span data-ttu-id="5dcb5-139">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5dcb5-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5dcb5-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5dcb5-140">createdDateTime</span></span>|<span data-ttu-id="5dcb5-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5dcb5-141">DateTimeOffset</span></span>|<span data-ttu-id="5dcb5-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="5dcb5-142">DateTime the object was created.</span></span> <span data-ttu-id="5dcb5-143">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5dcb5-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5dcb5-144">description</span><span class="sxs-lookup"><span data-stu-id="5dcb5-144">description</span></span>|<span data-ttu-id="5dcb5-145">String</span><span class="sxs-lookup"><span data-stu-id="5dcb5-145">String</span></span>|<span data-ttu-id="5dcb5-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="5dcb5-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5dcb5-147">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5dcb5-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5dcb5-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5dcb5-148">lastModifiedDateTime</span></span>|<span data-ttu-id="5dcb5-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5dcb5-149">DateTimeOffset</span></span>|<span data-ttu-id="5dcb5-150">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="5dcb5-150">DateTime the object was last modified.</span></span> <span data-ttu-id="5dcb5-151">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5dcb5-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5dcb5-152">displayName</span><span class="sxs-lookup"><span data-stu-id="5dcb5-152">displayName</span></span>|<span data-ttu-id="5dcb5-153">String</span><span class="sxs-lookup"><span data-stu-id="5dcb5-153">String</span></span>|<span data-ttu-id="5dcb5-154">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="5dcb5-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5dcb5-155">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5dcb5-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5dcb5-156">version</span><span class="sxs-lookup"><span data-stu-id="5dcb5-156">version</span></span>|<span data-ttu-id="5dcb5-157">Int32</span><span class="sxs-lookup"><span data-stu-id="5dcb5-157">Int32</span></span>|<span data-ttu-id="5dcb5-158">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="5dcb5-158">Version of the device configuration.</span></span> <span data-ttu-id="5dcb5-159">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5dcb5-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|



## <a name="response"></a><span data-ttu-id="5dcb5-160">响应</span><span class="sxs-lookup"><span data-stu-id="5dcb5-160">Response</span></span>
<span data-ttu-id="5dcb5-161">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5dcb5-161">If successful, this method returns a `200 OK` response code and an updated [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5dcb5-162">示例</span><span class="sxs-lookup"><span data-stu-id="5dcb5-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="5dcb5-163">请求</span><span class="sxs-lookup"><span data-stu-id="5dcb5-163">Request</span></span>
<span data-ttu-id="5dcb5-164">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5dcb5-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5dcb5-165">响应</span><span class="sxs-lookup"><span data-stu-id="5dcb5-165">Response</span></span>
<span data-ttu-id="5dcb5-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5dcb5-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





