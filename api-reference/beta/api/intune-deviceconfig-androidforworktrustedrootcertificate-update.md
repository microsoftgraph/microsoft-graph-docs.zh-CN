---
title: 更新 androidForWorkTrustedRootCertificate
description: 更新 androidForWorkTrustedRootCertificate 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 128f18b27b985503957872b46b55086e9bce031b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32478096"
---
# <a name="update-androidforworktrustedrootcertificate"></a><span data-ttu-id="d30d3-103">更新 androidForWorkTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="d30d3-103">Update androidForWorkTrustedRootCertificate</span></span>

> <span data-ttu-id="d30d3-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d30d3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d30d3-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d30d3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d30d3-106">更新[androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d30d3-106">Update the properties of a [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d30d3-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="d30d3-107">Prerequisites</span></span>
<span data-ttu-id="d30d3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d30d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d30d3-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d30d3-110">Permission type</span></span>|<span data-ttu-id="d30d3-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d30d3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d30d3-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d30d3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d30d3-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d30d3-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d30d3-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d30d3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d30d3-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d30d3-115">Not supported.</span></span>|
|<span data-ttu-id="d30d3-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d30d3-116">Application</span></span>|<span data-ttu-id="d30d3-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d30d3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d30d3-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d30d3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkEnterpriseWiFiConfiguration/rootCertificateForServerValidation
```

## <a name="request-headers"></a><span data-ttu-id="d30d3-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d30d3-119">Request headers</span></span>
|<span data-ttu-id="d30d3-120">标头</span><span class="sxs-lookup"><span data-stu-id="d30d3-120">Header</span></span>|<span data-ttu-id="d30d3-121">值</span><span class="sxs-lookup"><span data-stu-id="d30d3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d30d3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d30d3-122">Authorization</span></span>|<span data-ttu-id="d30d3-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d30d3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d30d3-124">接受</span><span class="sxs-lookup"><span data-stu-id="d30d3-124">Accept</span></span>|<span data-ttu-id="d30d3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d30d3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d30d3-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d30d3-126">Request body</span></span>
<span data-ttu-id="d30d3-127">在请求正文中, 提供[androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d30d3-127">In the request body, supply a JSON representation for the [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) object.</span></span>

<span data-ttu-id="d30d3-128">下表显示创建[androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d30d3-128">The following table shows the properties that are required when you create the [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md).</span></span>

|<span data-ttu-id="d30d3-129">属性</span><span class="sxs-lookup"><span data-stu-id="d30d3-129">Property</span></span>|<span data-ttu-id="d30d3-130">类型</span><span class="sxs-lookup"><span data-stu-id="d30d3-130">Type</span></span>|<span data-ttu-id="d30d3-131">说明</span><span class="sxs-lookup"><span data-stu-id="d30d3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d30d3-132">id</span><span class="sxs-lookup"><span data-stu-id="d30d3-132">id</span></span>|<span data-ttu-id="d30d3-133">String</span><span class="sxs-lookup"><span data-stu-id="d30d3-133">String</span></span>|<span data-ttu-id="d30d3-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d30d3-134">Key of the entity.</span></span> <span data-ttu-id="d30d3-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d30d3-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d30d3-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d30d3-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d30d3-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d30d3-137">DateTimeOffset</span></span>|<span data-ttu-id="d30d3-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d30d3-138">DateTime the object was last modified.</span></span> <span data-ttu-id="d30d3-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d30d3-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d30d3-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d30d3-140">roleScopeTagIds</span></span>|<span data-ttu-id="d30d3-141">String collection</span><span class="sxs-lookup"><span data-stu-id="d30d3-141">String collection</span></span>|<span data-ttu-id="d30d3-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="d30d3-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d30d3-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d30d3-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d30d3-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d30d3-144">supportsScopeTags</span></span>|<span data-ttu-id="d30d3-145">布尔</span><span class="sxs-lookup"><span data-stu-id="d30d3-145">Boolean</span></span>|<span data-ttu-id="d30d3-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="d30d3-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d30d3-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="d30d3-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d30d3-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="d30d3-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d30d3-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="d30d3-149">This property is read-only.</span></span> <span data-ttu-id="d30d3-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d30d3-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d30d3-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d30d3-151">createdDateTime</span></span>|<span data-ttu-id="d30d3-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d30d3-152">DateTimeOffset</span></span>|<span data-ttu-id="d30d3-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d30d3-153">DateTime the object was created.</span></span> <span data-ttu-id="d30d3-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d30d3-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d30d3-155">description</span><span class="sxs-lookup"><span data-stu-id="d30d3-155">description</span></span>|<span data-ttu-id="d30d3-156">字符串</span><span class="sxs-lookup"><span data-stu-id="d30d3-156">String</span></span>|<span data-ttu-id="d30d3-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="d30d3-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d30d3-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d30d3-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d30d3-159">displayName</span><span class="sxs-lookup"><span data-stu-id="d30d3-159">displayName</span></span>|<span data-ttu-id="d30d3-160">String</span><span class="sxs-lookup"><span data-stu-id="d30d3-160">String</span></span>|<span data-ttu-id="d30d3-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="d30d3-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d30d3-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d30d3-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d30d3-163">version</span><span class="sxs-lookup"><span data-stu-id="d30d3-163">version</span></span>|<span data-ttu-id="d30d3-164">Int32</span><span class="sxs-lookup"><span data-stu-id="d30d3-164">Int32</span></span>|<span data-ttu-id="d30d3-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="d30d3-165">Version of the device configuration.</span></span> <span data-ttu-id="d30d3-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d30d3-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d30d3-167">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="d30d3-167">trustedRootCertificate</span></span>|<span data-ttu-id="d30d3-168">Binary</span><span class="sxs-lookup"><span data-stu-id="d30d3-168">Binary</span></span>|<span data-ttu-id="d30d3-169">受信任的根证书</span><span class="sxs-lookup"><span data-stu-id="d30d3-169">Trusted Root Certificate</span></span>|
|<span data-ttu-id="d30d3-170">certFileName</span><span class="sxs-lookup"><span data-stu-id="d30d3-170">certFileName</span></span>|<span data-ttu-id="d30d3-171">字符串</span><span class="sxs-lookup"><span data-stu-id="d30d3-171">String</span></span>|<span data-ttu-id="d30d3-172">要在 UI 中显示的文件名。</span><span class="sxs-lookup"><span data-stu-id="d30d3-172">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="d30d3-173">响应</span><span class="sxs-lookup"><span data-stu-id="d30d3-173">Response</span></span>
<span data-ttu-id="d30d3-174">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d30d3-174">If successful, this method returns a `200 OK` response code and an updated [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d30d3-175">示例</span><span class="sxs-lookup"><span data-stu-id="d30d3-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="d30d3-176">请求</span><span class="sxs-lookup"><span data-stu-id="d30d3-176">Request</span></span>
<span data-ttu-id="d30d3-177">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d30d3-177">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate
Content-type: application/json
Content-length: 374

{
  "@odata.type": "#microsoft.graph.androidForWorkTrustedRootCertificate",
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

### <a name="response"></a><span data-ttu-id="d30d3-178">响应</span><span class="sxs-lookup"><span data-stu-id="d30d3-178">Response</span></span>
<span data-ttu-id="d30d3-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d30d3-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 546

{
  "@odata.type": "#microsoft.graph.androidForWorkTrustedRootCertificate",
  "id": "2f78834c-834c-2f78-4c83-782f4c83782f",
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





