---
title: 创建 managedDeviceCertificateState
description: 创建新的 managedDeviceCertificateState 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3510ca1d4f4d593ea0bb396d5fe34c56cf2ac5f5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32518301"
---
# <a name="create-manageddevicecertificatestate"></a><span data-ttu-id="32a0e-103">创建 managedDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="32a0e-103">Create managedDeviceCertificateState</span></span>

> <span data-ttu-id="32a0e-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="32a0e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="32a0e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="32a0e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32a0e-106">创建新的[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="32a0e-106">Create a new [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="32a0e-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="32a0e-107">Prerequisites</span></span>
<span data-ttu-id="32a0e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="32a0e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32a0e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="32a0e-110">Permission type</span></span>|<span data-ttu-id="32a0e-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="32a0e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32a0e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="32a0e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="32a0e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32a0e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="32a0e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="32a0e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32a0e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="32a0e-115">Not supported.</span></span>|
|<span data-ttu-id="32a0e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="32a0e-116">Application</span></span>|<span data-ttu-id="32a0e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="32a0e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="32a0e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="32a0e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidPkcsCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidScepCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosImportedPFXCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSImportedPFXCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidImportedPFXCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileScepCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkImportedPFXCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkPkcsCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkScepCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10PkcsCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10ImportedPFXCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windowsPhone81ImportedPFXCertificateProfile/managedDeviceCertificateStates
```

## <a name="request-headers"></a><span data-ttu-id="32a0e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="32a0e-119">Request headers</span></span>
|<span data-ttu-id="32a0e-120">标头</span><span class="sxs-lookup"><span data-stu-id="32a0e-120">Header</span></span>|<span data-ttu-id="32a0e-121">值</span><span class="sxs-lookup"><span data-stu-id="32a0e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="32a0e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="32a0e-122">Authorization</span></span>|<span data-ttu-id="32a0e-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="32a0e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="32a0e-124">接受</span><span class="sxs-lookup"><span data-stu-id="32a0e-124">Accept</span></span>|<span data-ttu-id="32a0e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="32a0e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="32a0e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="32a0e-126">Request body</span></span>
<span data-ttu-id="32a0e-127">在请求正文中, 提供 managedDeviceCertificateState 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="32a0e-127">In the request body, supply a JSON representation for the managedDeviceCertificateState object.</span></span>

<span data-ttu-id="32a0e-128">下表显示创建 managedDeviceCertificateState 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="32a0e-128">The following table shows the properties that are required when you create the managedDeviceCertificateState.</span></span>

|<span data-ttu-id="32a0e-129">属性</span><span class="sxs-lookup"><span data-stu-id="32a0e-129">Property</span></span>|<span data-ttu-id="32a0e-130">类型</span><span class="sxs-lookup"><span data-stu-id="32a0e-130">Type</span></span>|<span data-ttu-id="32a0e-131">说明</span><span class="sxs-lookup"><span data-stu-id="32a0e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32a0e-132">id</span><span class="sxs-lookup"><span data-stu-id="32a0e-132">id</span></span>|<span data-ttu-id="32a0e-133">String</span><span class="sxs-lookup"><span data-stu-id="32a0e-133">String</span></span>|<span data-ttu-id="32a0e-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="32a0e-134">Key of the entity.</span></span>|
|<span data-ttu-id="32a0e-135">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="32a0e-135">devicePlatform</span></span>|[<span data-ttu-id="32a0e-136">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="32a0e-136">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="32a0e-137">设备平台。</span><span class="sxs-lookup"><span data-stu-id="32a0e-137">Device platform.</span></span> <span data-ttu-id="32a0e-138">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`。</span><span class="sxs-lookup"><span data-stu-id="32a0e-138">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|
|<span data-ttu-id="32a0e-139">certificateKeyUsage</span><span class="sxs-lookup"><span data-stu-id="32a0e-139">certificateKeyUsage</span></span>|[<span data-ttu-id="32a0e-140">keyUsages</span><span class="sxs-lookup"><span data-stu-id="32a0e-140">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="32a0e-141">密钥用法。</span><span class="sxs-lookup"><span data-stu-id="32a0e-141">Key usage.</span></span> <span data-ttu-id="32a0e-142">可取值为：`keyEncipherment`、`digitalSignature`。</span><span class="sxs-lookup"><span data-stu-id="32a0e-142">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="32a0e-143">certificateValidityPeriodUnits</span><span class="sxs-lookup"><span data-stu-id="32a0e-143">certificateValidityPeriodUnits</span></span>|[<span data-ttu-id="32a0e-144">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="32a0e-144">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="32a0e-145">有效期单位。</span><span class="sxs-lookup"><span data-stu-id="32a0e-145">Validity period units.</span></span> <span data-ttu-id="32a0e-146">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="32a0e-146">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="32a0e-147">certificateIssuanceState</span><span class="sxs-lookup"><span data-stu-id="32a0e-147">certificateIssuanceState</span></span>|[<span data-ttu-id="32a0e-148">certificateIssuanceStates</span><span class="sxs-lookup"><span data-stu-id="32a0e-148">certificateIssuanceStates</span></span>](../resources/intune-deviceconfig-certificateissuancestates.md)|<span data-ttu-id="32a0e-149">颁发状态。</span><span class="sxs-lookup"><span data-stu-id="32a0e-149">Issuance State.</span></span> <span data-ttu-id="32a0e-150">可能的值为`unknown`: `challengeIssued`、 `challengeIssueFailed`、 `requestCreationFailed` `requestSubmitFailed` `challengeValidationSucceeded` `challengeValidationFailed` `issueFailed` `issuePending` `issued` `responseProcessingFailed` `responsePending` `enrollmentSucceeded`、、、、、、、、、、、、、、、、 `enrollmentNotNeeded` `revoked` `removedFromCollection` `renewVerified` `installFailed` `installed`, `deleteFailed`, `deleted`, `renewalRequested`, `requested`.</span><span class="sxs-lookup"><span data-stu-id="32a0e-150">Possible values are: `unknown`, `challengeIssued`, `challengeIssueFailed`, `requestCreationFailed`, `requestSubmitFailed`, `challengeValidationSucceeded`, `challengeValidationFailed`, `issueFailed`, `issuePending`, `issued`, `responseProcessingFailed`, `responsePending`, `enrollmentSucceeded`, `enrollmentNotNeeded`, `revoked`, `removedFromCollection`, `renewVerified`, `installFailed`, `installed`, `deleteFailed`, `deleted`, `renewalRequested`, `requested`.</span></span>|
|<span data-ttu-id="32a0e-151">certificateKeyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="32a0e-151">certificateKeyStorageProvider</span></span>|[<span data-ttu-id="32a0e-152">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="32a0e-152">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="32a0e-153">密钥存储提供程序。</span><span class="sxs-lookup"><span data-stu-id="32a0e-153">Key Storage Provider.</span></span> <span data-ttu-id="32a0e-154">可取值为：`useTpmKspOtherwiseUseSoftwareKsp`、`useTpmKspOtherwiseFail`、`usePassportForWorkKspOtherwiseFail`、`useSoftwareKsp`。</span><span class="sxs-lookup"><span data-stu-id="32a0e-154">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="32a0e-155">certificateSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="32a0e-155">certificateSubjectNameFormat</span></span>|[<span data-ttu-id="32a0e-156">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="32a0e-156">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="32a0e-157">使用者名称格式。</span><span class="sxs-lookup"><span data-stu-id="32a0e-157">Subject name format.</span></span> <span data-ttu-id="32a0e-158">可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。</span><span class="sxs-lookup"><span data-stu-id="32a0e-158">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="32a0e-159">certificateSubjectAlternativeNameFormat</span><span class="sxs-lookup"><span data-stu-id="32a0e-159">certificateSubjectAlternativeNameFormat</span></span>|[<span data-ttu-id="32a0e-160">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="32a0e-160">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="32a0e-161">使用者可选名称格式。</span><span class="sxs-lookup"><span data-stu-id="32a0e-161">Subject alternative name format.</span></span> <span data-ttu-id="32a0e-162">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute` 或 `domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="32a0e-162">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="32a0e-163">certificateRevokeStatus</span><span class="sxs-lookup"><span data-stu-id="32a0e-163">certificateRevokeStatus</span></span>|[<span data-ttu-id="32a0e-164">certificateRevocationStatus</span><span class="sxs-lookup"><span data-stu-id="32a0e-164">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="32a0e-165">撤消状态。</span><span class="sxs-lookup"><span data-stu-id="32a0e-165">Revoke status.</span></span> <span data-ttu-id="32a0e-166">可取值为：`none`、`pending`、`issued`、`failed` 或 `revoked`。</span><span class="sxs-lookup"><span data-stu-id="32a0e-166">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="32a0e-167">certificateProfileDisplayName</span><span class="sxs-lookup"><span data-stu-id="32a0e-167">certificateProfileDisplayName</span></span>|<span data-ttu-id="32a0e-168">字符串</span><span class="sxs-lookup"><span data-stu-id="32a0e-168">String</span></span>|<span data-ttu-id="32a0e-169">证书配置文件显示名称</span><span class="sxs-lookup"><span data-stu-id="32a0e-169">Certificate profile display name</span></span>|
|<span data-ttu-id="32a0e-170">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="32a0e-170">deviceDisplayName</span></span>|<span data-ttu-id="32a0e-171">String</span><span class="sxs-lookup"><span data-stu-id="32a0e-171">String</span></span>|<span data-ttu-id="32a0e-172">设备显示名称</span><span class="sxs-lookup"><span data-stu-id="32a0e-172">Device display name</span></span>|
|<span data-ttu-id="32a0e-173">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="32a0e-173">userDisplayName</span></span>|<span data-ttu-id="32a0e-174">String</span><span class="sxs-lookup"><span data-stu-id="32a0e-174">String</span></span>|<span data-ttu-id="32a0e-175">用户显示名称</span><span class="sxs-lookup"><span data-stu-id="32a0e-175">User display name</span></span>|
|<span data-ttu-id="32a0e-176">certificateExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="32a0e-176">certificateExpirationDateTime</span></span>|<span data-ttu-id="32a0e-177">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32a0e-177">DateTimeOffset</span></span>|<span data-ttu-id="32a0e-178">证书到期日期</span><span class="sxs-lookup"><span data-stu-id="32a0e-178">Certificate expiry date</span></span>|
|<span data-ttu-id="32a0e-179">certificateLastIssuanceStateChangedDateTime</span><span class="sxs-lookup"><span data-stu-id="32a0e-179">certificateLastIssuanceStateChangedDateTime</span></span>|<span data-ttu-id="32a0e-180">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32a0e-180">DateTimeOffset</span></span>|<span data-ttu-id="32a0e-181">上次证书颁发状态更改</span><span class="sxs-lookup"><span data-stu-id="32a0e-181">Last certificate issuance state change</span></span>|
|<span data-ttu-id="32a0e-182">lastCertificateStateChangeDateTime</span><span class="sxs-lookup"><span data-stu-id="32a0e-182">lastCertificateStateChangeDateTime</span></span>|<span data-ttu-id="32a0e-183">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32a0e-183">DateTimeOffset</span></span>|<span data-ttu-id="32a0e-184">上次证书颁发状态更改</span><span class="sxs-lookup"><span data-stu-id="32a0e-184">Last certificate issuance state change</span></span>|
|<span data-ttu-id="32a0e-185">certificateIssuer</span><span class="sxs-lookup"><span data-stu-id="32a0e-185">certificateIssuer</span></span>|<span data-ttu-id="32a0e-186">字符串</span><span class="sxs-lookup"><span data-stu-id="32a0e-186">String</span></span>|<span data-ttu-id="32a0e-187">颁发者</span><span class="sxs-lookup"><span data-stu-id="32a0e-187">Issuer</span></span>|
|<span data-ttu-id="32a0e-188">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="32a0e-188">certificateThumbprint</span></span>|<span data-ttu-id="32a0e-189">字符串</span><span class="sxs-lookup"><span data-stu-id="32a0e-189">String</span></span>|<span data-ttu-id="32a0e-190">为</span><span class="sxs-lookup"><span data-stu-id="32a0e-190">Thumbprint</span></span>|
|<span data-ttu-id="32a0e-191">certificateSerialNumber</span><span class="sxs-lookup"><span data-stu-id="32a0e-191">certificateSerialNumber</span></span>|<span data-ttu-id="32a0e-192">字符串</span><span class="sxs-lookup"><span data-stu-id="32a0e-192">String</span></span>|<span data-ttu-id="32a0e-193">序列号</span><span class="sxs-lookup"><span data-stu-id="32a0e-193">Serial number</span></span>|
|<span data-ttu-id="32a0e-194">certificateKeyLength</span><span class="sxs-lookup"><span data-stu-id="32a0e-194">certificateKeyLength</span></span>|<span data-ttu-id="32a0e-195">Int32</span><span class="sxs-lookup"><span data-stu-id="32a0e-195">Int32</span></span>|<span data-ttu-id="32a0e-196">密钥长度</span><span class="sxs-lookup"><span data-stu-id="32a0e-196">Key length</span></span>|
|<span data-ttu-id="32a0e-197">certificateEnhancedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="32a0e-197">certificateEnhancedKeyUsage</span></span>|<span data-ttu-id="32a0e-198">字符串</span><span class="sxs-lookup"><span data-stu-id="32a0e-198">String</span></span>|<span data-ttu-id="32a0e-199">扩展密钥用法</span><span class="sxs-lookup"><span data-stu-id="32a0e-199">Extended key usage</span></span>|
|<span data-ttu-id="32a0e-200">certificateValidityPeriod</span><span class="sxs-lookup"><span data-stu-id="32a0e-200">certificateValidityPeriod</span></span>|<span data-ttu-id="32a0e-201">Int32</span><span class="sxs-lookup"><span data-stu-id="32a0e-201">Int32</span></span>|<span data-ttu-id="32a0e-202">有效期</span><span class="sxs-lookup"><span data-stu-id="32a0e-202">Validity period</span></span>|
|<span data-ttu-id="32a0e-203">certificateSubjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="32a0e-203">certificateSubjectNameFormatString</span></span>|<span data-ttu-id="32a0e-204">字符串</span><span class="sxs-lookup"><span data-stu-id="32a0e-204">String</span></span>|<span data-ttu-id="32a0e-205">自定义主题名称格式的主题名称格式字符串</span><span class="sxs-lookup"><span data-stu-id="32a0e-205">Subject name format string for custom subject name formats</span></span>|
|<span data-ttu-id="32a0e-206">certificateSubjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="32a0e-206">certificateSubjectAlternativeNameFormatString</span></span>|<span data-ttu-id="32a0e-207">字符串</span><span class="sxs-lookup"><span data-stu-id="32a0e-207">String</span></span>|<span data-ttu-id="32a0e-208">自定义格式的使用者可选名称格式字符串</span><span class="sxs-lookup"><span data-stu-id="32a0e-208">Subject alternative name format string for custom formats</span></span>|
|<span data-ttu-id="32a0e-209">certificateIssuanceDateTime</span><span class="sxs-lookup"><span data-stu-id="32a0e-209">certificateIssuanceDateTime</span></span>|<span data-ttu-id="32a0e-210">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32a0e-210">DateTimeOffset</span></span>|<span data-ttu-id="32a0e-211">颁发日期</span><span class="sxs-lookup"><span data-stu-id="32a0e-211">Issuance date</span></span>|
|<span data-ttu-id="32a0e-212">certificateErrorCode</span><span class="sxs-lookup"><span data-stu-id="32a0e-212">certificateErrorCode</span></span>|<span data-ttu-id="32a0e-213">Int32</span><span class="sxs-lookup"><span data-stu-id="32a0e-213">Int32</span></span>|<span data-ttu-id="32a0e-214">错误代码</span><span class="sxs-lookup"><span data-stu-id="32a0e-214">Error code</span></span>|



## <a name="response"></a><span data-ttu-id="32a0e-215">响应</span><span class="sxs-lookup"><span data-stu-id="32a0e-215">Response</span></span>
<span data-ttu-id="32a0e-216">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="32a0e-216">If successful, this method returns a `201 Created` response code and a [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32a0e-217">示例</span><span class="sxs-lookup"><span data-stu-id="32a0e-217">Example</span></span>

### <a name="request"></a><span data-ttu-id="32a0e-218">请求</span><span class="sxs-lookup"><span data-stu-id="32a0e-218">Request</span></span>
<span data-ttu-id="32a0e-219">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="32a0e-219">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates
Content-type: application/json
Content-length: 1517

{
  "@odata.type": "#microsoft.graph.managedDeviceCertificateState",
  "devicePlatform": "androidForWork",
  "certificateKeyUsage": "digitalSignature",
  "certificateValidityPeriodUnits": "months",
  "certificateIssuanceState": "challengeIssued",
  "certificateKeyStorageProvider": "useTpmKspOtherwiseFail",
  "certificateSubjectNameFormat": "commonNameIncludingEmail",
  "certificateSubjectAlternativeNameFormat": "emailAddress",
  "certificateRevokeStatus": "pending",
  "certificateProfileDisplayName": "Certificate Profile Display Name value",
  "deviceDisplayName": "Device Display Name value",
  "userDisplayName": "User Display Name value",
  "certificateExpirationDateTime": "2017-01-01T00:02:14.9489247-08:00",
  "certificateLastIssuanceStateChangedDateTime": "2017-01-01T00:00:27.7468732-08:00",
  "lastCertificateStateChangeDateTime": "2017-01-01T00:01:10.7144639-08:00",
  "certificateIssuer": "Certificate Issuer value",
  "certificateThumbprint": "Certificate Thumbprint value",
  "certificateSerialNumber": "Certificate Serial Number value",
  "certificateKeyLength": 4,
  "certificateEnhancedKeyUsage": "Certificate Enhanced Key Usage value",
  "certificateValidityPeriod": 9,
  "certificateSubjectNameFormatString": "Certificate Subject Name Format String value",
  "certificateSubjectAlternativeNameFormatString": "Certificate Subject Alternative Name Format String value",
  "certificateIssuanceDateTime": "2016-12-31T23:59:41.5044473-08:00",
  "certificateErrorCode": 4
}
```

### <a name="response"></a><span data-ttu-id="32a0e-220">响应</span><span class="sxs-lookup"><span data-stu-id="32a0e-220">Response</span></span>
<span data-ttu-id="32a0e-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="32a0e-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1566

{
  "@odata.type": "#microsoft.graph.managedDeviceCertificateState",
  "id": "d99bc884-c884-d99b-84c8-9bd984c89bd9",
  "devicePlatform": "androidForWork",
  "certificateKeyUsage": "digitalSignature",
  "certificateValidityPeriodUnits": "months",
  "certificateIssuanceState": "challengeIssued",
  "certificateKeyStorageProvider": "useTpmKspOtherwiseFail",
  "certificateSubjectNameFormat": "commonNameIncludingEmail",
  "certificateSubjectAlternativeNameFormat": "emailAddress",
  "certificateRevokeStatus": "pending",
  "certificateProfileDisplayName": "Certificate Profile Display Name value",
  "deviceDisplayName": "Device Display Name value",
  "userDisplayName": "User Display Name value",
  "certificateExpirationDateTime": "2017-01-01T00:02:14.9489247-08:00",
  "certificateLastIssuanceStateChangedDateTime": "2017-01-01T00:00:27.7468732-08:00",
  "lastCertificateStateChangeDateTime": "2017-01-01T00:01:10.7144639-08:00",
  "certificateIssuer": "Certificate Issuer value",
  "certificateThumbprint": "Certificate Thumbprint value",
  "certificateSerialNumber": "Certificate Serial Number value",
  "certificateKeyLength": 4,
  "certificateEnhancedKeyUsage": "Certificate Enhanced Key Usage value",
  "certificateValidityPeriod": 9,
  "certificateSubjectNameFormatString": "Certificate Subject Name Format String value",
  "certificateSubjectAlternativeNameFormatString": "Certificate Subject Alternative Name Format String value",
  "certificateIssuanceDateTime": "2016-12-31T23:59:41.5044473-08:00",
  "certificateErrorCode": 4
}
```





