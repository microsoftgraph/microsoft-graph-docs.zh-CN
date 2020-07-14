---
title: 创建 managedAllDeviceCertificateState
description: 创建新的 managedAllDeviceCertificateState 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 44c9b00511dc3bd8e4a1c9fb9226e6e62a80dc22
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2020
ms.locfileid: "45122971"
---
# <a name="create-managedalldevicecertificatestate"></a><span data-ttu-id="d7768-103">创建 managedAllDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="d7768-103">Create managedAllDeviceCertificateState</span></span>

<span data-ttu-id="d7768-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7768-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d7768-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d7768-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d7768-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d7768-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7768-107">创建新的[managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d7768-107">Create a new [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d7768-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d7768-108">Prerequisites</span></span>
<span data-ttu-id="d7768-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="d7768-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="d7768-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7768-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7768-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d7768-111">Permission type</span></span>|<span data-ttu-id="d7768-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d7768-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d7768-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d7768-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d7768-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7768-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d7768-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d7768-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d7768-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d7768-116">Not supported.</span></span>|
|<span data-ttu-id="d7768-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d7768-117">Application</span></span>|<span data-ttu-id="d7768-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7768-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d7768-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d7768-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates
```

## <a name="request-headers"></a><span data-ttu-id="d7768-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d7768-120">Request headers</span></span>
|<span data-ttu-id="d7768-121">标头</span><span class="sxs-lookup"><span data-stu-id="d7768-121">Header</span></span>|<span data-ttu-id="d7768-122">值</span><span class="sxs-lookup"><span data-stu-id="d7768-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d7768-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7768-123">Authorization</span></span>|<span data-ttu-id="d7768-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d7768-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d7768-125">接受</span><span class="sxs-lookup"><span data-stu-id="d7768-125">Accept</span></span>|<span data-ttu-id="d7768-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d7768-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7768-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d7768-127">Request body</span></span>
<span data-ttu-id="d7768-128">在请求正文中，提供 managedAllDeviceCertificateState 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d7768-128">In the request body, supply a JSON representation for the managedAllDeviceCertificateState object.</span></span>

<span data-ttu-id="d7768-129">下表显示创建 managedAllDeviceCertificateState 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d7768-129">The following table shows the properties that are required when you create the managedAllDeviceCertificateState.</span></span>

|<span data-ttu-id="d7768-130">属性</span><span class="sxs-lookup"><span data-stu-id="d7768-130">Property</span></span>|<span data-ttu-id="d7768-131">类型</span><span class="sxs-lookup"><span data-stu-id="d7768-131">Type</span></span>|<span data-ttu-id="d7768-132">说明</span><span class="sxs-lookup"><span data-stu-id="d7768-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7768-133">id</span><span class="sxs-lookup"><span data-stu-id="d7768-133">id</span></span>|<span data-ttu-id="d7768-134">String</span><span class="sxs-lookup"><span data-stu-id="d7768-134">String</span></span>|<span data-ttu-id="d7768-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d7768-135">Key of the entity.</span></span>|
|<span data-ttu-id="d7768-136">certificateRevokeStatus</span><span class="sxs-lookup"><span data-stu-id="d7768-136">certificateRevokeStatus</span></span>|[<span data-ttu-id="d7768-137">certificateRevocationStatus</span><span class="sxs-lookup"><span data-stu-id="d7768-137">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="d7768-138">撤消状态。</span><span class="sxs-lookup"><span data-stu-id="d7768-138">Revoke status.</span></span> <span data-ttu-id="d7768-139">可取值为：`none`、`pending`、`issued`、`failed`、`revoked`。</span><span class="sxs-lookup"><span data-stu-id="d7768-139">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="d7768-140">certificateRevokeStatusLastChangeDateTime</span><span class="sxs-lookup"><span data-stu-id="d7768-140">certificateRevokeStatusLastChangeDateTime</span></span>|<span data-ttu-id="d7768-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7768-141">DateTimeOffset</span></span>|<span data-ttu-id="d7768-142">上次更改吊销状态的时间</span><span class="sxs-lookup"><span data-stu-id="d7768-142">The time the revoke status was last changed</span></span>|
|<span data-ttu-id="d7768-143">managedDeviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="d7768-143">managedDeviceDisplayName</span></span>|<span data-ttu-id="d7768-144">String</span><span class="sxs-lookup"><span data-stu-id="d7768-144">String</span></span>|<span data-ttu-id="d7768-145">设备显示名称</span><span class="sxs-lookup"><span data-stu-id="d7768-145">Device display name</span></span>|
|<span data-ttu-id="d7768-146">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d7768-146">userPrincipalName</span></span>|<span data-ttu-id="d7768-147">String</span><span class="sxs-lookup"><span data-stu-id="d7768-147">String</span></span>|<span data-ttu-id="d7768-148">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="d7768-148">User principal name</span></span>|
|<span data-ttu-id="d7768-149">certificateExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d7768-149">certificateExpirationDateTime</span></span>|<span data-ttu-id="d7768-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7768-150">DateTimeOffset</span></span>|<span data-ttu-id="d7768-151">证书到期日期</span><span class="sxs-lookup"><span data-stu-id="d7768-151">Certificate expiry date</span></span>|
|<span data-ttu-id="d7768-152">certificateIssuerName</span><span class="sxs-lookup"><span data-stu-id="d7768-152">certificateIssuerName</span></span>|<span data-ttu-id="d7768-153">String</span><span class="sxs-lookup"><span data-stu-id="d7768-153">String</span></span>|<span data-ttu-id="d7768-154">颁发者</span><span class="sxs-lookup"><span data-stu-id="d7768-154">Issuer</span></span>|
|<span data-ttu-id="d7768-155">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="d7768-155">certificateThumbprint</span></span>|<span data-ttu-id="d7768-156">String</span><span class="sxs-lookup"><span data-stu-id="d7768-156">String</span></span>|<span data-ttu-id="d7768-157">为</span><span class="sxs-lookup"><span data-stu-id="d7768-157">Thumbprint</span></span>|
|<span data-ttu-id="d7768-158">certificateSerialNumber</span><span class="sxs-lookup"><span data-stu-id="d7768-158">certificateSerialNumber</span></span>|<span data-ttu-id="d7768-159">String</span><span class="sxs-lookup"><span data-stu-id="d7768-159">String</span></span>|<span data-ttu-id="d7768-160">序列号</span><span class="sxs-lookup"><span data-stu-id="d7768-160">Serial number</span></span>|
|<span data-ttu-id="d7768-161">certificateSubjectName</span><span class="sxs-lookup"><span data-stu-id="d7768-161">certificateSubjectName</span></span>|<span data-ttu-id="d7768-162">String</span><span class="sxs-lookup"><span data-stu-id="d7768-162">String</span></span>|<span data-ttu-id="d7768-163">证书主题名称</span><span class="sxs-lookup"><span data-stu-id="d7768-163">Certificate subject name</span></span>|
|<span data-ttu-id="d7768-164">certificateKeyUsages</span><span class="sxs-lookup"><span data-stu-id="d7768-164">certificateKeyUsages</span></span>|<span data-ttu-id="d7768-165">Int32</span><span class="sxs-lookup"><span data-stu-id="d7768-165">Int32</span></span>|<span data-ttu-id="d7768-166">密钥用法</span><span class="sxs-lookup"><span data-stu-id="d7768-166">Key Usage</span></span>|
|<span data-ttu-id="d7768-167">certificateExtendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="d7768-167">certificateExtendedKeyUsages</span></span>|<span data-ttu-id="d7768-168">String</span><span class="sxs-lookup"><span data-stu-id="d7768-168">String</span></span>|<span data-ttu-id="d7768-169">增强型密钥使用</span><span class="sxs-lookup"><span data-stu-id="d7768-169">Enhanced Key Usage</span></span>|
|<span data-ttu-id="d7768-170">certificateIssuanceDateTime</span><span class="sxs-lookup"><span data-stu-id="d7768-170">certificateIssuanceDateTime</span></span>|<span data-ttu-id="d7768-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7768-171">DateTimeOffset</span></span>|<span data-ttu-id="d7768-172">颁发日期</span><span class="sxs-lookup"><span data-stu-id="d7768-172">Issuance date</span></span>|



## <a name="response"></a><span data-ttu-id="d7768-173">响应</span><span class="sxs-lookup"><span data-stu-id="d7768-173">Response</span></span>
<span data-ttu-id="d7768-174">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和[managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d7768-174">If successful, this method returns a `201 Created` response code and a [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7768-175">示例</span><span class="sxs-lookup"><span data-stu-id="d7768-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="d7768-176">请求</span><span class="sxs-lookup"><span data-stu-id="d7768-176">Request</span></span>
<span data-ttu-id="d7768-177">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d7768-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates
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

### <a name="response"></a><span data-ttu-id="d7768-178">响应</span><span class="sxs-lookup"><span data-stu-id="d7768-178">Response</span></span>
<span data-ttu-id="d7768-179">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="d7768-179">Here is an example of the response.</span></span> <span data-ttu-id="d7768-180">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="d7768-180">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="d7768-181">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="d7768-181">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



