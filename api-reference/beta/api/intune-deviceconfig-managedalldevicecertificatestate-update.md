---
title: 更新 managedAllDeviceCertificateState
description: 更新 managedAllDeviceCertificateState 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: feb45298263ee3fe4a3d02ec03f729dd7d2d382f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51155139"
---
# <a name="update-managedalldevicecertificatestate"></a><span data-ttu-id="23503-103">更新 managedAllDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="23503-103">Update managedAllDeviceCertificateState</span></span>

<span data-ttu-id="23503-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23503-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="23503-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="23503-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="23503-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="23503-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23503-107">更新 [managedAllDeviceCertificateState 对象](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="23503-107">Update the properties of a [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="23503-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="23503-108">Prerequisites</span></span>
<span data-ttu-id="23503-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="23503-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23503-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="23503-111">Permission type</span></span>|<span data-ttu-id="23503-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="23503-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="23503-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="23503-113">Delegated (work or school account)</span></span>|<span data-ttu-id="23503-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23503-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="23503-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="23503-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="23503-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="23503-116">Not supported.</span></span>|
|<span data-ttu-id="23503-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="23503-117">Application</span></span>|<span data-ttu-id="23503-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23503-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="23503-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="23503-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates/{managedAllDeviceCertificateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="23503-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="23503-120">Request headers</span></span>
|<span data-ttu-id="23503-121">标头</span><span class="sxs-lookup"><span data-stu-id="23503-121">Header</span></span>|<span data-ttu-id="23503-122">值</span><span class="sxs-lookup"><span data-stu-id="23503-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="23503-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="23503-123">Authorization</span></span>|<span data-ttu-id="23503-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="23503-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="23503-125">接受</span><span class="sxs-lookup"><span data-stu-id="23503-125">Accept</span></span>|<span data-ttu-id="23503-126">application/json</span><span class="sxs-lookup"><span data-stu-id="23503-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="23503-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="23503-127">Request body</span></span>
<span data-ttu-id="23503-128">在请求正文中，提供 [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="23503-128">In the request body, supply a JSON representation for the [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

<span data-ttu-id="23503-129">下表显示创建 [managedAllDeviceCertificateState 时所需的属性](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)。</span><span class="sxs-lookup"><span data-stu-id="23503-129">The following table shows the properties that are required when you create the [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md).</span></span>

|<span data-ttu-id="23503-130">属性</span><span class="sxs-lookup"><span data-stu-id="23503-130">Property</span></span>|<span data-ttu-id="23503-131">类型</span><span class="sxs-lookup"><span data-stu-id="23503-131">Type</span></span>|<span data-ttu-id="23503-132">说明</span><span class="sxs-lookup"><span data-stu-id="23503-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23503-133">id</span><span class="sxs-lookup"><span data-stu-id="23503-133">id</span></span>|<span data-ttu-id="23503-134">String</span><span class="sxs-lookup"><span data-stu-id="23503-134">String</span></span>|<span data-ttu-id="23503-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="23503-135">Key of the entity.</span></span>|
|<span data-ttu-id="23503-136">certificateRevokeStatus</span><span class="sxs-lookup"><span data-stu-id="23503-136">certificateRevokeStatus</span></span>|[<span data-ttu-id="23503-137">certificateRevocationStatus</span><span class="sxs-lookup"><span data-stu-id="23503-137">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="23503-138">撤销状态。</span><span class="sxs-lookup"><span data-stu-id="23503-138">Revoke status.</span></span> <span data-ttu-id="23503-139">可取值为：`none`、`pending`、`issued`、`failed`、`revoked`。</span><span class="sxs-lookup"><span data-stu-id="23503-139">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="23503-140">certificateRevokeStatusLastChangeDateTime</span><span class="sxs-lookup"><span data-stu-id="23503-140">certificateRevokeStatusLastChangeDateTime</span></span>|<span data-ttu-id="23503-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23503-141">DateTimeOffset</span></span>|<span data-ttu-id="23503-142">上次更改撤消状态的时间</span><span class="sxs-lookup"><span data-stu-id="23503-142">The time the revoke status was last changed</span></span>|
|<span data-ttu-id="23503-143">managedDeviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="23503-143">managedDeviceDisplayName</span></span>|<span data-ttu-id="23503-144">String</span><span class="sxs-lookup"><span data-stu-id="23503-144">String</span></span>|<span data-ttu-id="23503-145">设备显示名称</span><span class="sxs-lookup"><span data-stu-id="23503-145">Device display name</span></span>|
|<span data-ttu-id="23503-146">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="23503-146">userPrincipalName</span></span>|<span data-ttu-id="23503-147">String</span><span class="sxs-lookup"><span data-stu-id="23503-147">String</span></span>|<span data-ttu-id="23503-148">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="23503-148">User principal name</span></span>|
|<span data-ttu-id="23503-149">certificateExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="23503-149">certificateExpirationDateTime</span></span>|<span data-ttu-id="23503-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23503-150">DateTimeOffset</span></span>|<span data-ttu-id="23503-151">证书到期日期</span><span class="sxs-lookup"><span data-stu-id="23503-151">Certificate expiry date</span></span>|
|<span data-ttu-id="23503-152">certificateIssuerName</span><span class="sxs-lookup"><span data-stu-id="23503-152">certificateIssuerName</span></span>|<span data-ttu-id="23503-153">String</span><span class="sxs-lookup"><span data-stu-id="23503-153">String</span></span>|<span data-ttu-id="23503-154">颁发者</span><span class="sxs-lookup"><span data-stu-id="23503-154">Issuer</span></span>|
|<span data-ttu-id="23503-155">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="23503-155">certificateThumbprint</span></span>|<span data-ttu-id="23503-156">String</span><span class="sxs-lookup"><span data-stu-id="23503-156">String</span></span>|<span data-ttu-id="23503-157">指纹</span><span class="sxs-lookup"><span data-stu-id="23503-157">Thumbprint</span></span>|
|<span data-ttu-id="23503-158">certificateSerialNumber</span><span class="sxs-lookup"><span data-stu-id="23503-158">certificateSerialNumber</span></span>|<span data-ttu-id="23503-159">String</span><span class="sxs-lookup"><span data-stu-id="23503-159">String</span></span>|<span data-ttu-id="23503-160">序列号</span><span class="sxs-lookup"><span data-stu-id="23503-160">Serial number</span></span>|
|<span data-ttu-id="23503-161">certificateSubjectName</span><span class="sxs-lookup"><span data-stu-id="23503-161">certificateSubjectName</span></span>|<span data-ttu-id="23503-162">String</span><span class="sxs-lookup"><span data-stu-id="23503-162">String</span></span>|<span data-ttu-id="23503-163">证书主题名称</span><span class="sxs-lookup"><span data-stu-id="23503-163">Certificate subject name</span></span>|
|<span data-ttu-id="23503-164">certificateKeyUsages</span><span class="sxs-lookup"><span data-stu-id="23503-164">certificateKeyUsages</span></span>|<span data-ttu-id="23503-165">Int32</span><span class="sxs-lookup"><span data-stu-id="23503-165">Int32</span></span>|<span data-ttu-id="23503-166">密钥用法</span><span class="sxs-lookup"><span data-stu-id="23503-166">Key Usage</span></span>|
|<span data-ttu-id="23503-167">certificateExtendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="23503-167">certificateExtendedKeyUsages</span></span>|<span data-ttu-id="23503-168">String</span><span class="sxs-lookup"><span data-stu-id="23503-168">String</span></span>|<span data-ttu-id="23503-169">增强型密钥使用</span><span class="sxs-lookup"><span data-stu-id="23503-169">Enhanced Key Usage</span></span>|
|<span data-ttu-id="23503-170">certificateIssuanceDateTime</span><span class="sxs-lookup"><span data-stu-id="23503-170">certificateIssuanceDateTime</span></span>|<span data-ttu-id="23503-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23503-171">DateTimeOffset</span></span>|<span data-ttu-id="23503-172">发布日期</span><span class="sxs-lookup"><span data-stu-id="23503-172">Issuance date</span></span>|



## <a name="response"></a><span data-ttu-id="23503-173">响应</span><span class="sxs-lookup"><span data-stu-id="23503-173">Response</span></span>
<span data-ttu-id="23503-174">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="23503-174">If successful, this method returns a `200 OK` response code and an updated [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23503-175">示例</span><span class="sxs-lookup"><span data-stu-id="23503-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="23503-176">请求</span><span class="sxs-lookup"><span data-stu-id="23503-176">Request</span></span>
<span data-ttu-id="23503-177">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="23503-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="23503-178">响应</span><span class="sxs-lookup"><span data-stu-id="23503-178">Response</span></span>
<span data-ttu-id="23503-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="23503-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




