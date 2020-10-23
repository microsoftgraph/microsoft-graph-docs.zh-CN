---
title: 更新 managedAllDeviceCertificateState
description: 更新 managedAllDeviceCertificateState 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 82e9192aa6a99e5e7ce35ad9e5208ff098c97612
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48693470"
---
# <a name="update-managedalldevicecertificatestate"></a><span data-ttu-id="bca07-103">更新 managedAllDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="bca07-103">Update managedAllDeviceCertificateState</span></span>

<span data-ttu-id="bca07-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bca07-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bca07-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bca07-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bca07-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bca07-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bca07-107">更新 [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="bca07-107">Update the properties of a [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bca07-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="bca07-108">Prerequisites</span></span>
<span data-ttu-id="bca07-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bca07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bca07-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="bca07-111">Permission type</span></span>|<span data-ttu-id="bca07-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bca07-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bca07-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bca07-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bca07-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bca07-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bca07-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bca07-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bca07-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bca07-116">Not supported.</span></span>|
|<span data-ttu-id="bca07-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="bca07-117">Application</span></span>|<span data-ttu-id="bca07-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bca07-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bca07-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bca07-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates/{managedAllDeviceCertificateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="bca07-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="bca07-120">Request headers</span></span>
|<span data-ttu-id="bca07-121">标头</span><span class="sxs-lookup"><span data-stu-id="bca07-121">Header</span></span>|<span data-ttu-id="bca07-122">值</span><span class="sxs-lookup"><span data-stu-id="bca07-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bca07-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bca07-123">Authorization</span></span>|<span data-ttu-id="bca07-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bca07-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bca07-125">接受</span><span class="sxs-lookup"><span data-stu-id="bca07-125">Accept</span></span>|<span data-ttu-id="bca07-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bca07-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bca07-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bca07-127">Request body</span></span>
<span data-ttu-id="bca07-128">在请求正文中，提供 [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bca07-128">In the request body, supply a JSON representation for the [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

<span data-ttu-id="bca07-129">下表显示创建 [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="bca07-129">The following table shows the properties that are required when you create the [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md).</span></span>

|<span data-ttu-id="bca07-130">属性</span><span class="sxs-lookup"><span data-stu-id="bca07-130">Property</span></span>|<span data-ttu-id="bca07-131">类型</span><span class="sxs-lookup"><span data-stu-id="bca07-131">Type</span></span>|<span data-ttu-id="bca07-132">说明</span><span class="sxs-lookup"><span data-stu-id="bca07-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bca07-133">id</span><span class="sxs-lookup"><span data-stu-id="bca07-133">id</span></span>|<span data-ttu-id="bca07-134">String</span><span class="sxs-lookup"><span data-stu-id="bca07-134">String</span></span>|<span data-ttu-id="bca07-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="bca07-135">Key of the entity.</span></span>|
|<span data-ttu-id="bca07-136">certificateRevokeStatus</span><span class="sxs-lookup"><span data-stu-id="bca07-136">certificateRevokeStatus</span></span>|[<span data-ttu-id="bca07-137">certificateRevocationStatus</span><span class="sxs-lookup"><span data-stu-id="bca07-137">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="bca07-138">撤消状态。</span><span class="sxs-lookup"><span data-stu-id="bca07-138">Revoke status.</span></span> <span data-ttu-id="bca07-139">可取值为：`none`、`pending`、`issued`、`failed`、`revoked`。</span><span class="sxs-lookup"><span data-stu-id="bca07-139">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="bca07-140">certificateRevokeStatusLastChangeDateTime</span><span class="sxs-lookup"><span data-stu-id="bca07-140">certificateRevokeStatusLastChangeDateTime</span></span>|<span data-ttu-id="bca07-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bca07-141">DateTimeOffset</span></span>|<span data-ttu-id="bca07-142">上次更改吊销状态的时间</span><span class="sxs-lookup"><span data-stu-id="bca07-142">The time the revoke status was last changed</span></span>|
|<span data-ttu-id="bca07-143">managedDeviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="bca07-143">managedDeviceDisplayName</span></span>|<span data-ttu-id="bca07-144">String</span><span class="sxs-lookup"><span data-stu-id="bca07-144">String</span></span>|<span data-ttu-id="bca07-145">设备显示名称</span><span class="sxs-lookup"><span data-stu-id="bca07-145">Device display name</span></span>|
|<span data-ttu-id="bca07-146">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="bca07-146">userPrincipalName</span></span>|<span data-ttu-id="bca07-147">String</span><span class="sxs-lookup"><span data-stu-id="bca07-147">String</span></span>|<span data-ttu-id="bca07-148">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="bca07-148">User principal name</span></span>|
|<span data-ttu-id="bca07-149">certificateExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="bca07-149">certificateExpirationDateTime</span></span>|<span data-ttu-id="bca07-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bca07-150">DateTimeOffset</span></span>|<span data-ttu-id="bca07-151">证书到期日期</span><span class="sxs-lookup"><span data-stu-id="bca07-151">Certificate expiry date</span></span>|
|<span data-ttu-id="bca07-152">certificateIssuerName</span><span class="sxs-lookup"><span data-stu-id="bca07-152">certificateIssuerName</span></span>|<span data-ttu-id="bca07-153">String</span><span class="sxs-lookup"><span data-stu-id="bca07-153">String</span></span>|<span data-ttu-id="bca07-154">颁发者</span><span class="sxs-lookup"><span data-stu-id="bca07-154">Issuer</span></span>|
|<span data-ttu-id="bca07-155">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="bca07-155">certificateThumbprint</span></span>|<span data-ttu-id="bca07-156">String</span><span class="sxs-lookup"><span data-stu-id="bca07-156">String</span></span>|<span data-ttu-id="bca07-157">指纹</span><span class="sxs-lookup"><span data-stu-id="bca07-157">Thumbprint</span></span>|
|<span data-ttu-id="bca07-158">certificateSerialNumber</span><span class="sxs-lookup"><span data-stu-id="bca07-158">certificateSerialNumber</span></span>|<span data-ttu-id="bca07-159">String</span><span class="sxs-lookup"><span data-stu-id="bca07-159">String</span></span>|<span data-ttu-id="bca07-160">序列号</span><span class="sxs-lookup"><span data-stu-id="bca07-160">Serial number</span></span>|
|<span data-ttu-id="bca07-161">certificateSubjectName</span><span class="sxs-lookup"><span data-stu-id="bca07-161">certificateSubjectName</span></span>|<span data-ttu-id="bca07-162">String</span><span class="sxs-lookup"><span data-stu-id="bca07-162">String</span></span>|<span data-ttu-id="bca07-163">证书主题名称</span><span class="sxs-lookup"><span data-stu-id="bca07-163">Certificate subject name</span></span>|
|<span data-ttu-id="bca07-164">certificateKeyUsages</span><span class="sxs-lookup"><span data-stu-id="bca07-164">certificateKeyUsages</span></span>|<span data-ttu-id="bca07-165">Int32</span><span class="sxs-lookup"><span data-stu-id="bca07-165">Int32</span></span>|<span data-ttu-id="bca07-166">密钥用法</span><span class="sxs-lookup"><span data-stu-id="bca07-166">Key Usage</span></span>|
|<span data-ttu-id="bca07-167">certificateExtendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="bca07-167">certificateExtendedKeyUsages</span></span>|<span data-ttu-id="bca07-168">String</span><span class="sxs-lookup"><span data-stu-id="bca07-168">String</span></span>|<span data-ttu-id="bca07-169">增强型密钥使用</span><span class="sxs-lookup"><span data-stu-id="bca07-169">Enhanced Key Usage</span></span>|
|<span data-ttu-id="bca07-170">certificateIssuanceDateTime</span><span class="sxs-lookup"><span data-stu-id="bca07-170">certificateIssuanceDateTime</span></span>|<span data-ttu-id="bca07-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bca07-171">DateTimeOffset</span></span>|<span data-ttu-id="bca07-172">颁发日期</span><span class="sxs-lookup"><span data-stu-id="bca07-172">Issuance date</span></span>|



## <a name="response"></a><span data-ttu-id="bca07-173">响应</span><span class="sxs-lookup"><span data-stu-id="bca07-173">Response</span></span>
<span data-ttu-id="bca07-174">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bca07-174">If successful, this method returns a `200 OK` response code and an updated [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bca07-175">示例</span><span class="sxs-lookup"><span data-stu-id="bca07-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="bca07-176">请求</span><span class="sxs-lookup"><span data-stu-id="bca07-176">Request</span></span>
<span data-ttu-id="bca07-177">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bca07-177">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates/{managedAllDeviceCertificateStateId}
Content-type: application/json
Content-length: 820

{
  "@odata.type": "#microsoft.graph.managedAllDeviceCertificateState",
  "certificateRevokeStatus": "pending",
  "certificateRevokeStatusLastChangeDateTime": "2016-12-31T23:59:34.9547208-08:00",
  "managedDeviceDisplayName": "Managed Device Display Name value",
  "userPrincipalName": "User Principal Name value",
  "certificateExpirationDateTime": "2017-01-01T00:02:14.9489247-08:00",
  "certificateIssuerName": "Certificate Issuer Name value",
  "certificateThumbprint": "Certificate Thumbprint value",
  "certificateSerialNumber": "Certificate Serial Number value",
  "certificateSubjectName": "Certificate Subject Name value",
  "certificateKeyUsages": 4,
  "certificateExtendedKeyUsages": "Certificate Extended Key Usages value",
  "certificateIssuanceDateTime": "2016-12-31T23:59:41.5044473-08:00"
}
```

### <a name="response"></a><span data-ttu-id="bca07-178">响应</span><span class="sxs-lookup"><span data-stu-id="bca07-178">Response</span></span>
<span data-ttu-id="bca07-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bca07-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 869

{
  "@odata.type": "#microsoft.graph.managedAllDeviceCertificateState",
  "id": "987c6a17-6a17-987c-176a-7c98176a7c98",
  "certificateRevokeStatus": "pending",
  "certificateRevokeStatusLastChangeDateTime": "2016-12-31T23:59:34.9547208-08:00",
  "managedDeviceDisplayName": "Managed Device Display Name value",
  "userPrincipalName": "User Principal Name value",
  "certificateExpirationDateTime": "2017-01-01T00:02:14.9489247-08:00",
  "certificateIssuerName": "Certificate Issuer Name value",
  "certificateThumbprint": "Certificate Thumbprint value",
  "certificateSerialNumber": "Certificate Serial Number value",
  "certificateSubjectName": "Certificate Subject Name value",
  "certificateKeyUsages": 4,
  "certificateExtendedKeyUsages": "Certificate Extended Key Usages value",
  "certificateIssuanceDateTime": "2016-12-31T23:59:41.5044473-08:00"
}
```





