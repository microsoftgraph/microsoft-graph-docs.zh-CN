---
title: 创建 androidCustomConfiguration
description: 创建新的 androidCustomConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e7844f774f93a86e53b4115d51a8c07269e68c53
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33933254"
---
# <a name="create-androidcustomconfiguration"></a><span data-ttu-id="6a841-103">创建 androidCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="6a841-103">Create androidCustomConfiguration</span></span>

> <span data-ttu-id="6a841-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6a841-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a841-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6a841-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a841-106">创建新的 [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6a841-106">Create a new [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6a841-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="6a841-107">Prerequisites</span></span>
<span data-ttu-id="6a841-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6a841-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a841-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6a841-110">Permission type</span></span>|<span data-ttu-id="6a841-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6a841-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a841-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6a841-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6a841-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a841-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6a841-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6a841-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a841-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6a841-115">Not supported.</span></span>|
|<span data-ttu-id="6a841-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6a841-116">Application</span></span>|<span data-ttu-id="6a841-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="6a841-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a841-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6a841-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6a841-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6a841-119">Request headers</span></span>
|<span data-ttu-id="6a841-120">标头</span><span class="sxs-lookup"><span data-stu-id="6a841-120">Header</span></span>|<span data-ttu-id="6a841-121">值</span><span class="sxs-lookup"><span data-stu-id="6a841-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a841-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a841-122">Authorization</span></span>|<span data-ttu-id="6a841-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6a841-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a841-124">接受</span><span class="sxs-lookup"><span data-stu-id="6a841-124">Accept</span></span>|<span data-ttu-id="6a841-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6a841-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a841-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6a841-126">Request body</span></span>
<span data-ttu-id="6a841-127">在请求正文中，提供 androidCustomConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6a841-127">In the request body, supply a JSON representation for the androidCustomConfiguration object.</span></span>

<span data-ttu-id="6a841-128">下表显示了创建 androidCustomConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6a841-128">The following table shows the properties that are required when you create the androidCustomConfiguration.</span></span>

|<span data-ttu-id="6a841-129">属性</span><span class="sxs-lookup"><span data-stu-id="6a841-129">Property</span></span>|<span data-ttu-id="6a841-130">类型</span><span class="sxs-lookup"><span data-stu-id="6a841-130">Type</span></span>|<span data-ttu-id="6a841-131">说明</span><span class="sxs-lookup"><span data-stu-id="6a841-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a841-132">id</span><span class="sxs-lookup"><span data-stu-id="6a841-132">id</span></span>|<span data-ttu-id="6a841-133">字符串</span><span class="sxs-lookup"><span data-stu-id="6a841-133">String</span></span>|<span data-ttu-id="6a841-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6a841-134">Key of the entity.</span></span> <span data-ttu-id="6a841-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6a841-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6a841-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6a841-136">lastModifiedDateTime</span></span>|<span data-ttu-id="6a841-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a841-137">DateTimeOffset</span></span>|<span data-ttu-id="6a841-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6a841-138">DateTime the object was last modified.</span></span> <span data-ttu-id="6a841-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6a841-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6a841-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6a841-140">roleScopeTagIds</span></span>|<span data-ttu-id="6a841-141">String collection</span><span class="sxs-lookup"><span data-stu-id="6a841-141">String collection</span></span>|<span data-ttu-id="6a841-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="6a841-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6a841-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6a841-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6a841-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6a841-144">supportsScopeTags</span></span>|<span data-ttu-id="6a841-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="6a841-145">Boolean</span></span>|<span data-ttu-id="6a841-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="6a841-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6a841-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="6a841-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6a841-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="6a841-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6a841-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6a841-149">This property is read-only.</span></span> <span data-ttu-id="6a841-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6a841-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6a841-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6a841-151">createdDateTime</span></span>|<span data-ttu-id="6a841-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a841-152">DateTimeOffset</span></span>|<span data-ttu-id="6a841-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6a841-153">DateTime the object was created.</span></span> <span data-ttu-id="6a841-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6a841-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6a841-155">说明</span><span class="sxs-lookup"><span data-stu-id="6a841-155">description</span></span>|<span data-ttu-id="6a841-156">String</span><span class="sxs-lookup"><span data-stu-id="6a841-156">String</span></span>|<span data-ttu-id="6a841-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="6a841-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6a841-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6a841-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6a841-159">displayName</span><span class="sxs-lookup"><span data-stu-id="6a841-159">displayName</span></span>|<span data-ttu-id="6a841-160">String</span><span class="sxs-lookup"><span data-stu-id="6a841-160">String</span></span>|<span data-ttu-id="6a841-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="6a841-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6a841-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6a841-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6a841-163">version</span><span class="sxs-lookup"><span data-stu-id="6a841-163">version</span></span>|<span data-ttu-id="6a841-164">Int32</span><span class="sxs-lookup"><span data-stu-id="6a841-164">Int32</span></span>|<span data-ttu-id="6a841-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="6a841-165">Version of the device configuration.</span></span> <span data-ttu-id="6a841-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6a841-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6a841-167">omaSettings</span><span class="sxs-lookup"><span data-stu-id="6a841-167">omaSettings</span></span>|<span data-ttu-id="6a841-168">[omaSetting](../resources/intune-deviceconfig-omasetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6a841-168">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="6a841-169">OMA 设置。</span><span class="sxs-lookup"><span data-stu-id="6a841-169">OMA settings.</span></span> <span data-ttu-id="6a841-170">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="6a841-170">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="6a841-171">响应</span><span class="sxs-lookup"><span data-stu-id="6a841-171">Response</span></span>
<span data-ttu-id="6a841-172">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6a841-172">If successful, this method returns a `201 Created` response code and a [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a841-173">示例</span><span class="sxs-lookup"><span data-stu-id="6a841-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="6a841-174">请求</span><span class="sxs-lookup"><span data-stu-id="6a841-174">Request</span></span>
<span data-ttu-id="6a841-175">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6a841-175">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 494

{
  "@odata.type": "#microsoft.graph.androidCustomConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="6a841-176">响应</span><span class="sxs-lookup"><span data-stu-id="6a841-176">Response</span></span>
<span data-ttu-id="6a841-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6a841-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 666

{
  "@odata.type": "#microsoft.graph.androidCustomConfiguration",
  "id": "619b5e6d-5e6d-619b-6d5e-9b616d5e9b61",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5
    }
  ]
}
```




