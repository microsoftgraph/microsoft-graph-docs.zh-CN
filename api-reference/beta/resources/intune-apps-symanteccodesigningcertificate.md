---
title: symantecCodeSigningCertificate 资源类型
description: 尚未记录
ms.openlocfilehash: f867f5bf6b0cad43f32dcc5ad9320421eee6d5c5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044717"
---
# <a name="symanteccodesigningcertificate-resource-type"></a><span data-ttu-id="73dfd-103">symantecCodeSigningCertificate 资源类型</span><span class="sxs-lookup"><span data-stu-id="73dfd-103">symantecCodeSigningCertificate resource type</span></span>

> <span data-ttu-id="73dfd-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="73dfd-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="73dfd-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="73dfd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="73dfd-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="73dfd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="73dfd-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="73dfd-107">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="73dfd-108">方法</span><span class="sxs-lookup"><span data-stu-id="73dfd-108">Methods</span></span>
|<span data-ttu-id="73dfd-109">方法</span><span class="sxs-lookup"><span data-stu-id="73dfd-109">Method</span></span>|<span data-ttu-id="73dfd-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="73dfd-110">Return Type</span></span>|<span data-ttu-id="73dfd-111">说明</span><span class="sxs-lookup"><span data-stu-id="73dfd-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="73dfd-112">获取 symantecCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="73dfd-112">Get symantecCodeSigningCertificate</span></span>](../api/intune-apps-symanteccodesigningcertificate-get.md)|[<span data-ttu-id="73dfd-113">symantecCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="73dfd-113">symantecCodeSigningCertificate</span></span>](../resources/intune-apps-symanteccodesigningcertificate.md)|<span data-ttu-id="73dfd-114">读取属性和[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="73dfd-114">Read properties and relationships of the [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>|
|[<span data-ttu-id="73dfd-115">更新 symantecCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="73dfd-115">Update symantecCodeSigningCertificate</span></span>](../api/intune-apps-symanteccodesigningcertificate-update.md)|[<span data-ttu-id="73dfd-116">symantecCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="73dfd-116">symantecCodeSigningCertificate</span></span>](../resources/intune-apps-symanteccodesigningcertificate.md)|<span data-ttu-id="73dfd-117">更新[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="73dfd-117">Update the properties of a [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="73dfd-118">属性</span><span class="sxs-lookup"><span data-stu-id="73dfd-118">Properties</span></span>
|<span data-ttu-id="73dfd-119">属性</span><span class="sxs-lookup"><span data-stu-id="73dfd-119">Property</span></span>|<span data-ttu-id="73dfd-120">类型</span><span class="sxs-lookup"><span data-stu-id="73dfd-120">Type</span></span>|<span data-ttu-id="73dfd-121">说明</span><span class="sxs-lookup"><span data-stu-id="73dfd-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73dfd-122">id</span><span class="sxs-lookup"><span data-stu-id="73dfd-122">id</span></span>|<span data-ttu-id="73dfd-123">String</span><span class="sxs-lookup"><span data-stu-id="73dfd-123">String</span></span>|<span data-ttu-id="73dfd-124">实体的键。</span><span class="sxs-lookup"><span data-stu-id="73dfd-124">The key of the entity.</span></span>|
|<span data-ttu-id="73dfd-125">content</span><span class="sxs-lookup"><span data-stu-id="73dfd-125">content</span></span>|<span data-ttu-id="73dfd-126">二进制数</span><span class="sxs-lookup"><span data-stu-id="73dfd-126">Binary</span></span>|<span data-ttu-id="73dfd-127">中的原始数据格式的 Windows Symantec 代码签名证书。</span><span class="sxs-lookup"><span data-stu-id="73dfd-127">The Windows Symantec Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="73dfd-128">状态</span><span class="sxs-lookup"><span data-stu-id="73dfd-128">status</span></span>|[<span data-ttu-id="73dfd-129">certificateStatus</span><span class="sxs-lookup"><span data-stu-id="73dfd-129">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="73dfd-130">设置或未设置证书的状态。</span><span class="sxs-lookup"><span data-stu-id="73dfd-130">The Cert Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="73dfd-131">可取值为：`notProvisioned`、`provisioned`。</span><span class="sxs-lookup"><span data-stu-id="73dfd-131">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="73dfd-132">password</span><span class="sxs-lookup"><span data-stu-id="73dfd-132">password</span></span>|<span data-ttu-id="73dfd-133">字符串</span><span class="sxs-lookup"><span data-stu-id="73dfd-133">String</span></span>|<span data-ttu-id="73dfd-134">.Pfx 文件所需的密码。</span><span class="sxs-lookup"><span data-stu-id="73dfd-134">The Password required for .pfx file.</span></span>|
|<span data-ttu-id="73dfd-135">SubjectName</span><span class="sxs-lookup"><span data-stu-id="73dfd-135">subjectName</span></span>|<span data-ttu-id="73dfd-136">String</span><span class="sxs-lookup"><span data-stu-id="73dfd-136">String</span></span>|<span data-ttu-id="73dfd-137">证书使用者名称。</span><span class="sxs-lookup"><span data-stu-id="73dfd-137">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="73dfd-138">subject</span><span class="sxs-lookup"><span data-stu-id="73dfd-138">subject</span></span>|<span data-ttu-id="73dfd-139">字符串</span><span class="sxs-lookup"><span data-stu-id="73dfd-139">String</span></span>|<span data-ttu-id="73dfd-140">证书使用者值。</span><span class="sxs-lookup"><span data-stu-id="73dfd-140">The Subject value for the cert.</span></span>|
|<span data-ttu-id="73dfd-141">issuerName</span><span class="sxs-lookup"><span data-stu-id="73dfd-141">issuerName</span></span>|<span data-ttu-id="73dfd-142">字符串</span><span class="sxs-lookup"><span data-stu-id="73dfd-142">String</span></span>|<span data-ttu-id="73dfd-143">证书颁发者名称。</span><span class="sxs-lookup"><span data-stu-id="73dfd-143">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="73dfd-144">颁发者</span><span class="sxs-lookup"><span data-stu-id="73dfd-144">issuer</span></span>|<span data-ttu-id="73dfd-145">字符串</span><span class="sxs-lookup"><span data-stu-id="73dfd-145">String</span></span>|<span data-ttu-id="73dfd-146">证书颁发者值。</span><span class="sxs-lookup"><span data-stu-id="73dfd-146">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="73dfd-147">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="73dfd-147">expirationDateTime</span></span>|<span data-ttu-id="73dfd-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73dfd-148">DateTimeOffset</span></span>|<span data-ttu-id="73dfd-149">证书到期日期。</span><span class="sxs-lookup"><span data-stu-id="73dfd-149">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="73dfd-150">uploadDateTime</span><span class="sxs-lookup"><span data-stu-id="73dfd-150">uploadDateTime</span></span>|<span data-ttu-id="73dfd-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73dfd-151">DateTimeOffset</span></span>|<span data-ttu-id="73dfd-152">作为 Symantec Cert 代码签名证书的类型。</span><span class="sxs-lookup"><span data-stu-id="73dfd-152">The Type of the CodeSigning Cert as Symantec Cert.</span></span>|

## <a name="relationships"></a><span data-ttu-id="73dfd-153">Relationships</span><span class="sxs-lookup"><span data-stu-id="73dfd-153">Relationships</span></span>
<span data-ttu-id="73dfd-154">无</span><span class="sxs-lookup"><span data-stu-id="73dfd-154">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="73dfd-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="73dfd-155">JSON Representation</span></span>
<span data-ttu-id="73dfd-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="73dfd-156">Here is a JSON representation of the resource.</span></span>
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





