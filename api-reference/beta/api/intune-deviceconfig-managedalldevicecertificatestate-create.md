---
title: 创建 managedAllDeviceCertificateState
description: 创建新的 managedAllDeviceCertificateState 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b0924b2b581f758c256072d26531391b51c86453
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43432217"
---
# <a name="create-managedalldevicecertificatestate"></a><span data-ttu-id="d2a3b-103">创建 managedAllDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="d2a3b-103">Create managedAllDeviceCertificateState</span></span>

<span data-ttu-id="d2a3b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2a3b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d2a3b-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d2a3b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2a3b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d2a3b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2a3b-107">创建新的[managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d2a3b-107">Create a new [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d2a3b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d2a3b-108">Prerequisites</span></span>
<span data-ttu-id="d2a3b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d2a3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2a3b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d2a3b-111">Permission type</span></span>|<span data-ttu-id="d2a3b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d2a3b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2a3b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d2a3b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d2a3b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2a3b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d2a3b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d2a3b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2a3b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d2a3b-116">Not supported.</span></span>|
|<span data-ttu-id="d2a3b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d2a3b-117">Application</span></span>|<span data-ttu-id="d2a3b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2a3b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2a3b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d2a3b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates
```

## <a name="request-headers"></a><span data-ttu-id="d2a3b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d2a3b-120">Request headers</span></span>
|<span data-ttu-id="d2a3b-121">标头</span><span class="sxs-lookup"><span data-stu-id="d2a3b-121">Header</span></span>|<span data-ttu-id="d2a3b-122">值</span><span class="sxs-lookup"><span data-stu-id="d2a3b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d2a3b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2a3b-123">Authorization</span></span>|<span data-ttu-id="d2a3b-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d2a3b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d2a3b-125">接受</span><span class="sxs-lookup"><span data-stu-id="d2a3b-125">Accept</span></span>|<span data-ttu-id="d2a3b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d2a3b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2a3b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d2a3b-127">Request body</span></span>
<span data-ttu-id="d2a3b-128">在请求正文中，提供 managedAllDeviceCertificateState 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d2a3b-128">In the request body, supply a JSON representation for the managedAllDeviceCertificateState object.</span></span>

<span data-ttu-id="d2a3b-129">下表显示创建 managedAllDeviceCertificateState 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d2a3b-129">The following table shows the properties that are required when you create the managedAllDeviceCertificateState.</span></span>

|<span data-ttu-id="d2a3b-130">属性</span><span class="sxs-lookup"><span data-stu-id="d2a3b-130">Property</span></span>|<span data-ttu-id="d2a3b-131">类型</span><span class="sxs-lookup"><span data-stu-id="d2a3b-131">Type</span></span>|<span data-ttu-id="d2a3b-132">说明</span><span class="sxs-lookup"><span data-stu-id="d2a3b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2a3b-133">id</span><span class="sxs-lookup"><span data-stu-id="d2a3b-133">id</span></span>|<span data-ttu-id="d2a3b-134">String</span><span class="sxs-lookup"><span data-stu-id="d2a3b-134">String</span></span>|<span data-ttu-id="d2a3b-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d2a3b-135">Key of the entity.</span></span>|
|<span data-ttu-id="d2a3b-136">certificateRevokeStatus</span><span class="sxs-lookup"><span data-stu-id="d2a3b-136">certificateRevokeStatus</span></span>|[<span data-ttu-id="d2a3b-137">certificateRevocationStatus</span><span class="sxs-lookup"><span data-stu-id="d2a3b-137">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="d2a3b-138">撤消状态。</span><span class="sxs-lookup"><span data-stu-id="d2a3b-138">Revoke status.</span></span> <span data-ttu-id="d2a3b-139">可取值为：`none`、`pending`、`issued`、`failed`、`revoked`。</span><span class="sxs-lookup"><span data-stu-id="d2a3b-139">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="d2a3b-140">managedDeviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="d2a3b-140">managedDeviceDisplayName</span></span>|<span data-ttu-id="d2a3b-141">String</span><span class="sxs-lookup"><span data-stu-id="d2a3b-141">String</span></span>|<span data-ttu-id="d2a3b-142">设备显示名称</span><span class="sxs-lookup"><span data-stu-id="d2a3b-142">Device display name</span></span>|
|<span data-ttu-id="d2a3b-143">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d2a3b-143">userPrincipalName</span></span>|<span data-ttu-id="d2a3b-144">String</span><span class="sxs-lookup"><span data-stu-id="d2a3b-144">String</span></span>|<span data-ttu-id="d2a3b-145">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="d2a3b-145">User principal name</span></span>|
|<span data-ttu-id="d2a3b-146">certificateExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d2a3b-146">certificateExpirationDateTime</span></span>|<span data-ttu-id="d2a3b-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2a3b-147">DateTimeOffset</span></span>|<span data-ttu-id="d2a3b-148">证书到期日期</span><span class="sxs-lookup"><span data-stu-id="d2a3b-148">Certificate expiry date</span></span>|
|<span data-ttu-id="d2a3b-149">certificateIssuerName</span><span class="sxs-lookup"><span data-stu-id="d2a3b-149">certificateIssuerName</span></span>|<span data-ttu-id="d2a3b-150">String</span><span class="sxs-lookup"><span data-stu-id="d2a3b-150">String</span></span>|<span data-ttu-id="d2a3b-151">颁发者</span><span class="sxs-lookup"><span data-stu-id="d2a3b-151">Issuer</span></span>|
|<span data-ttu-id="d2a3b-152">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="d2a3b-152">certificateThumbprint</span></span>|<span data-ttu-id="d2a3b-153">String</span><span class="sxs-lookup"><span data-stu-id="d2a3b-153">String</span></span>|<span data-ttu-id="d2a3b-154">为</span><span class="sxs-lookup"><span data-stu-id="d2a3b-154">Thumbprint</span></span>|
|<span data-ttu-id="d2a3b-155">certificateSerialNumber</span><span class="sxs-lookup"><span data-stu-id="d2a3b-155">certificateSerialNumber</span></span>|<span data-ttu-id="d2a3b-156">String</span><span class="sxs-lookup"><span data-stu-id="d2a3b-156">String</span></span>|<span data-ttu-id="d2a3b-157">序列号</span><span class="sxs-lookup"><span data-stu-id="d2a3b-157">Serial number</span></span>|
|<span data-ttu-id="d2a3b-158">certificateSubjectName</span><span class="sxs-lookup"><span data-stu-id="d2a3b-158">certificateSubjectName</span></span>|<span data-ttu-id="d2a3b-159">String</span><span class="sxs-lookup"><span data-stu-id="d2a3b-159">String</span></span>|<span data-ttu-id="d2a3b-160">证书主题名称</span><span class="sxs-lookup"><span data-stu-id="d2a3b-160">Certificate subject name</span></span>|
|<span data-ttu-id="d2a3b-161">certificateKeyUsages</span><span class="sxs-lookup"><span data-stu-id="d2a3b-161">certificateKeyUsages</span></span>|<span data-ttu-id="d2a3b-162">Int32</span><span class="sxs-lookup"><span data-stu-id="d2a3b-162">Int32</span></span>|<span data-ttu-id="d2a3b-163">密钥用法</span><span class="sxs-lookup"><span data-stu-id="d2a3b-163">Key Usage</span></span>|
|<span data-ttu-id="d2a3b-164">certificateExtendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="d2a3b-164">certificateExtendedKeyUsages</span></span>|<span data-ttu-id="d2a3b-165">String</span><span class="sxs-lookup"><span data-stu-id="d2a3b-165">String</span></span>|<span data-ttu-id="d2a3b-166">增强型密钥使用</span><span class="sxs-lookup"><span data-stu-id="d2a3b-166">Enhanced Key Usage</span></span>|
|<span data-ttu-id="d2a3b-167">certificateIssuanceDateTime</span><span class="sxs-lookup"><span data-stu-id="d2a3b-167">certificateIssuanceDateTime</span></span>|<span data-ttu-id="d2a3b-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2a3b-168">DateTimeOffset</span></span>|<span data-ttu-id="d2a3b-169">颁发日期</span><span class="sxs-lookup"><span data-stu-id="d2a3b-169">Issuance date</span></span>|



## <a name="response"></a><span data-ttu-id="d2a3b-170">响应</span><span class="sxs-lookup"><span data-stu-id="d2a3b-170">Response</span></span>
<span data-ttu-id="d2a3b-171">如果成功，此方法在响应`201 Created`正文中返回响应代码和[managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d2a3b-171">If successful, this method returns a `201 Created` response code and a [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2a3b-172">示例</span><span class="sxs-lookup"><span data-stu-id="d2a3b-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="d2a3b-173">请求</span><span class="sxs-lookup"><span data-stu-id="d2a3b-173">Request</span></span>
<span data-ttu-id="d2a3b-174">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d2a3b-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates
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

### <a name="response"></a><span data-ttu-id="d2a3b-175">响应</span><span class="sxs-lookup"><span data-stu-id="d2a3b-175">Response</span></span>
<span data-ttu-id="d2a3b-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d2a3b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



