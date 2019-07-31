---
title: 更新 symantecCodeSigningCertificate
description: 更新 symantecCodeSigningCertificate 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3b0bdd179c7b6cd610a5a837c2f3de485c6ec0f7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35960424"
---
# <a name="update-symanteccodesigningcertificate"></a><span data-ttu-id="8d184-103">更新 symantecCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="8d184-103">Update symantecCodeSigningCertificate</span></span>

> <span data-ttu-id="8d184-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8d184-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8d184-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8d184-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d184-106">更新[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8d184-106">Update the properties of a [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8d184-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="8d184-107">Prerequisites</span></span>
<span data-ttu-id="8d184-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8d184-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d184-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8d184-110">Permission type</span></span>|<span data-ttu-id="8d184-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8d184-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d184-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8d184-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8d184-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d184-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8d184-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8d184-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d184-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8d184-115">Not supported.</span></span>|
|<span data-ttu-id="8d184-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8d184-116">Application</span></span>|<span data-ttu-id="8d184-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="8d184-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d184-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8d184-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/symantecCodeSigningCertificate
```

## <a name="request-headers"></a><span data-ttu-id="8d184-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8d184-119">Request headers</span></span>
|<span data-ttu-id="8d184-120">标头</span><span class="sxs-lookup"><span data-stu-id="8d184-120">Header</span></span>|<span data-ttu-id="8d184-121">值</span><span class="sxs-lookup"><span data-stu-id="8d184-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d184-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d184-122">Authorization</span></span>|<span data-ttu-id="8d184-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8d184-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d184-124">接受</span><span class="sxs-lookup"><span data-stu-id="8d184-124">Accept</span></span>|<span data-ttu-id="8d184-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8d184-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d184-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="8d184-126">Request body</span></span>
<span data-ttu-id="8d184-127">在请求正文中, 提供[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8d184-127">In the request body, supply a JSON representation for the [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>

<span data-ttu-id="8d184-128">下表显示创建[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8d184-128">The following table shows the properties that are required when you create the [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md).</span></span>

|<span data-ttu-id="8d184-129">属性</span><span class="sxs-lookup"><span data-stu-id="8d184-129">Property</span></span>|<span data-ttu-id="8d184-130">类型</span><span class="sxs-lookup"><span data-stu-id="8d184-130">Type</span></span>|<span data-ttu-id="8d184-131">说明</span><span class="sxs-lookup"><span data-stu-id="8d184-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d184-132">id</span><span class="sxs-lookup"><span data-stu-id="8d184-132">id</span></span>|<span data-ttu-id="8d184-133">字符串</span><span class="sxs-lookup"><span data-stu-id="8d184-133">String</span></span>|<span data-ttu-id="8d184-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="8d184-134">The key of the entity.</span></span>|
|<span data-ttu-id="8d184-135">content</span><span class="sxs-lookup"><span data-stu-id="8d184-135">content</span></span>|<span data-ttu-id="8d184-136">Binary</span><span class="sxs-lookup"><span data-stu-id="8d184-136">Binary</span></span>|<span data-ttu-id="8d184-137">原始数据格式的 Windows Symantec 代码签名证书。</span><span class="sxs-lookup"><span data-stu-id="8d184-137">The Windows Symantec Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="8d184-138">status</span><span class="sxs-lookup"><span data-stu-id="8d184-138">status</span></span>|[<span data-ttu-id="8d184-139">certificateStatus</span><span class="sxs-lookup"><span data-stu-id="8d184-139">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="8d184-140">证书状态已设置或未设置。</span><span class="sxs-lookup"><span data-stu-id="8d184-140">The Cert Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="8d184-141">可取值为：`notProvisioned`、`provisioned`。</span><span class="sxs-lookup"><span data-stu-id="8d184-141">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="8d184-142">密码</span><span class="sxs-lookup"><span data-stu-id="8d184-142">password</span></span>|<span data-ttu-id="8d184-143">字符串</span><span class="sxs-lookup"><span data-stu-id="8d184-143">String</span></span>|<span data-ttu-id="8d184-144">.Pfx 文件所需的密码。</span><span class="sxs-lookup"><span data-stu-id="8d184-144">The Password required for .pfx file.</span></span>|
|<span data-ttu-id="8d184-145">SubjectName</span><span class="sxs-lookup"><span data-stu-id="8d184-145">subjectName</span></span>|<span data-ttu-id="8d184-146">String</span><span class="sxs-lookup"><span data-stu-id="8d184-146">String</span></span>|<span data-ttu-id="8d184-147">证书的主题名称。</span><span class="sxs-lookup"><span data-stu-id="8d184-147">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="8d184-148">subject</span><span class="sxs-lookup"><span data-stu-id="8d184-148">subject</span></span>|<span data-ttu-id="8d184-149">String</span><span class="sxs-lookup"><span data-stu-id="8d184-149">String</span></span>|<span data-ttu-id="8d184-150">证书的主题值。</span><span class="sxs-lookup"><span data-stu-id="8d184-150">The Subject value for the cert.</span></span>|
|<span data-ttu-id="8d184-151">issuerName</span><span class="sxs-lookup"><span data-stu-id="8d184-151">issuerName</span></span>|<span data-ttu-id="8d184-152">String</span><span class="sxs-lookup"><span data-stu-id="8d184-152">String</span></span>|<span data-ttu-id="8d184-153">证书的颁发者名称。</span><span class="sxs-lookup"><span data-stu-id="8d184-153">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="8d184-154">常用</span><span class="sxs-lookup"><span data-stu-id="8d184-154">issuer</span></span>|<span data-ttu-id="8d184-155">String</span><span class="sxs-lookup"><span data-stu-id="8d184-155">String</span></span>|<span data-ttu-id="8d184-156">证书的 Issuer 值。</span><span class="sxs-lookup"><span data-stu-id="8d184-156">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="8d184-157">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="8d184-157">expirationDateTime</span></span>|<span data-ttu-id="8d184-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d184-158">DateTimeOffset</span></span>|<span data-ttu-id="8d184-159">证书到期日期。</span><span class="sxs-lookup"><span data-stu-id="8d184-159">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="8d184-160">uploadDateTime</span><span class="sxs-lookup"><span data-stu-id="8d184-160">uploadDateTime</span></span>|<span data-ttu-id="8d184-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d184-161">DateTimeOffset</span></span>|<span data-ttu-id="8d184-162">作为 Symantec 证书的 CodeSigning 证书的类型。</span><span class="sxs-lookup"><span data-stu-id="8d184-162">The Type of the CodeSigning Cert as Symantec Cert.</span></span>|



## <a name="response"></a><span data-ttu-id="8d184-163">响应</span><span class="sxs-lookup"><span data-stu-id="8d184-163">Response</span></span>
<span data-ttu-id="8d184-164">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8d184-164">If successful, this method returns a `200 OK` response code and an updated [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d184-165">示例</span><span class="sxs-lookup"><span data-stu-id="8d184-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="8d184-166">请求</span><span class="sxs-lookup"><span data-stu-id="8d184-166">Request</span></span>
<span data-ttu-id="8d184-167">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8d184-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8d184-168">响应</span><span class="sxs-lookup"><span data-stu-id="8d184-168">Response</span></span>
<span data-ttu-id="8d184-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8d184-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





