---
title: 创建 defaultDeviceCompliancePolicy
description: 创建新的 defaultDeviceCompliancePolicy 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 79911794adf153a18b7af7f58cec72baf56f3015
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964422"
---
# <a name="create-defaultdevicecompliancepolicy"></a><span data-ttu-id="195ed-103">创建 defaultDeviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="195ed-103">Create defaultDeviceCompliancePolicy</span></span>

> <span data-ttu-id="195ed-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="195ed-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="195ed-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="195ed-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="195ed-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="195ed-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="195ed-107">创建新的[defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="195ed-107">Create a new [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="195ed-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="195ed-108">Prerequisites</span></span>
<span data-ttu-id="195ed-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="195ed-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="195ed-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="195ed-111">Permission type</span></span>|<span data-ttu-id="195ed-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="195ed-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="195ed-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="195ed-113">Delegated (work or school account)</span></span>|<span data-ttu-id="195ed-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="195ed-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="195ed-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="195ed-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="195ed-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="195ed-116">Not supported.</span></span>|
|<span data-ttu-id="195ed-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="195ed-117">Application</span></span>|<span data-ttu-id="195ed-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="195ed-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="195ed-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="195ed-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="195ed-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="195ed-120">Request headers</span></span>
|<span data-ttu-id="195ed-121">标头</span><span class="sxs-lookup"><span data-stu-id="195ed-121">Header</span></span>|<span data-ttu-id="195ed-122">值</span><span class="sxs-lookup"><span data-stu-id="195ed-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="195ed-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="195ed-123">Authorization</span></span>|<span data-ttu-id="195ed-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="195ed-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="195ed-125">Accept</span><span class="sxs-lookup"><span data-stu-id="195ed-125">Accept</span></span>|<span data-ttu-id="195ed-126">application/json</span><span class="sxs-lookup"><span data-stu-id="195ed-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="195ed-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="195ed-127">Request body</span></span>
<span data-ttu-id="195ed-128">在请求正文中，提供 defaultDeviceCompliancePolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="195ed-128">In the request body, supply a JSON representation for the defaultDeviceCompliancePolicy object.</span></span>

<span data-ttu-id="195ed-129">下表显示时创建 defaultDeviceCompliancePolicy 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="195ed-129">The following table shows the properties that are required when you create the defaultDeviceCompliancePolicy.</span></span>

|<span data-ttu-id="195ed-130">属性</span><span class="sxs-lookup"><span data-stu-id="195ed-130">Property</span></span>|<span data-ttu-id="195ed-131">类型</span><span class="sxs-lookup"><span data-stu-id="195ed-131">Type</span></span>|<span data-ttu-id="195ed-132">说明</span><span class="sxs-lookup"><span data-stu-id="195ed-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="195ed-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="195ed-133">roleScopeTagIds</span></span>|<span data-ttu-id="195ed-134">String 集合</span><span class="sxs-lookup"><span data-stu-id="195ed-134">String collection</span></span>|<span data-ttu-id="195ed-135">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="195ed-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="195ed-136">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="195ed-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="195ed-137">id</span><span class="sxs-lookup"><span data-stu-id="195ed-137">id</span></span>|<span data-ttu-id="195ed-138">String</span><span class="sxs-lookup"><span data-stu-id="195ed-138">String</span></span>|<span data-ttu-id="195ed-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="195ed-139">Key of the entity.</span></span> <span data-ttu-id="195ed-140">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="195ed-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="195ed-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="195ed-141">createdDateTime</span></span>|<span data-ttu-id="195ed-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="195ed-142">DateTimeOffset</span></span>|<span data-ttu-id="195ed-143">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="195ed-143">DateTime the object was created.</span></span> <span data-ttu-id="195ed-144">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="195ed-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="195ed-145">description</span><span class="sxs-lookup"><span data-stu-id="195ed-145">description</span></span>|<span data-ttu-id="195ed-146">String</span><span class="sxs-lookup"><span data-stu-id="195ed-146">String</span></span>|<span data-ttu-id="195ed-147">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="195ed-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="195ed-148">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="195ed-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="195ed-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="195ed-149">lastModifiedDateTime</span></span>|<span data-ttu-id="195ed-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="195ed-150">DateTimeOffset</span></span>|<span data-ttu-id="195ed-151">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="195ed-151">DateTime the object was last modified.</span></span> <span data-ttu-id="195ed-152">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="195ed-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="195ed-153">displayName</span><span class="sxs-lookup"><span data-stu-id="195ed-153">displayName</span></span>|<span data-ttu-id="195ed-154">String</span><span class="sxs-lookup"><span data-stu-id="195ed-154">String</span></span>|<span data-ttu-id="195ed-155">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="195ed-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="195ed-156">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="195ed-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="195ed-157">version</span><span class="sxs-lookup"><span data-stu-id="195ed-157">version</span></span>|<span data-ttu-id="195ed-158">Int32</span><span class="sxs-lookup"><span data-stu-id="195ed-158">Int32</span></span>|<span data-ttu-id="195ed-159">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="195ed-159">Version of the device configuration.</span></span> <span data-ttu-id="195ed-160">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="195ed-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|



## <a name="response"></a><span data-ttu-id="195ed-161">响应</span><span class="sxs-lookup"><span data-stu-id="195ed-161">Response</span></span>
<span data-ttu-id="195ed-162">如果成功，此方法返回`201 Created`响应代码和响应正文中的[defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="195ed-162">If successful, this method returns a `201 Created` response code and a [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="195ed-163">示例</span><span class="sxs-lookup"><span data-stu-id="195ed-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="195ed-164">请求</span><span class="sxs-lookup"><span data-stu-id="195ed-164">Request</span></span>
<span data-ttu-id="195ed-165">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="195ed-165">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 293

{
  "@odata.type": "#microsoft.graph.defaultDeviceCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="195ed-166">响应</span><span class="sxs-lookup"><span data-stu-id="195ed-166">Response</span></span>
<span data-ttu-id="195ed-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="195ed-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





