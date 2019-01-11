---
title: 更新 enterpriseCodeSigningCertificate
description: 更新 enterpriseCodeSigningCertificate 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5272c0ff0e18fd7200e85ff51575c10825dbf7f5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829314"
---
# <a name="update-enterprisecodesigningcertificate"></a><span data-ttu-id="c409f-103">更新 enterpriseCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="c409f-103">Update enterpriseCodeSigningCertificate</span></span>

> <span data-ttu-id="c409f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c409f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c409f-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c409f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c409f-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c409f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c409f-107">更新[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c409f-107">Update the properties of a [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c409f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c409f-108">Prerequisites</span></span>
<span data-ttu-id="c409f-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="c409f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c409f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c409f-111">Permission type</span></span>|<span data-ttu-id="c409f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c409f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c409f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c409f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c409f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c409f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c409f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c409f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c409f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c409f-116">Not supported.</span></span>|
|<span data-ttu-id="c409f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c409f-117">Application</span></span>|<span data-ttu-id="c409f-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="c409f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c409f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c409f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/enterpriseCodeSigningCertificates/{enterpriseCodeSigningCertificateId}
```

## <a name="request-headers"></a><span data-ttu-id="c409f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c409f-120">Request headers</span></span>
|<span data-ttu-id="c409f-121">标头</span><span class="sxs-lookup"><span data-stu-id="c409f-121">Header</span></span>|<span data-ttu-id="c409f-122">值</span><span class="sxs-lookup"><span data-stu-id="c409f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c409f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c409f-123">Authorization</span></span>|<span data-ttu-id="c409f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c409f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c409f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c409f-125">Accept</span></span>|<span data-ttu-id="c409f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c409f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c409f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c409f-127">Request body</span></span>
<span data-ttu-id="c409f-128">在请求正文中，提供[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c409f-128">In the request body, supply a JSON representation for the [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object.</span></span>

<span data-ttu-id="c409f-129">下表显示时创建[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c409f-129">The following table shows the properties that are required when you create the [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md).</span></span>

|<span data-ttu-id="c409f-130">属性</span><span class="sxs-lookup"><span data-stu-id="c409f-130">Property</span></span>|<span data-ttu-id="c409f-131">类型</span><span class="sxs-lookup"><span data-stu-id="c409f-131">Type</span></span>|<span data-ttu-id="c409f-132">说明</span><span class="sxs-lookup"><span data-stu-id="c409f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c409f-133">id</span><span class="sxs-lookup"><span data-stu-id="c409f-133">id</span></span>|<span data-ttu-id="c409f-134">String</span><span class="sxs-lookup"><span data-stu-id="c409f-134">String</span></span>|<span data-ttu-id="c409f-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c409f-135">The key of the entity.</span></span>|
|<span data-ttu-id="c409f-136">content</span><span class="sxs-lookup"><span data-stu-id="c409f-136">content</span></span>|<span data-ttu-id="c409f-137">Binary</span><span class="sxs-lookup"><span data-stu-id="c409f-137">Binary</span></span>|<span data-ttu-id="c409f-138">中的原始数据格式的 Windows 企业代码签名证书。</span><span class="sxs-lookup"><span data-stu-id="c409f-138">The Windows Enterprise Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="c409f-139">status</span><span class="sxs-lookup"><span data-stu-id="c409f-139">status</span></span>|[<span data-ttu-id="c409f-140">certificateStatus</span><span class="sxs-lookup"><span data-stu-id="c409f-140">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="c409f-141">设置或未设置证书的状态。</span><span class="sxs-lookup"><span data-stu-id="c409f-141">The Certificate Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="c409f-142">可取值为：`notProvisioned`、`provisioned`。</span><span class="sxs-lookup"><span data-stu-id="c409f-142">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="c409f-143">SubjectName</span><span class="sxs-lookup"><span data-stu-id="c409f-143">subjectName</span></span>|<span data-ttu-id="c409f-144">String</span><span class="sxs-lookup"><span data-stu-id="c409f-144">String</span></span>|<span data-ttu-id="c409f-145">证书使用者名称。</span><span class="sxs-lookup"><span data-stu-id="c409f-145">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="c409f-146">subject</span><span class="sxs-lookup"><span data-stu-id="c409f-146">subject</span></span>|<span data-ttu-id="c409f-147">字符串</span><span class="sxs-lookup"><span data-stu-id="c409f-147">String</span></span>|<span data-ttu-id="c409f-148">证书使用者值。</span><span class="sxs-lookup"><span data-stu-id="c409f-148">The Subject Value for the cert.</span></span>|
|<span data-ttu-id="c409f-149">issuerName</span><span class="sxs-lookup"><span data-stu-id="c409f-149">issuerName</span></span>|<span data-ttu-id="c409f-150">字符串</span><span class="sxs-lookup"><span data-stu-id="c409f-150">String</span></span>|<span data-ttu-id="c409f-151">证书颁发者名称。</span><span class="sxs-lookup"><span data-stu-id="c409f-151">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="c409f-152">颁发者</span><span class="sxs-lookup"><span data-stu-id="c409f-152">issuer</span></span>|<span data-ttu-id="c409f-153">字符串</span><span class="sxs-lookup"><span data-stu-id="c409f-153">String</span></span>|<span data-ttu-id="c409f-154">证书颁发者值。</span><span class="sxs-lookup"><span data-stu-id="c409f-154">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="c409f-155">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="c409f-155">expirationDateTime</span></span>|<span data-ttu-id="c409f-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c409f-156">DateTimeOffset</span></span>|<span data-ttu-id="c409f-157">证书到期日期。</span><span class="sxs-lookup"><span data-stu-id="c409f-157">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="c409f-158">uploadDateTime</span><span class="sxs-lookup"><span data-stu-id="c409f-158">uploadDateTime</span></span>|<span data-ttu-id="c409f-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c409f-159">DateTimeOffset</span></span>|<span data-ttu-id="c409f-160">代码签名证书时它的上载日期时间。</span><span class="sxs-lookup"><span data-stu-id="c409f-160">The date time of CodeSigning Cert when it is uploaded.</span></span>|



## <a name="response"></a><span data-ttu-id="c409f-161">响应</span><span class="sxs-lookup"><span data-stu-id="c409f-161">Response</span></span>
<span data-ttu-id="c409f-162">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c409f-162">If successful, this method returns a `200 OK` response code and an updated [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c409f-163">示例</span><span class="sxs-lookup"><span data-stu-id="c409f-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="c409f-164">请求</span><span class="sxs-lookup"><span data-stu-id="c409f-164">Request</span></span>
<span data-ttu-id="c409f-165">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c409f-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/enterpriseCodeSigningCertificates/{enterpriseCodeSigningCertificateId}
Content-type: application/json
Content-length: 319

{
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

### <a name="response"></a><span data-ttu-id="c409f-166">响应</span><span class="sxs-lookup"><span data-stu-id="c409f-166">Response</span></span>
<span data-ttu-id="c409f-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c409f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





