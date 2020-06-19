---
title: 创建 managedAllDeviceCertificateState
description: 创建新的 managedAllDeviceCertificateState 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 58f061bd89c3633651e40578e23db1f1f4836406
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792735"
---
# <a name="create-managedalldevicecertificatestate"></a><span data-ttu-id="2a8cb-103">创建 managedAllDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="2a8cb-103">Create managedAllDeviceCertificateState</span></span>

<span data-ttu-id="2a8cb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a8cb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2a8cb-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2a8cb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2a8cb-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2a8cb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a8cb-107">创建新的[managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2a8cb-107">Create a new [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2a8cb-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="2a8cb-108">Prerequisites</span></span>
<span data-ttu-id="2a8cb-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="2a8cb-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="2a8cb-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a8cb-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a8cb-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2a8cb-111">Permission type</span></span>|<span data-ttu-id="2a8cb-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2a8cb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a8cb-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2a8cb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2a8cb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a8cb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2a8cb-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2a8cb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a8cb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2a8cb-116">Not supported.</span></span>|
|<span data-ttu-id="2a8cb-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2a8cb-117">Application</span></span>|<span data-ttu-id="2a8cb-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a8cb-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a8cb-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2a8cb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates
```

## <a name="request-headers"></a><span data-ttu-id="2a8cb-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2a8cb-120">Request headers</span></span>
|<span data-ttu-id="2a8cb-121">标头</span><span class="sxs-lookup"><span data-stu-id="2a8cb-121">Header</span></span>|<span data-ttu-id="2a8cb-122">值</span><span class="sxs-lookup"><span data-stu-id="2a8cb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a8cb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a8cb-123">Authorization</span></span>|<span data-ttu-id="2a8cb-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2a8cb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a8cb-125">接受</span><span class="sxs-lookup"><span data-stu-id="2a8cb-125">Accept</span></span>|<span data-ttu-id="2a8cb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2a8cb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a8cb-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2a8cb-127">Request body</span></span>
<span data-ttu-id="2a8cb-128">在请求正文中，提供 managedAllDeviceCertificateState 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2a8cb-128">In the request body, supply a JSON representation for the managedAllDeviceCertificateState object.</span></span>

<span data-ttu-id="2a8cb-129">下表显示创建 managedAllDeviceCertificateState 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2a8cb-129">The following table shows the properties that are required when you create the managedAllDeviceCertificateState.</span></span>

|<span data-ttu-id="2a8cb-130">属性</span><span class="sxs-lookup"><span data-stu-id="2a8cb-130">Property</span></span>|<span data-ttu-id="2a8cb-131">类型</span><span class="sxs-lookup"><span data-stu-id="2a8cb-131">Type</span></span>|<span data-ttu-id="2a8cb-132">说明</span><span class="sxs-lookup"><span data-stu-id="2a8cb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a8cb-133">id</span><span class="sxs-lookup"><span data-stu-id="2a8cb-133">id</span></span>|<span data-ttu-id="2a8cb-134">String</span><span class="sxs-lookup"><span data-stu-id="2a8cb-134">String</span></span>|<span data-ttu-id="2a8cb-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2a8cb-135">Key of the entity.</span></span>|
|<span data-ttu-id="2a8cb-136">certificateRevokeStatus</span><span class="sxs-lookup"><span data-stu-id="2a8cb-136">certificateRevokeStatus</span></span>|[<span data-ttu-id="2a8cb-137">certificateRevocationStatus</span><span class="sxs-lookup"><span data-stu-id="2a8cb-137">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="2a8cb-138">撤消状态。</span><span class="sxs-lookup"><span data-stu-id="2a8cb-138">Revoke status.</span></span> <span data-ttu-id="2a8cb-139">可取值为：`none`、`pending`、`issued`、`failed`、`revoked`。</span><span class="sxs-lookup"><span data-stu-id="2a8cb-139">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="2a8cb-140">managedDeviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="2a8cb-140">managedDeviceDisplayName</span></span>|<span data-ttu-id="2a8cb-141">String</span><span class="sxs-lookup"><span data-stu-id="2a8cb-141">String</span></span>|<span data-ttu-id="2a8cb-142">设备显示名称</span><span class="sxs-lookup"><span data-stu-id="2a8cb-142">Device display name</span></span>|
|<span data-ttu-id="2a8cb-143">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2a8cb-143">userPrincipalName</span></span>|<span data-ttu-id="2a8cb-144">String</span><span class="sxs-lookup"><span data-stu-id="2a8cb-144">String</span></span>|<span data-ttu-id="2a8cb-145">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="2a8cb-145">User principal name</span></span>|
|<span data-ttu-id="2a8cb-146">certificateExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="2a8cb-146">certificateExpirationDateTime</span></span>|<span data-ttu-id="2a8cb-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a8cb-147">DateTimeOffset</span></span>|<span data-ttu-id="2a8cb-148">证书到期日期</span><span class="sxs-lookup"><span data-stu-id="2a8cb-148">Certificate expiry date</span></span>|
|<span data-ttu-id="2a8cb-149">certificateIssuerName</span><span class="sxs-lookup"><span data-stu-id="2a8cb-149">certificateIssuerName</span></span>|<span data-ttu-id="2a8cb-150">String</span><span class="sxs-lookup"><span data-stu-id="2a8cb-150">String</span></span>|<span data-ttu-id="2a8cb-151">颁发者</span><span class="sxs-lookup"><span data-stu-id="2a8cb-151">Issuer</span></span>|
|<span data-ttu-id="2a8cb-152">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="2a8cb-152">certificateThumbprint</span></span>|<span data-ttu-id="2a8cb-153">String</span><span class="sxs-lookup"><span data-stu-id="2a8cb-153">String</span></span>|<span data-ttu-id="2a8cb-154">为</span><span class="sxs-lookup"><span data-stu-id="2a8cb-154">Thumbprint</span></span>|
|<span data-ttu-id="2a8cb-155">certificateSerialNumber</span><span class="sxs-lookup"><span data-stu-id="2a8cb-155">certificateSerialNumber</span></span>|<span data-ttu-id="2a8cb-156">String</span><span class="sxs-lookup"><span data-stu-id="2a8cb-156">String</span></span>|<span data-ttu-id="2a8cb-157">序列号</span><span class="sxs-lookup"><span data-stu-id="2a8cb-157">Serial number</span></span>|
|<span data-ttu-id="2a8cb-158">certificateSubjectName</span><span class="sxs-lookup"><span data-stu-id="2a8cb-158">certificateSubjectName</span></span>|<span data-ttu-id="2a8cb-159">String</span><span class="sxs-lookup"><span data-stu-id="2a8cb-159">String</span></span>|<span data-ttu-id="2a8cb-160">证书主题名称</span><span class="sxs-lookup"><span data-stu-id="2a8cb-160">Certificate subject name</span></span>|
|<span data-ttu-id="2a8cb-161">certificateKeyUsages</span><span class="sxs-lookup"><span data-stu-id="2a8cb-161">certificateKeyUsages</span></span>|<span data-ttu-id="2a8cb-162">Int32</span><span class="sxs-lookup"><span data-stu-id="2a8cb-162">Int32</span></span>|<span data-ttu-id="2a8cb-163">密钥用法</span><span class="sxs-lookup"><span data-stu-id="2a8cb-163">Key Usage</span></span>|
|<span data-ttu-id="2a8cb-164">certificateExtendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="2a8cb-164">certificateExtendedKeyUsages</span></span>|<span data-ttu-id="2a8cb-165">String</span><span class="sxs-lookup"><span data-stu-id="2a8cb-165">String</span></span>|<span data-ttu-id="2a8cb-166">增强型密钥使用</span><span class="sxs-lookup"><span data-stu-id="2a8cb-166">Enhanced Key Usage</span></span>|
|<span data-ttu-id="2a8cb-167">certificateIssuanceDateTime</span><span class="sxs-lookup"><span data-stu-id="2a8cb-167">certificateIssuanceDateTime</span></span>|<span data-ttu-id="2a8cb-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a8cb-168">DateTimeOffset</span></span>|<span data-ttu-id="2a8cb-169">颁发日期</span><span class="sxs-lookup"><span data-stu-id="2a8cb-169">Issuance date</span></span>|
|<span data-ttu-id="2a8cb-170">certificateRevokeStatusLastChangeDateTime</span><span class="sxs-lookup"><span data-stu-id="2a8cb-170">certificateRevokeStatusLastChangeDateTime</span></span>|<span data-ttu-id="2a8cb-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a8cb-171">DateTimeOffset</span></span>|<span data-ttu-id="2a8cb-172">上次更改吊销状态的时间</span><span class="sxs-lookup"><span data-stu-id="2a8cb-172">The time the revoke status was last changed</span></span>|



## <a name="response"></a><span data-ttu-id="2a8cb-173">响应</span><span class="sxs-lookup"><span data-stu-id="2a8cb-173">Response</span></span>
<span data-ttu-id="2a8cb-174">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和[managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2a8cb-174">If successful, this method returns a `201 Created` response code and a [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a8cb-175">示例</span><span class="sxs-lookup"><span data-stu-id="2a8cb-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="2a8cb-176">请求</span><span class="sxs-lookup"><span data-stu-id="2a8cb-176">Request</span></span>
<span data-ttu-id="2a8cb-177">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2a8cb-177">Here is an example of the request.</span></span>
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
  "certificateIssuanceDateTime": "2016-12-31T23:59:41.5044473-08:00",
  "certificateRevokeStatusLastChangeDateTime": "2016-12-31T23:59:41.5044473-08:00"
}
```

### <a name="response"></a><span data-ttu-id="2a8cb-178">响应</span><span class="sxs-lookup"><span data-stu-id="2a8cb-178">Response</span></span>
<span data-ttu-id="2a8cb-179">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="2a8cb-179">Here is an example of the response.</span></span> <span data-ttu-id="2a8cb-180">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="2a8cb-180">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="2a8cb-181">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="2a8cb-181">All of the properties will be returned from an actual call.</span></span>
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
  "certificateIssuanceDateTime": "2016-12-31T23:59:41.5044473-08:00",
  "certificateRevokeStatusLastChangeDateTime": "2016-12-31T23:59:41.5044473-08:00"
}
```



