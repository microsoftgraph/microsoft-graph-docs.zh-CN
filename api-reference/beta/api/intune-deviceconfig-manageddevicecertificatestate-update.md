---
title: 更新 managedDeviceCertificateState
description: 更新 managedDeviceCertificateState 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 466ad2062b60294c2884664fc82e434d2b07724b
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52663920"
---
# <a name="update-manageddevicecertificatestate"></a><span data-ttu-id="66aea-103">更新 managedDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="66aea-103">Update managedDeviceCertificateState</span></span>

<span data-ttu-id="66aea-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66aea-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="66aea-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="66aea-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66aea-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="66aea-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66aea-107">更新 [managedDeviceCertificateState 对象](../resources/intune-deviceconfig-manageddevicecertificatestate.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="66aea-107">Update the properties of a [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="66aea-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="66aea-108">Prerequisites</span></span>
<span data-ttu-id="66aea-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="66aea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66aea-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="66aea-111">Permission type</span></span>|<span data-ttu-id="66aea-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="66aea-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="66aea-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="66aea-113">Delegated (work or school account)</span></span>|<span data-ttu-id="66aea-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66aea-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="66aea-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="66aea-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66aea-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="66aea-116">Not supported.</span></span>|
|<span data-ttu-id="66aea-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="66aea-117">Application</span></span>|<span data-ttu-id="66aea-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66aea-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="66aea-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="66aea-119">HTTP Request</span></span>
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
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10PkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10ImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windowsPhone81ImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="66aea-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="66aea-120">Request headers</span></span>
|<span data-ttu-id="66aea-121">标头</span><span class="sxs-lookup"><span data-stu-id="66aea-121">Header</span></span>|<span data-ttu-id="66aea-122">值</span><span class="sxs-lookup"><span data-stu-id="66aea-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="66aea-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="66aea-123">Authorization</span></span>|<span data-ttu-id="66aea-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="66aea-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="66aea-125">接受</span><span class="sxs-lookup"><span data-stu-id="66aea-125">Accept</span></span>|<span data-ttu-id="66aea-126">application/json</span><span class="sxs-lookup"><span data-stu-id="66aea-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="66aea-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="66aea-127">Request body</span></span>
<span data-ttu-id="66aea-128">在请求正文中，提供 [managedDeviceCertificateState 对象的](../resources/intune-deviceconfig-manageddevicecertificatestate.md) JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="66aea-128">In the request body, supply a JSON representation for the [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object.</span></span>

<span data-ttu-id="66aea-129">下表显示创建 [managedDeviceCertificateState 时所需的属性](../resources/intune-deviceconfig-manageddevicecertificatestate.md)。</span><span class="sxs-lookup"><span data-stu-id="66aea-129">The following table shows the properties that are required when you create the [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md).</span></span>

|<span data-ttu-id="66aea-130">属性</span><span class="sxs-lookup"><span data-stu-id="66aea-130">Property</span></span>|<span data-ttu-id="66aea-131">类型</span><span class="sxs-lookup"><span data-stu-id="66aea-131">Type</span></span>|<span data-ttu-id="66aea-132">说明</span><span class="sxs-lookup"><span data-stu-id="66aea-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66aea-133">id</span><span class="sxs-lookup"><span data-stu-id="66aea-133">id</span></span>|<span data-ttu-id="66aea-134">String</span><span class="sxs-lookup"><span data-stu-id="66aea-134">String</span></span>|<span data-ttu-id="66aea-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="66aea-135">Key of the entity.</span></span>|
|<span data-ttu-id="66aea-136">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="66aea-136">devicePlatform</span></span>|[<span data-ttu-id="66aea-137">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="66aea-137">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="66aea-138">设备平台。</span><span class="sxs-lookup"><span data-stu-id="66aea-138">Device platform.</span></span> <span data-ttu-id="66aea-139">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`unknown`、`androidAOSP`。</span><span class="sxs-lookup"><span data-stu-id="66aea-139">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`, `androidAOSP`.</span></span>|
|<span data-ttu-id="66aea-140">certificateKeyUsage</span><span class="sxs-lookup"><span data-stu-id="66aea-140">certificateKeyUsage</span></span>|[<span data-ttu-id="66aea-141">keyUsages</span><span class="sxs-lookup"><span data-stu-id="66aea-141">keyUsages</span></span>](../resources/intune-shared-keyusages.md)|<span data-ttu-id="66aea-142">密钥用法。</span><span class="sxs-lookup"><span data-stu-id="66aea-142">Key usage.</span></span> <span data-ttu-id="66aea-143">可取值为：`keyEncipherment`、`digitalSignature`。</span><span class="sxs-lookup"><span data-stu-id="66aea-143">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="66aea-144">certificateValidityPeriodUnits</span><span class="sxs-lookup"><span data-stu-id="66aea-144">certificateValidityPeriodUnits</span></span>|[<span data-ttu-id="66aea-145">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="66aea-145">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="66aea-146">有效期单位。</span><span class="sxs-lookup"><span data-stu-id="66aea-146">Validity period units.</span></span> <span data-ttu-id="66aea-147">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="66aea-147">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="66aea-148">certificateIssuanceState</span><span class="sxs-lookup"><span data-stu-id="66aea-148">certificateIssuanceState</span></span>|[<span data-ttu-id="66aea-149">certificateIssuanceStates</span><span class="sxs-lookup"><span data-stu-id="66aea-149">certificateIssuanceStates</span></span>](../resources/intune-deviceconfig-certificateissuancestates.md)|<span data-ttu-id="66aea-150">颁发状态。</span><span class="sxs-lookup"><span data-stu-id="66aea-150">Issuance State.</span></span> <span data-ttu-id="66aea-151">可能的值是 `unknown` `challengeIssued` `challengeIssueFailed` ：、、、、、、、、、、 `requestCreationFailed` `requestSubmitFailed` `challengeValidationSucceeded` `challengeValidationFailed` `issueFailed` `issuePending` `issued` `responseProcessingFailed` `responsePending` `enrollmentSucceeded` `enrollmentNotNeeded` `revoked` `removedFromCollection` `renewVerified` `installFailed` `installed` `deleteFailed` `deleted` `renewalRequested` `requested` 。</span><span class="sxs-lookup"><span data-stu-id="66aea-151">Possible values are: `unknown`, `challengeIssued`, `challengeIssueFailed`, `requestCreationFailed`, `requestSubmitFailed`, `challengeValidationSucceeded`, `challengeValidationFailed`, `issueFailed`, `issuePending`, `issued`, `responseProcessingFailed`, `responsePending`, `enrollmentSucceeded`, `enrollmentNotNeeded`, `revoked`, `removedFromCollection`, `renewVerified`, `installFailed`, `installed`, `deleteFailed`, `deleted`, `renewalRequested`, `requested`.</span></span>|
|<span data-ttu-id="66aea-152">certificateKeyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="66aea-152">certificateKeyStorageProvider</span></span>|[<span data-ttu-id="66aea-153">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="66aea-153">keyStorageProviderOption</span></span>](../resources/intune-shared-keystorageprovideroption.md)|<span data-ttu-id="66aea-154">密钥存储提供程序。</span><span class="sxs-lookup"><span data-stu-id="66aea-154">Key Storage Provider.</span></span> <span data-ttu-id="66aea-155">可取值为：`useTpmKspOtherwiseUseSoftwareKsp`、`useTpmKspOtherwiseFail`、`usePassportForWorkKspOtherwiseFail`、`useSoftwareKsp`。</span><span class="sxs-lookup"><span data-stu-id="66aea-155">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="66aea-156">certificateSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="66aea-156">certificateSubjectNameFormat</span></span>|[<span data-ttu-id="66aea-157">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="66aea-157">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="66aea-158">主题名称格式。</span><span class="sxs-lookup"><span data-stu-id="66aea-158">Subject name format.</span></span> <span data-ttu-id="66aea-159">可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。</span><span class="sxs-lookup"><span data-stu-id="66aea-159">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="66aea-160">certificateSubjectAlternativeNameFormat</span><span class="sxs-lookup"><span data-stu-id="66aea-160">certificateSubjectAlternativeNameFormat</span></span>|[<span data-ttu-id="66aea-161">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="66aea-161">subjectAlternativeNameType</span></span>](../resources/intune-shared-subjectalternativenametype.md)|<span data-ttu-id="66aea-162">主题备用名称格式。</span><span class="sxs-lookup"><span data-stu-id="66aea-162">Subject alternative name format.</span></span> <span data-ttu-id="66aea-163">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`、`universalResourceIdentifier`。</span><span class="sxs-lookup"><span data-stu-id="66aea-163">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="66aea-164">certificateRevokeStatus</span><span class="sxs-lookup"><span data-stu-id="66aea-164">certificateRevokeStatus</span></span>|[<span data-ttu-id="66aea-165">certificateRevocationStatus</span><span class="sxs-lookup"><span data-stu-id="66aea-165">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="66aea-166">撤销状态。</span><span class="sxs-lookup"><span data-stu-id="66aea-166">Revoke status.</span></span> <span data-ttu-id="66aea-167">可取值为：`none`、`pending`、`issued`、`failed`、`revoked`。</span><span class="sxs-lookup"><span data-stu-id="66aea-167">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="66aea-168">certificateProfileDisplayName</span><span class="sxs-lookup"><span data-stu-id="66aea-168">certificateProfileDisplayName</span></span>|<span data-ttu-id="66aea-169">String</span><span class="sxs-lookup"><span data-stu-id="66aea-169">String</span></span>|<span data-ttu-id="66aea-170">证书配置文件显示名称</span><span class="sxs-lookup"><span data-stu-id="66aea-170">Certificate profile display name</span></span>|
|<span data-ttu-id="66aea-171">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="66aea-171">deviceDisplayName</span></span>|<span data-ttu-id="66aea-172">String</span><span class="sxs-lookup"><span data-stu-id="66aea-172">String</span></span>|<span data-ttu-id="66aea-173">设备显示名称</span><span class="sxs-lookup"><span data-stu-id="66aea-173">Device display name</span></span>|
|<span data-ttu-id="66aea-174">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="66aea-174">userDisplayName</span></span>|<span data-ttu-id="66aea-175">String</span><span class="sxs-lookup"><span data-stu-id="66aea-175">String</span></span>|<span data-ttu-id="66aea-176">用户显示名称</span><span class="sxs-lookup"><span data-stu-id="66aea-176">User display name</span></span>|
|<span data-ttu-id="66aea-177">certificateExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="66aea-177">certificateExpirationDateTime</span></span>|<span data-ttu-id="66aea-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66aea-178">DateTimeOffset</span></span>|<span data-ttu-id="66aea-179">证书到期日期</span><span class="sxs-lookup"><span data-stu-id="66aea-179">Certificate expiry date</span></span>|
|<span data-ttu-id="66aea-180">certificateLastIssuanceStateChangedDateTime</span><span class="sxs-lookup"><span data-stu-id="66aea-180">certificateLastIssuanceStateChangedDateTime</span></span>|<span data-ttu-id="66aea-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66aea-181">DateTimeOffset</span></span>|<span data-ttu-id="66aea-182">上次证书颁发状态更改</span><span class="sxs-lookup"><span data-stu-id="66aea-182">Last certificate issuance state change</span></span>|
|<span data-ttu-id="66aea-183">lastCertificateStateChangeDateTime</span><span class="sxs-lookup"><span data-stu-id="66aea-183">lastCertificateStateChangeDateTime</span></span>|<span data-ttu-id="66aea-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66aea-184">DateTimeOffset</span></span>|<span data-ttu-id="66aea-185">上次证书颁发状态更改</span><span class="sxs-lookup"><span data-stu-id="66aea-185">Last certificate issuance state change</span></span>|
|<span data-ttu-id="66aea-186">certificateIssuer</span><span class="sxs-lookup"><span data-stu-id="66aea-186">certificateIssuer</span></span>|<span data-ttu-id="66aea-187">String</span><span class="sxs-lookup"><span data-stu-id="66aea-187">String</span></span>|<span data-ttu-id="66aea-188">颁发者</span><span class="sxs-lookup"><span data-stu-id="66aea-188">Issuer</span></span>|
|<span data-ttu-id="66aea-189">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="66aea-189">certificateThumbprint</span></span>|<span data-ttu-id="66aea-190">String</span><span class="sxs-lookup"><span data-stu-id="66aea-190">String</span></span>|<span data-ttu-id="66aea-191">指纹</span><span class="sxs-lookup"><span data-stu-id="66aea-191">Thumbprint</span></span>|
|<span data-ttu-id="66aea-192">certificateSerialNumber</span><span class="sxs-lookup"><span data-stu-id="66aea-192">certificateSerialNumber</span></span>|<span data-ttu-id="66aea-193">String</span><span class="sxs-lookup"><span data-stu-id="66aea-193">String</span></span>|<span data-ttu-id="66aea-194">序列号</span><span class="sxs-lookup"><span data-stu-id="66aea-194">Serial number</span></span>|
|<span data-ttu-id="66aea-195">certificateKeyLength</span><span class="sxs-lookup"><span data-stu-id="66aea-195">certificateKeyLength</span></span>|<span data-ttu-id="66aea-196">Int32</span><span class="sxs-lookup"><span data-stu-id="66aea-196">Int32</span></span>|<span data-ttu-id="66aea-197">密钥长度</span><span class="sxs-lookup"><span data-stu-id="66aea-197">Key length</span></span>|
|<span data-ttu-id="66aea-198">certificateEnhancedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="66aea-198">certificateEnhancedKeyUsage</span></span>|<span data-ttu-id="66aea-199">String</span><span class="sxs-lookup"><span data-stu-id="66aea-199">String</span></span>|<span data-ttu-id="66aea-200">扩展密钥用法</span><span class="sxs-lookup"><span data-stu-id="66aea-200">Extended key usage</span></span>|
|<span data-ttu-id="66aea-201">certificateValidityPeriod</span><span class="sxs-lookup"><span data-stu-id="66aea-201">certificateValidityPeriod</span></span>|<span data-ttu-id="66aea-202">Int32</span><span class="sxs-lookup"><span data-stu-id="66aea-202">Int32</span></span>|<span data-ttu-id="66aea-203">有效期</span><span class="sxs-lookup"><span data-stu-id="66aea-203">Validity period</span></span>|
|<span data-ttu-id="66aea-204">certificateSubjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="66aea-204">certificateSubjectNameFormatString</span></span>|<span data-ttu-id="66aea-205">String</span><span class="sxs-lookup"><span data-stu-id="66aea-205">String</span></span>|<span data-ttu-id="66aea-206">自定义主题名称格式的主题名称格式字符串</span><span class="sxs-lookup"><span data-stu-id="66aea-206">Subject name format string for custom subject name formats</span></span>|
|<span data-ttu-id="66aea-207">certificateSubjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="66aea-207">certificateSubjectAlternativeNameFormatString</span></span>|<span data-ttu-id="66aea-208">String</span><span class="sxs-lookup"><span data-stu-id="66aea-208">String</span></span>|<span data-ttu-id="66aea-209">自定义格式的主题替代名称格式字符串</span><span class="sxs-lookup"><span data-stu-id="66aea-209">Subject alternative name format string for custom formats</span></span>|
|<span data-ttu-id="66aea-210">certificateIssuanceDateTime</span><span class="sxs-lookup"><span data-stu-id="66aea-210">certificateIssuanceDateTime</span></span>|<span data-ttu-id="66aea-211">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66aea-211">DateTimeOffset</span></span>|<span data-ttu-id="66aea-212">发布日期</span><span class="sxs-lookup"><span data-stu-id="66aea-212">Issuance date</span></span>|
|<span data-ttu-id="66aea-213">certificateErrorCode</span><span class="sxs-lookup"><span data-stu-id="66aea-213">certificateErrorCode</span></span>|<span data-ttu-id="66aea-214">Int32</span><span class="sxs-lookup"><span data-stu-id="66aea-214">Int32</span></span>|<span data-ttu-id="66aea-215">错误代码</span><span class="sxs-lookup"><span data-stu-id="66aea-215">Error code</span></span>|



## <a name="response"></a><span data-ttu-id="66aea-216">响应</span><span class="sxs-lookup"><span data-stu-id="66aea-216">Response</span></span>
<span data-ttu-id="66aea-217">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="66aea-217">If successful, this method returns a `200 OK` response code and an updated [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66aea-218">示例</span><span class="sxs-lookup"><span data-stu-id="66aea-218">Example</span></span>

### <a name="request"></a><span data-ttu-id="66aea-219">请求</span><span class="sxs-lookup"><span data-stu-id="66aea-219">Request</span></span>
<span data-ttu-id="66aea-220">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="66aea-220">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="66aea-221">响应</span><span class="sxs-lookup"><span data-stu-id="66aea-221">Response</span></span>
<span data-ttu-id="66aea-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="66aea-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




