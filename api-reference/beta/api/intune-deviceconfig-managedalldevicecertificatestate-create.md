---
title: 创建 managedAllDeviceCertificateState
description: 创建新的 managedAllDeviceCertificateState 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 50877255e069c70749ae77b515d7f45a90398a33
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36338586"
---
# <a name="create-managedalldevicecertificatestate"></a><span data-ttu-id="f4ec7-103">创建 managedAllDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="f4ec7-103">Create managedAllDeviceCertificateState</span></span>

> <span data-ttu-id="f4ec7-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f4ec7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4ec7-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f4ec7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4ec7-106">创建新的[managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f4ec7-106">Create a new [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4ec7-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="f4ec7-107">Prerequisites</span></span>
<span data-ttu-id="f4ec7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f4ec7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4ec7-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f4ec7-110">Permission type</span></span>|<span data-ttu-id="f4ec7-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f4ec7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4ec7-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f4ec7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f4ec7-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4ec7-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f4ec7-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f4ec7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4ec7-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f4ec7-115">Not supported.</span></span>|
|<span data-ttu-id="f4ec7-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f4ec7-116">Application</span></span>|<span data-ttu-id="f4ec7-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4ec7-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4ec7-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f4ec7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates
```

## <a name="request-headers"></a><span data-ttu-id="f4ec7-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f4ec7-119">Request headers</span></span>
|<span data-ttu-id="f4ec7-120">标头</span><span class="sxs-lookup"><span data-stu-id="f4ec7-120">Header</span></span>|<span data-ttu-id="f4ec7-121">值</span><span class="sxs-lookup"><span data-stu-id="f4ec7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4ec7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4ec7-122">Authorization</span></span>|<span data-ttu-id="f4ec7-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f4ec7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4ec7-124">接受</span><span class="sxs-lookup"><span data-stu-id="f4ec7-124">Accept</span></span>|<span data-ttu-id="f4ec7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f4ec7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4ec7-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f4ec7-126">Request body</span></span>
<span data-ttu-id="f4ec7-127">在请求正文中, 提供 managedAllDeviceCertificateState 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f4ec7-127">In the request body, supply a JSON representation for the managedAllDeviceCertificateState object.</span></span>

<span data-ttu-id="f4ec7-128">下表显示创建 managedAllDeviceCertificateState 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f4ec7-128">The following table shows the properties that are required when you create the managedAllDeviceCertificateState.</span></span>

|<span data-ttu-id="f4ec7-129">属性</span><span class="sxs-lookup"><span data-stu-id="f4ec7-129">Property</span></span>|<span data-ttu-id="f4ec7-130">类型</span><span class="sxs-lookup"><span data-stu-id="f4ec7-130">Type</span></span>|<span data-ttu-id="f4ec7-131">说明</span><span class="sxs-lookup"><span data-stu-id="f4ec7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4ec7-132">id</span><span class="sxs-lookup"><span data-stu-id="f4ec7-132">id</span></span>|<span data-ttu-id="f4ec7-133">String</span><span class="sxs-lookup"><span data-stu-id="f4ec7-133">String</span></span>|<span data-ttu-id="f4ec7-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f4ec7-134">Key of the entity.</span></span>|
|<span data-ttu-id="f4ec7-135">certificateRevokeStatus</span><span class="sxs-lookup"><span data-stu-id="f4ec7-135">certificateRevokeStatus</span></span>|[<span data-ttu-id="f4ec7-136">certificateRevocationStatus</span><span class="sxs-lookup"><span data-stu-id="f4ec7-136">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="f4ec7-137">撤消状态。</span><span class="sxs-lookup"><span data-stu-id="f4ec7-137">Revoke status.</span></span> <span data-ttu-id="f4ec7-138">可取值为：`none`、`pending`、`issued`、`failed`、`revoked`。</span><span class="sxs-lookup"><span data-stu-id="f4ec7-138">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="f4ec7-139">managedDeviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="f4ec7-139">managedDeviceDisplayName</span></span>|<span data-ttu-id="f4ec7-140">String</span><span class="sxs-lookup"><span data-stu-id="f4ec7-140">String</span></span>|<span data-ttu-id="f4ec7-141">设备显示名称</span><span class="sxs-lookup"><span data-stu-id="f4ec7-141">Device display name</span></span>|
|<span data-ttu-id="f4ec7-142">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f4ec7-142">userPrincipalName</span></span>|<span data-ttu-id="f4ec7-143">String</span><span class="sxs-lookup"><span data-stu-id="f4ec7-143">String</span></span>|<span data-ttu-id="f4ec7-144">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="f4ec7-144">User principal name</span></span>|
|<span data-ttu-id="f4ec7-145">certificateExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f4ec7-145">certificateExpirationDateTime</span></span>|<span data-ttu-id="f4ec7-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4ec7-146">DateTimeOffset</span></span>|<span data-ttu-id="f4ec7-147">证书到期日期</span><span class="sxs-lookup"><span data-stu-id="f4ec7-147">Certificate expiry date</span></span>|
|<span data-ttu-id="f4ec7-148">certificateIssuerName</span><span class="sxs-lookup"><span data-stu-id="f4ec7-148">certificateIssuerName</span></span>|<span data-ttu-id="f4ec7-149">String</span><span class="sxs-lookup"><span data-stu-id="f4ec7-149">String</span></span>|<span data-ttu-id="f4ec7-150">颁发者</span><span class="sxs-lookup"><span data-stu-id="f4ec7-150">Issuer</span></span>|
|<span data-ttu-id="f4ec7-151">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="f4ec7-151">certificateThumbprint</span></span>|<span data-ttu-id="f4ec7-152">String</span><span class="sxs-lookup"><span data-stu-id="f4ec7-152">String</span></span>|<span data-ttu-id="f4ec7-153">为</span><span class="sxs-lookup"><span data-stu-id="f4ec7-153">Thumbprint</span></span>|
|<span data-ttu-id="f4ec7-154">certificateSerialNumber</span><span class="sxs-lookup"><span data-stu-id="f4ec7-154">certificateSerialNumber</span></span>|<span data-ttu-id="f4ec7-155">String</span><span class="sxs-lookup"><span data-stu-id="f4ec7-155">String</span></span>|<span data-ttu-id="f4ec7-156">序列号</span><span class="sxs-lookup"><span data-stu-id="f4ec7-156">Serial number</span></span>|
|<span data-ttu-id="f4ec7-157">certificateSubjectName</span><span class="sxs-lookup"><span data-stu-id="f4ec7-157">certificateSubjectName</span></span>|<span data-ttu-id="f4ec7-158">String</span><span class="sxs-lookup"><span data-stu-id="f4ec7-158">String</span></span>|<span data-ttu-id="f4ec7-159">证书主题名称</span><span class="sxs-lookup"><span data-stu-id="f4ec7-159">Certificate subject name</span></span>|
|<span data-ttu-id="f4ec7-160">certificateKeyUsages</span><span class="sxs-lookup"><span data-stu-id="f4ec7-160">certificateKeyUsages</span></span>|<span data-ttu-id="f4ec7-161">Int32</span><span class="sxs-lookup"><span data-stu-id="f4ec7-161">Int32</span></span>|<span data-ttu-id="f4ec7-162">密钥用法</span><span class="sxs-lookup"><span data-stu-id="f4ec7-162">Key Usage</span></span>|
|<span data-ttu-id="f4ec7-163">certificateExtendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="f4ec7-163">certificateExtendedKeyUsages</span></span>|<span data-ttu-id="f4ec7-164">String</span><span class="sxs-lookup"><span data-stu-id="f4ec7-164">String</span></span>|<span data-ttu-id="f4ec7-165">增强型密钥使用</span><span class="sxs-lookup"><span data-stu-id="f4ec7-165">Enhanced Key Usage</span></span>|
|<span data-ttu-id="f4ec7-166">certificateIssuanceDateTime</span><span class="sxs-lookup"><span data-stu-id="f4ec7-166">certificateIssuanceDateTime</span></span>|<span data-ttu-id="f4ec7-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4ec7-167">DateTimeOffset</span></span>|<span data-ttu-id="f4ec7-168">颁发日期</span><span class="sxs-lookup"><span data-stu-id="f4ec7-168">Issuance date</span></span>|



## <a name="response"></a><span data-ttu-id="f4ec7-169">响应</span><span class="sxs-lookup"><span data-stu-id="f4ec7-169">Response</span></span>
<span data-ttu-id="f4ec7-170">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f4ec7-170">If successful, this method returns a `201 Created` response code and a [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4ec7-171">示例</span><span class="sxs-lookup"><span data-stu-id="f4ec7-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4ec7-172">请求</span><span class="sxs-lookup"><span data-stu-id="f4ec7-172">Request</span></span>
<span data-ttu-id="f4ec7-173">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f4ec7-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f4ec7-174">响应</span><span class="sxs-lookup"><span data-stu-id="f4ec7-174">Response</span></span>
<span data-ttu-id="f4ec7-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f4ec7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






