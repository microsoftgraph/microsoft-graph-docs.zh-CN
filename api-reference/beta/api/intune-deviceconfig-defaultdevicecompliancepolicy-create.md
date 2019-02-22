---
title: 创建 defaultDeviceCompliancePolicy
description: 创建新的 defaultDeviceCompliancePolicy 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c98272a691975b118aa17cf8d6ffb7cd33a3b3b4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30170782"
---
# <a name="create-defaultdevicecompliancepolicy"></a><span data-ttu-id="b6429-103">创建 defaultDeviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="b6429-103">Create defaultDeviceCompliancePolicy</span></span>

> <span data-ttu-id="b6429-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b6429-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b6429-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b6429-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6429-106">创建新的[defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b6429-106">Create a new [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b6429-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="b6429-107">Prerequisites</span></span>
<span data-ttu-id="b6429-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="b6429-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b6429-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b6429-110">Permission type</span></span>|<span data-ttu-id="b6429-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b6429-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6429-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b6429-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b6429-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6429-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b6429-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b6429-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6429-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b6429-115">Not supported.</span></span>|
|<span data-ttu-id="b6429-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b6429-116">Application</span></span>|<span data-ttu-id="b6429-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b6429-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6429-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b6429-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="b6429-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b6429-119">Request headers</span></span>
|<span data-ttu-id="b6429-120">标头</span><span class="sxs-lookup"><span data-stu-id="b6429-120">Header</span></span>|<span data-ttu-id="b6429-121">值</span><span class="sxs-lookup"><span data-stu-id="b6429-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6429-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6429-122">Authorization</span></span>|<span data-ttu-id="b6429-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b6429-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6429-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b6429-124">Accept</span></span>|<span data-ttu-id="b6429-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b6429-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6429-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b6429-126">Request body</span></span>
<span data-ttu-id="b6429-127">在请求正文中, 提供 defaultDeviceCompliancePolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b6429-127">In the request body, supply a JSON representation for the defaultDeviceCompliancePolicy object.</span></span>

<span data-ttu-id="b6429-128">下表显示创建 defaultDeviceCompliancePolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b6429-128">The following table shows the properties that are required when you create the defaultDeviceCompliancePolicy.</span></span>

|<span data-ttu-id="b6429-129">属性</span><span class="sxs-lookup"><span data-stu-id="b6429-129">Property</span></span>|<span data-ttu-id="b6429-130">类型</span><span class="sxs-lookup"><span data-stu-id="b6429-130">Type</span></span>|<span data-ttu-id="b6429-131">说明</span><span class="sxs-lookup"><span data-stu-id="b6429-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6429-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b6429-132">roleScopeTagIds</span></span>|<span data-ttu-id="b6429-133">String collection</span><span class="sxs-lookup"><span data-stu-id="b6429-133">String collection</span></span>|<span data-ttu-id="b6429-134">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="b6429-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b6429-135">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b6429-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b6429-136">id</span><span class="sxs-lookup"><span data-stu-id="b6429-136">id</span></span>|<span data-ttu-id="b6429-137">String</span><span class="sxs-lookup"><span data-stu-id="b6429-137">String</span></span>|<span data-ttu-id="b6429-138">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b6429-138">Key of the entity.</span></span> <span data-ttu-id="b6429-139">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b6429-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b6429-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b6429-140">createdDateTime</span></span>|<span data-ttu-id="b6429-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6429-141">DateTimeOffset</span></span>|<span data-ttu-id="b6429-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b6429-142">DateTime the object was created.</span></span> <span data-ttu-id="b6429-143">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b6429-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b6429-144">description</span><span class="sxs-lookup"><span data-stu-id="b6429-144">description</span></span>|<span data-ttu-id="b6429-145">String</span><span class="sxs-lookup"><span data-stu-id="b6429-145">String</span></span>|<span data-ttu-id="b6429-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="b6429-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b6429-147">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b6429-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b6429-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b6429-148">lastModifiedDateTime</span></span>|<span data-ttu-id="b6429-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6429-149">DateTimeOffset</span></span>|<span data-ttu-id="b6429-150">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b6429-150">DateTime the object was last modified.</span></span> <span data-ttu-id="b6429-151">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b6429-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b6429-152">displayName</span><span class="sxs-lookup"><span data-stu-id="b6429-152">displayName</span></span>|<span data-ttu-id="b6429-153">String</span><span class="sxs-lookup"><span data-stu-id="b6429-153">String</span></span>|<span data-ttu-id="b6429-154">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="b6429-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b6429-155">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b6429-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b6429-156">version</span><span class="sxs-lookup"><span data-stu-id="b6429-156">version</span></span>|<span data-ttu-id="b6429-157">Int32</span><span class="sxs-lookup"><span data-stu-id="b6429-157">Int32</span></span>|<span data-ttu-id="b6429-158">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="b6429-158">Version of the device configuration.</span></span> <span data-ttu-id="b6429-159">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b6429-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|



## <a name="response"></a><span data-ttu-id="b6429-160">响应</span><span class="sxs-lookup"><span data-stu-id="b6429-160">Response</span></span>
<span data-ttu-id="b6429-161">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b6429-161">If successful, this method returns a `201 Created` response code and a [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6429-162">示例</span><span class="sxs-lookup"><span data-stu-id="b6429-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="b6429-163">请求</span><span class="sxs-lookup"><span data-stu-id="b6429-163">Request</span></span>
<span data-ttu-id="b6429-164">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b6429-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b6429-165">响应</span><span class="sxs-lookup"><span data-stu-id="b6429-165">Response</span></span>
<span data-ttu-id="b6429-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b6429-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




