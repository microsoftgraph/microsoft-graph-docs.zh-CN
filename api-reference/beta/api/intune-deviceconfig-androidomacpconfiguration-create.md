---
title: 创建 androidOmaCpConfiguration
description: 创建新的 androidOmaCpConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bed436668e2b77332f41a32dfe19f66895010249
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30177817"
---
# <a name="create-androidomacpconfiguration"></a><span data-ttu-id="06cb8-103">创建 androidOmaCpConfiguration</span><span class="sxs-lookup"><span data-stu-id="06cb8-103">Create androidOmaCpConfiguration</span></span>

> <span data-ttu-id="06cb8-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="06cb8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="06cb8-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="06cb8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06cb8-106">创建新的[androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="06cb8-106">Create a new [androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="06cb8-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="06cb8-107">Prerequisites</span></span>
<span data-ttu-id="06cb8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="06cb8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="06cb8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="06cb8-110">Permission type</span></span>|<span data-ttu-id="06cb8-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="06cb8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06cb8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="06cb8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="06cb8-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06cb8-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="06cb8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="06cb8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06cb8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="06cb8-115">Not supported.</span></span>|
|<span data-ttu-id="06cb8-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="06cb8-116">Application</span></span>|<span data-ttu-id="06cb8-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="06cb8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="06cb8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="06cb8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="06cb8-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="06cb8-119">Request headers</span></span>
|<span data-ttu-id="06cb8-120">标头</span><span class="sxs-lookup"><span data-stu-id="06cb8-120">Header</span></span>|<span data-ttu-id="06cb8-121">值</span><span class="sxs-lookup"><span data-stu-id="06cb8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06cb8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="06cb8-122">Authorization</span></span>|<span data-ttu-id="06cb8-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="06cb8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06cb8-124">Accept</span><span class="sxs-lookup"><span data-stu-id="06cb8-124">Accept</span></span>|<span data-ttu-id="06cb8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="06cb8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06cb8-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="06cb8-126">Request body</span></span>
<span data-ttu-id="06cb8-127">在请求正文中, 提供 androidOmaCpConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="06cb8-127">In the request body, supply a JSON representation for the androidOmaCpConfiguration object.</span></span>

<span data-ttu-id="06cb8-128">下表显示创建 androidOmaCpConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="06cb8-128">The following table shows the properties that are required when you create the androidOmaCpConfiguration.</span></span>

|<span data-ttu-id="06cb8-129">属性</span><span class="sxs-lookup"><span data-stu-id="06cb8-129">Property</span></span>|<span data-ttu-id="06cb8-130">类型</span><span class="sxs-lookup"><span data-stu-id="06cb8-130">Type</span></span>|<span data-ttu-id="06cb8-131">说明</span><span class="sxs-lookup"><span data-stu-id="06cb8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06cb8-132">id</span><span class="sxs-lookup"><span data-stu-id="06cb8-132">id</span></span>|<span data-ttu-id="06cb8-133">String</span><span class="sxs-lookup"><span data-stu-id="06cb8-133">String</span></span>|<span data-ttu-id="06cb8-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="06cb8-134">Key of the entity.</span></span> <span data-ttu-id="06cb8-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06cb8-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06cb8-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="06cb8-136">lastModifiedDateTime</span></span>|<span data-ttu-id="06cb8-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06cb8-137">DateTimeOffset</span></span>|<span data-ttu-id="06cb8-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="06cb8-138">DateTime the object was last modified.</span></span> <span data-ttu-id="06cb8-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06cb8-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06cb8-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="06cb8-140">roleScopeTagIds</span></span>|<span data-ttu-id="06cb8-141">String collection</span><span class="sxs-lookup"><span data-stu-id="06cb8-141">String collection</span></span>|<span data-ttu-id="06cb8-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="06cb8-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="06cb8-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06cb8-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06cb8-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="06cb8-144">supportsScopeTags</span></span>|<span data-ttu-id="06cb8-145">布尔</span><span class="sxs-lookup"><span data-stu-id="06cb8-145">Boolean</span></span>|<span data-ttu-id="06cb8-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="06cb8-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="06cb8-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="06cb8-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="06cb8-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="06cb8-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="06cb8-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="06cb8-149">This property is read-only.</span></span> <span data-ttu-id="06cb8-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06cb8-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06cb8-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="06cb8-151">createdDateTime</span></span>|<span data-ttu-id="06cb8-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06cb8-152">DateTimeOffset</span></span>|<span data-ttu-id="06cb8-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="06cb8-153">DateTime the object was created.</span></span> <span data-ttu-id="06cb8-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06cb8-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06cb8-155">description</span><span class="sxs-lookup"><span data-stu-id="06cb8-155">description</span></span>|<span data-ttu-id="06cb8-156">String</span><span class="sxs-lookup"><span data-stu-id="06cb8-156">String</span></span>|<span data-ttu-id="06cb8-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="06cb8-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="06cb8-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06cb8-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06cb8-159">displayName</span><span class="sxs-lookup"><span data-stu-id="06cb8-159">displayName</span></span>|<span data-ttu-id="06cb8-160">String</span><span class="sxs-lookup"><span data-stu-id="06cb8-160">String</span></span>|<span data-ttu-id="06cb8-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="06cb8-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="06cb8-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06cb8-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06cb8-163">version</span><span class="sxs-lookup"><span data-stu-id="06cb8-163">version</span></span>|<span data-ttu-id="06cb8-164">Int32</span><span class="sxs-lookup"><span data-stu-id="06cb8-164">Int32</span></span>|<span data-ttu-id="06cb8-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="06cb8-165">Version of the device configuration.</span></span> <span data-ttu-id="06cb8-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06cb8-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06cb8-167">configurationXml</span><span class="sxs-lookup"><span data-stu-id="06cb8-167">configurationXml</span></span>|<span data-ttu-id="06cb8-168">Binary</span><span class="sxs-lookup"><span data-stu-id="06cb8-168">Binary</span></span>|<span data-ttu-id="06cb8-169">将应用于设备的配置 XML。</span><span class="sxs-lookup"><span data-stu-id="06cb8-169">Configuration XML that will be applied to the device.</span></span> <span data-ttu-id="06cb8-170">读取时, 它只提供占位符字符串, 因为原始数据经过加密和存储。</span><span class="sxs-lookup"><span data-stu-id="06cb8-170">When it is read, it only provides a placeholder string since the original data is encrypted and stored.</span></span>|



## <a name="response"></a><span data-ttu-id="06cb8-171">响应</span><span class="sxs-lookup"><span data-stu-id="06cb8-171">Response</span></span>
<span data-ttu-id="06cb8-172">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="06cb8-172">If successful, this method returns a `201 Created` response code and a [androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06cb8-173">示例</span><span class="sxs-lookup"><span data-stu-id="06cb8-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="06cb8-174">请求</span><span class="sxs-lookup"><span data-stu-id="06cb8-174">Request</span></span>
<span data-ttu-id="06cb8-175">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="06cb8-175">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 306

{
  "@odata.type": "#microsoft.graph.androidOmaCpConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "configurationXml": "Y29uZmlndXJhdGlvblhtbA=="
}
```

### <a name="response"></a><span data-ttu-id="06cb8-176">响应</span><span class="sxs-lookup"><span data-stu-id="06cb8-176">Response</span></span>
<span data-ttu-id="06cb8-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="06cb8-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 478

{
  "@odata.type": "#microsoft.graph.androidOmaCpConfiguration",
  "id": "5f682e4a-2e4a-5f68-4a2e-685f4a2e685f",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "configurationXml": "Y29uZmlndXJhdGlvblhtbA=="
}
```




