---
title: symantecCodeSigningCertificate 资源类型
description: 尚未记录
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5f22f86f6facfbe1b21bb0f857b8401393ed1a77
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425993"
---
# <a name="symanteccodesigningcertificate-resource-type"></a><span data-ttu-id="28c98-103">symantecCodeSigningCertificate 资源类型</span><span class="sxs-lookup"><span data-stu-id="28c98-103">symantecCodeSigningCertificate resource type</span></span>

> <span data-ttu-id="28c98-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="28c98-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="28c98-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="28c98-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="28c98-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="28c98-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28c98-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="28c98-107">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="28c98-108">方法</span><span class="sxs-lookup"><span data-stu-id="28c98-108">Methods</span></span>
|<span data-ttu-id="28c98-109">方法</span><span class="sxs-lookup"><span data-stu-id="28c98-109">Method</span></span>|<span data-ttu-id="28c98-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="28c98-110">Return Type</span></span>|<span data-ttu-id="28c98-111">说明</span><span class="sxs-lookup"><span data-stu-id="28c98-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="28c98-112">获取 symantecCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="28c98-112">Get symantecCodeSigningCertificate</span></span>](../api/intune-apps-symanteccodesigningcertificate-get.md)|[<span data-ttu-id="28c98-113">symantecCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="28c98-113">symantecCodeSigningCertificate</span></span>](../resources/intune-apps-symanteccodesigningcertificate.md)|<span data-ttu-id="28c98-114">读取属性和[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="28c98-114">Read properties and relationships of the [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>|
|[<span data-ttu-id="28c98-115">更新 symantecCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="28c98-115">Update symantecCodeSigningCertificate</span></span>](../api/intune-apps-symanteccodesigningcertificate-update.md)|[<span data-ttu-id="28c98-116">symantecCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="28c98-116">symantecCodeSigningCertificate</span></span>](../resources/intune-apps-symanteccodesigningcertificate.md)|<span data-ttu-id="28c98-117">更新[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="28c98-117">Update the properties of a [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="28c98-118">属性</span><span class="sxs-lookup"><span data-stu-id="28c98-118">Properties</span></span>
|<span data-ttu-id="28c98-119">属性</span><span class="sxs-lookup"><span data-stu-id="28c98-119">Property</span></span>|<span data-ttu-id="28c98-120">类型</span><span class="sxs-lookup"><span data-stu-id="28c98-120">Type</span></span>|<span data-ttu-id="28c98-121">说明</span><span class="sxs-lookup"><span data-stu-id="28c98-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28c98-122">id</span><span class="sxs-lookup"><span data-stu-id="28c98-122">id</span></span>|<span data-ttu-id="28c98-123">String</span><span class="sxs-lookup"><span data-stu-id="28c98-123">String</span></span>|<span data-ttu-id="28c98-124">实体的键。</span><span class="sxs-lookup"><span data-stu-id="28c98-124">The key of the entity.</span></span>|
|<span data-ttu-id="28c98-125">content</span><span class="sxs-lookup"><span data-stu-id="28c98-125">content</span></span>|<span data-ttu-id="28c98-126">Binary</span><span class="sxs-lookup"><span data-stu-id="28c98-126">Binary</span></span>|<span data-ttu-id="28c98-127">中的原始数据格式的 Windows Symantec 代码签名证书。</span><span class="sxs-lookup"><span data-stu-id="28c98-127">The Windows Symantec Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="28c98-128">status</span><span class="sxs-lookup"><span data-stu-id="28c98-128">status</span></span>|[<span data-ttu-id="28c98-129">certificateStatus</span><span class="sxs-lookup"><span data-stu-id="28c98-129">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="28c98-130">设置或未设置证书的状态。</span><span class="sxs-lookup"><span data-stu-id="28c98-130">The Cert Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="28c98-131">可取值为：`notProvisioned`、`provisioned`。</span><span class="sxs-lookup"><span data-stu-id="28c98-131">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="28c98-132">password</span><span class="sxs-lookup"><span data-stu-id="28c98-132">password</span></span>|<span data-ttu-id="28c98-133">String</span><span class="sxs-lookup"><span data-stu-id="28c98-133">String</span></span>|<span data-ttu-id="28c98-134">.Pfx 文件所需的密码。</span><span class="sxs-lookup"><span data-stu-id="28c98-134">The Password required for .pfx file.</span></span>|
|<span data-ttu-id="28c98-135">SubjectName</span><span class="sxs-lookup"><span data-stu-id="28c98-135">subjectName</span></span>|<span data-ttu-id="28c98-136">String</span><span class="sxs-lookup"><span data-stu-id="28c98-136">String</span></span>|<span data-ttu-id="28c98-137">证书使用者名称。</span><span class="sxs-lookup"><span data-stu-id="28c98-137">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="28c98-138">subject</span><span class="sxs-lookup"><span data-stu-id="28c98-138">subject</span></span>|<span data-ttu-id="28c98-139">String</span><span class="sxs-lookup"><span data-stu-id="28c98-139">String</span></span>|<span data-ttu-id="28c98-140">证书使用者值。</span><span class="sxs-lookup"><span data-stu-id="28c98-140">The Subject value for the cert.</span></span>|
|<span data-ttu-id="28c98-141">issuerName</span><span class="sxs-lookup"><span data-stu-id="28c98-141">issuerName</span></span>|<span data-ttu-id="28c98-142">String</span><span class="sxs-lookup"><span data-stu-id="28c98-142">String</span></span>|<span data-ttu-id="28c98-143">证书颁发者名称。</span><span class="sxs-lookup"><span data-stu-id="28c98-143">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="28c98-144">颁发者</span><span class="sxs-lookup"><span data-stu-id="28c98-144">issuer</span></span>|<span data-ttu-id="28c98-145">String</span><span class="sxs-lookup"><span data-stu-id="28c98-145">String</span></span>|<span data-ttu-id="28c98-146">证书颁发者值。</span><span class="sxs-lookup"><span data-stu-id="28c98-146">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="28c98-147">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="28c98-147">expirationDateTime</span></span>|<span data-ttu-id="28c98-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28c98-148">DateTimeOffset</span></span>|<span data-ttu-id="28c98-149">证书到期日期。</span><span class="sxs-lookup"><span data-stu-id="28c98-149">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="28c98-150">uploadDateTime</span><span class="sxs-lookup"><span data-stu-id="28c98-150">uploadDateTime</span></span>|<span data-ttu-id="28c98-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28c98-151">DateTimeOffset</span></span>|<span data-ttu-id="28c98-152">作为 Symantec Cert 代码签名证书的类型。</span><span class="sxs-lookup"><span data-stu-id="28c98-152">The Type of the CodeSigning Cert as Symantec Cert.</span></span>|

## <a name="relationships"></a><span data-ttu-id="28c98-153">关系</span><span class="sxs-lookup"><span data-stu-id="28c98-153">Relationships</span></span>
<span data-ttu-id="28c98-154">无</span><span class="sxs-lookup"><span data-stu-id="28c98-154">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="28c98-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="28c98-155">JSON Representation</span></span>
<span data-ttu-id="28c98-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="28c98-156">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.symantecCodeSigningCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.symantecCodeSigningCertificate",
  "id": "String (identifier)",
  "content": "binary",
  "status": "String",
  "password": "String",
  "subjectName": "String",
  "subject": "String",
  "issuerName": "String",
  "issuer": "String",
  "expirationDateTime": "String (timestamp)",
  "uploadDateTime": "String (timestamp)"
}
```




