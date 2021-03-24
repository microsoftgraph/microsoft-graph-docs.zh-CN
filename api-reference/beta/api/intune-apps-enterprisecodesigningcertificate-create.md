---
title: 创建 enterpriseCodeSigningCertificate
description: 创建新的 enterpriseCodeSigningCertificate 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d0c5d96d6e5362866c279211f4252bd9cd544c1e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51144287"
---
# <a name="create-enterprisecodesigningcertificate"></a><span data-ttu-id="a0c3c-103">创建 enterpriseCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="a0c3c-103">Create enterpriseCodeSigningCertificate</span></span>

<span data-ttu-id="a0c3c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0c3c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a0c3c-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a0c3c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a0c3c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a0c3c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0c3c-107">创建新的 [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a0c3c-107">Create a new [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a0c3c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a0c3c-108">Prerequisites</span></span>
<span data-ttu-id="a0c3c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a0c3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0c3c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a0c3c-111">Permission type</span></span>|<span data-ttu-id="a0c3c-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a0c3c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0c3c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a0c3c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a0c3c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0c3c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a0c3c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a0c3c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0c3c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a0c3c-116">Not supported.</span></span>|
|<span data-ttu-id="a0c3c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a0c3c-117">Application</span></span>|<span data-ttu-id="a0c3c-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0c3c-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0c3c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a0c3c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/enterpriseCodeSigningCertificates
```

## <a name="request-headers"></a><span data-ttu-id="a0c3c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a0c3c-120">Request headers</span></span>
|<span data-ttu-id="a0c3c-121">标头</span><span class="sxs-lookup"><span data-stu-id="a0c3c-121">Header</span></span>|<span data-ttu-id="a0c3c-122">值</span><span class="sxs-lookup"><span data-stu-id="a0c3c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0c3c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0c3c-123">Authorization</span></span>|<span data-ttu-id="a0c3c-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a0c3c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0c3c-125">接受</span><span class="sxs-lookup"><span data-stu-id="a0c3c-125">Accept</span></span>|<span data-ttu-id="a0c3c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a0c3c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0c3c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a0c3c-127">Request body</span></span>
<span data-ttu-id="a0c3c-128">在请求正文中，提供 enterpriseCodeSigningCertificate 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a0c3c-128">In the request body, supply a JSON representation for the enterpriseCodeSigningCertificate object.</span></span>

<span data-ttu-id="a0c3c-129">下表显示创建 enterpriseCodeSigningCertificate 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a0c3c-129">The following table shows the properties that are required when you create the enterpriseCodeSigningCertificate.</span></span>

|<span data-ttu-id="a0c3c-130">属性</span><span class="sxs-lookup"><span data-stu-id="a0c3c-130">Property</span></span>|<span data-ttu-id="a0c3c-131">类型</span><span class="sxs-lookup"><span data-stu-id="a0c3c-131">Type</span></span>|<span data-ttu-id="a0c3c-132">说明</span><span class="sxs-lookup"><span data-stu-id="a0c3c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0c3c-133">id</span><span class="sxs-lookup"><span data-stu-id="a0c3c-133">id</span></span>|<span data-ttu-id="a0c3c-134">String</span><span class="sxs-lookup"><span data-stu-id="a0c3c-134">String</span></span>|<span data-ttu-id="a0c3c-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a0c3c-135">The key of the entity.</span></span>|
|<span data-ttu-id="a0c3c-136">content</span><span class="sxs-lookup"><span data-stu-id="a0c3c-136">content</span></span>|<span data-ttu-id="a0c3c-137">Binary</span><span class="sxs-lookup"><span data-stu-id="a0c3c-137">Binary</span></span>|<span data-ttu-id="a0c3c-138">Windows 企业Code-Signing采用原始数据格式的证书。</span><span class="sxs-lookup"><span data-stu-id="a0c3c-138">The Windows Enterprise Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="a0c3c-139">状态</span><span class="sxs-lookup"><span data-stu-id="a0c3c-139">status</span></span>|[<span data-ttu-id="a0c3c-140">certificateStatus</span><span class="sxs-lookup"><span data-stu-id="a0c3c-140">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="a0c3c-141">证书状态已设置或未设置。</span><span class="sxs-lookup"><span data-stu-id="a0c3c-141">The Certificate Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="a0c3c-142">可取值为：`notProvisioned`、`provisioned`。</span><span class="sxs-lookup"><span data-stu-id="a0c3c-142">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="a0c3c-143">SubjectName</span><span class="sxs-lookup"><span data-stu-id="a0c3c-143">subjectName</span></span>|<span data-ttu-id="a0c3c-144">String</span><span class="sxs-lookup"><span data-stu-id="a0c3c-144">String</span></span>|<span data-ttu-id="a0c3c-145">证书的主题名称。</span><span class="sxs-lookup"><span data-stu-id="a0c3c-145">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="a0c3c-146">subject</span><span class="sxs-lookup"><span data-stu-id="a0c3c-146">subject</span></span>|<span data-ttu-id="a0c3c-147">String</span><span class="sxs-lookup"><span data-stu-id="a0c3c-147">String</span></span>|<span data-ttu-id="a0c3c-148">证书的主题值。</span><span class="sxs-lookup"><span data-stu-id="a0c3c-148">The Subject Value for the cert.</span></span>|
|<span data-ttu-id="a0c3c-149">issuerName</span><span class="sxs-lookup"><span data-stu-id="a0c3c-149">issuerName</span></span>|<span data-ttu-id="a0c3c-150">String</span><span class="sxs-lookup"><span data-stu-id="a0c3c-150">String</span></span>|<span data-ttu-id="a0c3c-151">证书的颁发者名称。</span><span class="sxs-lookup"><span data-stu-id="a0c3c-151">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="a0c3c-152">issuer</span><span class="sxs-lookup"><span data-stu-id="a0c3c-152">issuer</span></span>|<span data-ttu-id="a0c3c-153">String</span><span class="sxs-lookup"><span data-stu-id="a0c3c-153">String</span></span>|<span data-ttu-id="a0c3c-154">证书的 Issuer 值。</span><span class="sxs-lookup"><span data-stu-id="a0c3c-154">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="a0c3c-155">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a0c3c-155">expirationDateTime</span></span>|<span data-ttu-id="a0c3c-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0c3c-156">DateTimeOffset</span></span>|<span data-ttu-id="a0c3c-157">证书到期日期。</span><span class="sxs-lookup"><span data-stu-id="a0c3c-157">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="a0c3c-158">uploadDateTime</span><span class="sxs-lookup"><span data-stu-id="a0c3c-158">uploadDateTime</span></span>|<span data-ttu-id="a0c3c-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0c3c-159">DateTimeOffset</span></span>|<span data-ttu-id="a0c3c-160">CodeSigning 证书上载时的日期时间。</span><span class="sxs-lookup"><span data-stu-id="a0c3c-160">The date time of CodeSigning Cert when it is uploaded.</span></span>|



## <a name="response"></a><span data-ttu-id="a0c3c-161">响应</span><span class="sxs-lookup"><span data-stu-id="a0c3c-161">Response</span></span>
<span data-ttu-id="a0c3c-162">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a0c3c-162">If successful, this method returns a `201 Created` response code and a [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0c3c-163">示例</span><span class="sxs-lookup"><span data-stu-id="a0c3c-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="a0c3c-164">请求</span><span class="sxs-lookup"><span data-stu-id="a0c3c-164">Request</span></span>
<span data-ttu-id="a0c3c-165">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a0c3c-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a0c3c-166">响应</span><span class="sxs-lookup"><span data-stu-id="a0c3c-166">Response</span></span>
<span data-ttu-id="a0c3c-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a0c3c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




