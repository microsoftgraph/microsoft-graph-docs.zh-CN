---
title: 更新 windowsPhone81TrustedRootCertificate
description: 更新 windowsPhone81TrustedRootCertificate 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e0acc47bd427a61e9009db8ecb7cb16f65f0f2d8
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31803519"
---
# <a name="update-windowsphone81trustedrootcertificate"></a><span data-ttu-id="99067-103">更新 windowsPhone81TrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="99067-103">Update windowsPhone81TrustedRootCertificate</span></span>

> <span data-ttu-id="99067-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="99067-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="99067-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="99067-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99067-106">更新[windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="99067-106">Update the properties of a [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="99067-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="99067-107">Prerequisites</span></span>
<span data-ttu-id="99067-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="99067-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99067-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="99067-110">Permission type</span></span>|<span data-ttu-id="99067-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="99067-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="99067-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="99067-112">Delegated (work or school account)</span></span>|<span data-ttu-id="99067-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99067-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="99067-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="99067-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="99067-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="99067-115">Not supported.</span></span>|
|<span data-ttu-id="99067-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="99067-116">Application</span></span>|<span data-ttu-id="99067-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="99067-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="99067-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="99067-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/rootCertificate
```

## <a name="request-headers"></a><span data-ttu-id="99067-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="99067-119">Request headers</span></span>
|<span data-ttu-id="99067-120">标头</span><span class="sxs-lookup"><span data-stu-id="99067-120">Header</span></span>|<span data-ttu-id="99067-121">值</span><span class="sxs-lookup"><span data-stu-id="99067-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="99067-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="99067-122">Authorization</span></span>|<span data-ttu-id="99067-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="99067-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="99067-124">接受</span><span class="sxs-lookup"><span data-stu-id="99067-124">Accept</span></span>|<span data-ttu-id="99067-125">application/json</span><span class="sxs-lookup"><span data-stu-id="99067-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="99067-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="99067-126">Request body</span></span>
<span data-ttu-id="99067-127">在请求正文中, 提供[windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="99067-127">In the request body, supply a JSON representation for the [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) object.</span></span>

<span data-ttu-id="99067-128">下表显示创建[windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="99067-128">The following table shows the properties that are required when you create the [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md).</span></span>

|<span data-ttu-id="99067-129">属性</span><span class="sxs-lookup"><span data-stu-id="99067-129">Property</span></span>|<span data-ttu-id="99067-130">类型</span><span class="sxs-lookup"><span data-stu-id="99067-130">Type</span></span>|<span data-ttu-id="99067-131">说明</span><span class="sxs-lookup"><span data-stu-id="99067-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99067-132">id</span><span class="sxs-lookup"><span data-stu-id="99067-132">id</span></span>|<span data-ttu-id="99067-133">String</span><span class="sxs-lookup"><span data-stu-id="99067-133">String</span></span>|<span data-ttu-id="99067-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="99067-134">Key of the entity.</span></span> <span data-ttu-id="99067-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="99067-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="99067-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="99067-136">lastModifiedDateTime</span></span>|<span data-ttu-id="99067-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99067-137">DateTimeOffset</span></span>|<span data-ttu-id="99067-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="99067-138">DateTime the object was last modified.</span></span> <span data-ttu-id="99067-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="99067-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="99067-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="99067-140">roleScopeTagIds</span></span>|<span data-ttu-id="99067-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="99067-141">String collection</span></span>|<span data-ttu-id="99067-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="99067-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="99067-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="99067-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="99067-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="99067-144">supportsScopeTags</span></span>|<span data-ttu-id="99067-145">布尔值</span><span class="sxs-lookup"><span data-stu-id="99067-145">Boolean</span></span>|<span data-ttu-id="99067-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="99067-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="99067-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="99067-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="99067-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="99067-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="99067-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="99067-149">This property is read-only.</span></span> <span data-ttu-id="99067-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="99067-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="99067-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="99067-151">createdDateTime</span></span>|<span data-ttu-id="99067-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99067-152">DateTimeOffset</span></span>|<span data-ttu-id="99067-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="99067-153">DateTime the object was created.</span></span> <span data-ttu-id="99067-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="99067-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="99067-155">description</span><span class="sxs-lookup"><span data-stu-id="99067-155">description</span></span>|<span data-ttu-id="99067-156">String</span><span class="sxs-lookup"><span data-stu-id="99067-156">String</span></span>|<span data-ttu-id="99067-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="99067-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="99067-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="99067-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="99067-159">displayName</span><span class="sxs-lookup"><span data-stu-id="99067-159">displayName</span></span>|<span data-ttu-id="99067-160">String</span><span class="sxs-lookup"><span data-stu-id="99067-160">String</span></span>|<span data-ttu-id="99067-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="99067-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="99067-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="99067-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="99067-163">version</span><span class="sxs-lookup"><span data-stu-id="99067-163">version</span></span>|<span data-ttu-id="99067-164">Int32</span><span class="sxs-lookup"><span data-stu-id="99067-164">Int32</span></span>|<span data-ttu-id="99067-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="99067-165">Version of the device configuration.</span></span> <span data-ttu-id="99067-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="99067-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="99067-167">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="99067-167">trustedRootCertificate</span></span>|<span data-ttu-id="99067-168">Binary</span><span class="sxs-lookup"><span data-stu-id="99067-168">Binary</span></span>|<span data-ttu-id="99067-169">受信任的根证书</span><span class="sxs-lookup"><span data-stu-id="99067-169">Trusted Root Certificate</span></span>|
|<span data-ttu-id="99067-170">certFileName</span><span class="sxs-lookup"><span data-stu-id="99067-170">certFileName</span></span>|<span data-ttu-id="99067-171">String</span><span class="sxs-lookup"><span data-stu-id="99067-171">String</span></span>|<span data-ttu-id="99067-172">要在 UI 中显示的文件名。</span><span class="sxs-lookup"><span data-stu-id="99067-172">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="99067-173">响应</span><span class="sxs-lookup"><span data-stu-id="99067-173">Response</span></span>
<span data-ttu-id="99067-174">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="99067-174">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99067-175">示例</span><span class="sxs-lookup"><span data-stu-id="99067-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="99067-176">请求</span><span class="sxs-lookup"><span data-stu-id="99067-176">Request</span></span>
<span data-ttu-id="99067-177">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="99067-177">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/rootCertificate
Content-type: application/json
Content-length: 374

{
  "@odata.type": "#microsoft.graph.windowsPhone81TrustedRootCertificate",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
  "certFileName": "Cert File Name value"
}
```

### <a name="response"></a><span data-ttu-id="99067-178">响应</span><span class="sxs-lookup"><span data-stu-id="99067-178">Response</span></span>
<span data-ttu-id="99067-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="99067-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 546

{
  "@odata.type": "#microsoft.graph.windowsPhone81TrustedRootCertificate",
  "id": "6316bf01-bf01-6316-01bf-166301bf1663",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
  "certFileName": "Cert File Name value"
}
```





