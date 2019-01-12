---
title: 更新 managedDeviceCertificateState
description: 更新 managedDeviceCertificateState 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3e890649f3efbe6f5eb1e22a3c4274dab09d1e88
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970561"
---
# <a name="update-manageddevicecertificatestate"></a><span data-ttu-id="6fddb-103">更新 managedDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="6fddb-103">Update managedDeviceCertificateState</span></span>

> <span data-ttu-id="6fddb-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6fddb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6fddb-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6fddb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6fddb-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6fddb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6fddb-107">更新[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6fddb-107">Update the properties of a [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6fddb-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6fddb-108">Prerequisites</span></span>
<span data-ttu-id="6fddb-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="6fddb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6fddb-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6fddb-111">Permission type</span></span>|<span data-ttu-id="6fddb-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6fddb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6fddb-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6fddb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6fddb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fddb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6fddb-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6fddb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6fddb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6fddb-116">Not supported.</span></span>|
|<span data-ttu-id="6fddb-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6fddb-117">Application</span></span>|<span data-ttu-id="6fddb-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="6fddb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6fddb-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6fddb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10PkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10ImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windowsPhone81ImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="6fddb-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6fddb-120">Request headers</span></span>
|<span data-ttu-id="6fddb-121">标头</span><span class="sxs-lookup"><span data-stu-id="6fddb-121">Header</span></span>|<span data-ttu-id="6fddb-122">值</span><span class="sxs-lookup"><span data-stu-id="6fddb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6fddb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6fddb-123">Authorization</span></span>|<span data-ttu-id="6fddb-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6fddb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6fddb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6fddb-125">Accept</span></span>|<span data-ttu-id="6fddb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6fddb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6fddb-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6fddb-127">Request body</span></span>
<span data-ttu-id="6fddb-128">在请求正文中，提供[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6fddb-128">In the request body, supply a JSON representation for the [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object.</span></span>

<span data-ttu-id="6fddb-129">下表显示时创建[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6fddb-129">The following table shows the properties that are required when you create the [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md).</span></span>

|<span data-ttu-id="6fddb-130">属性</span><span class="sxs-lookup"><span data-stu-id="6fddb-130">Property</span></span>|<span data-ttu-id="6fddb-131">类型</span><span class="sxs-lookup"><span data-stu-id="6fddb-131">Type</span></span>|<span data-ttu-id="6fddb-132">说明</span><span class="sxs-lookup"><span data-stu-id="6fddb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fddb-133">id</span><span class="sxs-lookup"><span data-stu-id="6fddb-133">id</span></span>|<span data-ttu-id="6fddb-134">String</span><span class="sxs-lookup"><span data-stu-id="6fddb-134">String</span></span>|<span data-ttu-id="6fddb-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6fddb-135">Key of the entity.</span></span>|
|<span data-ttu-id="6fddb-136">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="6fddb-136">devicePlatform</span></span>|[<span data-ttu-id="6fddb-137">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="6fddb-137">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="6fddb-138">设备平台。</span><span class="sxs-lookup"><span data-stu-id="6fddb-138">Device platform.</span></span> <span data-ttu-id="6fddb-139">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`。</span><span class="sxs-lookup"><span data-stu-id="6fddb-139">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|
|<span data-ttu-id="6fddb-140">certificateKeyUsage</span><span class="sxs-lookup"><span data-stu-id="6fddb-140">certificateKeyUsage</span></span>|[<span data-ttu-id="6fddb-141">keyUsages</span><span class="sxs-lookup"><span data-stu-id="6fddb-141">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="6fddb-142">密钥用法。</span><span class="sxs-lookup"><span data-stu-id="6fddb-142">Key usage.</span></span> <span data-ttu-id="6fddb-143">可取值为：`keyEncipherment`、`digitalSignature`。</span><span class="sxs-lookup"><span data-stu-id="6fddb-143">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="6fddb-144">certificateValidityPeriodUnits</span><span class="sxs-lookup"><span data-stu-id="6fddb-144">certificateValidityPeriodUnits</span></span>|[<span data-ttu-id="6fddb-145">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="6fddb-145">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="6fddb-146">有效期单位。</span><span class="sxs-lookup"><span data-stu-id="6fddb-146">Validity period units.</span></span> <span data-ttu-id="6fddb-147">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="6fddb-147">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="6fddb-148">certificateIssuanceState</span><span class="sxs-lookup"><span data-stu-id="6fddb-148">certificateIssuanceState</span></span>|[<span data-ttu-id="6fddb-149">certificateIssuanceStates</span><span class="sxs-lookup"><span data-stu-id="6fddb-149">certificateIssuanceStates</span></span>](../resources/intune-deviceconfig-certificateissuancestates.md)|<span data-ttu-id="6fddb-150">发布状态。</span><span class="sxs-lookup"><span data-stu-id="6fddb-150">Issuance State.</span></span> <span data-ttu-id="6fddb-151">可能的值为： `unknown`， `challengeIssued`， `challengeIssueFailed`， `requestCreationFailed`， `requestSubmitFailed`， `challengeValidationSucceeded`， `challengeValidationFailed`， `issueFailed`， `issuePending`， `issued`， `responseProcessingFailed`， `responsePending`， `enrollmentSucceeded`， `enrollmentNotNeeded`， `revoked`， `removedFromCollection`， `renewVerified`， `installFailed`， `installed`, `deleteFailed`, `deleted`, `renewalRequested`, `requested`.</span><span class="sxs-lookup"><span data-stu-id="6fddb-151">Possible values are: `unknown`, `challengeIssued`, `challengeIssueFailed`, `requestCreationFailed`, `requestSubmitFailed`, `challengeValidationSucceeded`, `challengeValidationFailed`, `issueFailed`, `issuePending`, `issued`, `responseProcessingFailed`, `responsePending`, `enrollmentSucceeded`, `enrollmentNotNeeded`, `revoked`, `removedFromCollection`, `renewVerified`, `installFailed`, `installed`, `deleteFailed`, `deleted`, `renewalRequested`, `requested`.</span></span>|
|<span data-ttu-id="6fddb-152">certificateKeyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="6fddb-152">certificateKeyStorageProvider</span></span>|[<span data-ttu-id="6fddb-153">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="6fddb-153">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="6fddb-154">密钥存储提供程序。</span><span class="sxs-lookup"><span data-stu-id="6fddb-154">Key Storage Provider.</span></span> <span data-ttu-id="6fddb-155">可取值为：`useTpmKspOtherwiseUseSoftwareKsp`、`useTpmKspOtherwiseFail`、`usePassportForWorkKspOtherwiseFail`、`useSoftwareKsp`。</span><span class="sxs-lookup"><span data-stu-id="6fddb-155">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="6fddb-156">certificateSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="6fddb-156">certificateSubjectNameFormat</span></span>|[<span data-ttu-id="6fddb-157">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="6fddb-157">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="6fddb-158">使用者名称格式。</span><span class="sxs-lookup"><span data-stu-id="6fddb-158">Subject name format.</span></span> <span data-ttu-id="6fddb-159">可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。</span><span class="sxs-lookup"><span data-stu-id="6fddb-159">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="6fddb-160">certificateSubjectAlternativeNameFormat</span><span class="sxs-lookup"><span data-stu-id="6fddb-160">certificateSubjectAlternativeNameFormat</span></span>|[<span data-ttu-id="6fddb-161">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="6fddb-161">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="6fddb-162">使用者替代名称格式。</span><span class="sxs-lookup"><span data-stu-id="6fddb-162">Subject alternative name format.</span></span> <span data-ttu-id="6fddb-163">可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`。</span><span class="sxs-lookup"><span data-stu-id="6fddb-163">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="6fddb-164">certificateRevokeStatus</span><span class="sxs-lookup"><span data-stu-id="6fddb-164">certificateRevokeStatus</span></span>|[<span data-ttu-id="6fddb-165">certificateRevocationStatus</span><span class="sxs-lookup"><span data-stu-id="6fddb-165">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="6fddb-166">吊销状态。</span><span class="sxs-lookup"><span data-stu-id="6fddb-166">Revoke status.</span></span> <span data-ttu-id="6fddb-167">可取值为：`none`、`pending`、`issued`、`failed`、`revoked`。</span><span class="sxs-lookup"><span data-stu-id="6fddb-167">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="6fddb-168">certificateProfileDisplayName</span><span class="sxs-lookup"><span data-stu-id="6fddb-168">certificateProfileDisplayName</span></span>|<span data-ttu-id="6fddb-169">字符串</span><span class="sxs-lookup"><span data-stu-id="6fddb-169">String</span></span>|<span data-ttu-id="6fddb-170">证书配置文件的显示名称</span><span class="sxs-lookup"><span data-stu-id="6fddb-170">Certificate profile display name</span></span>|
|<span data-ttu-id="6fddb-171">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="6fddb-171">deviceDisplayName</span></span>|<span data-ttu-id="6fddb-172">String</span><span class="sxs-lookup"><span data-stu-id="6fddb-172">String</span></span>|<span data-ttu-id="6fddb-173">设备显示名称</span><span class="sxs-lookup"><span data-stu-id="6fddb-173">Device display name</span></span>|
|<span data-ttu-id="6fddb-174">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="6fddb-174">userDisplayName</span></span>|<span data-ttu-id="6fddb-175">String</span><span class="sxs-lookup"><span data-stu-id="6fddb-175">String</span></span>|<span data-ttu-id="6fddb-176">用户显示名称</span><span class="sxs-lookup"><span data-stu-id="6fddb-176">User display name</span></span>|
|<span data-ttu-id="6fddb-177">certificateExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="6fddb-177">certificateExpirationDateTime</span></span>|<span data-ttu-id="6fddb-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6fddb-178">DateTimeOffset</span></span>|<span data-ttu-id="6fddb-179">证书到期日期</span><span class="sxs-lookup"><span data-stu-id="6fddb-179">Certificate expiry date</span></span>|
|<span data-ttu-id="6fddb-180">certificateLastIssuanceStateChangedDateTime</span><span class="sxs-lookup"><span data-stu-id="6fddb-180">certificateLastIssuanceStateChangedDateTime</span></span>|<span data-ttu-id="6fddb-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6fddb-181">DateTimeOffset</span></span>|<span data-ttu-id="6fddb-182">最后一个证书颁发状态更改</span><span class="sxs-lookup"><span data-stu-id="6fddb-182">Last certificate issuance state change</span></span>|
|<span data-ttu-id="6fddb-183">lastCertificateStateChangeDateTime</span><span class="sxs-lookup"><span data-stu-id="6fddb-183">lastCertificateStateChangeDateTime</span></span>|<span data-ttu-id="6fddb-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6fddb-184">DateTimeOffset</span></span>|<span data-ttu-id="6fddb-185">最后一个证书颁发状态更改</span><span class="sxs-lookup"><span data-stu-id="6fddb-185">Last certificate issuance state change</span></span>|
|<span data-ttu-id="6fddb-186">certificateIssuer</span><span class="sxs-lookup"><span data-stu-id="6fddb-186">certificateIssuer</span></span>|<span data-ttu-id="6fddb-187">字符串</span><span class="sxs-lookup"><span data-stu-id="6fddb-187">String</span></span>|<span data-ttu-id="6fddb-188">颁发者</span><span class="sxs-lookup"><span data-stu-id="6fddb-188">Issuer</span></span>|
|<span data-ttu-id="6fddb-189">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="6fddb-189">certificateThumbprint</span></span>|<span data-ttu-id="6fddb-190">字符串</span><span class="sxs-lookup"><span data-stu-id="6fddb-190">String</span></span>|<span data-ttu-id="6fddb-191">指纹</span><span class="sxs-lookup"><span data-stu-id="6fddb-191">Thumbprint</span></span>|
|<span data-ttu-id="6fddb-192">certificateSerialNumber</span><span class="sxs-lookup"><span data-stu-id="6fddb-192">certificateSerialNumber</span></span>|<span data-ttu-id="6fddb-193">字符串</span><span class="sxs-lookup"><span data-stu-id="6fddb-193">String</span></span>|<span data-ttu-id="6fddb-194">序列号</span><span class="sxs-lookup"><span data-stu-id="6fddb-194">Serial number</span></span>|
|<span data-ttu-id="6fddb-195">certificateKeyLength</span><span class="sxs-lookup"><span data-stu-id="6fddb-195">certificateKeyLength</span></span>|<span data-ttu-id="6fddb-196">Int32</span><span class="sxs-lookup"><span data-stu-id="6fddb-196">Int32</span></span>|<span data-ttu-id="6fddb-197">密钥长度</span><span class="sxs-lookup"><span data-stu-id="6fddb-197">Key length</span></span>|
|<span data-ttu-id="6fddb-198">certificateEnhancedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="6fddb-198">certificateEnhancedKeyUsage</span></span>|<span data-ttu-id="6fddb-199">字符串</span><span class="sxs-lookup"><span data-stu-id="6fddb-199">String</span></span>|<span data-ttu-id="6fddb-200">扩展的密钥用法</span><span class="sxs-lookup"><span data-stu-id="6fddb-200">Extended key usage</span></span>|
|<span data-ttu-id="6fddb-201">certificateValidityPeriod</span><span class="sxs-lookup"><span data-stu-id="6fddb-201">certificateValidityPeriod</span></span>|<span data-ttu-id="6fddb-202">Int32</span><span class="sxs-lookup"><span data-stu-id="6fddb-202">Int32</span></span>|<span data-ttu-id="6fddb-203">有效期</span><span class="sxs-lookup"><span data-stu-id="6fddb-203">Validity period</span></span>|
|<span data-ttu-id="6fddb-204">certificateSubjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="6fddb-204">certificateSubjectNameFormatString</span></span>|<span data-ttu-id="6fddb-205">字符串</span><span class="sxs-lookup"><span data-stu-id="6fddb-205">String</span></span>|<span data-ttu-id="6fddb-206">自定义主题名称格式的使用者名称格式字符串</span><span class="sxs-lookup"><span data-stu-id="6fddb-206">Subject name format string for custom subject name formats</span></span>|
|<span data-ttu-id="6fddb-207">certificateSubjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="6fddb-207">certificateSubjectAlternativeNameFormatString</span></span>|<span data-ttu-id="6fddb-208">字符串</span><span class="sxs-lookup"><span data-stu-id="6fddb-208">String</span></span>|<span data-ttu-id="6fddb-209">自定义格式的使用者替代名称格式字符串</span><span class="sxs-lookup"><span data-stu-id="6fddb-209">Subject alternative name format string for custom formats</span></span>|
|<span data-ttu-id="6fddb-210">certificateIssuanceDateTime</span><span class="sxs-lookup"><span data-stu-id="6fddb-210">certificateIssuanceDateTime</span></span>|<span data-ttu-id="6fddb-211">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6fddb-211">DateTimeOffset</span></span>|<span data-ttu-id="6fddb-212">发布日期</span><span class="sxs-lookup"><span data-stu-id="6fddb-212">Issuance date</span></span>|
|<span data-ttu-id="6fddb-213">certificateErrorCode</span><span class="sxs-lookup"><span data-stu-id="6fddb-213">certificateErrorCode</span></span>|<span data-ttu-id="6fddb-214">Int32</span><span class="sxs-lookup"><span data-stu-id="6fddb-214">Int32</span></span>|<span data-ttu-id="6fddb-215">错误代码</span><span class="sxs-lookup"><span data-stu-id="6fddb-215">Error code</span></span>|



## <a name="response"></a><span data-ttu-id="6fddb-216">响应</span><span class="sxs-lookup"><span data-stu-id="6fddb-216">Response</span></span>
<span data-ttu-id="6fddb-217">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6fddb-217">If successful, this method returns a `200 OK` response code and an updated [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6fddb-218">示例</span><span class="sxs-lookup"><span data-stu-id="6fddb-218">Example</span></span>
### <a name="request"></a><span data-ttu-id="6fddb-219">请求</span><span class="sxs-lookup"><span data-stu-id="6fddb-219">Request</span></span>
<span data-ttu-id="6fddb-220">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6fddb-220">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
Content-type: application/json
Content-length: 1449

{
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

### <a name="response"></a><span data-ttu-id="6fddb-221">响应</span><span class="sxs-lookup"><span data-stu-id="6fddb-221">Response</span></span>
<span data-ttu-id="6fddb-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6fddb-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





