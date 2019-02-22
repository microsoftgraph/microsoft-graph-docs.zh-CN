---
title: symantecCodeSigningCertificate 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 550ba33f81db9fb38f6d19f3b756a67d7c3b9aa1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30158714"
---
# <a name="symanteccodesigningcertificate-resource-type"></a><span data-ttu-id="c07b7-103">symantecCodeSigningCertificate 资源类型</span><span class="sxs-lookup"><span data-stu-id="c07b7-103">symantecCodeSigningCertificate resource type</span></span>

> <span data-ttu-id="c07b7-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c07b7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c07b7-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c07b7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c07b7-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c07b7-106">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="c07b7-107">方法</span><span class="sxs-lookup"><span data-stu-id="c07b7-107">Methods</span></span>
|<span data-ttu-id="c07b7-108">方法</span><span class="sxs-lookup"><span data-stu-id="c07b7-108">Method</span></span>|<span data-ttu-id="c07b7-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="c07b7-109">Return Type</span></span>|<span data-ttu-id="c07b7-110">说明</span><span class="sxs-lookup"><span data-stu-id="c07b7-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c07b7-111">获取 symantecCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="c07b7-111">Get symantecCodeSigningCertificate</span></span>](../api/intune-apps-symanteccodesigningcertificate-get.md)|[<span data-ttu-id="c07b7-112">symantecCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="c07b7-112">symantecCodeSigningCertificate</span></span>](../resources/intune-apps-symanteccodesigningcertificate.md)|<span data-ttu-id="c07b7-113">读取[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c07b7-113">Read properties and relationships of the [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>|
|[<span data-ttu-id="c07b7-114">更新 symantecCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="c07b7-114">Update symantecCodeSigningCertificate</span></span>](../api/intune-apps-symanteccodesigningcertificate-update.md)|[<span data-ttu-id="c07b7-115">symantecCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="c07b7-115">symantecCodeSigningCertificate</span></span>](../resources/intune-apps-symanteccodesigningcertificate.md)|<span data-ttu-id="c07b7-116">更新[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c07b7-116">Update the properties of a [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c07b7-117">属性</span><span class="sxs-lookup"><span data-stu-id="c07b7-117">Properties</span></span>
|<span data-ttu-id="c07b7-118">属性</span><span class="sxs-lookup"><span data-stu-id="c07b7-118">Property</span></span>|<span data-ttu-id="c07b7-119">类型</span><span class="sxs-lookup"><span data-stu-id="c07b7-119">Type</span></span>|<span data-ttu-id="c07b7-120">说明</span><span class="sxs-lookup"><span data-stu-id="c07b7-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c07b7-121">id</span><span class="sxs-lookup"><span data-stu-id="c07b7-121">id</span></span>|<span data-ttu-id="c07b7-122">String</span><span class="sxs-lookup"><span data-stu-id="c07b7-122">String</span></span>|<span data-ttu-id="c07b7-123">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c07b7-123">The key of the entity.</span></span>|
|<span data-ttu-id="c07b7-124">content</span><span class="sxs-lookup"><span data-stu-id="c07b7-124">content</span></span>|<span data-ttu-id="c07b7-125">Binary</span><span class="sxs-lookup"><span data-stu-id="c07b7-125">Binary</span></span>|<span data-ttu-id="c07b7-126">原始数据格式的 Windows Symantec 代码签名证书。</span><span class="sxs-lookup"><span data-stu-id="c07b7-126">The Windows Symantec Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="c07b7-127">status</span><span class="sxs-lookup"><span data-stu-id="c07b7-127">status</span></span>|[<span data-ttu-id="c07b7-128">certificateStatus</span><span class="sxs-lookup"><span data-stu-id="c07b7-128">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="c07b7-129">证书状态已设置或未设置。</span><span class="sxs-lookup"><span data-stu-id="c07b7-129">The Cert Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="c07b7-130">可取值为：`notProvisioned`、`provisioned`。</span><span class="sxs-lookup"><span data-stu-id="c07b7-130">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="c07b7-131">password</span><span class="sxs-lookup"><span data-stu-id="c07b7-131">password</span></span>|<span data-ttu-id="c07b7-132">字符串</span><span class="sxs-lookup"><span data-stu-id="c07b7-132">String</span></span>|<span data-ttu-id="c07b7-133">.pfx 文件所需的密码。</span><span class="sxs-lookup"><span data-stu-id="c07b7-133">The Password required for .pfx file.</span></span>|
|<span data-ttu-id="c07b7-134">SubjectName</span><span class="sxs-lookup"><span data-stu-id="c07b7-134">subjectName</span></span>|<span data-ttu-id="c07b7-135">String</span><span class="sxs-lookup"><span data-stu-id="c07b7-135">String</span></span>|<span data-ttu-id="c07b7-136">证书的主题名称。</span><span class="sxs-lookup"><span data-stu-id="c07b7-136">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="c07b7-137">subject</span><span class="sxs-lookup"><span data-stu-id="c07b7-137">subject</span></span>|<span data-ttu-id="c07b7-138">字符串</span><span class="sxs-lookup"><span data-stu-id="c07b7-138">String</span></span>|<span data-ttu-id="c07b7-139">证书的主题值。</span><span class="sxs-lookup"><span data-stu-id="c07b7-139">The Subject value for the cert.</span></span>|
|<span data-ttu-id="c07b7-140">issuerName</span><span class="sxs-lookup"><span data-stu-id="c07b7-140">issuerName</span></span>|<span data-ttu-id="c07b7-141">字符串</span><span class="sxs-lookup"><span data-stu-id="c07b7-141">String</span></span>|<span data-ttu-id="c07b7-142">证书的颁发者名称。</span><span class="sxs-lookup"><span data-stu-id="c07b7-142">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="c07b7-143">常用</span><span class="sxs-lookup"><span data-stu-id="c07b7-143">issuer</span></span>|<span data-ttu-id="c07b7-144">字符串</span><span class="sxs-lookup"><span data-stu-id="c07b7-144">String</span></span>|<span data-ttu-id="c07b7-145">证书的 Issuer 值。</span><span class="sxs-lookup"><span data-stu-id="c07b7-145">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="c07b7-146">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="c07b7-146">expirationDateTime</span></span>|<span data-ttu-id="c07b7-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c07b7-147">DateTimeOffset</span></span>|<span data-ttu-id="c07b7-148">证书到期日期。</span><span class="sxs-lookup"><span data-stu-id="c07b7-148">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="c07b7-149">uploadDateTime</span><span class="sxs-lookup"><span data-stu-id="c07b7-149">uploadDateTime</span></span>|<span data-ttu-id="c07b7-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c07b7-150">DateTimeOffset</span></span>|<span data-ttu-id="c07b7-151">作为 Symantec 证书的 CodeSigning 证书的类型。</span><span class="sxs-lookup"><span data-stu-id="c07b7-151">The Type of the CodeSigning Cert as Symantec Cert.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c07b7-152">关系</span><span class="sxs-lookup"><span data-stu-id="c07b7-152">Relationships</span></span>
<span data-ttu-id="c07b7-153">无</span><span class="sxs-lookup"><span data-stu-id="c07b7-153">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c07b7-154">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c07b7-154">JSON Representation</span></span>
<span data-ttu-id="c07b7-155">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c07b7-155">Here is a JSON representation of the resource.</span></span>
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




