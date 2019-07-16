---
title: 更新 managedAllDeviceCertificateState
description: 更新 managedAllDeviceCertificateState 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aac2d6f42ee093c3af745d37da9917db20492006
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35725871"
---
# <a name="update-managedalldevicecertificatestate"></a><span data-ttu-id="a01dc-103">更新 managedAllDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="a01dc-103">Update managedAllDeviceCertificateState</span></span>

> <span data-ttu-id="a01dc-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a01dc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a01dc-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a01dc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a01dc-106">更新[managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a01dc-106">Update the properties of a [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a01dc-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a01dc-107">Prerequisites</span></span>
<span data-ttu-id="a01dc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a01dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a01dc-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a01dc-110">Permission type</span></span>|<span data-ttu-id="a01dc-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a01dc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a01dc-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a01dc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a01dc-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a01dc-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a01dc-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a01dc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a01dc-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a01dc-115">Not supported.</span></span>|
|<span data-ttu-id="a01dc-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a01dc-116">Application</span></span>|<span data-ttu-id="a01dc-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a01dc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a01dc-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a01dc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates/{managedAllDeviceCertificateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="a01dc-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a01dc-119">Request headers</span></span>
|<span data-ttu-id="a01dc-120">标头</span><span class="sxs-lookup"><span data-stu-id="a01dc-120">Header</span></span>|<span data-ttu-id="a01dc-121">值</span><span class="sxs-lookup"><span data-stu-id="a01dc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a01dc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a01dc-122">Authorization</span></span>|<span data-ttu-id="a01dc-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a01dc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a01dc-124">接受</span><span class="sxs-lookup"><span data-stu-id="a01dc-124">Accept</span></span>|<span data-ttu-id="a01dc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a01dc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a01dc-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a01dc-126">Request body</span></span>
<span data-ttu-id="a01dc-127">在请求正文中, 提供[managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a01dc-127">In the request body, supply a JSON representation for the [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

<span data-ttu-id="a01dc-128">下表显示创建[managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a01dc-128">The following table shows the properties that are required when you create the [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md).</span></span>

|<span data-ttu-id="a01dc-129">属性</span><span class="sxs-lookup"><span data-stu-id="a01dc-129">Property</span></span>|<span data-ttu-id="a01dc-130">类型</span><span class="sxs-lookup"><span data-stu-id="a01dc-130">Type</span></span>|<span data-ttu-id="a01dc-131">说明</span><span class="sxs-lookup"><span data-stu-id="a01dc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a01dc-132">id</span><span class="sxs-lookup"><span data-stu-id="a01dc-132">id</span></span>|<span data-ttu-id="a01dc-133">String</span><span class="sxs-lookup"><span data-stu-id="a01dc-133">String</span></span>|<span data-ttu-id="a01dc-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a01dc-134">Key of the entity.</span></span>|
|<span data-ttu-id="a01dc-135">certificateRevokeStatus</span><span class="sxs-lookup"><span data-stu-id="a01dc-135">certificateRevokeStatus</span></span>|[<span data-ttu-id="a01dc-136">certificateRevocationStatus</span><span class="sxs-lookup"><span data-stu-id="a01dc-136">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="a01dc-137">撤消状态。</span><span class="sxs-lookup"><span data-stu-id="a01dc-137">Revoke status.</span></span> <span data-ttu-id="a01dc-138">可取值为：`none`、`pending`、`issued`、`failed`、`revoked`。</span><span class="sxs-lookup"><span data-stu-id="a01dc-138">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="a01dc-139">managedDeviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="a01dc-139">managedDeviceDisplayName</span></span>|<span data-ttu-id="a01dc-140">String</span><span class="sxs-lookup"><span data-stu-id="a01dc-140">String</span></span>|<span data-ttu-id="a01dc-141">设备显示名称</span><span class="sxs-lookup"><span data-stu-id="a01dc-141">Device display name</span></span>|
|<span data-ttu-id="a01dc-142">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a01dc-142">userPrincipalName</span></span>|<span data-ttu-id="a01dc-143">String</span><span class="sxs-lookup"><span data-stu-id="a01dc-143">String</span></span>|<span data-ttu-id="a01dc-144">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="a01dc-144">User principal name</span></span>|
|<span data-ttu-id="a01dc-145">certificateExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a01dc-145">certificateExpirationDateTime</span></span>|<span data-ttu-id="a01dc-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a01dc-146">DateTimeOffset</span></span>|<span data-ttu-id="a01dc-147">证书到期日期</span><span class="sxs-lookup"><span data-stu-id="a01dc-147">Certificate expiry date</span></span>|
|<span data-ttu-id="a01dc-148">certificateIssuerName</span><span class="sxs-lookup"><span data-stu-id="a01dc-148">certificateIssuerName</span></span>|<span data-ttu-id="a01dc-149">String</span><span class="sxs-lookup"><span data-stu-id="a01dc-149">String</span></span>|<span data-ttu-id="a01dc-150">颁发者</span><span class="sxs-lookup"><span data-stu-id="a01dc-150">Issuer</span></span>|
|<span data-ttu-id="a01dc-151">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="a01dc-151">certificateThumbprint</span></span>|<span data-ttu-id="a01dc-152">String</span><span class="sxs-lookup"><span data-stu-id="a01dc-152">String</span></span>|<span data-ttu-id="a01dc-153">为</span><span class="sxs-lookup"><span data-stu-id="a01dc-153">Thumbprint</span></span>|
|<span data-ttu-id="a01dc-154">certificateSerialNumber</span><span class="sxs-lookup"><span data-stu-id="a01dc-154">certificateSerialNumber</span></span>|<span data-ttu-id="a01dc-155">String</span><span class="sxs-lookup"><span data-stu-id="a01dc-155">String</span></span>|<span data-ttu-id="a01dc-156">序列号</span><span class="sxs-lookup"><span data-stu-id="a01dc-156">Serial number</span></span>|
|<span data-ttu-id="a01dc-157">certificateSubjectName</span><span class="sxs-lookup"><span data-stu-id="a01dc-157">certificateSubjectName</span></span>|<span data-ttu-id="a01dc-158">String</span><span class="sxs-lookup"><span data-stu-id="a01dc-158">String</span></span>|<span data-ttu-id="a01dc-159">证书主题名称</span><span class="sxs-lookup"><span data-stu-id="a01dc-159">Certificate subject name</span></span>|
|<span data-ttu-id="a01dc-160">certificateKeyUsages</span><span class="sxs-lookup"><span data-stu-id="a01dc-160">certificateKeyUsages</span></span>|<span data-ttu-id="a01dc-161">Int32</span><span class="sxs-lookup"><span data-stu-id="a01dc-161">Int32</span></span>|<span data-ttu-id="a01dc-162">密钥用法</span><span class="sxs-lookup"><span data-stu-id="a01dc-162">Key Usage</span></span>|
|<span data-ttu-id="a01dc-163">certificateExtendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="a01dc-163">certificateExtendedKeyUsages</span></span>|<span data-ttu-id="a01dc-164">String</span><span class="sxs-lookup"><span data-stu-id="a01dc-164">String</span></span>|<span data-ttu-id="a01dc-165">增强型密钥使用</span><span class="sxs-lookup"><span data-stu-id="a01dc-165">Enhanced Key Usage</span></span>|
|<span data-ttu-id="a01dc-166">certificateIssuanceDateTime</span><span class="sxs-lookup"><span data-stu-id="a01dc-166">certificateIssuanceDateTime</span></span>|<span data-ttu-id="a01dc-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a01dc-167">DateTimeOffset</span></span>|<span data-ttu-id="a01dc-168">颁发日期</span><span class="sxs-lookup"><span data-stu-id="a01dc-168">Issuance date</span></span>|



## <a name="response"></a><span data-ttu-id="a01dc-169">响应</span><span class="sxs-lookup"><span data-stu-id="a01dc-169">Response</span></span>
<span data-ttu-id="a01dc-170">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a01dc-170">If successful, this method returns a `200 OK` response code and an updated [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a01dc-171">示例</span><span class="sxs-lookup"><span data-stu-id="a01dc-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="a01dc-172">请求</span><span class="sxs-lookup"><span data-stu-id="a01dc-172">Request</span></span>
<span data-ttu-id="a01dc-173">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a01dc-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates/{managedAllDeviceCertificateStateId}
Content-type: application/json
Content-length: 735

{
  "@odata.type": "#microsoft.graph.managedAllDeviceCertificateState",
  "certificateRevokeStatus": "pending",
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

### <a name="response"></a><span data-ttu-id="a01dc-174">响应</span><span class="sxs-lookup"><span data-stu-id="a01dc-174">Response</span></span>
<span data-ttu-id="a01dc-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a01dc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 784

{
  "@odata.type": "#microsoft.graph.managedAllDeviceCertificateState",
  "id": "987c6a17-6a17-987c-176a-7c98176a7c98",
  "certificateRevokeStatus": "pending",
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





