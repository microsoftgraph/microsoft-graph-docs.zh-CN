---
title: 更新 symantecCodeSigningCertificate
description: 更新 symantecCodeSigningCertificate 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5da263a8b4c2bbf121fb994b4d20168c45da9e03
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414023"
---
# <a name="update-symanteccodesigningcertificate"></a><span data-ttu-id="c5a8d-103">更新 symantecCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="c5a8d-103">Update symantecCodeSigningCertificate</span></span>

> <span data-ttu-id="c5a8d-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="c5a8d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c5a8d-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c5a8d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c5a8d-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c5a8d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5a8d-107">更新[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c5a8d-107">Update the properties of a [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c5a8d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c5a8d-108">Prerequisites</span></span>
<span data-ttu-id="c5a8d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="c5a8d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c5a8d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c5a8d-111">Permission type</span></span>|<span data-ttu-id="c5a8d-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c5a8d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5a8d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c5a8d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c5a8d-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5a8d-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c5a8d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c5a8d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5a8d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c5a8d-116">Not supported.</span></span>|
|<span data-ttu-id="c5a8d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c5a8d-117">Application</span></span>|<span data-ttu-id="c5a8d-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="c5a8d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5a8d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c5a8d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/symantecCodeSigningCertificate
```

## <a name="request-headers"></a><span data-ttu-id="c5a8d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c5a8d-120">Request headers</span></span>
|<span data-ttu-id="c5a8d-121">标头</span><span class="sxs-lookup"><span data-stu-id="c5a8d-121">Header</span></span>|<span data-ttu-id="c5a8d-122">值</span><span class="sxs-lookup"><span data-stu-id="c5a8d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5a8d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5a8d-123">Authorization</span></span>|<span data-ttu-id="c5a8d-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c5a8d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5a8d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c5a8d-125">Accept</span></span>|<span data-ttu-id="c5a8d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c5a8d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5a8d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c5a8d-127">Request body</span></span>
<span data-ttu-id="c5a8d-128">在请求正文中，提供[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c5a8d-128">In the request body, supply a JSON representation for the [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>

<span data-ttu-id="c5a8d-129">下表显示时创建[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c5a8d-129">The following table shows the properties that are required when you create the [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md).</span></span>

|<span data-ttu-id="c5a8d-130">属性</span><span class="sxs-lookup"><span data-stu-id="c5a8d-130">Property</span></span>|<span data-ttu-id="c5a8d-131">类型</span><span class="sxs-lookup"><span data-stu-id="c5a8d-131">Type</span></span>|<span data-ttu-id="c5a8d-132">说明</span><span class="sxs-lookup"><span data-stu-id="c5a8d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5a8d-133">id</span><span class="sxs-lookup"><span data-stu-id="c5a8d-133">id</span></span>|<span data-ttu-id="c5a8d-134">String</span><span class="sxs-lookup"><span data-stu-id="c5a8d-134">String</span></span>|<span data-ttu-id="c5a8d-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c5a8d-135">The key of the entity.</span></span>|
|<span data-ttu-id="c5a8d-136">content</span><span class="sxs-lookup"><span data-stu-id="c5a8d-136">content</span></span>|<span data-ttu-id="c5a8d-137">Binary</span><span class="sxs-lookup"><span data-stu-id="c5a8d-137">Binary</span></span>|<span data-ttu-id="c5a8d-138">中的原始数据格式的 Windows Symantec 代码签名证书。</span><span class="sxs-lookup"><span data-stu-id="c5a8d-138">The Windows Symantec Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="c5a8d-139">status</span><span class="sxs-lookup"><span data-stu-id="c5a8d-139">status</span></span>|[<span data-ttu-id="c5a8d-140">certificateStatus</span><span class="sxs-lookup"><span data-stu-id="c5a8d-140">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="c5a8d-141">设置或未设置证书的状态。</span><span class="sxs-lookup"><span data-stu-id="c5a8d-141">The Cert Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="c5a8d-142">可取值为：`notProvisioned`、`provisioned`。</span><span class="sxs-lookup"><span data-stu-id="c5a8d-142">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="c5a8d-143">password</span><span class="sxs-lookup"><span data-stu-id="c5a8d-143">password</span></span>|<span data-ttu-id="c5a8d-144">String</span><span class="sxs-lookup"><span data-stu-id="c5a8d-144">String</span></span>|<span data-ttu-id="c5a8d-145">.Pfx 文件所需的密码。</span><span class="sxs-lookup"><span data-stu-id="c5a8d-145">The Password required for .pfx file.</span></span>|
|<span data-ttu-id="c5a8d-146">SubjectName</span><span class="sxs-lookup"><span data-stu-id="c5a8d-146">subjectName</span></span>|<span data-ttu-id="c5a8d-147">String</span><span class="sxs-lookup"><span data-stu-id="c5a8d-147">String</span></span>|<span data-ttu-id="c5a8d-148">证书使用者名称。</span><span class="sxs-lookup"><span data-stu-id="c5a8d-148">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="c5a8d-149">subject</span><span class="sxs-lookup"><span data-stu-id="c5a8d-149">subject</span></span>|<span data-ttu-id="c5a8d-150">String</span><span class="sxs-lookup"><span data-stu-id="c5a8d-150">String</span></span>|<span data-ttu-id="c5a8d-151">证书使用者值。</span><span class="sxs-lookup"><span data-stu-id="c5a8d-151">The Subject value for the cert.</span></span>|
|<span data-ttu-id="c5a8d-152">issuerName</span><span class="sxs-lookup"><span data-stu-id="c5a8d-152">issuerName</span></span>|<span data-ttu-id="c5a8d-153">String</span><span class="sxs-lookup"><span data-stu-id="c5a8d-153">String</span></span>|<span data-ttu-id="c5a8d-154">证书颁发者名称。</span><span class="sxs-lookup"><span data-stu-id="c5a8d-154">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="c5a8d-155">颁发者</span><span class="sxs-lookup"><span data-stu-id="c5a8d-155">issuer</span></span>|<span data-ttu-id="c5a8d-156">String</span><span class="sxs-lookup"><span data-stu-id="c5a8d-156">String</span></span>|<span data-ttu-id="c5a8d-157">证书颁发者值。</span><span class="sxs-lookup"><span data-stu-id="c5a8d-157">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="c5a8d-158">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="c5a8d-158">expirationDateTime</span></span>|<span data-ttu-id="c5a8d-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5a8d-159">DateTimeOffset</span></span>|<span data-ttu-id="c5a8d-160">证书到期日期。</span><span class="sxs-lookup"><span data-stu-id="c5a8d-160">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="c5a8d-161">uploadDateTime</span><span class="sxs-lookup"><span data-stu-id="c5a8d-161">uploadDateTime</span></span>|<span data-ttu-id="c5a8d-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5a8d-162">DateTimeOffset</span></span>|<span data-ttu-id="c5a8d-163">作为 Symantec Cert 代码签名证书的类型。</span><span class="sxs-lookup"><span data-stu-id="c5a8d-163">The Type of the CodeSigning Cert as Symantec Cert.</span></span>|



## <a name="response"></a><span data-ttu-id="c5a8d-164">响应</span><span class="sxs-lookup"><span data-stu-id="c5a8d-164">Response</span></span>
<span data-ttu-id="c5a8d-165">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c5a8d-165">If successful, this method returns a `200 OK` response code and an updated [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5a8d-166">示例</span><span class="sxs-lookup"><span data-stu-id="c5a8d-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="c5a8d-167">请求</span><span class="sxs-lookup"><span data-stu-id="c5a8d-167">Request</span></span>
<span data-ttu-id="c5a8d-168">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c5a8d-168">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c5a8d-169">响应</span><span class="sxs-lookup"><span data-stu-id="c5a8d-169">Response</span></span>
<span data-ttu-id="c5a8d-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c5a8d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




