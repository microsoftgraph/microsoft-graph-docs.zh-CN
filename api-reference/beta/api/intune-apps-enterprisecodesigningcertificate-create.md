---
title: 创建 enterpriseCodeSigningCertificate
description: 创建新的 enterpriseCodeSigningCertificate 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 88c98f528fc1ea410170486fb4846b11a1527512
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37178009"
---
# <a name="create-enterprisecodesigningcertificate"></a><span data-ttu-id="f542b-103">创建 enterpriseCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="f542b-103">Create enterpriseCodeSigningCertificate</span></span>

> <span data-ttu-id="f542b-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f542b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f542b-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f542b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f542b-106">创建新的[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f542b-106">Create a new [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f542b-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="f542b-107">Prerequisites</span></span>
<span data-ttu-id="f542b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f542b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f542b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f542b-110">Permission type</span></span>|<span data-ttu-id="f542b-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f542b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f542b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f542b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f542b-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f542b-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f542b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f542b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f542b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f542b-115">Not supported.</span></span>|
|<span data-ttu-id="f542b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f542b-116">Application</span></span>|<span data-ttu-id="f542b-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f542b-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f542b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f542b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/enterpriseCodeSigningCertificates
```

## <a name="request-headers"></a><span data-ttu-id="f542b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f542b-119">Request headers</span></span>
|<span data-ttu-id="f542b-120">标头</span><span class="sxs-lookup"><span data-stu-id="f542b-120">Header</span></span>|<span data-ttu-id="f542b-121">值</span><span class="sxs-lookup"><span data-stu-id="f542b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f542b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f542b-122">Authorization</span></span>|<span data-ttu-id="f542b-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f542b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f542b-124">接受</span><span class="sxs-lookup"><span data-stu-id="f542b-124">Accept</span></span>|<span data-ttu-id="f542b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f542b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f542b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f542b-126">Request body</span></span>
<span data-ttu-id="f542b-127">在请求正文中，提供 enterpriseCodeSigningCertificate 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f542b-127">In the request body, supply a JSON representation for the enterpriseCodeSigningCertificate object.</span></span>

<span data-ttu-id="f542b-128">下表显示创建 enterpriseCodeSigningCertificate 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f542b-128">The following table shows the properties that are required when you create the enterpriseCodeSigningCertificate.</span></span>

|<span data-ttu-id="f542b-129">属性</span><span class="sxs-lookup"><span data-stu-id="f542b-129">Property</span></span>|<span data-ttu-id="f542b-130">类型</span><span class="sxs-lookup"><span data-stu-id="f542b-130">Type</span></span>|<span data-ttu-id="f542b-131">说明</span><span class="sxs-lookup"><span data-stu-id="f542b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f542b-132">id</span><span class="sxs-lookup"><span data-stu-id="f542b-132">id</span></span>|<span data-ttu-id="f542b-133">字符串</span><span class="sxs-lookup"><span data-stu-id="f542b-133">String</span></span>|<span data-ttu-id="f542b-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f542b-134">The key of the entity.</span></span>|
|<span data-ttu-id="f542b-135">content</span><span class="sxs-lookup"><span data-stu-id="f542b-135">content</span></span>|<span data-ttu-id="f542b-136">Binary</span><span class="sxs-lookup"><span data-stu-id="f542b-136">Binary</span></span>|<span data-ttu-id="f542b-137">原始数据格式的 Windows 企业代码签名证书。</span><span class="sxs-lookup"><span data-stu-id="f542b-137">The Windows Enterprise Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="f542b-138">status</span><span class="sxs-lookup"><span data-stu-id="f542b-138">status</span></span>|[<span data-ttu-id="f542b-139">certificateStatus</span><span class="sxs-lookup"><span data-stu-id="f542b-139">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="f542b-140">证书状态已设置或未设置。</span><span class="sxs-lookup"><span data-stu-id="f542b-140">The Certificate Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="f542b-141">可取值为：`notProvisioned`、`provisioned`。</span><span class="sxs-lookup"><span data-stu-id="f542b-141">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="f542b-142">SubjectName</span><span class="sxs-lookup"><span data-stu-id="f542b-142">subjectName</span></span>|<span data-ttu-id="f542b-143">String</span><span class="sxs-lookup"><span data-stu-id="f542b-143">String</span></span>|<span data-ttu-id="f542b-144">证书的主题名称。</span><span class="sxs-lookup"><span data-stu-id="f542b-144">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="f542b-145">subject</span><span class="sxs-lookup"><span data-stu-id="f542b-145">subject</span></span>|<span data-ttu-id="f542b-146">String</span><span class="sxs-lookup"><span data-stu-id="f542b-146">String</span></span>|<span data-ttu-id="f542b-147">证书的主题值。</span><span class="sxs-lookup"><span data-stu-id="f542b-147">The Subject Value for the cert.</span></span>|
|<span data-ttu-id="f542b-148">issuerName</span><span class="sxs-lookup"><span data-stu-id="f542b-148">issuerName</span></span>|<span data-ttu-id="f542b-149">String</span><span class="sxs-lookup"><span data-stu-id="f542b-149">String</span></span>|<span data-ttu-id="f542b-150">证书的颁发者名称。</span><span class="sxs-lookup"><span data-stu-id="f542b-150">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="f542b-151">常用</span><span class="sxs-lookup"><span data-stu-id="f542b-151">issuer</span></span>|<span data-ttu-id="f542b-152">String</span><span class="sxs-lookup"><span data-stu-id="f542b-152">String</span></span>|<span data-ttu-id="f542b-153">证书的 Issuer 值。</span><span class="sxs-lookup"><span data-stu-id="f542b-153">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="f542b-154">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f542b-154">expirationDateTime</span></span>|<span data-ttu-id="f542b-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f542b-155">DateTimeOffset</span></span>|<span data-ttu-id="f542b-156">证书到期日期。</span><span class="sxs-lookup"><span data-stu-id="f542b-156">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="f542b-157">uploadDateTime</span><span class="sxs-lookup"><span data-stu-id="f542b-157">uploadDateTime</span></span>|<span data-ttu-id="f542b-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f542b-158">DateTimeOffset</span></span>|<span data-ttu-id="f542b-159">上传 CodeSigning 证书时的日期时间。</span><span class="sxs-lookup"><span data-stu-id="f542b-159">The date time of CodeSigning Cert when it is uploaded.</span></span>|



## <a name="response"></a><span data-ttu-id="f542b-160">响应</span><span class="sxs-lookup"><span data-stu-id="f542b-160">Response</span></span>
<span data-ttu-id="f542b-161">如果成功，此方法在响应`201 Created`正文中返回响应代码和[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f542b-161">If successful, this method returns a `201 Created` response code and a [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f542b-162">示例</span><span class="sxs-lookup"><span data-stu-id="f542b-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="f542b-163">请求</span><span class="sxs-lookup"><span data-stu-id="f542b-163">Request</span></span>
<span data-ttu-id="f542b-164">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f542b-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/enterpriseCodeSigningCertificates
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

### <a name="response"></a><span data-ttu-id="f542b-165">响应</span><span class="sxs-lookup"><span data-stu-id="f542b-165">Response</span></span>
<span data-ttu-id="f542b-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f542b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




