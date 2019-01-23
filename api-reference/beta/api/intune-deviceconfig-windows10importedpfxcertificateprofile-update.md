---
title: 更新 windows10ImportedPFXCertificateProfile
description: 更新 windows10ImportedPFXCertificateProfile 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0a525c64bbf2e0210acb200488d7426b08b23052
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411818"
---
# <a name="update-windows10importedpfxcertificateprofile"></a><span data-ttu-id="a8d0f-103">更新 windows10ImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="a8d0f-103">Update windows10ImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="a8d0f-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="a8d0f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a8d0f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a8d0f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a8d0f-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a8d0f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8d0f-107">更新[windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a8d0f-107">Update the properties of a [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a8d0f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a8d0f-108">Prerequisites</span></span>
<span data-ttu-id="a8d0f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a8d0f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a8d0f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a8d0f-111">Permission type</span></span>|<span data-ttu-id="a8d0f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a8d0f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8d0f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a8d0f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a8d0f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8d0f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a8d0f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a8d0f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8d0f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a8d0f-116">Not supported.</span></span>|
|<span data-ttu-id="a8d0f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a8d0f-117">Application</span></span>|<span data-ttu-id="a8d0f-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="a8d0f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8d0f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a8d0f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a8d0f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a8d0f-120">Request headers</span></span>
|<span data-ttu-id="a8d0f-121">标头</span><span class="sxs-lookup"><span data-stu-id="a8d0f-121">Header</span></span>|<span data-ttu-id="a8d0f-122">值</span><span class="sxs-lookup"><span data-stu-id="a8d0f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a8d0f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8d0f-123">Authorization</span></span>|<span data-ttu-id="a8d0f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a8d0f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a8d0f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a8d0f-125">Accept</span></span>|<span data-ttu-id="a8d0f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a8d0f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8d0f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a8d0f-127">Request body</span></span>
<span data-ttu-id="a8d0f-128">在请求正文中，提供[windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a8d0f-128">In the request body, supply a JSON representation for the [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) object.</span></span>

<span data-ttu-id="a8d0f-129">下表显示时创建[windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a8d0f-129">The following table shows the properties that are required when you create the [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md).</span></span>

|<span data-ttu-id="a8d0f-130">属性</span><span class="sxs-lookup"><span data-stu-id="a8d0f-130">Property</span></span>|<span data-ttu-id="a8d0f-131">类型</span><span class="sxs-lookup"><span data-stu-id="a8d0f-131">Type</span></span>|<span data-ttu-id="a8d0f-132">说明</span><span class="sxs-lookup"><span data-stu-id="a8d0f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8d0f-133">id</span><span class="sxs-lookup"><span data-stu-id="a8d0f-133">id</span></span>|<span data-ttu-id="a8d0f-134">String</span><span class="sxs-lookup"><span data-stu-id="a8d0f-134">String</span></span>|<span data-ttu-id="a8d0f-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a8d0f-135">Key of the entity.</span></span> <span data-ttu-id="a8d0f-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8d0f-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8d0f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a8d0f-137">lastModifiedDateTime</span></span>|<span data-ttu-id="a8d0f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8d0f-138">DateTimeOffset</span></span>|<span data-ttu-id="a8d0f-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a8d0f-139">DateTime the object was last modified.</span></span> <span data-ttu-id="a8d0f-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8d0f-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8d0f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a8d0f-141">roleScopeTagIds</span></span>|<span data-ttu-id="a8d0f-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="a8d0f-142">String collection</span></span>|<span data-ttu-id="a8d0f-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="a8d0f-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a8d0f-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8d0f-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8d0f-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a8d0f-145">supportsScopeTags</span></span>|<span data-ttu-id="a8d0f-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8d0f-146">Boolean</span></span>|<span data-ttu-id="a8d0f-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="a8d0f-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a8d0f-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="a8d0f-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a8d0f-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="a8d0f-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a8d0f-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="a8d0f-150">This property is read-only.</span></span> <span data-ttu-id="a8d0f-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8d0f-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8d0f-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a8d0f-152">createdDateTime</span></span>|<span data-ttu-id="a8d0f-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8d0f-153">DateTimeOffset</span></span>|<span data-ttu-id="a8d0f-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a8d0f-154">DateTime the object was created.</span></span> <span data-ttu-id="a8d0f-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8d0f-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8d0f-156">description</span><span class="sxs-lookup"><span data-stu-id="a8d0f-156">description</span></span>|<span data-ttu-id="a8d0f-157">String</span><span class="sxs-lookup"><span data-stu-id="a8d0f-157">String</span></span>|<span data-ttu-id="a8d0f-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="a8d0f-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a8d0f-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8d0f-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8d0f-160">displayName</span><span class="sxs-lookup"><span data-stu-id="a8d0f-160">displayName</span></span>|<span data-ttu-id="a8d0f-161">String</span><span class="sxs-lookup"><span data-stu-id="a8d0f-161">String</span></span>|<span data-ttu-id="a8d0f-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="a8d0f-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a8d0f-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8d0f-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8d0f-164">version</span><span class="sxs-lookup"><span data-stu-id="a8d0f-164">version</span></span>|<span data-ttu-id="a8d0f-165">Int32</span><span class="sxs-lookup"><span data-stu-id="a8d0f-165">Int32</span></span>|<span data-ttu-id="a8d0f-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="a8d0f-166">Version of the device configuration.</span></span> <span data-ttu-id="a8d0f-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8d0f-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8d0f-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="a8d0f-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="a8d0f-169">Int32</span><span class="sxs-lookup"><span data-stu-id="a8d0f-169">Int32</span></span>|<span data-ttu-id="a8d0f-170">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="a8d0f-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="a8d0f-171">有效值 1 到 99 继承自[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="a8d0f-171">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="a8d0f-172">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="a8d0f-172">keyStorageProvider</span></span>|[<span data-ttu-id="a8d0f-173">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="a8d0f-173">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="a8d0f-174">从[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)键存储提供程序 (KSP) 继承。</span><span class="sxs-lookup"><span data-stu-id="a8d0f-174">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="a8d0f-175">可取值为：`useTpmKspOtherwiseUseSoftwareKsp`、`useTpmKspOtherwiseFail`、`usePassportForWorkKspOtherwiseFail`、`useSoftwareKsp`。</span><span class="sxs-lookup"><span data-stu-id="a8d0f-175">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="a8d0f-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="a8d0f-176">subjectNameFormat</span></span>|[<span data-ttu-id="a8d0f-177">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="a8d0f-177">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="a8d0f-178">证书使用者名称格式继承自[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="a8d0f-178">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="a8d0f-179">可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。</span><span class="sxs-lookup"><span data-stu-id="a8d0f-179">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="a8d0f-180">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="a8d0f-180">subjectAlternativeNameType</span></span>|[<span data-ttu-id="a8d0f-181">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="a8d0f-181">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="a8d0f-182">证书使用者替代名称类型继承自[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="a8d0f-182">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="a8d0f-183">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="a8d0f-183">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="a8d0f-184">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="a8d0f-184">certificateValidityPeriodValue</span></span>|<span data-ttu-id="a8d0f-185">Int32</span><span class="sxs-lookup"><span data-stu-id="a8d0f-185">Int32</span></span>|<span data-ttu-id="a8d0f-186">证书有效性段继承自[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)值</span><span class="sxs-lookup"><span data-stu-id="a8d0f-186">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="a8d0f-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="a8d0f-187">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="a8d0f-188">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="a8d0f-188">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="a8d0f-189">证书有效性段继承自[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)的小数位数。</span><span class="sxs-lookup"><span data-stu-id="a8d0f-189">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="a8d0f-190">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="a8d0f-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="a8d0f-191">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="a8d0f-191">intendedPurpose</span></span>|[<span data-ttu-id="a8d0f-192">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="a8d0f-192">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="a8d0f-193">尚未编档。</span><span class="sxs-lookup"><span data-stu-id="a8d0f-193">Not yet documented.</span></span> <span data-ttu-id="a8d0f-194">可取值为：`unassigned`、`smimeEncryption`、`smimeSigning`、`vpn`、`wifi`。</span><span class="sxs-lookup"><span data-stu-id="a8d0f-194">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="a8d0f-195">响应</span><span class="sxs-lookup"><span data-stu-id="a8d0f-195">Response</span></span>
<span data-ttu-id="a8d0f-196">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a8d0f-196">If successful, this method returns a `200 OK` response code and an updated [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8d0f-197">示例</span><span class="sxs-lookup"><span data-stu-id="a8d0f-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="a8d0f-198">请求</span><span class="sxs-lookup"><span data-stu-id="a8d0f-198">Request</span></span>
<span data-ttu-id="a8d0f-199">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a8d0f-199">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 586

{
  "@odata.type": "#microsoft.graph.windows10ImportedPFXCertificateProfile",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "renewalThresholdPercentage": 10,
  "keyStorageProvider": "useTpmKspOtherwiseFail",
  "subjectNameFormat": "commonNameIncludingEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "intendedPurpose": "smimeEncryption"
}
```

### <a name="response"></a><span data-ttu-id="a8d0f-200">响应</span><span class="sxs-lookup"><span data-stu-id="a8d0f-200">Response</span></span>
<span data-ttu-id="a8d0f-p117">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a8d0f-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 758

{
  "@odata.type": "#microsoft.graph.windows10ImportedPFXCertificateProfile",
  "id": "b582514b-514b-b582-4b51-82b54b5182b5",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "renewalThresholdPercentage": 10,
  "keyStorageProvider": "useTpmKspOtherwiseFail",
  "subjectNameFormat": "commonNameIncludingEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "intendedPurpose": "smimeEncryption"
}
```




