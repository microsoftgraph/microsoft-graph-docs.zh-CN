---
title: 更新 enterpriseCodeSigningCertificate
description: 更新 enterpriseCodeSigningCertificate 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 13ecfc92d483a6fe9a3f71e0bc1b6c68dc79eaa3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48006270"
---
# <a name="update-enterprisecodesigningcertificate"></a><span data-ttu-id="6c9fd-103">更新 enterpriseCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="6c9fd-103">Update enterpriseCodeSigningCertificate</span></span>

<span data-ttu-id="6c9fd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c9fd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6c9fd-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6c9fd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c9fd-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6c9fd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c9fd-107">更新 [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6c9fd-107">Update the properties of a [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6c9fd-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6c9fd-108">Prerequisites</span></span>
<span data-ttu-id="6c9fd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6c9fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c9fd-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6c9fd-111">Permission type</span></span>|<span data-ttu-id="6c9fd-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6c9fd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c9fd-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6c9fd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6c9fd-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c9fd-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6c9fd-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6c9fd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c9fd-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6c9fd-116">Not supported.</span></span>|
|<span data-ttu-id="6c9fd-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6c9fd-117">Application</span></span>|<span data-ttu-id="6c9fd-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c9fd-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c9fd-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6c9fd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/enterpriseCodeSigningCertificates/{enterpriseCodeSigningCertificateId}
```

## <a name="request-headers"></a><span data-ttu-id="6c9fd-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6c9fd-120">Request headers</span></span>
|<span data-ttu-id="6c9fd-121">标头</span><span class="sxs-lookup"><span data-stu-id="6c9fd-121">Header</span></span>|<span data-ttu-id="6c9fd-122">值</span><span class="sxs-lookup"><span data-stu-id="6c9fd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c9fd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c9fd-123">Authorization</span></span>|<span data-ttu-id="6c9fd-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6c9fd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c9fd-125">接受</span><span class="sxs-lookup"><span data-stu-id="6c9fd-125">Accept</span></span>|<span data-ttu-id="6c9fd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6c9fd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c9fd-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6c9fd-127">Request body</span></span>
<span data-ttu-id="6c9fd-128">在请求正文中，提供 [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6c9fd-128">In the request body, supply a JSON representation for the [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object.</span></span>

<span data-ttu-id="6c9fd-129">下表显示创建 [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6c9fd-129">The following table shows the properties that are required when you create the [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md).</span></span>

|<span data-ttu-id="6c9fd-130">属性</span><span class="sxs-lookup"><span data-stu-id="6c9fd-130">Property</span></span>|<span data-ttu-id="6c9fd-131">类型</span><span class="sxs-lookup"><span data-stu-id="6c9fd-131">Type</span></span>|<span data-ttu-id="6c9fd-132">说明</span><span class="sxs-lookup"><span data-stu-id="6c9fd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c9fd-133">id</span><span class="sxs-lookup"><span data-stu-id="6c9fd-133">id</span></span>|<span data-ttu-id="6c9fd-134">String</span><span class="sxs-lookup"><span data-stu-id="6c9fd-134">String</span></span>|<span data-ttu-id="6c9fd-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6c9fd-135">The key of the entity.</span></span>|
|<span data-ttu-id="6c9fd-136">content</span><span class="sxs-lookup"><span data-stu-id="6c9fd-136">content</span></span>|<span data-ttu-id="6c9fd-137">Binary</span><span class="sxs-lookup"><span data-stu-id="6c9fd-137">Binary</span></span>|<span data-ttu-id="6c9fd-138">原始数据格式的 Windows 企业代码签名证书。</span><span class="sxs-lookup"><span data-stu-id="6c9fd-138">The Windows Enterprise Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="6c9fd-139">状态</span><span class="sxs-lookup"><span data-stu-id="6c9fd-139">status</span></span>|[<span data-ttu-id="6c9fd-140">certificateStatus</span><span class="sxs-lookup"><span data-stu-id="6c9fd-140">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="6c9fd-141">证书状态已设置或未设置。</span><span class="sxs-lookup"><span data-stu-id="6c9fd-141">The Certificate Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="6c9fd-142">可取值为：`notProvisioned`、`provisioned`。</span><span class="sxs-lookup"><span data-stu-id="6c9fd-142">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="6c9fd-143">SubjectName</span><span class="sxs-lookup"><span data-stu-id="6c9fd-143">subjectName</span></span>|<span data-ttu-id="6c9fd-144">String</span><span class="sxs-lookup"><span data-stu-id="6c9fd-144">String</span></span>|<span data-ttu-id="6c9fd-145">证书的主题名称。</span><span class="sxs-lookup"><span data-stu-id="6c9fd-145">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="6c9fd-146">subject</span><span class="sxs-lookup"><span data-stu-id="6c9fd-146">subject</span></span>|<span data-ttu-id="6c9fd-147">String</span><span class="sxs-lookup"><span data-stu-id="6c9fd-147">String</span></span>|<span data-ttu-id="6c9fd-148">证书的主题值。</span><span class="sxs-lookup"><span data-stu-id="6c9fd-148">The Subject Value for the cert.</span></span>|
|<span data-ttu-id="6c9fd-149">issuerName</span><span class="sxs-lookup"><span data-stu-id="6c9fd-149">issuerName</span></span>|<span data-ttu-id="6c9fd-150">String</span><span class="sxs-lookup"><span data-stu-id="6c9fd-150">String</span></span>|<span data-ttu-id="6c9fd-151">证书的颁发者名称。</span><span class="sxs-lookup"><span data-stu-id="6c9fd-151">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="6c9fd-152">常用</span><span class="sxs-lookup"><span data-stu-id="6c9fd-152">issuer</span></span>|<span data-ttu-id="6c9fd-153">String</span><span class="sxs-lookup"><span data-stu-id="6c9fd-153">String</span></span>|<span data-ttu-id="6c9fd-154">证书的 Issuer 值。</span><span class="sxs-lookup"><span data-stu-id="6c9fd-154">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="6c9fd-155">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="6c9fd-155">expirationDateTime</span></span>|<span data-ttu-id="6c9fd-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c9fd-156">DateTimeOffset</span></span>|<span data-ttu-id="6c9fd-157">证书到期日期。</span><span class="sxs-lookup"><span data-stu-id="6c9fd-157">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="6c9fd-158">uploadDateTime</span><span class="sxs-lookup"><span data-stu-id="6c9fd-158">uploadDateTime</span></span>|<span data-ttu-id="6c9fd-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c9fd-159">DateTimeOffset</span></span>|<span data-ttu-id="6c9fd-160">上传 CodeSigning 证书时的日期时间。</span><span class="sxs-lookup"><span data-stu-id="6c9fd-160">The date time of CodeSigning Cert when it is uploaded.</span></span>|



## <a name="response"></a><span data-ttu-id="6c9fd-161">响应</span><span class="sxs-lookup"><span data-stu-id="6c9fd-161">Response</span></span>
<span data-ttu-id="6c9fd-162">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6c9fd-162">If successful, this method returns a `200 OK` response code and an updated [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c9fd-163">示例</span><span class="sxs-lookup"><span data-stu-id="6c9fd-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="6c9fd-164">请求</span><span class="sxs-lookup"><span data-stu-id="6c9fd-164">Request</span></span>
<span data-ttu-id="6c9fd-165">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6c9fd-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/enterpriseCodeSigningCertificates/{enterpriseCodeSigningCertificateId}
Content-type: application/json
Content-length: 390

{
  "@odata.type": "#microsoft.graph.enterpriseCodeSigningCertificate",
  "content": "Y29udGVudA==",
  "status": "provisioned",
  "subjectName": "Subject Name value",
  "subject": "Subject value",
  "issuerName": "Issuer Name value",
  "issuer": "Issuer value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "uploadDateTime": "2016-12-31T23:58:46.5747426-08:00"
}
```

### <a name="response"></a><span data-ttu-id="6c9fd-166">响应</span><span class="sxs-lookup"><span data-stu-id="6c9fd-166">Response</span></span>
<span data-ttu-id="6c9fd-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6c9fd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 439

{
  "@odata.type": "#microsoft.graph.enterpriseCodeSigningCertificate",
  "id": "b20d3703-3703-b20d-0337-0db203370db2",
  "content": "Y29udGVudA==",
  "status": "provisioned",
  "subjectName": "Subject Name value",
  "subject": "Subject value",
  "issuerName": "Issuer Name value",
  "issuer": "Issuer value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "uploadDateTime": "2016-12-31T23:58:46.5747426-08:00"
}
```






