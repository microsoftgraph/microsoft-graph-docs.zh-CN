---
title: symantecCodeSigningCertificate 资源类型
description: 尚未记录
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2fe681f00f3a14f7199416366cd5a28e6a0ff8d6
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797708"
---
# <a name="symanteccodesigningcertificate-resource-type"></a><span data-ttu-id="aa0c4-103">symantecCodeSigningCertificate 资源类型</span><span class="sxs-lookup"><span data-stu-id="aa0c4-103">symantecCodeSigningCertificate resource type</span></span>

> <span data-ttu-id="aa0c4-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="aa0c4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aa0c4-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="aa0c4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa0c4-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="aa0c4-106">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="aa0c4-107">方法</span><span class="sxs-lookup"><span data-stu-id="aa0c4-107">Methods</span></span>
|<span data-ttu-id="aa0c4-108">方法</span><span class="sxs-lookup"><span data-stu-id="aa0c4-108">Method</span></span>|<span data-ttu-id="aa0c4-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="aa0c4-109">Return Type</span></span>|<span data-ttu-id="aa0c4-110">说明</span><span class="sxs-lookup"><span data-stu-id="aa0c4-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="aa0c4-111">获取 symantecCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="aa0c4-111">Get symantecCodeSigningCertificate</span></span>](../api/intune-apps-symanteccodesigningcertificate-get.md)|[<span data-ttu-id="aa0c4-112">symantecCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="aa0c4-112">symantecCodeSigningCertificate</span></span>](../resources/intune-apps-symanteccodesigningcertificate.md)|<span data-ttu-id="aa0c4-113">读取[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="aa0c4-113">Read properties and relationships of the [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>|
|[<span data-ttu-id="aa0c4-114">更新 symantecCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="aa0c4-114">Update symantecCodeSigningCertificate</span></span>](../api/intune-apps-symanteccodesigningcertificate-update.md)|[<span data-ttu-id="aa0c4-115">symantecCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="aa0c4-115">symantecCodeSigningCertificate</span></span>](../resources/intune-apps-symanteccodesigningcertificate.md)|<span data-ttu-id="aa0c4-116">更新[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="aa0c4-116">Update the properties of a [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="aa0c4-117">属性</span><span class="sxs-lookup"><span data-stu-id="aa0c4-117">Properties</span></span>
|<span data-ttu-id="aa0c4-118">属性</span><span class="sxs-lookup"><span data-stu-id="aa0c4-118">Property</span></span>|<span data-ttu-id="aa0c4-119">类型</span><span class="sxs-lookup"><span data-stu-id="aa0c4-119">Type</span></span>|<span data-ttu-id="aa0c4-120">说明</span><span class="sxs-lookup"><span data-stu-id="aa0c4-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa0c4-121">id</span><span class="sxs-lookup"><span data-stu-id="aa0c4-121">id</span></span>|<span data-ttu-id="aa0c4-122">字符串</span><span class="sxs-lookup"><span data-stu-id="aa0c4-122">String</span></span>|<span data-ttu-id="aa0c4-123">实体的键。</span><span class="sxs-lookup"><span data-stu-id="aa0c4-123">The key of the entity.</span></span>|
|<span data-ttu-id="aa0c4-124">content</span><span class="sxs-lookup"><span data-stu-id="aa0c4-124">content</span></span>|<span data-ttu-id="aa0c4-125">Binary</span><span class="sxs-lookup"><span data-stu-id="aa0c4-125">Binary</span></span>|<span data-ttu-id="aa0c4-126">原始数据格式的 Windows Symantec 代码签名证书。</span><span class="sxs-lookup"><span data-stu-id="aa0c4-126">The Windows Symantec Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="aa0c4-127">状态</span><span class="sxs-lookup"><span data-stu-id="aa0c4-127">status</span></span>|[<span data-ttu-id="aa0c4-128">certificateStatus</span><span class="sxs-lookup"><span data-stu-id="aa0c4-128">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="aa0c4-129">证书状态已设置或未设置。</span><span class="sxs-lookup"><span data-stu-id="aa0c4-129">The Cert Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="aa0c4-130">可取值为：`notProvisioned`、`provisioned`。</span><span class="sxs-lookup"><span data-stu-id="aa0c4-130">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="aa0c4-131">密码</span><span class="sxs-lookup"><span data-stu-id="aa0c4-131">password</span></span>|<span data-ttu-id="aa0c4-132">字符串</span><span class="sxs-lookup"><span data-stu-id="aa0c4-132">String</span></span>|<span data-ttu-id="aa0c4-133">.Pfx 文件所需的密码。</span><span class="sxs-lookup"><span data-stu-id="aa0c4-133">The Password required for .pfx file.</span></span>|
|<span data-ttu-id="aa0c4-134">SubjectName</span><span class="sxs-lookup"><span data-stu-id="aa0c4-134">subjectName</span></span>|<span data-ttu-id="aa0c4-135">String</span><span class="sxs-lookup"><span data-stu-id="aa0c4-135">String</span></span>|<span data-ttu-id="aa0c4-136">证书的主题名称。</span><span class="sxs-lookup"><span data-stu-id="aa0c4-136">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="aa0c4-137">subject</span><span class="sxs-lookup"><span data-stu-id="aa0c4-137">subject</span></span>|<span data-ttu-id="aa0c4-138">String</span><span class="sxs-lookup"><span data-stu-id="aa0c4-138">String</span></span>|<span data-ttu-id="aa0c4-139">证书的主题值。</span><span class="sxs-lookup"><span data-stu-id="aa0c4-139">The Subject value for the cert.</span></span>|
|<span data-ttu-id="aa0c4-140">issuerName</span><span class="sxs-lookup"><span data-stu-id="aa0c4-140">issuerName</span></span>|<span data-ttu-id="aa0c4-141">String</span><span class="sxs-lookup"><span data-stu-id="aa0c4-141">String</span></span>|<span data-ttu-id="aa0c4-142">证书的颁发者名称。</span><span class="sxs-lookup"><span data-stu-id="aa0c4-142">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="aa0c4-143">常用</span><span class="sxs-lookup"><span data-stu-id="aa0c4-143">issuer</span></span>|<span data-ttu-id="aa0c4-144">String</span><span class="sxs-lookup"><span data-stu-id="aa0c4-144">String</span></span>|<span data-ttu-id="aa0c4-145">证书的 Issuer 值。</span><span class="sxs-lookup"><span data-stu-id="aa0c4-145">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="aa0c4-146">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="aa0c4-146">expirationDateTime</span></span>|<span data-ttu-id="aa0c4-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa0c4-147">DateTimeOffset</span></span>|<span data-ttu-id="aa0c4-148">证书到期日期。</span><span class="sxs-lookup"><span data-stu-id="aa0c4-148">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="aa0c4-149">uploadDateTime</span><span class="sxs-lookup"><span data-stu-id="aa0c4-149">uploadDateTime</span></span>|<span data-ttu-id="aa0c4-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa0c4-150">DateTimeOffset</span></span>|<span data-ttu-id="aa0c4-151">作为 Symantec 证书的 CodeSigning 证书的类型。</span><span class="sxs-lookup"><span data-stu-id="aa0c4-151">The Type of the CodeSigning Cert as Symantec Cert.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aa0c4-152">关系</span><span class="sxs-lookup"><span data-stu-id="aa0c4-152">Relationships</span></span>
<span data-ttu-id="aa0c4-153">无</span><span class="sxs-lookup"><span data-stu-id="aa0c4-153">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="aa0c4-154">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aa0c4-154">JSON Representation</span></span>
<span data-ttu-id="aa0c4-155">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aa0c4-155">Here is a JSON representation of the resource.</span></span>
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



