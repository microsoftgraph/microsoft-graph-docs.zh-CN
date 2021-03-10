---
title: 更新 managedDeviceCertificateState
description: 更新 managedDeviceCertificateState 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b2634415308c24de1d0ac3b6723fa0547e82422c
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50626002"
---
# <a name="update-manageddevicecertificatestate"></a><span data-ttu-id="ed36e-103">更新 managedDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="ed36e-103">Update managedDeviceCertificateState</span></span>

<span data-ttu-id="ed36e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed36e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ed36e-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ed36e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ed36e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ed36e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed36e-107">更新 [managedDeviceCertificateState 对象](../resources/intune-deviceconfig-manageddevicecertificatestate.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="ed36e-107">Update the properties of a [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ed36e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ed36e-108">Prerequisites</span></span>
<span data-ttu-id="ed36e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ed36e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed36e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ed36e-111">Permission type</span></span>|<span data-ttu-id="ed36e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ed36e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed36e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ed36e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ed36e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed36e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ed36e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ed36e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed36e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ed36e-116">Not supported.</span></span>|
|<span data-ttu-id="ed36e-117">Application</span><span class="sxs-lookup"><span data-stu-id="ed36e-117">Application</span></span>|<span data-ttu-id="ed36e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed36e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed36e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ed36e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfilePkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10PkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10ImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windowsPhone81ImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="ed36e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ed36e-120">Request headers</span></span>
|<span data-ttu-id="ed36e-121">标头</span><span class="sxs-lookup"><span data-stu-id="ed36e-121">Header</span></span>|<span data-ttu-id="ed36e-122">值</span><span class="sxs-lookup"><span data-stu-id="ed36e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ed36e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed36e-123">Authorization</span></span>|<span data-ttu-id="ed36e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ed36e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ed36e-125">接受</span><span class="sxs-lookup"><span data-stu-id="ed36e-125">Accept</span></span>|<span data-ttu-id="ed36e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ed36e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed36e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ed36e-127">Request body</span></span>
<span data-ttu-id="ed36e-128">在请求正文中，提供 [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ed36e-128">In the request body, supply a JSON representation for the [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object.</span></span>

<span data-ttu-id="ed36e-129">下表显示创建 [managedDeviceCertificateState 时所需的属性](../resources/intune-deviceconfig-manageddevicecertificatestate.md)。</span><span class="sxs-lookup"><span data-stu-id="ed36e-129">The following table shows the properties that are required when you create the [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md).</span></span>

|<span data-ttu-id="ed36e-130">属性</span><span class="sxs-lookup"><span data-stu-id="ed36e-130">Property</span></span>|<span data-ttu-id="ed36e-131">类型</span><span class="sxs-lookup"><span data-stu-id="ed36e-131">Type</span></span>|<span data-ttu-id="ed36e-132">说明</span><span class="sxs-lookup"><span data-stu-id="ed36e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed36e-133">id</span><span class="sxs-lookup"><span data-stu-id="ed36e-133">id</span></span>|<span data-ttu-id="ed36e-134">String</span><span class="sxs-lookup"><span data-stu-id="ed36e-134">String</span></span>|<span data-ttu-id="ed36e-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ed36e-135">Key of the entity.</span></span>|
|<span data-ttu-id="ed36e-136">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="ed36e-136">devicePlatform</span></span>|[<span data-ttu-id="ed36e-137">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="ed36e-137">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="ed36e-138">设备平台。</span><span class="sxs-lookup"><span data-stu-id="ed36e-138">Device platform.</span></span> <span data-ttu-id="ed36e-139">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="ed36e-139">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="ed36e-140">certificateKeyUsage</span><span class="sxs-lookup"><span data-stu-id="ed36e-140">certificateKeyUsage</span></span>|[<span data-ttu-id="ed36e-141">keyUsages</span><span class="sxs-lookup"><span data-stu-id="ed36e-141">keyUsages</span></span>](../resources/intune-shared-keyusages.md)|<span data-ttu-id="ed36e-142">密钥用法。</span><span class="sxs-lookup"><span data-stu-id="ed36e-142">Key usage.</span></span> <span data-ttu-id="ed36e-143">可取值为：`keyEncipherment`、`digitalSignature`。</span><span class="sxs-lookup"><span data-stu-id="ed36e-143">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="ed36e-144">certificateValidityPeriodUnits</span><span class="sxs-lookup"><span data-stu-id="ed36e-144">certificateValidityPeriodUnits</span></span>|[<span data-ttu-id="ed36e-145">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="ed36e-145">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="ed36e-146">有效期单位。</span><span class="sxs-lookup"><span data-stu-id="ed36e-146">Validity period units.</span></span> <span data-ttu-id="ed36e-147">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="ed36e-147">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="ed36e-148">certificateIssuanceState</span><span class="sxs-lookup"><span data-stu-id="ed36e-148">certificateIssuanceState</span></span>|[<span data-ttu-id="ed36e-149">certificateIssuanceStates</span><span class="sxs-lookup"><span data-stu-id="ed36e-149">certificateIssuanceStates</span></span>](../resources/intune-deviceconfig-certificateissuancestates.md)|<span data-ttu-id="ed36e-150">颁发状态。</span><span class="sxs-lookup"><span data-stu-id="ed36e-150">Issuance State.</span></span> <span data-ttu-id="ed36e-151">可能的值是： `unknown` ， ， ， ， ， ， `challengeIssued` ， `challengeIssueFailed` `requestCreationFailed` `requestSubmitFailed` `challengeValidationSucceeded` `challengeValidationFailed` `issueFailed` `issuePending` `issued` `responseProcessingFailed` `responsePending` `enrollmentSucceeded` `enrollmentNotNeeded` `revoked` `removedFromCollection` `renewVerified` `installFailed` `installed` `deleteFailed` `deleted` `renewalRequested` `requested` 。</span><span class="sxs-lookup"><span data-stu-id="ed36e-151">Possible values are: `unknown`, `challengeIssued`, `challengeIssueFailed`, `requestCreationFailed`, `requestSubmitFailed`, `challengeValidationSucceeded`, `challengeValidationFailed`, `issueFailed`, `issuePending`, `issued`, `responseProcessingFailed`, `responsePending`, `enrollmentSucceeded`, `enrollmentNotNeeded`, `revoked`, `removedFromCollection`, `renewVerified`, `installFailed`, `installed`, `deleteFailed`, `deleted`, `renewalRequested`, `requested`.</span></span>|
|<span data-ttu-id="ed36e-152">certificateKeyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="ed36e-152">certificateKeyStorageProvider</span></span>|[<span data-ttu-id="ed36e-153">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="ed36e-153">keyStorageProviderOption</span></span>](../resources/intune-shared-keystorageprovideroption.md)|<span data-ttu-id="ed36e-154">密钥存储提供程序。</span><span class="sxs-lookup"><span data-stu-id="ed36e-154">Key Storage Provider.</span></span> <span data-ttu-id="ed36e-155">可取值为：`useTpmKspOtherwiseUseSoftwareKsp`、`useTpmKspOtherwiseFail`、`usePassportForWorkKspOtherwiseFail`、`useSoftwareKsp`。</span><span class="sxs-lookup"><span data-stu-id="ed36e-155">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="ed36e-156">certificateSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="ed36e-156">certificateSubjectNameFormat</span></span>|[<span data-ttu-id="ed36e-157">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="ed36e-157">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="ed36e-158">主题名称格式。</span><span class="sxs-lookup"><span data-stu-id="ed36e-158">Subject name format.</span></span> <span data-ttu-id="ed36e-159">可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。</span><span class="sxs-lookup"><span data-stu-id="ed36e-159">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="ed36e-160">certificateSubjectAlternativeNameFormat</span><span class="sxs-lookup"><span data-stu-id="ed36e-160">certificateSubjectAlternativeNameFormat</span></span>|[<span data-ttu-id="ed36e-161">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="ed36e-161">subjectAlternativeNameType</span></span>](../resources/intune-shared-subjectalternativenametype.md)|<span data-ttu-id="ed36e-162">主题备用名称格式。</span><span class="sxs-lookup"><span data-stu-id="ed36e-162">Subject alternative name format.</span></span> <span data-ttu-id="ed36e-163">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`、`universalResourceIdentifier`。</span><span class="sxs-lookup"><span data-stu-id="ed36e-163">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="ed36e-164">certificateRevokeStatus</span><span class="sxs-lookup"><span data-stu-id="ed36e-164">certificateRevokeStatus</span></span>|[<span data-ttu-id="ed36e-165">certificateRevocationStatus</span><span class="sxs-lookup"><span data-stu-id="ed36e-165">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="ed36e-166">撤销状态。</span><span class="sxs-lookup"><span data-stu-id="ed36e-166">Revoke status.</span></span> <span data-ttu-id="ed36e-167">可取值为：`none`、`pending`、`issued`、`failed`、`revoked`。</span><span class="sxs-lookup"><span data-stu-id="ed36e-167">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="ed36e-168">certificateProfileDisplayName</span><span class="sxs-lookup"><span data-stu-id="ed36e-168">certificateProfileDisplayName</span></span>|<span data-ttu-id="ed36e-169">String</span><span class="sxs-lookup"><span data-stu-id="ed36e-169">String</span></span>|<span data-ttu-id="ed36e-170">证书配置文件显示名称</span><span class="sxs-lookup"><span data-stu-id="ed36e-170">Certificate profile display name</span></span>|
|<span data-ttu-id="ed36e-171">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="ed36e-171">deviceDisplayName</span></span>|<span data-ttu-id="ed36e-172">String</span><span class="sxs-lookup"><span data-stu-id="ed36e-172">String</span></span>|<span data-ttu-id="ed36e-173">设备显示名称</span><span class="sxs-lookup"><span data-stu-id="ed36e-173">Device display name</span></span>|
|<span data-ttu-id="ed36e-174">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="ed36e-174">userDisplayName</span></span>|<span data-ttu-id="ed36e-175">String</span><span class="sxs-lookup"><span data-stu-id="ed36e-175">String</span></span>|<span data-ttu-id="ed36e-176">用户显示名称</span><span class="sxs-lookup"><span data-stu-id="ed36e-176">User display name</span></span>|
|<span data-ttu-id="ed36e-177">certificateExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ed36e-177">certificateExpirationDateTime</span></span>|<span data-ttu-id="ed36e-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed36e-178">DateTimeOffset</span></span>|<span data-ttu-id="ed36e-179">证书到期日期</span><span class="sxs-lookup"><span data-stu-id="ed36e-179">Certificate expiry date</span></span>|
|<span data-ttu-id="ed36e-180">certificateLastIssuanceStateChangedDateTime</span><span class="sxs-lookup"><span data-stu-id="ed36e-180">certificateLastIssuanceStateChangedDateTime</span></span>|<span data-ttu-id="ed36e-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed36e-181">DateTimeOffset</span></span>|<span data-ttu-id="ed36e-182">上次证书颁发状态更改</span><span class="sxs-lookup"><span data-stu-id="ed36e-182">Last certificate issuance state change</span></span>|
|<span data-ttu-id="ed36e-183">lastCertificateStateChangeDateTime</span><span class="sxs-lookup"><span data-stu-id="ed36e-183">lastCertificateStateChangeDateTime</span></span>|<span data-ttu-id="ed36e-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed36e-184">DateTimeOffset</span></span>|<span data-ttu-id="ed36e-185">上次证书颁发状态更改</span><span class="sxs-lookup"><span data-stu-id="ed36e-185">Last certificate issuance state change</span></span>|
|<span data-ttu-id="ed36e-186">certificateIssuer</span><span class="sxs-lookup"><span data-stu-id="ed36e-186">certificateIssuer</span></span>|<span data-ttu-id="ed36e-187">String</span><span class="sxs-lookup"><span data-stu-id="ed36e-187">String</span></span>|<span data-ttu-id="ed36e-188">颁发者</span><span class="sxs-lookup"><span data-stu-id="ed36e-188">Issuer</span></span>|
|<span data-ttu-id="ed36e-189">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="ed36e-189">certificateThumbprint</span></span>|<span data-ttu-id="ed36e-190">String</span><span class="sxs-lookup"><span data-stu-id="ed36e-190">String</span></span>|<span data-ttu-id="ed36e-191">指纹</span><span class="sxs-lookup"><span data-stu-id="ed36e-191">Thumbprint</span></span>|
|<span data-ttu-id="ed36e-192">certificateSerialNumber</span><span class="sxs-lookup"><span data-stu-id="ed36e-192">certificateSerialNumber</span></span>|<span data-ttu-id="ed36e-193">String</span><span class="sxs-lookup"><span data-stu-id="ed36e-193">String</span></span>|<span data-ttu-id="ed36e-194">序列号</span><span class="sxs-lookup"><span data-stu-id="ed36e-194">Serial number</span></span>|
|<span data-ttu-id="ed36e-195">certificateKeyLength</span><span class="sxs-lookup"><span data-stu-id="ed36e-195">certificateKeyLength</span></span>|<span data-ttu-id="ed36e-196">Int32</span><span class="sxs-lookup"><span data-stu-id="ed36e-196">Int32</span></span>|<span data-ttu-id="ed36e-197">密钥长度</span><span class="sxs-lookup"><span data-stu-id="ed36e-197">Key length</span></span>|
|<span data-ttu-id="ed36e-198">certificateEnhancedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="ed36e-198">certificateEnhancedKeyUsage</span></span>|<span data-ttu-id="ed36e-199">String</span><span class="sxs-lookup"><span data-stu-id="ed36e-199">String</span></span>|<span data-ttu-id="ed36e-200">扩展密钥用法</span><span class="sxs-lookup"><span data-stu-id="ed36e-200">Extended key usage</span></span>|
|<span data-ttu-id="ed36e-201">certificateValidityPeriod</span><span class="sxs-lookup"><span data-stu-id="ed36e-201">certificateValidityPeriod</span></span>|<span data-ttu-id="ed36e-202">Int32</span><span class="sxs-lookup"><span data-stu-id="ed36e-202">Int32</span></span>|<span data-ttu-id="ed36e-203">有效期</span><span class="sxs-lookup"><span data-stu-id="ed36e-203">Validity period</span></span>|
|<span data-ttu-id="ed36e-204">certificateSubjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="ed36e-204">certificateSubjectNameFormatString</span></span>|<span data-ttu-id="ed36e-205">String</span><span class="sxs-lookup"><span data-stu-id="ed36e-205">String</span></span>|<span data-ttu-id="ed36e-206">自定义主题名称格式的主题名称格式字符串</span><span class="sxs-lookup"><span data-stu-id="ed36e-206">Subject name format string for custom subject name formats</span></span>|
|<span data-ttu-id="ed36e-207">certificateSubjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="ed36e-207">certificateSubjectAlternativeNameFormatString</span></span>|<span data-ttu-id="ed36e-208">String</span><span class="sxs-lookup"><span data-stu-id="ed36e-208">String</span></span>|<span data-ttu-id="ed36e-209">自定义格式的主题替代名称格式字符串</span><span class="sxs-lookup"><span data-stu-id="ed36e-209">Subject alternative name format string for custom formats</span></span>|
|<span data-ttu-id="ed36e-210">certificateIssuanceDateTime</span><span class="sxs-lookup"><span data-stu-id="ed36e-210">certificateIssuanceDateTime</span></span>|<span data-ttu-id="ed36e-211">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed36e-211">DateTimeOffset</span></span>|<span data-ttu-id="ed36e-212">发布日期</span><span class="sxs-lookup"><span data-stu-id="ed36e-212">Issuance date</span></span>|
|<span data-ttu-id="ed36e-213">certificateErrorCode</span><span class="sxs-lookup"><span data-stu-id="ed36e-213">certificateErrorCode</span></span>|<span data-ttu-id="ed36e-214">Int32</span><span class="sxs-lookup"><span data-stu-id="ed36e-214">Int32</span></span>|<span data-ttu-id="ed36e-215">错误代码</span><span class="sxs-lookup"><span data-stu-id="ed36e-215">Error code</span></span>|



## <a name="response"></a><span data-ttu-id="ed36e-216">响应</span><span class="sxs-lookup"><span data-stu-id="ed36e-216">Response</span></span>
<span data-ttu-id="ed36e-217">如果成功，此方法在响应正文中返回响应代码和更新 `200 OK` [的 managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ed36e-217">If successful, this method returns a `200 OK` response code and an updated [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed36e-218">示例</span><span class="sxs-lookup"><span data-stu-id="ed36e-218">Example</span></span>

### <a name="request"></a><span data-ttu-id="ed36e-219">请求</span><span class="sxs-lookup"><span data-stu-id="ed36e-219">Request</span></span>
<span data-ttu-id="ed36e-220">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ed36e-220">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
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

### <a name="response"></a><span data-ttu-id="ed36e-221">响应</span><span class="sxs-lookup"><span data-stu-id="ed36e-221">Response</span></span>
<span data-ttu-id="ed36e-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ed36e-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




