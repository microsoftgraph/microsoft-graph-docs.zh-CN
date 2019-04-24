---
title: 更新 enterpriseCodeSigningCertificate
description: 更新 enterpriseCodeSigningCertificate 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cc97e3cceada031747dbbc32b40e0c9b6b8c31e6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32496476"
---
# <a name="update-enterprisecodesigningcertificate"></a><span data-ttu-id="f9728-103">更新 enterpriseCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="f9728-103">Update enterpriseCodeSigningCertificate</span></span>

> <span data-ttu-id="f9728-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f9728-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f9728-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f9728-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9728-106">更新[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f9728-106">Update the properties of a [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f9728-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="f9728-107">Prerequisites</span></span>
<span data-ttu-id="f9728-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f9728-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9728-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f9728-110">Permission type</span></span>|<span data-ttu-id="f9728-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f9728-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9728-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f9728-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f9728-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9728-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f9728-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f9728-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9728-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f9728-115">Not supported.</span></span>|
|<span data-ttu-id="f9728-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f9728-116">Application</span></span>|<span data-ttu-id="f9728-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f9728-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9728-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f9728-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/enterpriseCodeSigningCertificates/{enterpriseCodeSigningCertificateId}
```

## <a name="request-headers"></a><span data-ttu-id="f9728-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f9728-119">Request headers</span></span>
|<span data-ttu-id="f9728-120">标头</span><span class="sxs-lookup"><span data-stu-id="f9728-120">Header</span></span>|<span data-ttu-id="f9728-121">值</span><span class="sxs-lookup"><span data-stu-id="f9728-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9728-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9728-122">Authorization</span></span>|<span data-ttu-id="f9728-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f9728-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9728-124">接受</span><span class="sxs-lookup"><span data-stu-id="f9728-124">Accept</span></span>|<span data-ttu-id="f9728-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f9728-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9728-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f9728-126">Request body</span></span>
<span data-ttu-id="f9728-127">在请求正文中, 提供[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f9728-127">In the request body, supply a JSON representation for the [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object.</span></span>

<span data-ttu-id="f9728-128">下表显示创建[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f9728-128">The following table shows the properties that are required when you create the [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md).</span></span>

|<span data-ttu-id="f9728-129">属性</span><span class="sxs-lookup"><span data-stu-id="f9728-129">Property</span></span>|<span data-ttu-id="f9728-130">类型</span><span class="sxs-lookup"><span data-stu-id="f9728-130">Type</span></span>|<span data-ttu-id="f9728-131">说明</span><span class="sxs-lookup"><span data-stu-id="f9728-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9728-132">id</span><span class="sxs-lookup"><span data-stu-id="f9728-132">id</span></span>|<span data-ttu-id="f9728-133">String</span><span class="sxs-lookup"><span data-stu-id="f9728-133">String</span></span>|<span data-ttu-id="f9728-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f9728-134">The key of the entity.</span></span>|
|<span data-ttu-id="f9728-135">content</span><span class="sxs-lookup"><span data-stu-id="f9728-135">content</span></span>|<span data-ttu-id="f9728-136">Binary</span><span class="sxs-lookup"><span data-stu-id="f9728-136">Binary</span></span>|<span data-ttu-id="f9728-137">原始数据格式的 Windows 企业代码签名证书。</span><span class="sxs-lookup"><span data-stu-id="f9728-137">The Windows Enterprise Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="f9728-138">status</span><span class="sxs-lookup"><span data-stu-id="f9728-138">status</span></span>|[<span data-ttu-id="f9728-139">certificateStatus</span><span class="sxs-lookup"><span data-stu-id="f9728-139">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="f9728-140">证书状态已设置或未设置。</span><span class="sxs-lookup"><span data-stu-id="f9728-140">The Certificate Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="f9728-141">可取值为：`notProvisioned`、`provisioned`。</span><span class="sxs-lookup"><span data-stu-id="f9728-141">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="f9728-142">SubjectName</span><span class="sxs-lookup"><span data-stu-id="f9728-142">subjectName</span></span>|<span data-ttu-id="f9728-143">String</span><span class="sxs-lookup"><span data-stu-id="f9728-143">String</span></span>|<span data-ttu-id="f9728-144">证书的主题名称。</span><span class="sxs-lookup"><span data-stu-id="f9728-144">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="f9728-145">subject</span><span class="sxs-lookup"><span data-stu-id="f9728-145">subject</span></span>|<span data-ttu-id="f9728-146">String</span><span class="sxs-lookup"><span data-stu-id="f9728-146">String</span></span>|<span data-ttu-id="f9728-147">证书的主题值。</span><span class="sxs-lookup"><span data-stu-id="f9728-147">The Subject Value for the cert.</span></span>|
|<span data-ttu-id="f9728-148">issuerName</span><span class="sxs-lookup"><span data-stu-id="f9728-148">issuerName</span></span>|<span data-ttu-id="f9728-149">字符串</span><span class="sxs-lookup"><span data-stu-id="f9728-149">String</span></span>|<span data-ttu-id="f9728-150">证书的颁发者名称。</span><span class="sxs-lookup"><span data-stu-id="f9728-150">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="f9728-151">常用</span><span class="sxs-lookup"><span data-stu-id="f9728-151">issuer</span></span>|<span data-ttu-id="f9728-152">字符串</span><span class="sxs-lookup"><span data-stu-id="f9728-152">String</span></span>|<span data-ttu-id="f9728-153">证书的 Issuer 值。</span><span class="sxs-lookup"><span data-stu-id="f9728-153">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="f9728-154">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f9728-154">expirationDateTime</span></span>|<span data-ttu-id="f9728-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9728-155">DateTimeOffset</span></span>|<span data-ttu-id="f9728-156">证书到期日期。</span><span class="sxs-lookup"><span data-stu-id="f9728-156">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="f9728-157">uploadDateTime</span><span class="sxs-lookup"><span data-stu-id="f9728-157">uploadDateTime</span></span>|<span data-ttu-id="f9728-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9728-158">DateTimeOffset</span></span>|<span data-ttu-id="f9728-159">上传 CodeSigning 证书时的日期时间。</span><span class="sxs-lookup"><span data-stu-id="f9728-159">The date time of CodeSigning Cert when it is uploaded.</span></span>|



## <a name="response"></a><span data-ttu-id="f9728-160">响应</span><span class="sxs-lookup"><span data-stu-id="f9728-160">Response</span></span>
<span data-ttu-id="f9728-161">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f9728-161">If successful, this method returns a `200 OK` response code and an updated [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9728-162">示例</span><span class="sxs-lookup"><span data-stu-id="f9728-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="f9728-163">请求</span><span class="sxs-lookup"><span data-stu-id="f9728-163">Request</span></span>
<span data-ttu-id="f9728-164">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f9728-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f9728-165">响应</span><span class="sxs-lookup"><span data-stu-id="f9728-165">Response</span></span>
<span data-ttu-id="f9728-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f9728-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





