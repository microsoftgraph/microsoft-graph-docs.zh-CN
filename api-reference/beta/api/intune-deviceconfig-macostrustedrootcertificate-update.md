---
title: 更新 macOSTrustedRootCertificate
description: 更新 macOSTrustedRootCertificate 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f825680cfd0c4826aeba1c491cc8761a61b10ce7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30158112"
---
# <a name="update-macostrustedrootcertificate"></a><span data-ttu-id="3b303-103">更新 macOSTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="3b303-103">Update macOSTrustedRootCertificate</span></span>

> <span data-ttu-id="3b303-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3b303-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3b303-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3b303-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b303-106">更新[macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3b303-106">Update the properties of a [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3b303-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="3b303-107">Prerequisites</span></span>
<span data-ttu-id="3b303-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="3b303-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3b303-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3b303-110">Permission type</span></span>|<span data-ttu-id="3b303-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3b303-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b303-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3b303-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3b303-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b303-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3b303-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3b303-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b303-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3b303-115">Not supported.</span></span>|
|<span data-ttu-id="3b303-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3b303-116">Application</span></span>|<span data-ttu-id="3b303-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="3b303-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b303-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3b303-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSEnterpriseWiFiConfiguration/rootCertificateForServerValidation
```

## <a name="request-headers"></a><span data-ttu-id="3b303-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3b303-119">Request headers</span></span>
|<span data-ttu-id="3b303-120">标头</span><span class="sxs-lookup"><span data-stu-id="3b303-120">Header</span></span>|<span data-ttu-id="3b303-121">值</span><span class="sxs-lookup"><span data-stu-id="3b303-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b303-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b303-122">Authorization</span></span>|<span data-ttu-id="3b303-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3b303-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b303-124">Accept</span><span class="sxs-lookup"><span data-stu-id="3b303-124">Accept</span></span>|<span data-ttu-id="3b303-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3b303-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b303-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="3b303-126">Request body</span></span>
<span data-ttu-id="3b303-127">在请求正文中, 提供[macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3b303-127">In the request body, supply a JSON representation for the [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) object.</span></span>

<span data-ttu-id="3b303-128">下表显示创建[macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3b303-128">The following table shows the properties that are required when you create the [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md).</span></span>

|<span data-ttu-id="3b303-129">属性</span><span class="sxs-lookup"><span data-stu-id="3b303-129">Property</span></span>|<span data-ttu-id="3b303-130">类型</span><span class="sxs-lookup"><span data-stu-id="3b303-130">Type</span></span>|<span data-ttu-id="3b303-131">说明</span><span class="sxs-lookup"><span data-stu-id="3b303-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b303-132">id</span><span class="sxs-lookup"><span data-stu-id="3b303-132">id</span></span>|<span data-ttu-id="3b303-133">String</span><span class="sxs-lookup"><span data-stu-id="3b303-133">String</span></span>|<span data-ttu-id="3b303-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="3b303-134">Key of the entity.</span></span> <span data-ttu-id="3b303-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3b303-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3b303-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3b303-136">lastModifiedDateTime</span></span>|<span data-ttu-id="3b303-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b303-137">DateTimeOffset</span></span>|<span data-ttu-id="3b303-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="3b303-138">DateTime the object was last modified.</span></span> <span data-ttu-id="3b303-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3b303-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3b303-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3b303-140">roleScopeTagIds</span></span>|<span data-ttu-id="3b303-141">String collection</span><span class="sxs-lookup"><span data-stu-id="3b303-141">String collection</span></span>|<span data-ttu-id="3b303-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="3b303-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3b303-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3b303-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3b303-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="3b303-144">supportsScopeTags</span></span>|<span data-ttu-id="3b303-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="3b303-145">Boolean</span></span>|<span data-ttu-id="3b303-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="3b303-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3b303-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="3b303-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3b303-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="3b303-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3b303-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="3b303-149">This property is read-only.</span></span> <span data-ttu-id="3b303-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3b303-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3b303-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3b303-151">createdDateTime</span></span>|<span data-ttu-id="3b303-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b303-152">DateTimeOffset</span></span>|<span data-ttu-id="3b303-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="3b303-153">DateTime the object was created.</span></span> <span data-ttu-id="3b303-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3b303-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3b303-155">description</span><span class="sxs-lookup"><span data-stu-id="3b303-155">description</span></span>|<span data-ttu-id="3b303-156">String</span><span class="sxs-lookup"><span data-stu-id="3b303-156">String</span></span>|<span data-ttu-id="3b303-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="3b303-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3b303-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3b303-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3b303-159">displayName</span><span class="sxs-lookup"><span data-stu-id="3b303-159">displayName</span></span>|<span data-ttu-id="3b303-160">String</span><span class="sxs-lookup"><span data-stu-id="3b303-160">String</span></span>|<span data-ttu-id="3b303-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="3b303-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3b303-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3b303-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3b303-163">version</span><span class="sxs-lookup"><span data-stu-id="3b303-163">version</span></span>|<span data-ttu-id="3b303-164">Int32</span><span class="sxs-lookup"><span data-stu-id="3b303-164">Int32</span></span>|<span data-ttu-id="3b303-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="3b303-165">Version of the device configuration.</span></span> <span data-ttu-id="3b303-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3b303-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3b303-167">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="3b303-167">trustedRootCertificate</span></span>|<span data-ttu-id="3b303-168">Binary</span><span class="sxs-lookup"><span data-stu-id="3b303-168">Binary</span></span>|<span data-ttu-id="3b303-169">受信任的根证书。</span><span class="sxs-lookup"><span data-stu-id="3b303-169">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="3b303-170">certFileName</span><span class="sxs-lookup"><span data-stu-id="3b303-170">certFileName</span></span>|<span data-ttu-id="3b303-171">String</span><span class="sxs-lookup"><span data-stu-id="3b303-171">String</span></span>|<span data-ttu-id="3b303-172">要在 UI 中显示的文件名。</span><span class="sxs-lookup"><span data-stu-id="3b303-172">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="3b303-173">响应</span><span class="sxs-lookup"><span data-stu-id="3b303-173">Response</span></span>
<span data-ttu-id="3b303-174">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3b303-174">If successful, this method returns a `200 OK` response code and an updated [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b303-175">示例</span><span class="sxs-lookup"><span data-stu-id="3b303-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="3b303-176">请求</span><span class="sxs-lookup"><span data-stu-id="3b303-176">Request</span></span>
<span data-ttu-id="3b303-177">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3b303-177">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate
Content-type: application/json
Content-length: 365

{
  "@odata.type": "#microsoft.graph.macOSTrustedRootCertificate",
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

### <a name="response"></a><span data-ttu-id="3b303-178">响应</span><span class="sxs-lookup"><span data-stu-id="3b303-178">Response</span></span>
<span data-ttu-id="3b303-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3b303-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 537

{
  "@odata.type": "#microsoft.graph.macOSTrustedRootCertificate",
  "id": "c5fac954-c954-c5fa-54c9-fac554c9fac5",
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




