---
title: 更新 managedDeviceCertificateState
description: 更新 managedDeviceCertificateState 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b060137765444db66aaebce884fa30fe07830afa
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2020
ms.locfileid: "45122880"
---
# <a name="update-manageddevicecertificatestate"></a><span data-ttu-id="dacd2-103">更新 managedDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="dacd2-103">Update managedDeviceCertificateState</span></span>

<span data-ttu-id="dacd2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dacd2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dacd2-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="dacd2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dacd2-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dacd2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dacd2-107">更新[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="dacd2-107">Update the properties of a [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dacd2-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="dacd2-108">Prerequisites</span></span>
<span data-ttu-id="dacd2-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="dacd2-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="dacd2-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dacd2-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dacd2-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="dacd2-111">Permission type</span></span>|<span data-ttu-id="dacd2-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="dacd2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dacd2-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dacd2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dacd2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dacd2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dacd2-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dacd2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dacd2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="dacd2-116">Not supported.</span></span>|
|<span data-ttu-id="dacd2-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="dacd2-117">Application</span></span>|<span data-ttu-id="dacd2-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dacd2-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dacd2-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dacd2-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="dacd2-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="dacd2-120">Request headers</span></span>
|<span data-ttu-id="dacd2-121">标头</span><span class="sxs-lookup"><span data-stu-id="dacd2-121">Header</span></span>|<span data-ttu-id="dacd2-122">值</span><span class="sxs-lookup"><span data-stu-id="dacd2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dacd2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dacd2-123">Authorization</span></span>|<span data-ttu-id="dacd2-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="dacd2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dacd2-125">接受</span><span class="sxs-lookup"><span data-stu-id="dacd2-125">Accept</span></span>|<span data-ttu-id="dacd2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dacd2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dacd2-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="dacd2-127">Request body</span></span>
<span data-ttu-id="dacd2-128">在请求正文中，提供[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dacd2-128">In the request body, supply a JSON representation for the [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object.</span></span>

<span data-ttu-id="dacd2-129">下表显示创建[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="dacd2-129">The following table shows the properties that are required when you create the [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md).</span></span>

|<span data-ttu-id="dacd2-130">属性</span><span class="sxs-lookup"><span data-stu-id="dacd2-130">Property</span></span>|<span data-ttu-id="dacd2-131">类型</span><span class="sxs-lookup"><span data-stu-id="dacd2-131">Type</span></span>|<span data-ttu-id="dacd2-132">说明</span><span class="sxs-lookup"><span data-stu-id="dacd2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dacd2-133">id</span><span class="sxs-lookup"><span data-stu-id="dacd2-133">id</span></span>|<span data-ttu-id="dacd2-134">字符串</span><span class="sxs-lookup"><span data-stu-id="dacd2-134">String</span></span>|<span data-ttu-id="dacd2-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="dacd2-135">Key of the entity.</span></span>|
|<span data-ttu-id="dacd2-136">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="dacd2-136">devicePlatform</span></span>|[<span data-ttu-id="dacd2-137">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="dacd2-137">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="dacd2-138">设备平台。</span><span class="sxs-lookup"><span data-stu-id="dacd2-138">Device platform.</span></span> <span data-ttu-id="dacd2-139">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="dacd2-139">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="dacd2-140">certificateKeyUsage</span><span class="sxs-lookup"><span data-stu-id="dacd2-140">certificateKeyUsage</span></span>|[<span data-ttu-id="dacd2-141">keyUsages</span><span class="sxs-lookup"><span data-stu-id="dacd2-141">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="dacd2-142">密钥用法。</span><span class="sxs-lookup"><span data-stu-id="dacd2-142">Key usage.</span></span> <span data-ttu-id="dacd2-143">可取值为：`keyEncipherment`、`digitalSignature`。</span><span class="sxs-lookup"><span data-stu-id="dacd2-143">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="dacd2-144">certificateValidityPeriodUnits</span><span class="sxs-lookup"><span data-stu-id="dacd2-144">certificateValidityPeriodUnits</span></span>|[<span data-ttu-id="dacd2-145">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="dacd2-145">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="dacd2-146">有效期单位。</span><span class="sxs-lookup"><span data-stu-id="dacd2-146">Validity period units.</span></span> <span data-ttu-id="dacd2-147">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="dacd2-147">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="dacd2-148">certificateIssuanceState</span><span class="sxs-lookup"><span data-stu-id="dacd2-148">certificateIssuanceState</span></span>|[<span data-ttu-id="dacd2-149">certificateIssuanceStates</span><span class="sxs-lookup"><span data-stu-id="dacd2-149">certificateIssuanceStates</span></span>](../resources/intune-deviceconfig-certificateissuancestates.md)|<span data-ttu-id="dacd2-150">颁发状态。</span><span class="sxs-lookup"><span data-stu-id="dacd2-150">Issuance State.</span></span> <span data-ttu-id="dacd2-151">可能的值为：、、、、、、、、、、、、、、、、、、、、、、 `unknown` `challengeIssued` `challengeIssueFailed` `requestCreationFailed` `requestSubmitFailed` `challengeValidationSucceeded` `challengeValidationFailed` `issueFailed` `issuePending` `issued` `responseProcessingFailed` `responsePending` `enrollmentSucceeded` `enrollmentNotNeeded` `revoked` `removedFromCollection` `renewVerified` `installFailed` `installed` `deleteFailed` `deleted` `renewalRequested` `requested` 。</span><span class="sxs-lookup"><span data-stu-id="dacd2-151">Possible values are: `unknown`, `challengeIssued`, `challengeIssueFailed`, `requestCreationFailed`, `requestSubmitFailed`, `challengeValidationSucceeded`, `challengeValidationFailed`, `issueFailed`, `issuePending`, `issued`, `responseProcessingFailed`, `responsePending`, `enrollmentSucceeded`, `enrollmentNotNeeded`, `revoked`, `removedFromCollection`, `renewVerified`, `installFailed`, `installed`, `deleteFailed`, `deleted`, `renewalRequested`, `requested`.</span></span>|
|<span data-ttu-id="dacd2-152">certificateKeyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="dacd2-152">certificateKeyStorageProvider</span></span>|[<span data-ttu-id="dacd2-153">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="dacd2-153">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="dacd2-154">密钥存储提供程序。</span><span class="sxs-lookup"><span data-stu-id="dacd2-154">Key Storage Provider.</span></span> <span data-ttu-id="dacd2-155">可取值为：`useTpmKspOtherwiseUseSoftwareKsp`、`useTpmKspOtherwiseFail`、`usePassportForWorkKspOtherwiseFail`、`useSoftwareKsp`。</span><span class="sxs-lookup"><span data-stu-id="dacd2-155">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="dacd2-156">certificateSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="dacd2-156">certificateSubjectNameFormat</span></span>|[<span data-ttu-id="dacd2-157">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="dacd2-157">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="dacd2-158">使用者名称格式。</span><span class="sxs-lookup"><span data-stu-id="dacd2-158">Subject name format.</span></span> <span data-ttu-id="dacd2-159">可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。</span><span class="sxs-lookup"><span data-stu-id="dacd2-159">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="dacd2-160">certificateSubjectAlternativeNameFormat</span><span class="sxs-lookup"><span data-stu-id="dacd2-160">certificateSubjectAlternativeNameFormat</span></span>|[<span data-ttu-id="dacd2-161">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="dacd2-161">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="dacd2-162">使用者可选名称格式。</span><span class="sxs-lookup"><span data-stu-id="dacd2-162">Subject alternative name format.</span></span> <span data-ttu-id="dacd2-163">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="dacd2-163">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="dacd2-164">certificateRevokeStatus</span><span class="sxs-lookup"><span data-stu-id="dacd2-164">certificateRevokeStatus</span></span>|[<span data-ttu-id="dacd2-165">certificateRevocationStatus</span><span class="sxs-lookup"><span data-stu-id="dacd2-165">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="dacd2-166">撤消状态。</span><span class="sxs-lookup"><span data-stu-id="dacd2-166">Revoke status.</span></span> <span data-ttu-id="dacd2-167">可取值为：`none`、`pending`、`issued`、`failed`、`revoked`。</span><span class="sxs-lookup"><span data-stu-id="dacd2-167">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="dacd2-168">certificateProfileDisplayName</span><span class="sxs-lookup"><span data-stu-id="dacd2-168">certificateProfileDisplayName</span></span>|<span data-ttu-id="dacd2-169">String</span><span class="sxs-lookup"><span data-stu-id="dacd2-169">String</span></span>|<span data-ttu-id="dacd2-170">证书配置文件显示名称</span><span class="sxs-lookup"><span data-stu-id="dacd2-170">Certificate profile display name</span></span>|
|<span data-ttu-id="dacd2-171">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="dacd2-171">deviceDisplayName</span></span>|<span data-ttu-id="dacd2-172">String</span><span class="sxs-lookup"><span data-stu-id="dacd2-172">String</span></span>|<span data-ttu-id="dacd2-173">设备显示名称</span><span class="sxs-lookup"><span data-stu-id="dacd2-173">Device display name</span></span>|
|<span data-ttu-id="dacd2-174">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="dacd2-174">userDisplayName</span></span>|<span data-ttu-id="dacd2-175">String</span><span class="sxs-lookup"><span data-stu-id="dacd2-175">String</span></span>|<span data-ttu-id="dacd2-176">用户显示名称</span><span class="sxs-lookup"><span data-stu-id="dacd2-176">User display name</span></span>|
|<span data-ttu-id="dacd2-177">certificateExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="dacd2-177">certificateExpirationDateTime</span></span>|<span data-ttu-id="dacd2-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dacd2-178">DateTimeOffset</span></span>|<span data-ttu-id="dacd2-179">证书到期日期</span><span class="sxs-lookup"><span data-stu-id="dacd2-179">Certificate expiry date</span></span>|
|<span data-ttu-id="dacd2-180">certificateLastIssuanceStateChangedDateTime</span><span class="sxs-lookup"><span data-stu-id="dacd2-180">certificateLastIssuanceStateChangedDateTime</span></span>|<span data-ttu-id="dacd2-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dacd2-181">DateTimeOffset</span></span>|<span data-ttu-id="dacd2-182">上次证书颁发状态更改</span><span class="sxs-lookup"><span data-stu-id="dacd2-182">Last certificate issuance state change</span></span>|
|<span data-ttu-id="dacd2-183">lastCertificateStateChangeDateTime</span><span class="sxs-lookup"><span data-stu-id="dacd2-183">lastCertificateStateChangeDateTime</span></span>|<span data-ttu-id="dacd2-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dacd2-184">DateTimeOffset</span></span>|<span data-ttu-id="dacd2-185">上次证书颁发状态更改</span><span class="sxs-lookup"><span data-stu-id="dacd2-185">Last certificate issuance state change</span></span>|
|<span data-ttu-id="dacd2-186">certificateIssuer</span><span class="sxs-lookup"><span data-stu-id="dacd2-186">certificateIssuer</span></span>|<span data-ttu-id="dacd2-187">String</span><span class="sxs-lookup"><span data-stu-id="dacd2-187">String</span></span>|<span data-ttu-id="dacd2-188">颁发者</span><span class="sxs-lookup"><span data-stu-id="dacd2-188">Issuer</span></span>|
|<span data-ttu-id="dacd2-189">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="dacd2-189">certificateThumbprint</span></span>|<span data-ttu-id="dacd2-190">String</span><span class="sxs-lookup"><span data-stu-id="dacd2-190">String</span></span>|<span data-ttu-id="dacd2-191">为</span><span class="sxs-lookup"><span data-stu-id="dacd2-191">Thumbprint</span></span>|
|<span data-ttu-id="dacd2-192">certificateSerialNumber</span><span class="sxs-lookup"><span data-stu-id="dacd2-192">certificateSerialNumber</span></span>|<span data-ttu-id="dacd2-193">String</span><span class="sxs-lookup"><span data-stu-id="dacd2-193">String</span></span>|<span data-ttu-id="dacd2-194">序列号</span><span class="sxs-lookup"><span data-stu-id="dacd2-194">Serial number</span></span>|
|<span data-ttu-id="dacd2-195">certificateKeyLength</span><span class="sxs-lookup"><span data-stu-id="dacd2-195">certificateKeyLength</span></span>|<span data-ttu-id="dacd2-196">Int32</span><span class="sxs-lookup"><span data-stu-id="dacd2-196">Int32</span></span>|<span data-ttu-id="dacd2-197">密钥长度</span><span class="sxs-lookup"><span data-stu-id="dacd2-197">Key length</span></span>|
|<span data-ttu-id="dacd2-198">certificateEnhancedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="dacd2-198">certificateEnhancedKeyUsage</span></span>|<span data-ttu-id="dacd2-199">String</span><span class="sxs-lookup"><span data-stu-id="dacd2-199">String</span></span>|<span data-ttu-id="dacd2-200">扩展密钥用法</span><span class="sxs-lookup"><span data-stu-id="dacd2-200">Extended key usage</span></span>|
|<span data-ttu-id="dacd2-201">certificateValidityPeriod</span><span class="sxs-lookup"><span data-stu-id="dacd2-201">certificateValidityPeriod</span></span>|<span data-ttu-id="dacd2-202">Int32</span><span class="sxs-lookup"><span data-stu-id="dacd2-202">Int32</span></span>|<span data-ttu-id="dacd2-203">有效期</span><span class="sxs-lookup"><span data-stu-id="dacd2-203">Validity period</span></span>|
|<span data-ttu-id="dacd2-204">certificateSubjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="dacd2-204">certificateSubjectNameFormatString</span></span>|<span data-ttu-id="dacd2-205">String</span><span class="sxs-lookup"><span data-stu-id="dacd2-205">String</span></span>|<span data-ttu-id="dacd2-206">自定义主题名称格式的主题名称格式字符串</span><span class="sxs-lookup"><span data-stu-id="dacd2-206">Subject name format string for custom subject name formats</span></span>|
|<span data-ttu-id="dacd2-207">certificateSubjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="dacd2-207">certificateSubjectAlternativeNameFormatString</span></span>|<span data-ttu-id="dacd2-208">String</span><span class="sxs-lookup"><span data-stu-id="dacd2-208">String</span></span>|<span data-ttu-id="dacd2-209">自定义格式的使用者可选名称格式字符串</span><span class="sxs-lookup"><span data-stu-id="dacd2-209">Subject alternative name format string for custom formats</span></span>|
|<span data-ttu-id="dacd2-210">certificateIssuanceDateTime</span><span class="sxs-lookup"><span data-stu-id="dacd2-210">certificateIssuanceDateTime</span></span>|<span data-ttu-id="dacd2-211">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dacd2-211">DateTimeOffset</span></span>|<span data-ttu-id="dacd2-212">颁发日期</span><span class="sxs-lookup"><span data-stu-id="dacd2-212">Issuance date</span></span>|
|<span data-ttu-id="dacd2-213">certificateErrorCode</span><span class="sxs-lookup"><span data-stu-id="dacd2-213">certificateErrorCode</span></span>|<span data-ttu-id="dacd2-214">Int32</span><span class="sxs-lookup"><span data-stu-id="dacd2-214">Int32</span></span>|<span data-ttu-id="dacd2-215">错误代码</span><span class="sxs-lookup"><span data-stu-id="dacd2-215">Error code</span></span>|



## <a name="response"></a><span data-ttu-id="dacd2-216">响应</span><span class="sxs-lookup"><span data-stu-id="dacd2-216">Response</span></span>
<span data-ttu-id="dacd2-217">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="dacd2-217">If successful, this method returns a `200 OK` response code and an updated [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dacd2-218">示例</span><span class="sxs-lookup"><span data-stu-id="dacd2-218">Example</span></span>

### <a name="request"></a><span data-ttu-id="dacd2-219">请求</span><span class="sxs-lookup"><span data-stu-id="dacd2-219">Request</span></span>
<span data-ttu-id="dacd2-220">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dacd2-220">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="dacd2-221">响应</span><span class="sxs-lookup"><span data-stu-id="dacd2-221">Response</span></span>
<span data-ttu-id="dacd2-222">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="dacd2-222">Here is an example of the response.</span></span> <span data-ttu-id="dacd2-223">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="dacd2-223">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="dacd2-224">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="dacd2-224">All of the properties will be returned from an actual call.</span></span>
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



