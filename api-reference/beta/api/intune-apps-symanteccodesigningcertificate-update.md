---
title: 更新 symantecCodeSigningCertificate
description: 更新 symantecCodeSigningCertificate 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 27d4833c82819c5a646cbad25959bdb6071a782c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42450627"
---
# <a name="update-symanteccodesigningcertificate"></a><span data-ttu-id="e5494-103">更新 symantecCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="e5494-103">Update symantecCodeSigningCertificate</span></span>

<span data-ttu-id="e5494-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="e5494-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e5494-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e5494-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5494-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e5494-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5494-107">更新[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e5494-107">Update the properties of a [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e5494-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e5494-108">Prerequisites</span></span>
<span data-ttu-id="e5494-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e5494-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5494-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e5494-111">Permission type</span></span>|<span data-ttu-id="e5494-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e5494-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5494-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e5494-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e5494-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5494-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e5494-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e5494-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5494-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e5494-116">Not supported.</span></span>|
|<span data-ttu-id="e5494-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e5494-117">Application</span></span>|<span data-ttu-id="e5494-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5494-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5494-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e5494-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/symantecCodeSigningCertificate
```

## <a name="request-headers"></a><span data-ttu-id="e5494-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e5494-120">Request headers</span></span>
|<span data-ttu-id="e5494-121">标头</span><span class="sxs-lookup"><span data-stu-id="e5494-121">Header</span></span>|<span data-ttu-id="e5494-122">值</span><span class="sxs-lookup"><span data-stu-id="e5494-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e5494-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5494-123">Authorization</span></span>|<span data-ttu-id="e5494-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e5494-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e5494-125">接受</span><span class="sxs-lookup"><span data-stu-id="e5494-125">Accept</span></span>|<span data-ttu-id="e5494-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e5494-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5494-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e5494-127">Request body</span></span>
<span data-ttu-id="e5494-128">在请求正文中，提供[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e5494-128">In the request body, supply a JSON representation for the [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>

<span data-ttu-id="e5494-129">下表显示创建[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e5494-129">The following table shows the properties that are required when you create the [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md).</span></span>

|<span data-ttu-id="e5494-130">属性</span><span class="sxs-lookup"><span data-stu-id="e5494-130">Property</span></span>|<span data-ttu-id="e5494-131">类型</span><span class="sxs-lookup"><span data-stu-id="e5494-131">Type</span></span>|<span data-ttu-id="e5494-132">说明</span><span class="sxs-lookup"><span data-stu-id="e5494-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5494-133">id</span><span class="sxs-lookup"><span data-stu-id="e5494-133">id</span></span>|<span data-ttu-id="e5494-134">字符串</span><span class="sxs-lookup"><span data-stu-id="e5494-134">String</span></span>|<span data-ttu-id="e5494-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e5494-135">The key of the entity.</span></span>|
|<span data-ttu-id="e5494-136">content</span><span class="sxs-lookup"><span data-stu-id="e5494-136">content</span></span>|<span data-ttu-id="e5494-137">Binary</span><span class="sxs-lookup"><span data-stu-id="e5494-137">Binary</span></span>|<span data-ttu-id="e5494-138">原始数据格式的 Windows Symantec 代码签名证书。</span><span class="sxs-lookup"><span data-stu-id="e5494-138">The Windows Symantec Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="e5494-139">status</span><span class="sxs-lookup"><span data-stu-id="e5494-139">status</span></span>|[<span data-ttu-id="e5494-140">certificateStatus</span><span class="sxs-lookup"><span data-stu-id="e5494-140">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="e5494-141">证书状态已设置或未设置。</span><span class="sxs-lookup"><span data-stu-id="e5494-141">The Cert Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="e5494-142">可取值为：`notProvisioned`、`provisioned`。</span><span class="sxs-lookup"><span data-stu-id="e5494-142">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="e5494-143">密码</span><span class="sxs-lookup"><span data-stu-id="e5494-143">password</span></span>|<span data-ttu-id="e5494-144">字符串</span><span class="sxs-lookup"><span data-stu-id="e5494-144">String</span></span>|<span data-ttu-id="e5494-145">.Pfx 文件所需的密码。</span><span class="sxs-lookup"><span data-stu-id="e5494-145">The Password required for .pfx file.</span></span>|
|<span data-ttu-id="e5494-146">SubjectName</span><span class="sxs-lookup"><span data-stu-id="e5494-146">subjectName</span></span>|<span data-ttu-id="e5494-147">String</span><span class="sxs-lookup"><span data-stu-id="e5494-147">String</span></span>|<span data-ttu-id="e5494-148">证书的主题名称。</span><span class="sxs-lookup"><span data-stu-id="e5494-148">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="e5494-149">subject</span><span class="sxs-lookup"><span data-stu-id="e5494-149">subject</span></span>|<span data-ttu-id="e5494-150">String</span><span class="sxs-lookup"><span data-stu-id="e5494-150">String</span></span>|<span data-ttu-id="e5494-151">证书的主题值。</span><span class="sxs-lookup"><span data-stu-id="e5494-151">The Subject value for the cert.</span></span>|
|<span data-ttu-id="e5494-152">issuerName</span><span class="sxs-lookup"><span data-stu-id="e5494-152">issuerName</span></span>|<span data-ttu-id="e5494-153">String</span><span class="sxs-lookup"><span data-stu-id="e5494-153">String</span></span>|<span data-ttu-id="e5494-154">证书的颁发者名称。</span><span class="sxs-lookup"><span data-stu-id="e5494-154">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="e5494-155">常用</span><span class="sxs-lookup"><span data-stu-id="e5494-155">issuer</span></span>|<span data-ttu-id="e5494-156">String</span><span class="sxs-lookup"><span data-stu-id="e5494-156">String</span></span>|<span data-ttu-id="e5494-157">证书的 Issuer 值。</span><span class="sxs-lookup"><span data-stu-id="e5494-157">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="e5494-158">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="e5494-158">expirationDateTime</span></span>|<span data-ttu-id="e5494-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5494-159">DateTimeOffset</span></span>|<span data-ttu-id="e5494-160">证书到期日期。</span><span class="sxs-lookup"><span data-stu-id="e5494-160">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="e5494-161">uploadDateTime</span><span class="sxs-lookup"><span data-stu-id="e5494-161">uploadDateTime</span></span>|<span data-ttu-id="e5494-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5494-162">DateTimeOffset</span></span>|<span data-ttu-id="e5494-163">作为 Symantec 证书的 CodeSigning 证书的类型。</span><span class="sxs-lookup"><span data-stu-id="e5494-163">The Type of the CodeSigning Cert as Symantec Cert.</span></span>|



## <a name="response"></a><span data-ttu-id="e5494-164">响应</span><span class="sxs-lookup"><span data-stu-id="e5494-164">Response</span></span>
<span data-ttu-id="e5494-165">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e5494-165">If successful, this method returns a `200 OK` response code and an updated [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5494-166">示例</span><span class="sxs-lookup"><span data-stu-id="e5494-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="e5494-167">请求</span><span class="sxs-lookup"><span data-stu-id="e5494-167">Request</span></span>
<span data-ttu-id="e5494-168">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e5494-168">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/symantecCodeSigningCertificate
Content-type: application/json
Content-length: 421

{
  "@odata.type": "#microsoft.graph.symantecCodeSigningCertificate",
  "content": "Y29udGVudA==",
  "status": "provisioned",
  "password": "Password value",
  "subjectName": "Subject Name value",
  "subject": "Subject value",
  "issuerName": "Issuer Name value",
  "issuer": "Issuer value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "uploadDateTime": "2016-12-31T23:58:46.5747426-08:00"
}
```

### <a name="response"></a><span data-ttu-id="e5494-169">响应</span><span class="sxs-lookup"><span data-stu-id="e5494-169">Response</span></span>
<span data-ttu-id="e5494-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e5494-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 470

{
  "@odata.type": "#microsoft.graph.symantecCodeSigningCertificate",
  "id": "00ffe83e-e83e-00ff-3ee8-ff003ee8ff00",
  "content": "Y29udGVudA==",
  "status": "provisioned",
  "password": "Password value",
  "subjectName": "Subject Name value",
  "subject": "Subject value",
  "issuerName": "Issuer Name value",
  "issuer": "Issuer value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "uploadDateTime": "2016-12-31T23:58:46.5747426-08:00"
}
```





