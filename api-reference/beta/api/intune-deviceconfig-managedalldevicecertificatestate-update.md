---
title: 更新 managedAllDeviceCertificateState
description: 更新 managedAllDeviceCertificateState 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fcd25b88d46eddadeedf6d53474e209cc70e3c10
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2020
ms.locfileid: "45122950"
---
# <a name="update-managedalldevicecertificatestate"></a><span data-ttu-id="7926e-103">更新 managedAllDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="7926e-103">Update managedAllDeviceCertificateState</span></span>

<span data-ttu-id="7926e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7926e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7926e-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7926e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7926e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7926e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7926e-107">更新[managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7926e-107">Update the properties of a [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7926e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7926e-108">Prerequisites</span></span>
<span data-ttu-id="7926e-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="7926e-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="7926e-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7926e-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7926e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7926e-111">Permission type</span></span>|<span data-ttu-id="7926e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7926e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7926e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7926e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7926e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7926e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7926e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7926e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7926e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7926e-116">Not supported.</span></span>|
|<span data-ttu-id="7926e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7926e-117">Application</span></span>|<span data-ttu-id="7926e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7926e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7926e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7926e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates/{managedAllDeviceCertificateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="7926e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7926e-120">Request headers</span></span>
|<span data-ttu-id="7926e-121">标头</span><span class="sxs-lookup"><span data-stu-id="7926e-121">Header</span></span>|<span data-ttu-id="7926e-122">值</span><span class="sxs-lookup"><span data-stu-id="7926e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7926e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7926e-123">Authorization</span></span>|<span data-ttu-id="7926e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7926e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7926e-125">接受</span><span class="sxs-lookup"><span data-stu-id="7926e-125">Accept</span></span>|<span data-ttu-id="7926e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7926e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7926e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7926e-127">Request body</span></span>
<span data-ttu-id="7926e-128">在请求正文中，提供[managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7926e-128">In the request body, supply a JSON representation for the [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

<span data-ttu-id="7926e-129">下表显示创建[managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7926e-129">The following table shows the properties that are required when you create the [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md).</span></span>

|<span data-ttu-id="7926e-130">属性</span><span class="sxs-lookup"><span data-stu-id="7926e-130">Property</span></span>|<span data-ttu-id="7926e-131">类型</span><span class="sxs-lookup"><span data-stu-id="7926e-131">Type</span></span>|<span data-ttu-id="7926e-132">说明</span><span class="sxs-lookup"><span data-stu-id="7926e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7926e-133">id</span><span class="sxs-lookup"><span data-stu-id="7926e-133">id</span></span>|<span data-ttu-id="7926e-134">String</span><span class="sxs-lookup"><span data-stu-id="7926e-134">String</span></span>|<span data-ttu-id="7926e-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="7926e-135">Key of the entity.</span></span>|
|<span data-ttu-id="7926e-136">certificateRevokeStatus</span><span class="sxs-lookup"><span data-stu-id="7926e-136">certificateRevokeStatus</span></span>|[<span data-ttu-id="7926e-137">certificateRevocationStatus</span><span class="sxs-lookup"><span data-stu-id="7926e-137">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="7926e-138">撤消状态。</span><span class="sxs-lookup"><span data-stu-id="7926e-138">Revoke status.</span></span> <span data-ttu-id="7926e-139">可取值为：`none`、`pending`、`issued`、`failed`、`revoked`。</span><span class="sxs-lookup"><span data-stu-id="7926e-139">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="7926e-140">certificateRevokeStatusLastChangeDateTime</span><span class="sxs-lookup"><span data-stu-id="7926e-140">certificateRevokeStatusLastChangeDateTime</span></span>|<span data-ttu-id="7926e-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7926e-141">DateTimeOffset</span></span>|<span data-ttu-id="7926e-142">上次更改吊销状态的时间</span><span class="sxs-lookup"><span data-stu-id="7926e-142">The time the revoke status was last changed</span></span>|
|<span data-ttu-id="7926e-143">managedDeviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="7926e-143">managedDeviceDisplayName</span></span>|<span data-ttu-id="7926e-144">String</span><span class="sxs-lookup"><span data-stu-id="7926e-144">String</span></span>|<span data-ttu-id="7926e-145">设备显示名称</span><span class="sxs-lookup"><span data-stu-id="7926e-145">Device display name</span></span>|
|<span data-ttu-id="7926e-146">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7926e-146">userPrincipalName</span></span>|<span data-ttu-id="7926e-147">String</span><span class="sxs-lookup"><span data-stu-id="7926e-147">String</span></span>|<span data-ttu-id="7926e-148">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="7926e-148">User principal name</span></span>|
|<span data-ttu-id="7926e-149">certificateExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="7926e-149">certificateExpirationDateTime</span></span>|<span data-ttu-id="7926e-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7926e-150">DateTimeOffset</span></span>|<span data-ttu-id="7926e-151">证书到期日期</span><span class="sxs-lookup"><span data-stu-id="7926e-151">Certificate expiry date</span></span>|
|<span data-ttu-id="7926e-152">certificateIssuerName</span><span class="sxs-lookup"><span data-stu-id="7926e-152">certificateIssuerName</span></span>|<span data-ttu-id="7926e-153">String</span><span class="sxs-lookup"><span data-stu-id="7926e-153">String</span></span>|<span data-ttu-id="7926e-154">颁发者</span><span class="sxs-lookup"><span data-stu-id="7926e-154">Issuer</span></span>|
|<span data-ttu-id="7926e-155">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="7926e-155">certificateThumbprint</span></span>|<span data-ttu-id="7926e-156">String</span><span class="sxs-lookup"><span data-stu-id="7926e-156">String</span></span>|<span data-ttu-id="7926e-157">为</span><span class="sxs-lookup"><span data-stu-id="7926e-157">Thumbprint</span></span>|
|<span data-ttu-id="7926e-158">certificateSerialNumber</span><span class="sxs-lookup"><span data-stu-id="7926e-158">certificateSerialNumber</span></span>|<span data-ttu-id="7926e-159">String</span><span class="sxs-lookup"><span data-stu-id="7926e-159">String</span></span>|<span data-ttu-id="7926e-160">序列号</span><span class="sxs-lookup"><span data-stu-id="7926e-160">Serial number</span></span>|
|<span data-ttu-id="7926e-161">certificateSubjectName</span><span class="sxs-lookup"><span data-stu-id="7926e-161">certificateSubjectName</span></span>|<span data-ttu-id="7926e-162">String</span><span class="sxs-lookup"><span data-stu-id="7926e-162">String</span></span>|<span data-ttu-id="7926e-163">证书主题名称</span><span class="sxs-lookup"><span data-stu-id="7926e-163">Certificate subject name</span></span>|
|<span data-ttu-id="7926e-164">certificateKeyUsages</span><span class="sxs-lookup"><span data-stu-id="7926e-164">certificateKeyUsages</span></span>|<span data-ttu-id="7926e-165">Int32</span><span class="sxs-lookup"><span data-stu-id="7926e-165">Int32</span></span>|<span data-ttu-id="7926e-166">密钥用法</span><span class="sxs-lookup"><span data-stu-id="7926e-166">Key Usage</span></span>|
|<span data-ttu-id="7926e-167">certificateExtendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="7926e-167">certificateExtendedKeyUsages</span></span>|<span data-ttu-id="7926e-168">String</span><span class="sxs-lookup"><span data-stu-id="7926e-168">String</span></span>|<span data-ttu-id="7926e-169">增强型密钥使用</span><span class="sxs-lookup"><span data-stu-id="7926e-169">Enhanced Key Usage</span></span>|
|<span data-ttu-id="7926e-170">certificateIssuanceDateTime</span><span class="sxs-lookup"><span data-stu-id="7926e-170">certificateIssuanceDateTime</span></span>|<span data-ttu-id="7926e-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7926e-171">DateTimeOffset</span></span>|<span data-ttu-id="7926e-172">颁发日期</span><span class="sxs-lookup"><span data-stu-id="7926e-172">Issuance date</span></span>|



## <a name="response"></a><span data-ttu-id="7926e-173">响应</span><span class="sxs-lookup"><span data-stu-id="7926e-173">Response</span></span>
<span data-ttu-id="7926e-174">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的[managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7926e-174">If successful, this method returns a `200 OK` response code and an updated [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7926e-175">示例</span><span class="sxs-lookup"><span data-stu-id="7926e-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="7926e-176">请求</span><span class="sxs-lookup"><span data-stu-id="7926e-176">Request</span></span>
<span data-ttu-id="7926e-177">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7926e-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7926e-178">响应</span><span class="sxs-lookup"><span data-stu-id="7926e-178">Response</span></span>
<span data-ttu-id="7926e-179">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="7926e-179">Here is an example of the response.</span></span> <span data-ttu-id="7926e-180">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="7926e-180">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="7926e-181">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="7926e-181">All of the properties will be returned from an actual call.</span></span>
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



