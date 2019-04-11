---
title: 创建 androidWorkProfileCustomConfiguration
description: 创建新的 androidWorkProfileCustomConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7be58aa92448fcd352d1073077476f338d56dd28
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31787391"
---
# <a name="create-androidworkprofilecustomconfiguration"></a><span data-ttu-id="1e01f-103">创建 androidWorkProfileCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="1e01f-103">Create androidWorkProfileCustomConfiguration</span></span>

> <span data-ttu-id="1e01f-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1e01f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1e01f-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1e01f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e01f-106">创建新的[androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1e01f-106">Create a new [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1e01f-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="1e01f-107">Prerequisites</span></span>
<span data-ttu-id="1e01f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1e01f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e01f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1e01f-110">Permission type</span></span>|<span data-ttu-id="1e01f-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1e01f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e01f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1e01f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1e01f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e01f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1e01f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1e01f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e01f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1e01f-115">Not supported.</span></span>|
|<span data-ttu-id="1e01f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1e01f-116">Application</span></span>|<span data-ttu-id="1e01f-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="1e01f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e01f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1e01f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1e01f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="1e01f-119">Request headers</span></span>
|<span data-ttu-id="1e01f-120">标头</span><span class="sxs-lookup"><span data-stu-id="1e01f-120">Header</span></span>|<span data-ttu-id="1e01f-121">值</span><span class="sxs-lookup"><span data-stu-id="1e01f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1e01f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e01f-122">Authorization</span></span>|<span data-ttu-id="1e01f-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1e01f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1e01f-124">接受</span><span class="sxs-lookup"><span data-stu-id="1e01f-124">Accept</span></span>|<span data-ttu-id="1e01f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1e01f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e01f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="1e01f-126">Request body</span></span>
<span data-ttu-id="1e01f-127">在请求正文中, 提供 androidWorkProfileCustomConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1e01f-127">In the request body, supply a JSON representation for the androidWorkProfileCustomConfiguration object.</span></span>

<span data-ttu-id="1e01f-128">下表显示创建 androidWorkProfileCustomConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1e01f-128">The following table shows the properties that are required when you create the androidWorkProfileCustomConfiguration.</span></span>

|<span data-ttu-id="1e01f-129">属性</span><span class="sxs-lookup"><span data-stu-id="1e01f-129">Property</span></span>|<span data-ttu-id="1e01f-130">类型</span><span class="sxs-lookup"><span data-stu-id="1e01f-130">Type</span></span>|<span data-ttu-id="1e01f-131">说明</span><span class="sxs-lookup"><span data-stu-id="1e01f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e01f-132">id</span><span class="sxs-lookup"><span data-stu-id="1e01f-132">id</span></span>|<span data-ttu-id="1e01f-133">String</span><span class="sxs-lookup"><span data-stu-id="1e01f-133">String</span></span>|<span data-ttu-id="1e01f-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1e01f-134">Key of the entity.</span></span> <span data-ttu-id="1e01f-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e01f-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1e01f-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1e01f-136">lastModifiedDateTime</span></span>|<span data-ttu-id="1e01f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e01f-137">DateTimeOffset</span></span>|<span data-ttu-id="1e01f-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1e01f-138">DateTime the object was last modified.</span></span> <span data-ttu-id="1e01f-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e01f-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1e01f-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1e01f-140">roleScopeTagIds</span></span>|<span data-ttu-id="1e01f-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="1e01f-141">String collection</span></span>|<span data-ttu-id="1e01f-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="1e01f-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1e01f-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e01f-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1e01f-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1e01f-144">supportsScopeTags</span></span>|<span data-ttu-id="1e01f-145">布尔值</span><span class="sxs-lookup"><span data-stu-id="1e01f-145">Boolean</span></span>|<span data-ttu-id="1e01f-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="1e01f-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1e01f-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="1e01f-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1e01f-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="1e01f-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1e01f-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="1e01f-149">This property is read-only.</span></span> <span data-ttu-id="1e01f-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e01f-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1e01f-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1e01f-151">createdDateTime</span></span>|<span data-ttu-id="1e01f-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e01f-152">DateTimeOffset</span></span>|<span data-ttu-id="1e01f-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1e01f-153">DateTime the object was created.</span></span> <span data-ttu-id="1e01f-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e01f-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1e01f-155">description</span><span class="sxs-lookup"><span data-stu-id="1e01f-155">description</span></span>|<span data-ttu-id="1e01f-156">String</span><span class="sxs-lookup"><span data-stu-id="1e01f-156">String</span></span>|<span data-ttu-id="1e01f-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="1e01f-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1e01f-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e01f-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1e01f-159">displayName</span><span class="sxs-lookup"><span data-stu-id="1e01f-159">displayName</span></span>|<span data-ttu-id="1e01f-160">String</span><span class="sxs-lookup"><span data-stu-id="1e01f-160">String</span></span>|<span data-ttu-id="1e01f-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="1e01f-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1e01f-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e01f-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1e01f-163">version</span><span class="sxs-lookup"><span data-stu-id="1e01f-163">version</span></span>|<span data-ttu-id="1e01f-164">Int32</span><span class="sxs-lookup"><span data-stu-id="1e01f-164">Int32</span></span>|<span data-ttu-id="1e01f-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="1e01f-165">Version of the device configuration.</span></span> <span data-ttu-id="1e01f-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e01f-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1e01f-167">omaSettings</span><span class="sxs-lookup"><span data-stu-id="1e01f-167">omaSettings</span></span>|<span data-ttu-id="1e01f-168">[omaSetting](../resources/intune-deviceconfig-omasetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1e01f-168">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="1e01f-169">OMA 设置。</span><span class="sxs-lookup"><span data-stu-id="1e01f-169">OMA settings.</span></span> <span data-ttu-id="1e01f-170">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="1e01f-170">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="1e01f-171">响应</span><span class="sxs-lookup"><span data-stu-id="1e01f-171">Response</span></span>
<span data-ttu-id="1e01f-172">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1e01f-172">If successful, this method returns a `201 Created` response code and a [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e01f-173">示例</span><span class="sxs-lookup"><span data-stu-id="1e01f-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="1e01f-174">请求</span><span class="sxs-lookup"><span data-stu-id="1e01f-174">Request</span></span>
<span data-ttu-id="1e01f-175">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1e01f-175">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 505

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="1e01f-176">响应</span><span class="sxs-lookup"><span data-stu-id="1e01f-176">Response</span></span>
<span data-ttu-id="1e01f-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1e01f-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 677

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
  "id": "76c5d59b-d59b-76c5-9bd5-c5769bd5c576",
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





