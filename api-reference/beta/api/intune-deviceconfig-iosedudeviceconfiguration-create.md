---
title: 创建 iosEduDeviceConfiguration
description: 创建新的 iosEduDeviceConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4f6d0016aca3eff6e699ec82b96aad4d18577d6e
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30973353"
---
# <a name="create-iosedudeviceconfiguration"></a><span data-ttu-id="a6f0c-103">创建 iosEduDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="a6f0c-103">Create iosEduDeviceConfiguration</span></span>

> <span data-ttu-id="a6f0c-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a6f0c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a6f0c-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a6f0c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6f0c-106">创建新的[iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a6f0c-106">Create a new [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a6f0c-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a6f0c-107">Prerequisites</span></span>
<span data-ttu-id="a6f0c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a6f0c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6f0c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a6f0c-110">Permission type</span></span>|<span data-ttu-id="a6f0c-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a6f0c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6f0c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a6f0c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a6f0c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6f0c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a6f0c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a6f0c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6f0c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a6f0c-115">Not supported.</span></span>|
|<span data-ttu-id="a6f0c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a6f0c-116">Application</span></span>|<span data-ttu-id="a6f0c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a6f0c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6f0c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a6f0c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a6f0c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a6f0c-119">Request headers</span></span>
|<span data-ttu-id="a6f0c-120">标头</span><span class="sxs-lookup"><span data-stu-id="a6f0c-120">Header</span></span>|<span data-ttu-id="a6f0c-121">值</span><span class="sxs-lookup"><span data-stu-id="a6f0c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6f0c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6f0c-122">Authorization</span></span>|<span data-ttu-id="a6f0c-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a6f0c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6f0c-124">接受</span><span class="sxs-lookup"><span data-stu-id="a6f0c-124">Accept</span></span>|<span data-ttu-id="a6f0c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a6f0c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6f0c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a6f0c-126">Request body</span></span>
<span data-ttu-id="a6f0c-127">在请求正文中, 提供 iosEduDeviceConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a6f0c-127">In the request body, supply a JSON representation for the iosEduDeviceConfiguration object.</span></span>

<span data-ttu-id="a6f0c-128">下表显示创建 iosEduDeviceConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a6f0c-128">The following table shows the properties that are required when you create the iosEduDeviceConfiguration.</span></span>

|<span data-ttu-id="a6f0c-129">属性</span><span class="sxs-lookup"><span data-stu-id="a6f0c-129">Property</span></span>|<span data-ttu-id="a6f0c-130">类型</span><span class="sxs-lookup"><span data-stu-id="a6f0c-130">Type</span></span>|<span data-ttu-id="a6f0c-131">说明</span><span class="sxs-lookup"><span data-stu-id="a6f0c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6f0c-132">id</span><span class="sxs-lookup"><span data-stu-id="a6f0c-132">id</span></span>|<span data-ttu-id="a6f0c-133">String</span><span class="sxs-lookup"><span data-stu-id="a6f0c-133">String</span></span>|<span data-ttu-id="a6f0c-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a6f0c-134">Key of the entity.</span></span> <span data-ttu-id="a6f0c-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6f0c-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6f0c-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a6f0c-136">lastModifiedDateTime</span></span>|<span data-ttu-id="a6f0c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6f0c-137">DateTimeOffset</span></span>|<span data-ttu-id="a6f0c-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a6f0c-138">DateTime the object was last modified.</span></span> <span data-ttu-id="a6f0c-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6f0c-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6f0c-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a6f0c-140">roleScopeTagIds</span></span>|<span data-ttu-id="a6f0c-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="a6f0c-141">String collection</span></span>|<span data-ttu-id="a6f0c-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="a6f0c-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a6f0c-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6f0c-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6f0c-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a6f0c-144">supportsScopeTags</span></span>|<span data-ttu-id="a6f0c-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="a6f0c-145">Boolean</span></span>|<span data-ttu-id="a6f0c-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="a6f0c-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a6f0c-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="a6f0c-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a6f0c-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="a6f0c-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a6f0c-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="a6f0c-149">This property is read-only.</span></span> <span data-ttu-id="a6f0c-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6f0c-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6f0c-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a6f0c-151">createdDateTime</span></span>|<span data-ttu-id="a6f0c-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6f0c-152">DateTimeOffset</span></span>|<span data-ttu-id="a6f0c-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a6f0c-153">DateTime the object was created.</span></span> <span data-ttu-id="a6f0c-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6f0c-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6f0c-155">description</span><span class="sxs-lookup"><span data-stu-id="a6f0c-155">description</span></span>|<span data-ttu-id="a6f0c-156">String</span><span class="sxs-lookup"><span data-stu-id="a6f0c-156">String</span></span>|<span data-ttu-id="a6f0c-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="a6f0c-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a6f0c-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6f0c-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6f0c-159">displayName</span><span class="sxs-lookup"><span data-stu-id="a6f0c-159">displayName</span></span>|<span data-ttu-id="a6f0c-160">String</span><span class="sxs-lookup"><span data-stu-id="a6f0c-160">String</span></span>|<span data-ttu-id="a6f0c-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="a6f0c-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a6f0c-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6f0c-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6f0c-163">version</span><span class="sxs-lookup"><span data-stu-id="a6f0c-163">version</span></span>|<span data-ttu-id="a6f0c-164">Int32</span><span class="sxs-lookup"><span data-stu-id="a6f0c-164">Int32</span></span>|<span data-ttu-id="a6f0c-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="a6f0c-165">Version of the device configuration.</span></span> <span data-ttu-id="a6f0c-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6f0c-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6f0c-167">teacherCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="a6f0c-167">teacherCertificateSettings</span></span>|[<span data-ttu-id="a6f0c-168">iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="a6f0c-168">iosEduCertificateSettings</span></span>](../resources/intune-deviceconfig-ioseducertificatesettings.md)|<span data-ttu-id="a6f0c-169">教师的受信任的根证书和 PFX 证书</span><span class="sxs-lookup"><span data-stu-id="a6f0c-169">The Trusted Root and PFX certificates for Teacher</span></span>|
|<span data-ttu-id="a6f0c-170">studentCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="a6f0c-170">studentCertificateSettings</span></span>|[<span data-ttu-id="a6f0c-171">iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="a6f0c-171">iosEduCertificateSettings</span></span>](../resources/intune-deviceconfig-ioseducertificatesettings.md)|<span data-ttu-id="a6f0c-172">学生的受信任的根证书和 PFX 证书</span><span class="sxs-lookup"><span data-stu-id="a6f0c-172">The Trusted Root and PFX certificates for Student</span></span>|
|<span data-ttu-id="a6f0c-173">deviceCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="a6f0c-173">deviceCertificateSettings</span></span>|[<span data-ttu-id="a6f0c-174">iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="a6f0c-174">iosEduCertificateSettings</span></span>](../resources/intune-deviceconfig-ioseducertificatesettings.md)|<span data-ttu-id="a6f0c-175">设备的受信任的根证书和 PFX 证书</span><span class="sxs-lookup"><span data-stu-id="a6f0c-175">The Trusted Root and PFX certificates for Device</span></span>|



## <a name="response"></a><span data-ttu-id="a6f0c-176">响应</span><span class="sxs-lookup"><span data-stu-id="a6f0c-176">Response</span></span>
<span data-ttu-id="a6f0c-177">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a6f0c-177">If successful, this method returns a `201 Created` response code and a [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6f0c-178">示例</span><span class="sxs-lookup"><span data-stu-id="a6f0c-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="a6f0c-179">请求</span><span class="sxs-lookup"><span data-stu-id="a6f0c-179">Request</span></span>
<span data-ttu-id="a6f0c-180">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a6f0c-180">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1910

{
  "@odata.type": "#microsoft.graph.iosEduDeviceConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "teacherCertificateSettings": {
    "@odata.type": "microsoft.graph.iosEduCertificateSettings",
    "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
    "certFileName": "Cert File Name value",
    "certificationAuthority": "Certification Authority value",
    "certificationAuthorityName": "Certification Authority Name value",
    "certificateTemplateName": "Certificate Template Name value",
    "renewalThresholdPercentage": 10,
    "certificateValidityPeriodValue": 14,
    "certificateValidityPeriodScale": "months"
  },
  "studentCertificateSettings": {
    "@odata.type": "microsoft.graph.iosEduCertificateSettings",
    "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
    "certFileName": "Cert File Name value",
    "certificationAuthority": "Certification Authority value",
    "certificationAuthorityName": "Certification Authority Name value",
    "certificateTemplateName": "Certificate Template Name value",
    "renewalThresholdPercentage": 10,
    "certificateValidityPeriodValue": 14,
    "certificateValidityPeriodScale": "months"
  },
  "deviceCertificateSettings": {
    "@odata.type": "microsoft.graph.iosEduCertificateSettings",
    "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
    "certFileName": "Cert File Name value",
    "certificationAuthority": "Certification Authority value",
    "certificationAuthorityName": "Certification Authority Name value",
    "certificateTemplateName": "Certificate Template Name value",
    "renewalThresholdPercentage": 10,
    "certificateValidityPeriodValue": 14,
    "certificateValidityPeriodScale": "months"
  }
}
```

### <a name="response"></a><span data-ttu-id="a6f0c-181">响应</span><span class="sxs-lookup"><span data-stu-id="a6f0c-181">Response</span></span>
<span data-ttu-id="a6f0c-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a6f0c-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2082

{
  "@odata.type": "#microsoft.graph.iosEduDeviceConfiguration",
  "id": "4c5df9b6-f9b6-4c5d-b6f9-5d4cb6f95d4c",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "teacherCertificateSettings": {
    "@odata.type": "microsoft.graph.iosEduCertificateSettings",
    "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
    "certFileName": "Cert File Name value",
    "certificationAuthority": "Certification Authority value",
    "certificationAuthorityName": "Certification Authority Name value",
    "certificateTemplateName": "Certificate Template Name value",
    "renewalThresholdPercentage": 10,
    "certificateValidityPeriodValue": 14,
    "certificateValidityPeriodScale": "months"
  },
  "studentCertificateSettings": {
    "@odata.type": "microsoft.graph.iosEduCertificateSettings",
    "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
    "certFileName": "Cert File Name value",
    "certificationAuthority": "Certification Authority value",
    "certificationAuthorityName": "Certification Authority Name value",
    "certificateTemplateName": "Certificate Template Name value",
    "renewalThresholdPercentage": 10,
    "certificateValidityPeriodValue": 14,
    "certificateValidityPeriodScale": "months"
  },
  "deviceCertificateSettings": {
    "@odata.type": "microsoft.graph.iosEduCertificateSettings",
    "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
    "certFileName": "Cert File Name value",
    "certificationAuthority": "Certification Authority value",
    "certificationAuthorityName": "Certification Authority Name value",
    "certificateTemplateName": "Certificate Template Name value",
    "renewalThresholdPercentage": 10,
    "certificateValidityPeriodValue": 14,
    "certificateValidityPeriodScale": "months"
  }
}
```




