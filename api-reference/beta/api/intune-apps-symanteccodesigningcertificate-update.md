---
title: 更新 symantecCodeSigningCertificate
description: 更新 symantecCodeSigningCertificate 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f0a938fcb207ee242115eb89cd45da0b1c092a6f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968783"
---
# <a name="update-symanteccodesigningcertificate"></a><span data-ttu-id="ea4aa-103">更新 symantecCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="ea4aa-103">Update symantecCodeSigningCertificate</span></span>

> <span data-ttu-id="ea4aa-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ea4aa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ea4aa-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ea4aa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ea4aa-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ea4aa-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ea4aa-107">更新[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ea4aa-107">Update the properties of a [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ea4aa-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ea4aa-108">Prerequisites</span></span>
<span data-ttu-id="ea4aa-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="ea4aa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea4aa-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ea4aa-111">Permission type</span></span>|<span data-ttu-id="ea4aa-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ea4aa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea4aa-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ea4aa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ea4aa-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea4aa-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ea4aa-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ea4aa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea4aa-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ea4aa-116">Not supported.</span></span>|
|<span data-ttu-id="ea4aa-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ea4aa-117">Application</span></span>|<span data-ttu-id="ea4aa-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="ea4aa-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea4aa-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ea4aa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/symantecCodeSigningCertificate
```

## <a name="request-headers"></a><span data-ttu-id="ea4aa-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ea4aa-120">Request headers</span></span>
|<span data-ttu-id="ea4aa-121">标头</span><span class="sxs-lookup"><span data-stu-id="ea4aa-121">Header</span></span>|<span data-ttu-id="ea4aa-122">值</span><span class="sxs-lookup"><span data-stu-id="ea4aa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea4aa-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea4aa-123">Authorization</span></span>|<span data-ttu-id="ea4aa-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ea4aa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea4aa-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ea4aa-125">Accept</span></span>|<span data-ttu-id="ea4aa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ea4aa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea4aa-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ea4aa-127">Request body</span></span>
<span data-ttu-id="ea4aa-128">在请求正文中，提供[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ea4aa-128">In the request body, supply a JSON representation for the [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>

<span data-ttu-id="ea4aa-129">下表显示时创建[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ea4aa-129">The following table shows the properties that are required when you create the [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md).</span></span>

|<span data-ttu-id="ea4aa-130">属性</span><span class="sxs-lookup"><span data-stu-id="ea4aa-130">Property</span></span>|<span data-ttu-id="ea4aa-131">类型</span><span class="sxs-lookup"><span data-stu-id="ea4aa-131">Type</span></span>|<span data-ttu-id="ea4aa-132">说明</span><span class="sxs-lookup"><span data-stu-id="ea4aa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea4aa-133">id</span><span class="sxs-lookup"><span data-stu-id="ea4aa-133">id</span></span>|<span data-ttu-id="ea4aa-134">String</span><span class="sxs-lookup"><span data-stu-id="ea4aa-134">String</span></span>|<span data-ttu-id="ea4aa-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ea4aa-135">The key of the entity.</span></span>|
|<span data-ttu-id="ea4aa-136">content</span><span class="sxs-lookup"><span data-stu-id="ea4aa-136">content</span></span>|<span data-ttu-id="ea4aa-137">Binary</span><span class="sxs-lookup"><span data-stu-id="ea4aa-137">Binary</span></span>|<span data-ttu-id="ea4aa-138">中的原始数据格式的 Windows Symantec 代码签名证书。</span><span class="sxs-lookup"><span data-stu-id="ea4aa-138">The Windows Symantec Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="ea4aa-139">status</span><span class="sxs-lookup"><span data-stu-id="ea4aa-139">status</span></span>|[<span data-ttu-id="ea4aa-140">certificateStatus</span><span class="sxs-lookup"><span data-stu-id="ea4aa-140">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="ea4aa-141">设置或未设置证书的状态。</span><span class="sxs-lookup"><span data-stu-id="ea4aa-141">The Cert Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="ea4aa-142">可取值为：`notProvisioned`、`provisioned`。</span><span class="sxs-lookup"><span data-stu-id="ea4aa-142">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="ea4aa-143">password</span><span class="sxs-lookup"><span data-stu-id="ea4aa-143">password</span></span>|<span data-ttu-id="ea4aa-144">字符串</span><span class="sxs-lookup"><span data-stu-id="ea4aa-144">String</span></span>|<span data-ttu-id="ea4aa-145">.Pfx 文件所需的密码。</span><span class="sxs-lookup"><span data-stu-id="ea4aa-145">The Password required for .pfx file.</span></span>|
|<span data-ttu-id="ea4aa-146">SubjectName</span><span class="sxs-lookup"><span data-stu-id="ea4aa-146">subjectName</span></span>|<span data-ttu-id="ea4aa-147">String</span><span class="sxs-lookup"><span data-stu-id="ea4aa-147">String</span></span>|<span data-ttu-id="ea4aa-148">证书使用者名称。</span><span class="sxs-lookup"><span data-stu-id="ea4aa-148">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="ea4aa-149">subject</span><span class="sxs-lookup"><span data-stu-id="ea4aa-149">subject</span></span>|<span data-ttu-id="ea4aa-150">字符串</span><span class="sxs-lookup"><span data-stu-id="ea4aa-150">String</span></span>|<span data-ttu-id="ea4aa-151">证书使用者值。</span><span class="sxs-lookup"><span data-stu-id="ea4aa-151">The Subject value for the cert.</span></span>|
|<span data-ttu-id="ea4aa-152">issuerName</span><span class="sxs-lookup"><span data-stu-id="ea4aa-152">issuerName</span></span>|<span data-ttu-id="ea4aa-153">字符串</span><span class="sxs-lookup"><span data-stu-id="ea4aa-153">String</span></span>|<span data-ttu-id="ea4aa-154">证书颁发者名称。</span><span class="sxs-lookup"><span data-stu-id="ea4aa-154">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="ea4aa-155">颁发者</span><span class="sxs-lookup"><span data-stu-id="ea4aa-155">issuer</span></span>|<span data-ttu-id="ea4aa-156">字符串</span><span class="sxs-lookup"><span data-stu-id="ea4aa-156">String</span></span>|<span data-ttu-id="ea4aa-157">证书颁发者值。</span><span class="sxs-lookup"><span data-stu-id="ea4aa-157">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="ea4aa-158">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ea4aa-158">expirationDateTime</span></span>|<span data-ttu-id="ea4aa-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea4aa-159">DateTimeOffset</span></span>|<span data-ttu-id="ea4aa-160">证书到期日期。</span><span class="sxs-lookup"><span data-stu-id="ea4aa-160">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="ea4aa-161">uploadDateTime</span><span class="sxs-lookup"><span data-stu-id="ea4aa-161">uploadDateTime</span></span>|<span data-ttu-id="ea4aa-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea4aa-162">DateTimeOffset</span></span>|<span data-ttu-id="ea4aa-163">作为 Symantec Cert 代码签名证书的类型。</span><span class="sxs-lookup"><span data-stu-id="ea4aa-163">The Type of the CodeSigning Cert as Symantec Cert.</span></span>|



## <a name="response"></a><span data-ttu-id="ea4aa-164">响应</span><span class="sxs-lookup"><span data-stu-id="ea4aa-164">Response</span></span>
<span data-ttu-id="ea4aa-165">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ea4aa-165">If successful, this method returns a `200 OK` response code and an updated [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea4aa-166">示例</span><span class="sxs-lookup"><span data-stu-id="ea4aa-166">Example</span></span>
### <a name="request"></a><span data-ttu-id="ea4aa-167">请求</span><span class="sxs-lookup"><span data-stu-id="ea4aa-167">Request</span></span>
<span data-ttu-id="ea4aa-168">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ea4aa-168">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/symantecCodeSigningCertificate
Content-type: application/json
Content-length: 352

{
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

### <a name="response"></a><span data-ttu-id="ea4aa-169">响应</span><span class="sxs-lookup"><span data-stu-id="ea4aa-169">Response</span></span>
<span data-ttu-id="ea4aa-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ea4aa-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





