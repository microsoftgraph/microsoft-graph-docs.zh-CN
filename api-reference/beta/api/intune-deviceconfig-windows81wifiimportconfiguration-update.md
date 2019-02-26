---
title: 更新 windows81WifiImportConfiguration
description: 更新 windows81WifiImportConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3163018e7f8822dbdf151f19949bf1be626c0f66
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30162865"
---
# <a name="update-windows81wifiimportconfiguration"></a><span data-ttu-id="fd645-103">更新 windows81WifiImportConfiguration</span><span class="sxs-lookup"><span data-stu-id="fd645-103">Update windows81WifiImportConfiguration</span></span>

> <span data-ttu-id="fd645-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fd645-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fd645-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fd645-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd645-106">更新[windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="fd645-106">Update the properties of a [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fd645-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="fd645-107">Prerequisites</span></span>
<span data-ttu-id="fd645-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="fd645-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fd645-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="fd645-110">Permission type</span></span>|<span data-ttu-id="fd645-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fd645-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fd645-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fd645-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fd645-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd645-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fd645-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fd645-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd645-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="fd645-115">Not supported.</span></span>|
|<span data-ttu-id="fd645-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="fd645-116">Application</span></span>|<span data-ttu-id="fd645-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="fd645-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fd645-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fd645-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="fd645-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="fd645-119">Request headers</span></span>
|<span data-ttu-id="fd645-120">标头</span><span class="sxs-lookup"><span data-stu-id="fd645-120">Header</span></span>|<span data-ttu-id="fd645-121">值</span><span class="sxs-lookup"><span data-stu-id="fd645-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fd645-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd645-122">Authorization</span></span>|<span data-ttu-id="fd645-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fd645-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fd645-124">Accept</span><span class="sxs-lookup"><span data-stu-id="fd645-124">Accept</span></span>|<span data-ttu-id="fd645-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fd645-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd645-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="fd645-126">Request body</span></span>
<span data-ttu-id="fd645-127">在请求正文中, 提供[windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fd645-127">In the request body, supply a JSON representation for the [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object.</span></span>

<span data-ttu-id="fd645-128">下表显示创建[windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="fd645-128">The following table shows the properties that are required when you create the [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md).</span></span>

|<span data-ttu-id="fd645-129">属性</span><span class="sxs-lookup"><span data-stu-id="fd645-129">Property</span></span>|<span data-ttu-id="fd645-130">类型</span><span class="sxs-lookup"><span data-stu-id="fd645-130">Type</span></span>|<span data-ttu-id="fd645-131">说明</span><span class="sxs-lookup"><span data-stu-id="fd645-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd645-132">id</span><span class="sxs-lookup"><span data-stu-id="fd645-132">id</span></span>|<span data-ttu-id="fd645-133">字符串</span><span class="sxs-lookup"><span data-stu-id="fd645-133">String</span></span>|<span data-ttu-id="fd645-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="fd645-134">Key of the entity.</span></span> <span data-ttu-id="fd645-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fd645-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fd645-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fd645-136">lastModifiedDateTime</span></span>|<span data-ttu-id="fd645-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd645-137">DateTimeOffset</span></span>|<span data-ttu-id="fd645-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="fd645-138">DateTime the object was last modified.</span></span> <span data-ttu-id="fd645-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fd645-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fd645-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fd645-140">roleScopeTagIds</span></span>|<span data-ttu-id="fd645-141">String collection</span><span class="sxs-lookup"><span data-stu-id="fd645-141">String collection</span></span>|<span data-ttu-id="fd645-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="fd645-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="fd645-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fd645-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fd645-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="fd645-144">supportsScopeTags</span></span>|<span data-ttu-id="fd645-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="fd645-145">Boolean</span></span>|<span data-ttu-id="fd645-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="fd645-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="fd645-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="fd645-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="fd645-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="fd645-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="fd645-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="fd645-149">This property is read-only.</span></span> <span data-ttu-id="fd645-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fd645-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fd645-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fd645-151">createdDateTime</span></span>|<span data-ttu-id="fd645-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd645-152">DateTimeOffset</span></span>|<span data-ttu-id="fd645-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="fd645-153">DateTime the object was created.</span></span> <span data-ttu-id="fd645-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fd645-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fd645-155">description</span><span class="sxs-lookup"><span data-stu-id="fd645-155">description</span></span>|<span data-ttu-id="fd645-156">String</span><span class="sxs-lookup"><span data-stu-id="fd645-156">String</span></span>|<span data-ttu-id="fd645-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="fd645-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fd645-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fd645-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fd645-159">displayName</span><span class="sxs-lookup"><span data-stu-id="fd645-159">displayName</span></span>|<span data-ttu-id="fd645-160">String</span><span class="sxs-lookup"><span data-stu-id="fd645-160">String</span></span>|<span data-ttu-id="fd645-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="fd645-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fd645-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fd645-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fd645-163">version</span><span class="sxs-lookup"><span data-stu-id="fd645-163">version</span></span>|<span data-ttu-id="fd645-164">Int32</span><span class="sxs-lookup"><span data-stu-id="fd645-164">Int32</span></span>|<span data-ttu-id="fd645-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="fd645-165">Version of the device configuration.</span></span> <span data-ttu-id="fd645-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fd645-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fd645-167">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="fd645-167">payloadFileName</span></span>|<span data-ttu-id="fd645-168">String</span><span class="sxs-lookup"><span data-stu-id="fd645-168">String</span></span>|<span data-ttu-id="fd645-169">有效负载文件名 (\* .xml)。</span><span class="sxs-lookup"><span data-stu-id="fd645-169">Payload file name (\*.xml).</span></span>|
|<span data-ttu-id="fd645-170">profileName</span><span class="sxs-lookup"><span data-stu-id="fd645-170">profileName</span></span>|<span data-ttu-id="fd645-171">String</span><span class="sxs-lookup"><span data-stu-id="fd645-171">String</span></span>|<span data-ttu-id="fd645-172">UI 中显示的配置文件名称。</span><span class="sxs-lookup"><span data-stu-id="fd645-172">Profile name displayed in the UI.</span></span>|
|<span data-ttu-id="fd645-173">payload</span><span class="sxs-lookup"><span data-stu-id="fd645-173">payload</span></span>|<span data-ttu-id="fd645-174">Binary</span><span class="sxs-lookup"><span data-stu-id="fd645-174">Binary</span></span>|<span data-ttu-id="fd645-175">有效负载。</span><span class="sxs-lookup"><span data-stu-id="fd645-175">Payload.</span></span> <span data-ttu-id="fd645-176">(UTF8 编码的字节数组)。</span><span class="sxs-lookup"><span data-stu-id="fd645-176">(UTF8 encoded byte array).</span></span> <span data-ttu-id="fd645-177">这是保存在用于连接到 wi-fi 终结点的设备上的 XML 文件。</span><span class="sxs-lookup"><span data-stu-id="fd645-177">This is the XML file saved on the device you used to connect to the Wi-Fi endpoint.</span></span>|



## <a name="response"></a><span data-ttu-id="fd645-178">响应</span><span class="sxs-lookup"><span data-stu-id="fd645-178">Response</span></span>
<span data-ttu-id="fd645-179">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="fd645-179">If successful, this method returns a `200 OK` response code and an updated [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd645-180">示例</span><span class="sxs-lookup"><span data-stu-id="fd645-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="fd645-181">请求</span><span class="sxs-lookup"><span data-stu-id="fd645-181">Request</span></span>
<span data-ttu-id="fd645-182">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fd645-182">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="fd645-183">响应</span><span class="sxs-lookup"><span data-stu-id="fd645-183">Response</span></span>
<span data-ttu-id="fd645-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fd645-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




