---
title: 更新 defaultDeviceCompliancePolicy
description: 更新 defaultDeviceCompliancePolicy 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fc10784e016417f4df4982511c2acf3709153451
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42449360"
---
# <a name="update-defaultdevicecompliancepolicy"></a><span data-ttu-id="050a5-103">更新 defaultDeviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="050a5-103">Update defaultDeviceCompliancePolicy</span></span>

<span data-ttu-id="050a5-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="050a5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="050a5-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="050a5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="050a5-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="050a5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="050a5-107">更新[defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="050a5-107">Update the properties of a [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="050a5-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="050a5-108">Prerequisites</span></span>
<span data-ttu-id="050a5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="050a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="050a5-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="050a5-111">Permission type</span></span>|<span data-ttu-id="050a5-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="050a5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="050a5-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="050a5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="050a5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="050a5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="050a5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="050a5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="050a5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="050a5-116">Not supported.</span></span>|
|<span data-ttu-id="050a5-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="050a5-117">Application</span></span>|<span data-ttu-id="050a5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="050a5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="050a5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="050a5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="050a5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="050a5-120">Request headers</span></span>
|<span data-ttu-id="050a5-121">标头</span><span class="sxs-lookup"><span data-stu-id="050a5-121">Header</span></span>|<span data-ttu-id="050a5-122">值</span><span class="sxs-lookup"><span data-stu-id="050a5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="050a5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="050a5-123">Authorization</span></span>|<span data-ttu-id="050a5-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="050a5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="050a5-125">接受</span><span class="sxs-lookup"><span data-stu-id="050a5-125">Accept</span></span>|<span data-ttu-id="050a5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="050a5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="050a5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="050a5-127">Request body</span></span>
<span data-ttu-id="050a5-128">在请求正文中，提供[defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="050a5-128">In the request body, supply a JSON representation for the [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>

<span data-ttu-id="050a5-129">下表显示创建[defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="050a5-129">The following table shows the properties that are required when you create the [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md).</span></span>

|<span data-ttu-id="050a5-130">属性</span><span class="sxs-lookup"><span data-stu-id="050a5-130">Property</span></span>|<span data-ttu-id="050a5-131">类型</span><span class="sxs-lookup"><span data-stu-id="050a5-131">Type</span></span>|<span data-ttu-id="050a5-132">说明</span><span class="sxs-lookup"><span data-stu-id="050a5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="050a5-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="050a5-133">roleScopeTagIds</span></span>|<span data-ttu-id="050a5-134">String 集合</span><span class="sxs-lookup"><span data-stu-id="050a5-134">String collection</span></span>|<span data-ttu-id="050a5-135">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="050a5-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="050a5-136">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="050a5-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="050a5-137">id</span><span class="sxs-lookup"><span data-stu-id="050a5-137">id</span></span>|<span data-ttu-id="050a5-138">字符串</span><span class="sxs-lookup"><span data-stu-id="050a5-138">String</span></span>|<span data-ttu-id="050a5-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="050a5-139">Key of the entity.</span></span> <span data-ttu-id="050a5-140">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="050a5-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="050a5-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="050a5-141">createdDateTime</span></span>|<span data-ttu-id="050a5-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="050a5-142">DateTimeOffset</span></span>|<span data-ttu-id="050a5-143">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="050a5-143">DateTime the object was created.</span></span> <span data-ttu-id="050a5-144">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="050a5-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="050a5-145">说明</span><span class="sxs-lookup"><span data-stu-id="050a5-145">description</span></span>|<span data-ttu-id="050a5-146">String</span><span class="sxs-lookup"><span data-stu-id="050a5-146">String</span></span>|<span data-ttu-id="050a5-147">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="050a5-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="050a5-148">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="050a5-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="050a5-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="050a5-149">lastModifiedDateTime</span></span>|<span data-ttu-id="050a5-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="050a5-150">DateTimeOffset</span></span>|<span data-ttu-id="050a5-151">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="050a5-151">DateTime the object was last modified.</span></span> <span data-ttu-id="050a5-152">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="050a5-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="050a5-153">displayName</span><span class="sxs-lookup"><span data-stu-id="050a5-153">displayName</span></span>|<span data-ttu-id="050a5-154">String</span><span class="sxs-lookup"><span data-stu-id="050a5-154">String</span></span>|<span data-ttu-id="050a5-155">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="050a5-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="050a5-156">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="050a5-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="050a5-157">version</span><span class="sxs-lookup"><span data-stu-id="050a5-157">version</span></span>|<span data-ttu-id="050a5-158">Int32</span><span class="sxs-lookup"><span data-stu-id="050a5-158">Int32</span></span>|<span data-ttu-id="050a5-159">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="050a5-159">Version of the device configuration.</span></span> <span data-ttu-id="050a5-160">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="050a5-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|



## <a name="response"></a><span data-ttu-id="050a5-161">响应</span><span class="sxs-lookup"><span data-stu-id="050a5-161">Response</span></span>
<span data-ttu-id="050a5-162">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="050a5-162">If successful, this method returns a `200 OK` response code and an updated [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="050a5-163">示例</span><span class="sxs-lookup"><span data-stu-id="050a5-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="050a5-164">请求</span><span class="sxs-lookup"><span data-stu-id="050a5-164">Request</span></span>
<span data-ttu-id="050a5-165">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="050a5-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="050a5-166">响应</span><span class="sxs-lookup"><span data-stu-id="050a5-166">Response</span></span>
<span data-ttu-id="050a5-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="050a5-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





