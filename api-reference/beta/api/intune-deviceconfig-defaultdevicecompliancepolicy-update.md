---
title: 更新 defaultDeviceCompliancePolicy
description: 更新 defaultDeviceCompliancePolicy 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 462ebc7b3a73673a9dabd547cca1553ccf26c1a9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48048132"
---
# <a name="update-defaultdevicecompliancepolicy"></a><span data-ttu-id="2747b-103">更新 defaultDeviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="2747b-103">Update defaultDeviceCompliancePolicy</span></span>

<span data-ttu-id="2747b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2747b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2747b-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2747b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2747b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2747b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2747b-107">更新 [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2747b-107">Update the properties of a [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2747b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="2747b-108">Prerequisites</span></span>
<span data-ttu-id="2747b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2747b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2747b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2747b-111">Permission type</span></span>|<span data-ttu-id="2747b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2747b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2747b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2747b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2747b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2747b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2747b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2747b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2747b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2747b-116">Not supported.</span></span>|
|<span data-ttu-id="2747b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2747b-117">Application</span></span>|<span data-ttu-id="2747b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2747b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2747b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2747b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="2747b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2747b-120">Request headers</span></span>
|<span data-ttu-id="2747b-121">标头</span><span class="sxs-lookup"><span data-stu-id="2747b-121">Header</span></span>|<span data-ttu-id="2747b-122">值</span><span class="sxs-lookup"><span data-stu-id="2747b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2747b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2747b-123">Authorization</span></span>|<span data-ttu-id="2747b-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2747b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2747b-125">接受</span><span class="sxs-lookup"><span data-stu-id="2747b-125">Accept</span></span>|<span data-ttu-id="2747b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2747b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2747b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2747b-127">Request body</span></span>
<span data-ttu-id="2747b-128">在请求正文中，提供 [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2747b-128">In the request body, supply a JSON representation for the [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>

<span data-ttu-id="2747b-129">下表显示创建 [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2747b-129">The following table shows the properties that are required when you create the [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md).</span></span>

|<span data-ttu-id="2747b-130">属性</span><span class="sxs-lookup"><span data-stu-id="2747b-130">Property</span></span>|<span data-ttu-id="2747b-131">类型</span><span class="sxs-lookup"><span data-stu-id="2747b-131">Type</span></span>|<span data-ttu-id="2747b-132">说明</span><span class="sxs-lookup"><span data-stu-id="2747b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2747b-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2747b-133">roleScopeTagIds</span></span>|<span data-ttu-id="2747b-134">String 集合</span><span class="sxs-lookup"><span data-stu-id="2747b-134">String collection</span></span>|<span data-ttu-id="2747b-135">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="2747b-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2747b-136">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2747b-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2747b-137">id</span><span class="sxs-lookup"><span data-stu-id="2747b-137">id</span></span>|<span data-ttu-id="2747b-138">String</span><span class="sxs-lookup"><span data-stu-id="2747b-138">String</span></span>|<span data-ttu-id="2747b-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2747b-139">Key of the entity.</span></span> <span data-ttu-id="2747b-140">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2747b-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2747b-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2747b-141">createdDateTime</span></span>|<span data-ttu-id="2747b-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2747b-142">DateTimeOffset</span></span>|<span data-ttu-id="2747b-143">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2747b-143">DateTime the object was created.</span></span> <span data-ttu-id="2747b-144">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2747b-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2747b-145">description</span><span class="sxs-lookup"><span data-stu-id="2747b-145">description</span></span>|<span data-ttu-id="2747b-146">String</span><span class="sxs-lookup"><span data-stu-id="2747b-146">String</span></span>|<span data-ttu-id="2747b-147">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="2747b-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2747b-148">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2747b-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2747b-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2747b-149">lastModifiedDateTime</span></span>|<span data-ttu-id="2747b-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2747b-150">DateTimeOffset</span></span>|<span data-ttu-id="2747b-151">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2747b-151">DateTime the object was last modified.</span></span> <span data-ttu-id="2747b-152">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2747b-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2747b-153">displayName</span><span class="sxs-lookup"><span data-stu-id="2747b-153">displayName</span></span>|<span data-ttu-id="2747b-154">String</span><span class="sxs-lookup"><span data-stu-id="2747b-154">String</span></span>|<span data-ttu-id="2747b-155">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="2747b-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2747b-156">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2747b-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2747b-157">version</span><span class="sxs-lookup"><span data-stu-id="2747b-157">version</span></span>|<span data-ttu-id="2747b-158">Int32</span><span class="sxs-lookup"><span data-stu-id="2747b-158">Int32</span></span>|<span data-ttu-id="2747b-159">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="2747b-159">Version of the device configuration.</span></span> <span data-ttu-id="2747b-160">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2747b-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|



## <a name="response"></a><span data-ttu-id="2747b-161">响应</span><span class="sxs-lookup"><span data-stu-id="2747b-161">Response</span></span>
<span data-ttu-id="2747b-162">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2747b-162">If successful, this method returns a `200 OK` response code and an updated [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2747b-163">示例</span><span class="sxs-lookup"><span data-stu-id="2747b-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="2747b-164">请求</span><span class="sxs-lookup"><span data-stu-id="2747b-164">Request</span></span>
<span data-ttu-id="2747b-165">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2747b-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2747b-166">响应</span><span class="sxs-lookup"><span data-stu-id="2747b-166">Response</span></span>
<span data-ttu-id="2747b-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2747b-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






