---
title: 创建 enterpriseCodeSigningCertificate
description: 创建新的 enterpriseCodeSigningCertificate 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e5ba50739903fce6e462f5c1a2602a4a61221eb3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402550"
---
# <a name="create-enterprisecodesigningcertificate"></a><span data-ttu-id="88f2c-103">创建 enterpriseCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="88f2c-103">Create enterpriseCodeSigningCertificate</span></span>

> <span data-ttu-id="88f2c-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="88f2c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="88f2c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="88f2c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="88f2c-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="88f2c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88f2c-107">创建新的[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="88f2c-107">Create a new [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="88f2c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="88f2c-108">Prerequisites</span></span>
<span data-ttu-id="88f2c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="88f2c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="88f2c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="88f2c-111">Permission type</span></span>|<span data-ttu-id="88f2c-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="88f2c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88f2c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="88f2c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="88f2c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88f2c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="88f2c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="88f2c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88f2c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="88f2c-116">Not supported.</span></span>|
|<span data-ttu-id="88f2c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="88f2c-117">Application</span></span>|<span data-ttu-id="88f2c-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="88f2c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="88f2c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="88f2c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/enterpriseCodeSigningCertificates
```

## <a name="request-headers"></a><span data-ttu-id="88f2c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="88f2c-120">Request headers</span></span>
|<span data-ttu-id="88f2c-121">标头</span><span class="sxs-lookup"><span data-stu-id="88f2c-121">Header</span></span>|<span data-ttu-id="88f2c-122">值</span><span class="sxs-lookup"><span data-stu-id="88f2c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88f2c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="88f2c-123">Authorization</span></span>|<span data-ttu-id="88f2c-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="88f2c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88f2c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="88f2c-125">Accept</span></span>|<span data-ttu-id="88f2c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="88f2c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88f2c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="88f2c-127">Request body</span></span>
<span data-ttu-id="88f2c-128">在请求正文中，提供 enterpriseCodeSigningCertificate 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="88f2c-128">In the request body, supply a JSON representation for the enterpriseCodeSigningCertificate object.</span></span>

<span data-ttu-id="88f2c-129">下表显示时创建 enterpriseCodeSigningCertificate 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="88f2c-129">The following table shows the properties that are required when you create the enterpriseCodeSigningCertificate.</span></span>

|<span data-ttu-id="88f2c-130">属性</span><span class="sxs-lookup"><span data-stu-id="88f2c-130">Property</span></span>|<span data-ttu-id="88f2c-131">类型</span><span class="sxs-lookup"><span data-stu-id="88f2c-131">Type</span></span>|<span data-ttu-id="88f2c-132">说明</span><span class="sxs-lookup"><span data-stu-id="88f2c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88f2c-133">id</span><span class="sxs-lookup"><span data-stu-id="88f2c-133">id</span></span>|<span data-ttu-id="88f2c-134">String</span><span class="sxs-lookup"><span data-stu-id="88f2c-134">String</span></span>|<span data-ttu-id="88f2c-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="88f2c-135">The key of the entity.</span></span>|
|<span data-ttu-id="88f2c-136">content</span><span class="sxs-lookup"><span data-stu-id="88f2c-136">content</span></span>|<span data-ttu-id="88f2c-137">Binary</span><span class="sxs-lookup"><span data-stu-id="88f2c-137">Binary</span></span>|<span data-ttu-id="88f2c-138">中的原始数据格式的 Windows 企业代码签名证书。</span><span class="sxs-lookup"><span data-stu-id="88f2c-138">The Windows Enterprise Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="88f2c-139">status</span><span class="sxs-lookup"><span data-stu-id="88f2c-139">status</span></span>|[<span data-ttu-id="88f2c-140">certificateStatus</span><span class="sxs-lookup"><span data-stu-id="88f2c-140">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="88f2c-141">设置或未设置证书的状态。</span><span class="sxs-lookup"><span data-stu-id="88f2c-141">The Certificate Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="88f2c-142">可取值为：`notProvisioned`、`provisioned`。</span><span class="sxs-lookup"><span data-stu-id="88f2c-142">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="88f2c-143">SubjectName</span><span class="sxs-lookup"><span data-stu-id="88f2c-143">subjectName</span></span>|<span data-ttu-id="88f2c-144">String</span><span class="sxs-lookup"><span data-stu-id="88f2c-144">String</span></span>|<span data-ttu-id="88f2c-145">证书使用者名称。</span><span class="sxs-lookup"><span data-stu-id="88f2c-145">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="88f2c-146">subject</span><span class="sxs-lookup"><span data-stu-id="88f2c-146">subject</span></span>|<span data-ttu-id="88f2c-147">String</span><span class="sxs-lookup"><span data-stu-id="88f2c-147">String</span></span>|<span data-ttu-id="88f2c-148">证书使用者值。</span><span class="sxs-lookup"><span data-stu-id="88f2c-148">The Subject Value for the cert.</span></span>|
|<span data-ttu-id="88f2c-149">issuerName</span><span class="sxs-lookup"><span data-stu-id="88f2c-149">issuerName</span></span>|<span data-ttu-id="88f2c-150">String</span><span class="sxs-lookup"><span data-stu-id="88f2c-150">String</span></span>|<span data-ttu-id="88f2c-151">证书颁发者名称。</span><span class="sxs-lookup"><span data-stu-id="88f2c-151">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="88f2c-152">颁发者</span><span class="sxs-lookup"><span data-stu-id="88f2c-152">issuer</span></span>|<span data-ttu-id="88f2c-153">String</span><span class="sxs-lookup"><span data-stu-id="88f2c-153">String</span></span>|<span data-ttu-id="88f2c-154">证书颁发者值。</span><span class="sxs-lookup"><span data-stu-id="88f2c-154">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="88f2c-155">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="88f2c-155">expirationDateTime</span></span>|<span data-ttu-id="88f2c-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88f2c-156">DateTimeOffset</span></span>|<span data-ttu-id="88f2c-157">证书到期日期。</span><span class="sxs-lookup"><span data-stu-id="88f2c-157">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="88f2c-158">uploadDateTime</span><span class="sxs-lookup"><span data-stu-id="88f2c-158">uploadDateTime</span></span>|<span data-ttu-id="88f2c-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88f2c-159">DateTimeOffset</span></span>|<span data-ttu-id="88f2c-160">代码签名证书时它的上载日期时间。</span><span class="sxs-lookup"><span data-stu-id="88f2c-160">The date time of CodeSigning Cert when it is uploaded.</span></span>|



## <a name="response"></a><span data-ttu-id="88f2c-161">响应</span><span class="sxs-lookup"><span data-stu-id="88f2c-161">Response</span></span>
<span data-ttu-id="88f2c-162">如果成功，此方法返回`201 Created`响应代码和响应正文中的[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="88f2c-162">If successful, this method returns a `201 Created` response code and a [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88f2c-163">示例</span><span class="sxs-lookup"><span data-stu-id="88f2c-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="88f2c-164">请求</span><span class="sxs-lookup"><span data-stu-id="88f2c-164">Request</span></span>
<span data-ttu-id="88f2c-165">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="88f2c-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="88f2c-166">响应</span><span class="sxs-lookup"><span data-stu-id="88f2c-166">Response</span></span>
<span data-ttu-id="88f2c-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="88f2c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




