---
title: 创建 managedDeviceCertificateState
description: 创建新的 managedDeviceCertificateState 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0b48550d3cea0fef3e57821f0ef89a75bdcc412a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945403"
---
# <a name="create-manageddevicecertificatestate"></a><span data-ttu-id="e0184-103">创建 managedDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="e0184-103">Create managedDeviceCertificateState</span></span>

> <span data-ttu-id="e0184-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e0184-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e0184-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e0184-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e0184-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e0184-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e0184-107">创建新的[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e0184-107">Create a new [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e0184-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e0184-108">Prerequisites</span></span>
<span data-ttu-id="e0184-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="e0184-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0184-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e0184-111">Permission type</span></span>|<span data-ttu-id="e0184-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e0184-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e0184-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e0184-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e0184-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0184-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e0184-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e0184-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0184-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e0184-116">Not supported.</span></span>|
|<span data-ttu-id="e0184-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e0184-117">Application</span></span>|<span data-ttu-id="e0184-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="e0184-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0184-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e0184-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="e0184-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e0184-120">Request headers</span></span>
|<span data-ttu-id="e0184-121">标头</span><span class="sxs-lookup"><span data-stu-id="e0184-121">Header</span></span>|<span data-ttu-id="e0184-122">值</span><span class="sxs-lookup"><span data-stu-id="e0184-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e0184-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0184-123">Authorization</span></span>|<span data-ttu-id="e0184-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e0184-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e0184-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e0184-125">Accept</span></span>|<span data-ttu-id="e0184-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e0184-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0184-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e0184-127">Request body</span></span>
<span data-ttu-id="e0184-128">在请求正文中，提供 managedDeviceCertificateState 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e0184-128">In the request body, supply a JSON representation for the managedDeviceCertificateState object.</span></span>

<span data-ttu-id="e0184-129">下表显示时创建 managedDeviceCertificateState 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e0184-129">The following table shows the properties that are required when you create the managedDeviceCertificateState.</span></span>

|<span data-ttu-id="e0184-130">属性</span><span class="sxs-lookup"><span data-stu-id="e0184-130">Property</span></span>|<span data-ttu-id="e0184-131">类型</span><span class="sxs-lookup"><span data-stu-id="e0184-131">Type</span></span>|<span data-ttu-id="e0184-132">说明</span><span class="sxs-lookup"><span data-stu-id="e0184-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0184-133">id</span><span class="sxs-lookup"><span data-stu-id="e0184-133">id</span></span>|<span data-ttu-id="e0184-134">String</span><span class="sxs-lookup"><span data-stu-id="e0184-134">String</span></span>|<span data-ttu-id="e0184-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e0184-135">Key of the entity.</span></span>|
|<span data-ttu-id="e0184-136">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="e0184-136">devicePlatform</span></span>|[<span data-ttu-id="e0184-137">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="e0184-137">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="e0184-138">设备平台。</span><span class="sxs-lookup"><span data-stu-id="e0184-138">Device platform.</span></span> <span data-ttu-id="e0184-139">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`。</span><span class="sxs-lookup"><span data-stu-id="e0184-139">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|
|<span data-ttu-id="e0184-140">certificateKeyUsage</span><span class="sxs-lookup"><span data-stu-id="e0184-140">certificateKeyUsage</span></span>|[<span data-ttu-id="e0184-141">keyUsages</span><span class="sxs-lookup"><span data-stu-id="e0184-141">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="e0184-142">密钥用法。</span><span class="sxs-lookup"><span data-stu-id="e0184-142">Key usage.</span></span> <span data-ttu-id="e0184-143">可取值为：`keyEncipherment`、`digitalSignature`。</span><span class="sxs-lookup"><span data-stu-id="e0184-143">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="e0184-144">certificateValidityPeriodUnits</span><span class="sxs-lookup"><span data-stu-id="e0184-144">certificateValidityPeriodUnits</span></span>|[<span data-ttu-id="e0184-145">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="e0184-145">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="e0184-146">有效期单位。</span><span class="sxs-lookup"><span data-stu-id="e0184-146">Validity period units.</span></span> <span data-ttu-id="e0184-147">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="e0184-147">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="e0184-148">certificateIssuanceState</span><span class="sxs-lookup"><span data-stu-id="e0184-148">certificateIssuanceState</span></span>|[<span data-ttu-id="e0184-149">certificateIssuanceStates</span><span class="sxs-lookup"><span data-stu-id="e0184-149">certificateIssuanceStates</span></span>](../resources/intune-deviceconfig-certificateissuancestates.md)|<span data-ttu-id="e0184-150">发布状态。</span><span class="sxs-lookup"><span data-stu-id="e0184-150">Issuance State.</span></span> <span data-ttu-id="e0184-151">可能的值为： `unknown`， `challengeIssued`， `challengeIssueFailed`， `requestCreationFailed`， `requestSubmitFailed`， `challengeValidationSucceeded`， `challengeValidationFailed`， `issueFailed`， `issuePending`， `issued`， `responseProcessingFailed`， `responsePending`， `enrollmentSucceeded`， `enrollmentNotNeeded`， `revoked`， `removedFromCollection`， `renewVerified`， `installFailed`， `installed`, `deleteFailed`, `deleted`, `renewalRequested`, `requested`.</span><span class="sxs-lookup"><span data-stu-id="e0184-151">Possible values are: `unknown`, `challengeIssued`, `challengeIssueFailed`, `requestCreationFailed`, `requestSubmitFailed`, `challengeValidationSucceeded`, `challengeValidationFailed`, `issueFailed`, `issuePending`, `issued`, `responseProcessingFailed`, `responsePending`, `enrollmentSucceeded`, `enrollmentNotNeeded`, `revoked`, `removedFromCollection`, `renewVerified`, `installFailed`, `installed`, `deleteFailed`, `deleted`, `renewalRequested`, `requested`.</span></span>|
|<span data-ttu-id="e0184-152">certificateKeyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="e0184-152">certificateKeyStorageProvider</span></span>|[<span data-ttu-id="e0184-153">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="e0184-153">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="e0184-154">密钥存储提供程序。</span><span class="sxs-lookup"><span data-stu-id="e0184-154">Key Storage Provider.</span></span> <span data-ttu-id="e0184-155">可取值为：`useTpmKspOtherwiseUseSoftwareKsp`、`useTpmKspOtherwiseFail`、`usePassportForWorkKspOtherwiseFail`、`useSoftwareKsp`。</span><span class="sxs-lookup"><span data-stu-id="e0184-155">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="e0184-156">certificateSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="e0184-156">certificateSubjectNameFormat</span></span>|[<span data-ttu-id="e0184-157">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="e0184-157">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="e0184-158">使用者名称格式。</span><span class="sxs-lookup"><span data-stu-id="e0184-158">Subject name format.</span></span> <span data-ttu-id="e0184-159">可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。</span><span class="sxs-lookup"><span data-stu-id="e0184-159">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="e0184-160">certificateSubjectAlternativeNameFormat</span><span class="sxs-lookup"><span data-stu-id="e0184-160">certificateSubjectAlternativeNameFormat</span></span>|[<span data-ttu-id="e0184-161">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="e0184-161">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="e0184-162">使用者替代名称格式。</span><span class="sxs-lookup"><span data-stu-id="e0184-162">Subject alternative name format.</span></span> <span data-ttu-id="e0184-163">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="e0184-163">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="e0184-164">certificateRevokeStatus</span><span class="sxs-lookup"><span data-stu-id="e0184-164">certificateRevokeStatus</span></span>|[<span data-ttu-id="e0184-165">certificateRevocationStatus</span><span class="sxs-lookup"><span data-stu-id="e0184-165">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="e0184-166">吊销状态。</span><span class="sxs-lookup"><span data-stu-id="e0184-166">Revoke status.</span></span> <span data-ttu-id="e0184-167">可取值为：`none`、`pending`、`issued`、`failed`、`revoked`。</span><span class="sxs-lookup"><span data-stu-id="e0184-167">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="e0184-168">certificateProfileDisplayName</span><span class="sxs-lookup"><span data-stu-id="e0184-168">certificateProfileDisplayName</span></span>|<span data-ttu-id="e0184-169">字符串</span><span class="sxs-lookup"><span data-stu-id="e0184-169">String</span></span>|<span data-ttu-id="e0184-170">证书配置文件的显示名称</span><span class="sxs-lookup"><span data-stu-id="e0184-170">Certificate profile display name</span></span>|
|<span data-ttu-id="e0184-171">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="e0184-171">deviceDisplayName</span></span>|<span data-ttu-id="e0184-172">String</span><span class="sxs-lookup"><span data-stu-id="e0184-172">String</span></span>|<span data-ttu-id="e0184-173">设备显示名称</span><span class="sxs-lookup"><span data-stu-id="e0184-173">Device display name</span></span>|
|<span data-ttu-id="e0184-174">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="e0184-174">userDisplayName</span></span>|<span data-ttu-id="e0184-175">String</span><span class="sxs-lookup"><span data-stu-id="e0184-175">String</span></span>|<span data-ttu-id="e0184-176">用户显示名称</span><span class="sxs-lookup"><span data-stu-id="e0184-176">User display name</span></span>|
|<span data-ttu-id="e0184-177">certificateExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="e0184-177">certificateExpirationDateTime</span></span>|<span data-ttu-id="e0184-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0184-178">DateTimeOffset</span></span>|<span data-ttu-id="e0184-179">证书到期日期</span><span class="sxs-lookup"><span data-stu-id="e0184-179">Certificate expiry date</span></span>|
|<span data-ttu-id="e0184-180">certificateLastIssuanceStateChangedDateTime</span><span class="sxs-lookup"><span data-stu-id="e0184-180">certificateLastIssuanceStateChangedDateTime</span></span>|<span data-ttu-id="e0184-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0184-181">DateTimeOffset</span></span>|<span data-ttu-id="e0184-182">最后一个证书颁发状态更改</span><span class="sxs-lookup"><span data-stu-id="e0184-182">Last certificate issuance state change</span></span>|
|<span data-ttu-id="e0184-183">lastCertificateStateChangeDateTime</span><span class="sxs-lookup"><span data-stu-id="e0184-183">lastCertificateStateChangeDateTime</span></span>|<span data-ttu-id="e0184-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0184-184">DateTimeOffset</span></span>|<span data-ttu-id="e0184-185">最后一个证书颁发状态更改</span><span class="sxs-lookup"><span data-stu-id="e0184-185">Last certificate issuance state change</span></span>|
|<span data-ttu-id="e0184-186">certificateIssuer</span><span class="sxs-lookup"><span data-stu-id="e0184-186">certificateIssuer</span></span>|<span data-ttu-id="e0184-187">字符串</span><span class="sxs-lookup"><span data-stu-id="e0184-187">String</span></span>|<span data-ttu-id="e0184-188">颁发者</span><span class="sxs-lookup"><span data-stu-id="e0184-188">Issuer</span></span>|
|<span data-ttu-id="e0184-189">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="e0184-189">certificateThumbprint</span></span>|<span data-ttu-id="e0184-190">字符串</span><span class="sxs-lookup"><span data-stu-id="e0184-190">String</span></span>|<span data-ttu-id="e0184-191">指纹</span><span class="sxs-lookup"><span data-stu-id="e0184-191">Thumbprint</span></span>|
|<span data-ttu-id="e0184-192">certificateSerialNumber</span><span class="sxs-lookup"><span data-stu-id="e0184-192">certificateSerialNumber</span></span>|<span data-ttu-id="e0184-193">字符串</span><span class="sxs-lookup"><span data-stu-id="e0184-193">String</span></span>|<span data-ttu-id="e0184-194">序列号</span><span class="sxs-lookup"><span data-stu-id="e0184-194">Serial number</span></span>|
|<span data-ttu-id="e0184-195">certificateKeyLength</span><span class="sxs-lookup"><span data-stu-id="e0184-195">certificateKeyLength</span></span>|<span data-ttu-id="e0184-196">Int32</span><span class="sxs-lookup"><span data-stu-id="e0184-196">Int32</span></span>|<span data-ttu-id="e0184-197">密钥长度</span><span class="sxs-lookup"><span data-stu-id="e0184-197">Key length</span></span>|
|<span data-ttu-id="e0184-198">certificateEnhancedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="e0184-198">certificateEnhancedKeyUsage</span></span>|<span data-ttu-id="e0184-199">字符串</span><span class="sxs-lookup"><span data-stu-id="e0184-199">String</span></span>|<span data-ttu-id="e0184-200">扩展的密钥用法</span><span class="sxs-lookup"><span data-stu-id="e0184-200">Extended key usage</span></span>|
|<span data-ttu-id="e0184-201">certificateValidityPeriod</span><span class="sxs-lookup"><span data-stu-id="e0184-201">certificateValidityPeriod</span></span>|<span data-ttu-id="e0184-202">Int32</span><span class="sxs-lookup"><span data-stu-id="e0184-202">Int32</span></span>|<span data-ttu-id="e0184-203">有效期</span><span class="sxs-lookup"><span data-stu-id="e0184-203">Validity period</span></span>|
|<span data-ttu-id="e0184-204">certificateSubjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="e0184-204">certificateSubjectNameFormatString</span></span>|<span data-ttu-id="e0184-205">字符串</span><span class="sxs-lookup"><span data-stu-id="e0184-205">String</span></span>|<span data-ttu-id="e0184-206">自定义主题名称格式的使用者名称格式字符串</span><span class="sxs-lookup"><span data-stu-id="e0184-206">Subject name format string for custom subject name formats</span></span>|
|<span data-ttu-id="e0184-207">certificateSubjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="e0184-207">certificateSubjectAlternativeNameFormatString</span></span>|<span data-ttu-id="e0184-208">字符串</span><span class="sxs-lookup"><span data-stu-id="e0184-208">String</span></span>|<span data-ttu-id="e0184-209">自定义格式的使用者替代名称格式字符串</span><span class="sxs-lookup"><span data-stu-id="e0184-209">Subject alternative name format string for custom formats</span></span>|
|<span data-ttu-id="e0184-210">certificateIssuanceDateTime</span><span class="sxs-lookup"><span data-stu-id="e0184-210">certificateIssuanceDateTime</span></span>|<span data-ttu-id="e0184-211">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0184-211">DateTimeOffset</span></span>|<span data-ttu-id="e0184-212">发布日期</span><span class="sxs-lookup"><span data-stu-id="e0184-212">Issuance date</span></span>|
|<span data-ttu-id="e0184-213">certificateErrorCode</span><span class="sxs-lookup"><span data-stu-id="e0184-213">certificateErrorCode</span></span>|<span data-ttu-id="e0184-214">Int32</span><span class="sxs-lookup"><span data-stu-id="e0184-214">Int32</span></span>|<span data-ttu-id="e0184-215">错误代码</span><span class="sxs-lookup"><span data-stu-id="e0184-215">Error code</span></span>|



## <a name="response"></a><span data-ttu-id="e0184-216">响应</span><span class="sxs-lookup"><span data-stu-id="e0184-216">Response</span></span>
<span data-ttu-id="e0184-217">如果成功，此方法返回`201 Created`响应代码和响应正文中的[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e0184-217">If successful, this method returns a `201 Created` response code and a [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0184-218">示例</span><span class="sxs-lookup"><span data-stu-id="e0184-218">Example</span></span>
### <a name="request"></a><span data-ttu-id="e0184-219">请求</span><span class="sxs-lookup"><span data-stu-id="e0184-219">Request</span></span>
<span data-ttu-id="e0184-220">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e0184-220">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e0184-221">响应</span><span class="sxs-lookup"><span data-stu-id="e0184-221">Response</span></span>
<span data-ttu-id="e0184-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e0184-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





