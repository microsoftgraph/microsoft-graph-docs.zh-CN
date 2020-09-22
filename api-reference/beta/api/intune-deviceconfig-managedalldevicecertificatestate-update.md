---
title: 更新 managedAllDeviceCertificateState
description: 更新 managedAllDeviceCertificateState 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d445652f6605be74806f762e09f62a9c11b588ef
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48065793"
---
# <a name="update-managedalldevicecertificatestate"></a><span data-ttu-id="cdbdd-103">更新 managedAllDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="cdbdd-103">Update managedAllDeviceCertificateState</span></span>

<span data-ttu-id="cdbdd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cdbdd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cdbdd-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cdbdd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cdbdd-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cdbdd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cdbdd-107">更新 [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="cdbdd-107">Update the properties of a [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cdbdd-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="cdbdd-108">Prerequisites</span></span>
<span data-ttu-id="cdbdd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cdbdd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cdbdd-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="cdbdd-111">Permission type</span></span>|<span data-ttu-id="cdbdd-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cdbdd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cdbdd-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cdbdd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cdbdd-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdbdd-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cdbdd-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cdbdd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cdbdd-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cdbdd-116">Not supported.</span></span>|
|<span data-ttu-id="cdbdd-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="cdbdd-117">Application</span></span>|<span data-ttu-id="cdbdd-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdbdd-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cdbdd-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cdbdd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates/{managedAllDeviceCertificateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="cdbdd-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="cdbdd-120">Request headers</span></span>
|<span data-ttu-id="cdbdd-121">标头</span><span class="sxs-lookup"><span data-stu-id="cdbdd-121">Header</span></span>|<span data-ttu-id="cdbdd-122">值</span><span class="sxs-lookup"><span data-stu-id="cdbdd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cdbdd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cdbdd-123">Authorization</span></span>|<span data-ttu-id="cdbdd-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cdbdd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cdbdd-125">接受</span><span class="sxs-lookup"><span data-stu-id="cdbdd-125">Accept</span></span>|<span data-ttu-id="cdbdd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cdbdd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cdbdd-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="cdbdd-127">Request body</span></span>
<span data-ttu-id="cdbdd-128">在请求正文中，提供 [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cdbdd-128">In the request body, supply a JSON representation for the [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

<span data-ttu-id="cdbdd-129">下表显示创建 [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="cdbdd-129">The following table shows the properties that are required when you create the [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md).</span></span>

|<span data-ttu-id="cdbdd-130">属性</span><span class="sxs-lookup"><span data-stu-id="cdbdd-130">Property</span></span>|<span data-ttu-id="cdbdd-131">类型</span><span class="sxs-lookup"><span data-stu-id="cdbdd-131">Type</span></span>|<span data-ttu-id="cdbdd-132">说明</span><span class="sxs-lookup"><span data-stu-id="cdbdd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cdbdd-133">id</span><span class="sxs-lookup"><span data-stu-id="cdbdd-133">id</span></span>|<span data-ttu-id="cdbdd-134">String</span><span class="sxs-lookup"><span data-stu-id="cdbdd-134">String</span></span>|<span data-ttu-id="cdbdd-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="cdbdd-135">Key of the entity.</span></span>|
|<span data-ttu-id="cdbdd-136">certificateRevokeStatus</span><span class="sxs-lookup"><span data-stu-id="cdbdd-136">certificateRevokeStatus</span></span>|[<span data-ttu-id="cdbdd-137">certificateRevocationStatus</span><span class="sxs-lookup"><span data-stu-id="cdbdd-137">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="cdbdd-138">撤消状态。</span><span class="sxs-lookup"><span data-stu-id="cdbdd-138">Revoke status.</span></span> <span data-ttu-id="cdbdd-139">可取值为：`none`、`pending`、`issued`、`failed`、`revoked`。</span><span class="sxs-lookup"><span data-stu-id="cdbdd-139">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="cdbdd-140">certificateRevokeStatusLastChangeDateTime</span><span class="sxs-lookup"><span data-stu-id="cdbdd-140">certificateRevokeStatusLastChangeDateTime</span></span>|<span data-ttu-id="cdbdd-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cdbdd-141">DateTimeOffset</span></span>|<span data-ttu-id="cdbdd-142">上次更改吊销状态的时间</span><span class="sxs-lookup"><span data-stu-id="cdbdd-142">The time the revoke status was last changed</span></span>|
|<span data-ttu-id="cdbdd-143">managedDeviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="cdbdd-143">managedDeviceDisplayName</span></span>|<span data-ttu-id="cdbdd-144">String</span><span class="sxs-lookup"><span data-stu-id="cdbdd-144">String</span></span>|<span data-ttu-id="cdbdd-145">设备显示名称</span><span class="sxs-lookup"><span data-stu-id="cdbdd-145">Device display name</span></span>|
|<span data-ttu-id="cdbdd-146">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="cdbdd-146">userPrincipalName</span></span>|<span data-ttu-id="cdbdd-147">String</span><span class="sxs-lookup"><span data-stu-id="cdbdd-147">String</span></span>|<span data-ttu-id="cdbdd-148">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="cdbdd-148">User principal name</span></span>|
|<span data-ttu-id="cdbdd-149">certificateExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="cdbdd-149">certificateExpirationDateTime</span></span>|<span data-ttu-id="cdbdd-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cdbdd-150">DateTimeOffset</span></span>|<span data-ttu-id="cdbdd-151">证书到期日期</span><span class="sxs-lookup"><span data-stu-id="cdbdd-151">Certificate expiry date</span></span>|
|<span data-ttu-id="cdbdd-152">certificateIssuerName</span><span class="sxs-lookup"><span data-stu-id="cdbdd-152">certificateIssuerName</span></span>|<span data-ttu-id="cdbdd-153">String</span><span class="sxs-lookup"><span data-stu-id="cdbdd-153">String</span></span>|<span data-ttu-id="cdbdd-154">颁发者</span><span class="sxs-lookup"><span data-stu-id="cdbdd-154">Issuer</span></span>|
|<span data-ttu-id="cdbdd-155">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="cdbdd-155">certificateThumbprint</span></span>|<span data-ttu-id="cdbdd-156">String</span><span class="sxs-lookup"><span data-stu-id="cdbdd-156">String</span></span>|<span data-ttu-id="cdbdd-157">为</span><span class="sxs-lookup"><span data-stu-id="cdbdd-157">Thumbprint</span></span>|
|<span data-ttu-id="cdbdd-158">certificateSerialNumber</span><span class="sxs-lookup"><span data-stu-id="cdbdd-158">certificateSerialNumber</span></span>|<span data-ttu-id="cdbdd-159">String</span><span class="sxs-lookup"><span data-stu-id="cdbdd-159">String</span></span>|<span data-ttu-id="cdbdd-160">序列号</span><span class="sxs-lookup"><span data-stu-id="cdbdd-160">Serial number</span></span>|
|<span data-ttu-id="cdbdd-161">certificateSubjectName</span><span class="sxs-lookup"><span data-stu-id="cdbdd-161">certificateSubjectName</span></span>|<span data-ttu-id="cdbdd-162">String</span><span class="sxs-lookup"><span data-stu-id="cdbdd-162">String</span></span>|<span data-ttu-id="cdbdd-163">证书主题名称</span><span class="sxs-lookup"><span data-stu-id="cdbdd-163">Certificate subject name</span></span>|
|<span data-ttu-id="cdbdd-164">certificateKeyUsages</span><span class="sxs-lookup"><span data-stu-id="cdbdd-164">certificateKeyUsages</span></span>|<span data-ttu-id="cdbdd-165">Int32</span><span class="sxs-lookup"><span data-stu-id="cdbdd-165">Int32</span></span>|<span data-ttu-id="cdbdd-166">密钥用法</span><span class="sxs-lookup"><span data-stu-id="cdbdd-166">Key Usage</span></span>|
|<span data-ttu-id="cdbdd-167">certificateExtendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="cdbdd-167">certificateExtendedKeyUsages</span></span>|<span data-ttu-id="cdbdd-168">String</span><span class="sxs-lookup"><span data-stu-id="cdbdd-168">String</span></span>|<span data-ttu-id="cdbdd-169">增强型密钥使用</span><span class="sxs-lookup"><span data-stu-id="cdbdd-169">Enhanced Key Usage</span></span>|
|<span data-ttu-id="cdbdd-170">certificateIssuanceDateTime</span><span class="sxs-lookup"><span data-stu-id="cdbdd-170">certificateIssuanceDateTime</span></span>|<span data-ttu-id="cdbdd-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cdbdd-171">DateTimeOffset</span></span>|<span data-ttu-id="cdbdd-172">颁发日期</span><span class="sxs-lookup"><span data-stu-id="cdbdd-172">Issuance date</span></span>|



## <a name="response"></a><span data-ttu-id="cdbdd-173">响应</span><span class="sxs-lookup"><span data-stu-id="cdbdd-173">Response</span></span>
<span data-ttu-id="cdbdd-174">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cdbdd-174">If successful, this method returns a `200 OK` response code and an updated [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cdbdd-175">示例</span><span class="sxs-lookup"><span data-stu-id="cdbdd-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="cdbdd-176">请求</span><span class="sxs-lookup"><span data-stu-id="cdbdd-176">Request</span></span>
<span data-ttu-id="cdbdd-177">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cdbdd-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cdbdd-178">响应</span><span class="sxs-lookup"><span data-stu-id="cdbdd-178">Response</span></span>
<span data-ttu-id="cdbdd-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cdbdd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






