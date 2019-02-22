---
title: 更新 symantecCodeSigningCertificate
description: 更新 symantecCodeSigningCertificate 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 26a56296956c3955808a308989a0ca8ded5d4ae5
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168752"
---
# <a name="update-symanteccodesigningcertificate"></a><span data-ttu-id="f8085-103">更新 symantecCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="f8085-103">Update symantecCodeSigningCertificate</span></span>

> <span data-ttu-id="f8085-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f8085-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f8085-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f8085-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8085-106">更新[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f8085-106">Update the properties of a [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f8085-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="f8085-107">Prerequisites</span></span>
<span data-ttu-id="f8085-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="f8085-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f8085-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f8085-110">Permission type</span></span>|<span data-ttu-id="f8085-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f8085-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8085-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f8085-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f8085-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8085-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f8085-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f8085-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8085-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f8085-115">Not supported.</span></span>|
|<span data-ttu-id="f8085-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f8085-116">Application</span></span>|<span data-ttu-id="f8085-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f8085-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8085-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f8085-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/symantecCodeSigningCertificate
```

## <a name="request-headers"></a><span data-ttu-id="f8085-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f8085-119">Request headers</span></span>
|<span data-ttu-id="f8085-120">标头</span><span class="sxs-lookup"><span data-stu-id="f8085-120">Header</span></span>|<span data-ttu-id="f8085-121">值</span><span class="sxs-lookup"><span data-stu-id="f8085-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8085-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8085-122">Authorization</span></span>|<span data-ttu-id="f8085-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f8085-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8085-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f8085-124">Accept</span></span>|<span data-ttu-id="f8085-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f8085-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8085-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f8085-126">Request body</span></span>
<span data-ttu-id="f8085-127">在请求正文中, 提供[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f8085-127">In the request body, supply a JSON representation for the [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>

<span data-ttu-id="f8085-128">下表显示创建[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f8085-128">The following table shows the properties that are required when you create the [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md).</span></span>

|<span data-ttu-id="f8085-129">属性</span><span class="sxs-lookup"><span data-stu-id="f8085-129">Property</span></span>|<span data-ttu-id="f8085-130">类型</span><span class="sxs-lookup"><span data-stu-id="f8085-130">Type</span></span>|<span data-ttu-id="f8085-131">说明</span><span class="sxs-lookup"><span data-stu-id="f8085-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8085-132">id</span><span class="sxs-lookup"><span data-stu-id="f8085-132">id</span></span>|<span data-ttu-id="f8085-133">String</span><span class="sxs-lookup"><span data-stu-id="f8085-133">String</span></span>|<span data-ttu-id="f8085-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f8085-134">The key of the entity.</span></span>|
|<span data-ttu-id="f8085-135">content</span><span class="sxs-lookup"><span data-stu-id="f8085-135">content</span></span>|<span data-ttu-id="f8085-136">Binary</span><span class="sxs-lookup"><span data-stu-id="f8085-136">Binary</span></span>|<span data-ttu-id="f8085-137">原始数据格式的 Windows Symantec 代码签名证书。</span><span class="sxs-lookup"><span data-stu-id="f8085-137">The Windows Symantec Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="f8085-138">status</span><span class="sxs-lookup"><span data-stu-id="f8085-138">status</span></span>|[<span data-ttu-id="f8085-139">certificateStatus</span><span class="sxs-lookup"><span data-stu-id="f8085-139">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="f8085-140">证书状态已设置或未设置。</span><span class="sxs-lookup"><span data-stu-id="f8085-140">The Cert Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="f8085-141">可取值为：`notProvisioned`、`provisioned`。</span><span class="sxs-lookup"><span data-stu-id="f8085-141">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="f8085-142">password</span><span class="sxs-lookup"><span data-stu-id="f8085-142">password</span></span>|<span data-ttu-id="f8085-143">字符串</span><span class="sxs-lookup"><span data-stu-id="f8085-143">String</span></span>|<span data-ttu-id="f8085-144">.pfx 文件所需的密码。</span><span class="sxs-lookup"><span data-stu-id="f8085-144">The Password required for .pfx file.</span></span>|
|<span data-ttu-id="f8085-145">SubjectName</span><span class="sxs-lookup"><span data-stu-id="f8085-145">subjectName</span></span>|<span data-ttu-id="f8085-146">String</span><span class="sxs-lookup"><span data-stu-id="f8085-146">String</span></span>|<span data-ttu-id="f8085-147">证书的主题名称。</span><span class="sxs-lookup"><span data-stu-id="f8085-147">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="f8085-148">subject</span><span class="sxs-lookup"><span data-stu-id="f8085-148">subject</span></span>|<span data-ttu-id="f8085-149">字符串</span><span class="sxs-lookup"><span data-stu-id="f8085-149">String</span></span>|<span data-ttu-id="f8085-150">证书的主题值。</span><span class="sxs-lookup"><span data-stu-id="f8085-150">The Subject value for the cert.</span></span>|
|<span data-ttu-id="f8085-151">issuerName</span><span class="sxs-lookup"><span data-stu-id="f8085-151">issuerName</span></span>|<span data-ttu-id="f8085-152">字符串</span><span class="sxs-lookup"><span data-stu-id="f8085-152">String</span></span>|<span data-ttu-id="f8085-153">证书的颁发者名称。</span><span class="sxs-lookup"><span data-stu-id="f8085-153">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="f8085-154">常用</span><span class="sxs-lookup"><span data-stu-id="f8085-154">issuer</span></span>|<span data-ttu-id="f8085-155">字符串</span><span class="sxs-lookup"><span data-stu-id="f8085-155">String</span></span>|<span data-ttu-id="f8085-156">证书的 Issuer 值。</span><span class="sxs-lookup"><span data-stu-id="f8085-156">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="f8085-157">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f8085-157">expirationDateTime</span></span>|<span data-ttu-id="f8085-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8085-158">DateTimeOffset</span></span>|<span data-ttu-id="f8085-159">证书到期日期。</span><span class="sxs-lookup"><span data-stu-id="f8085-159">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="f8085-160">uploadDateTime</span><span class="sxs-lookup"><span data-stu-id="f8085-160">uploadDateTime</span></span>|<span data-ttu-id="f8085-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8085-161">DateTimeOffset</span></span>|<span data-ttu-id="f8085-162">作为 Symantec 证书的 CodeSigning 证书的类型。</span><span class="sxs-lookup"><span data-stu-id="f8085-162">The Type of the CodeSigning Cert as Symantec Cert.</span></span>|



## <a name="response"></a><span data-ttu-id="f8085-163">响应</span><span class="sxs-lookup"><span data-stu-id="f8085-163">Response</span></span>
<span data-ttu-id="f8085-164">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f8085-164">If successful, this method returns a `200 OK` response code and an updated [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8085-165">示例</span><span class="sxs-lookup"><span data-stu-id="f8085-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="f8085-166">请求</span><span class="sxs-lookup"><span data-stu-id="f8085-166">Request</span></span>
<span data-ttu-id="f8085-167">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f8085-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f8085-168">响应</span><span class="sxs-lookup"><span data-stu-id="f8085-168">Response</span></span>
<span data-ttu-id="f8085-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f8085-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




