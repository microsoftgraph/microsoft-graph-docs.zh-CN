---
title: symantecCodeSigningCertificate 资源类型
description: 尚未记录
author: tfitzmac
ms.openlocfilehash: 979502f51674b32f10627762d08d8216a466dff9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27357237"
---
# <a name="symanteccodesigningcertificate-resource-type"></a><span data-ttu-id="dfff2-103">symantecCodeSigningCertificate 资源类型</span><span class="sxs-lookup"><span data-stu-id="dfff2-103">symantecCodeSigningCertificate resource type</span></span>

> <span data-ttu-id="dfff2-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="dfff2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dfff2-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="dfff2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dfff2-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="dfff2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dfff2-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="dfff2-107">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="dfff2-108">方法</span><span class="sxs-lookup"><span data-stu-id="dfff2-108">Methods</span></span>
|<span data-ttu-id="dfff2-109">方法</span><span class="sxs-lookup"><span data-stu-id="dfff2-109">Method</span></span>|<span data-ttu-id="dfff2-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="dfff2-110">Return Type</span></span>|<span data-ttu-id="dfff2-111">说明</span><span class="sxs-lookup"><span data-stu-id="dfff2-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="dfff2-112">获取 symantecCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="dfff2-112">Get symantecCodeSigningCertificate</span></span>](../api/intune-apps-symanteccodesigningcertificate-get.md)|[<span data-ttu-id="dfff2-113">symantecCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="dfff2-113">symantecCodeSigningCertificate</span></span>](../resources/intune-apps-symanteccodesigningcertificate.md)|<span data-ttu-id="dfff2-114">读取属性和[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="dfff2-114">Read properties and relationships of the [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>|
|[<span data-ttu-id="dfff2-115">更新 symantecCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="dfff2-115">Update symantecCodeSigningCertificate</span></span>](../api/intune-apps-symanteccodesigningcertificate-update.md)|[<span data-ttu-id="dfff2-116">symantecCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="dfff2-116">symantecCodeSigningCertificate</span></span>](../resources/intune-apps-symanteccodesigningcertificate.md)|<span data-ttu-id="dfff2-117">更新[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="dfff2-117">Update the properties of a [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="dfff2-118">属性</span><span class="sxs-lookup"><span data-stu-id="dfff2-118">Properties</span></span>
|<span data-ttu-id="dfff2-119">属性</span><span class="sxs-lookup"><span data-stu-id="dfff2-119">Property</span></span>|<span data-ttu-id="dfff2-120">类型</span><span class="sxs-lookup"><span data-stu-id="dfff2-120">Type</span></span>|<span data-ttu-id="dfff2-121">说明</span><span class="sxs-lookup"><span data-stu-id="dfff2-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dfff2-122">id</span><span class="sxs-lookup"><span data-stu-id="dfff2-122">id</span></span>|<span data-ttu-id="dfff2-123">String</span><span class="sxs-lookup"><span data-stu-id="dfff2-123">String</span></span>|<span data-ttu-id="dfff2-124">实体的键。</span><span class="sxs-lookup"><span data-stu-id="dfff2-124">The key of the entity.</span></span>|
|<span data-ttu-id="dfff2-125">content</span><span class="sxs-lookup"><span data-stu-id="dfff2-125">content</span></span>|<span data-ttu-id="dfff2-126">Binary</span><span class="sxs-lookup"><span data-stu-id="dfff2-126">Binary</span></span>|<span data-ttu-id="dfff2-127">中的原始数据格式的 Windows Symantec 代码签名证书。</span><span class="sxs-lookup"><span data-stu-id="dfff2-127">The Windows Symantec Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="dfff2-128">status</span><span class="sxs-lookup"><span data-stu-id="dfff2-128">status</span></span>|[<span data-ttu-id="dfff2-129">certificateStatus</span><span class="sxs-lookup"><span data-stu-id="dfff2-129">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="dfff2-130">设置或未设置证书的状态。</span><span class="sxs-lookup"><span data-stu-id="dfff2-130">The Cert Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="dfff2-131">可取值为：`notProvisioned`、`provisioned`。</span><span class="sxs-lookup"><span data-stu-id="dfff2-131">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="dfff2-132">password</span><span class="sxs-lookup"><span data-stu-id="dfff2-132">password</span></span>|<span data-ttu-id="dfff2-133">字符串</span><span class="sxs-lookup"><span data-stu-id="dfff2-133">String</span></span>|<span data-ttu-id="dfff2-134">.Pfx 文件所需的密码。</span><span class="sxs-lookup"><span data-stu-id="dfff2-134">The Password required for .pfx file.</span></span>|
|<span data-ttu-id="dfff2-135">SubjectName</span><span class="sxs-lookup"><span data-stu-id="dfff2-135">subjectName</span></span>|<span data-ttu-id="dfff2-136">String</span><span class="sxs-lookup"><span data-stu-id="dfff2-136">String</span></span>|<span data-ttu-id="dfff2-137">证书使用者名称。</span><span class="sxs-lookup"><span data-stu-id="dfff2-137">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="dfff2-138">subject</span><span class="sxs-lookup"><span data-stu-id="dfff2-138">subject</span></span>|<span data-ttu-id="dfff2-139">字符串</span><span class="sxs-lookup"><span data-stu-id="dfff2-139">String</span></span>|<span data-ttu-id="dfff2-140">证书使用者值。</span><span class="sxs-lookup"><span data-stu-id="dfff2-140">The Subject value for the cert.</span></span>|
|<span data-ttu-id="dfff2-141">issuerName</span><span class="sxs-lookup"><span data-stu-id="dfff2-141">issuerName</span></span>|<span data-ttu-id="dfff2-142">字符串</span><span class="sxs-lookup"><span data-stu-id="dfff2-142">String</span></span>|<span data-ttu-id="dfff2-143">证书颁发者名称。</span><span class="sxs-lookup"><span data-stu-id="dfff2-143">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="dfff2-144">颁发者</span><span class="sxs-lookup"><span data-stu-id="dfff2-144">issuer</span></span>|<span data-ttu-id="dfff2-145">字符串</span><span class="sxs-lookup"><span data-stu-id="dfff2-145">String</span></span>|<span data-ttu-id="dfff2-146">证书颁发者值。</span><span class="sxs-lookup"><span data-stu-id="dfff2-146">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="dfff2-147">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="dfff2-147">expirationDateTime</span></span>|<span data-ttu-id="dfff2-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dfff2-148">DateTimeOffset</span></span>|<span data-ttu-id="dfff2-149">证书到期日期。</span><span class="sxs-lookup"><span data-stu-id="dfff2-149">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="dfff2-150">uploadDateTime</span><span class="sxs-lookup"><span data-stu-id="dfff2-150">uploadDateTime</span></span>|<span data-ttu-id="dfff2-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dfff2-151">DateTimeOffset</span></span>|<span data-ttu-id="dfff2-152">作为 Symantec Cert 代码签名证书的类型。</span><span class="sxs-lookup"><span data-stu-id="dfff2-152">The Type of the CodeSigning Cert as Symantec Cert.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dfff2-153">Relationships</span><span class="sxs-lookup"><span data-stu-id="dfff2-153">Relationships</span></span>
<span data-ttu-id="dfff2-154">无</span><span class="sxs-lookup"><span data-stu-id="dfff2-154">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="dfff2-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dfff2-155">JSON Representation</span></span>
<span data-ttu-id="dfff2-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dfff2-156">Here is a JSON representation of the resource.</span></span>
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





