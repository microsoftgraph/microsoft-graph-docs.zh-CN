---
title: 创建 windows81WifiImportConfiguration
description: 创建新的 windows81WifiImportConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 47e8f9f818b48a5ddb30e1bce6afbc0c103df40b
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31796834"
---
# <a name="create-windows81wifiimportconfiguration"></a><span data-ttu-id="192f4-103">创建 windows81WifiImportConfiguration</span><span class="sxs-lookup"><span data-stu-id="192f4-103">Create windows81WifiImportConfiguration</span></span>

> <span data-ttu-id="192f4-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="192f4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="192f4-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="192f4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="192f4-106">创建新的[windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="192f4-106">Create a new [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="192f4-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="192f4-107">Prerequisites</span></span>
<span data-ttu-id="192f4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="192f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="192f4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="192f4-110">Permission type</span></span>|<span data-ttu-id="192f4-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="192f4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="192f4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="192f4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="192f4-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="192f4-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="192f4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="192f4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="192f4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="192f4-115">Not supported.</span></span>|
|<span data-ttu-id="192f4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="192f4-116">Application</span></span>|<span data-ttu-id="192f4-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="192f4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="192f4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="192f4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="192f4-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="192f4-119">Request headers</span></span>
|<span data-ttu-id="192f4-120">标头</span><span class="sxs-lookup"><span data-stu-id="192f4-120">Header</span></span>|<span data-ttu-id="192f4-121">值</span><span class="sxs-lookup"><span data-stu-id="192f4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="192f4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="192f4-122">Authorization</span></span>|<span data-ttu-id="192f4-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="192f4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="192f4-124">接受</span><span class="sxs-lookup"><span data-stu-id="192f4-124">Accept</span></span>|<span data-ttu-id="192f4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="192f4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="192f4-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="192f4-126">Request body</span></span>
<span data-ttu-id="192f4-127">在请求正文中, 提供 windows81WifiImportConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="192f4-127">In the request body, supply a JSON representation for the windows81WifiImportConfiguration object.</span></span>

<span data-ttu-id="192f4-128">下表显示创建 windows81WifiImportConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="192f4-128">The following table shows the properties that are required when you create the windows81WifiImportConfiguration.</span></span>

|<span data-ttu-id="192f4-129">属性</span><span class="sxs-lookup"><span data-stu-id="192f4-129">Property</span></span>|<span data-ttu-id="192f4-130">类型</span><span class="sxs-lookup"><span data-stu-id="192f4-130">Type</span></span>|<span data-ttu-id="192f4-131">说明</span><span class="sxs-lookup"><span data-stu-id="192f4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="192f4-132">id</span><span class="sxs-lookup"><span data-stu-id="192f4-132">id</span></span>|<span data-ttu-id="192f4-133">String</span><span class="sxs-lookup"><span data-stu-id="192f4-133">String</span></span>|<span data-ttu-id="192f4-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="192f4-134">Key of the entity.</span></span> <span data-ttu-id="192f4-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="192f4-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="192f4-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="192f4-136">lastModifiedDateTime</span></span>|<span data-ttu-id="192f4-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="192f4-137">DateTimeOffset</span></span>|<span data-ttu-id="192f4-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="192f4-138">DateTime the object was last modified.</span></span> <span data-ttu-id="192f4-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="192f4-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="192f4-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="192f4-140">roleScopeTagIds</span></span>|<span data-ttu-id="192f4-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="192f4-141">String collection</span></span>|<span data-ttu-id="192f4-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="192f4-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="192f4-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="192f4-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="192f4-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="192f4-144">supportsScopeTags</span></span>|<span data-ttu-id="192f4-145">布尔值</span><span class="sxs-lookup"><span data-stu-id="192f4-145">Boolean</span></span>|<span data-ttu-id="192f4-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="192f4-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="192f4-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="192f4-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="192f4-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="192f4-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="192f4-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="192f4-149">This property is read-only.</span></span> <span data-ttu-id="192f4-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="192f4-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="192f4-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="192f4-151">createdDateTime</span></span>|<span data-ttu-id="192f4-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="192f4-152">DateTimeOffset</span></span>|<span data-ttu-id="192f4-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="192f4-153">DateTime the object was created.</span></span> <span data-ttu-id="192f4-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="192f4-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="192f4-155">description</span><span class="sxs-lookup"><span data-stu-id="192f4-155">description</span></span>|<span data-ttu-id="192f4-156">String</span><span class="sxs-lookup"><span data-stu-id="192f4-156">String</span></span>|<span data-ttu-id="192f4-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="192f4-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="192f4-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="192f4-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="192f4-159">displayName</span><span class="sxs-lookup"><span data-stu-id="192f4-159">displayName</span></span>|<span data-ttu-id="192f4-160">String</span><span class="sxs-lookup"><span data-stu-id="192f4-160">String</span></span>|<span data-ttu-id="192f4-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="192f4-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="192f4-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="192f4-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="192f4-163">version</span><span class="sxs-lookup"><span data-stu-id="192f4-163">version</span></span>|<span data-ttu-id="192f4-164">Int32</span><span class="sxs-lookup"><span data-stu-id="192f4-164">Int32</span></span>|<span data-ttu-id="192f4-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="192f4-165">Version of the device configuration.</span></span> <span data-ttu-id="192f4-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="192f4-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="192f4-167">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="192f4-167">payloadFileName</span></span>|<span data-ttu-id="192f4-168">String</span><span class="sxs-lookup"><span data-stu-id="192f4-168">String</span></span>|<span data-ttu-id="192f4-169">有效负载文件名 (\* .xml)。</span><span class="sxs-lookup"><span data-stu-id="192f4-169">Payload file name (\*.xml).</span></span>|
|<span data-ttu-id="192f4-170">profileName</span><span class="sxs-lookup"><span data-stu-id="192f4-170">profileName</span></span>|<span data-ttu-id="192f4-171">String</span><span class="sxs-lookup"><span data-stu-id="192f4-171">String</span></span>|<span data-ttu-id="192f4-172">UI 中显示的配置文件名称。</span><span class="sxs-lookup"><span data-stu-id="192f4-172">Profile name displayed in the UI.</span></span>|
|<span data-ttu-id="192f4-173">payload</span><span class="sxs-lookup"><span data-stu-id="192f4-173">payload</span></span>|<span data-ttu-id="192f4-174">Binary</span><span class="sxs-lookup"><span data-stu-id="192f4-174">Binary</span></span>|<span data-ttu-id="192f4-175">有效负载。</span><span class="sxs-lookup"><span data-stu-id="192f4-175">Payload.</span></span> <span data-ttu-id="192f4-176">(UTF8 编码的字节数组)。</span><span class="sxs-lookup"><span data-stu-id="192f4-176">(UTF8 encoded byte array).</span></span> <span data-ttu-id="192f4-177">这是保存在用于连接到 wi-fi 终结点的设备上的 XML 文件。</span><span class="sxs-lookup"><span data-stu-id="192f4-177">This is the XML file saved on the device you used to connect to the Wi-Fi endpoint.</span></span>|



## <a name="response"></a><span data-ttu-id="192f4-178">响应</span><span class="sxs-lookup"><span data-stu-id="192f4-178">Response</span></span>
<span data-ttu-id="192f4-179">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="192f4-179">If successful, this method returns a `201 Created` response code and a [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="192f4-180">示例</span><span class="sxs-lookup"><span data-stu-id="192f4-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="192f4-181">请求</span><span class="sxs-lookup"><span data-stu-id="192f4-181">Request</span></span>
<span data-ttu-id="192f4-182">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="192f4-182">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 381

{
  "@odata.type": "#microsoft.graph.windows81WifiImportConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadFileName": "Payload File Name value",
  "profileName": "Profile Name value",
  "payload": "cGF5bG9hZA=="
}
```

### <a name="response"></a><span data-ttu-id="192f4-183">响应</span><span class="sxs-lookup"><span data-stu-id="192f4-183">Response</span></span>
<span data-ttu-id="192f4-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="192f4-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 553

{
  "@odata.type": "#microsoft.graph.windows81WifiImportConfiguration",
  "id": "534a2f07-2f07-534a-072f-4a53072f4a53",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadFileName": "Payload File Name value",
  "profileName": "Profile Name value",
  "payload": "cGF5bG9hZA=="
}
```





