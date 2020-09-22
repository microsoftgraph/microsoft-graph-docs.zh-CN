---
title: symantecCodeSigningCertificate 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1761e5d9d98c1d2cae7a0d76193e874518f94dac
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078421"
---
# <a name="symanteccodesigningcertificate-resource-type"></a><span data-ttu-id="47c68-103">symantecCodeSigningCertificate 资源类型</span><span class="sxs-lookup"><span data-stu-id="47c68-103">symantecCodeSigningCertificate resource type</span></span>

<span data-ttu-id="47c68-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47c68-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="47c68-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="47c68-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47c68-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="47c68-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47c68-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="47c68-107">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="47c68-108">方法</span><span class="sxs-lookup"><span data-stu-id="47c68-108">Methods</span></span>
|<span data-ttu-id="47c68-109">方法</span><span class="sxs-lookup"><span data-stu-id="47c68-109">Method</span></span>|<span data-ttu-id="47c68-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="47c68-110">Return Type</span></span>|<span data-ttu-id="47c68-111">说明</span><span class="sxs-lookup"><span data-stu-id="47c68-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="47c68-112">获取 symantecCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="47c68-112">Get symantecCodeSigningCertificate</span></span>](../api/intune-apps-symanteccodesigningcertificate-get.md)|[<span data-ttu-id="47c68-113">symantecCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="47c68-113">symantecCodeSigningCertificate</span></span>](../resources/intune-apps-symanteccodesigningcertificate.md)|<span data-ttu-id="47c68-114">读取 [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="47c68-114">Read properties and relationships of the [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>|
|[<span data-ttu-id="47c68-115">更新 symantecCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="47c68-115">Update symantecCodeSigningCertificate</span></span>](../api/intune-apps-symanteccodesigningcertificate-update.md)|[<span data-ttu-id="47c68-116">symantecCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="47c68-116">symantecCodeSigningCertificate</span></span>](../resources/intune-apps-symanteccodesigningcertificate.md)|<span data-ttu-id="47c68-117">更新 [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="47c68-117">Update the properties of a [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="47c68-118">属性</span><span class="sxs-lookup"><span data-stu-id="47c68-118">Properties</span></span>
|<span data-ttu-id="47c68-119">属性</span><span class="sxs-lookup"><span data-stu-id="47c68-119">Property</span></span>|<span data-ttu-id="47c68-120">类型</span><span class="sxs-lookup"><span data-stu-id="47c68-120">Type</span></span>|<span data-ttu-id="47c68-121">说明</span><span class="sxs-lookup"><span data-stu-id="47c68-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47c68-122">id</span><span class="sxs-lookup"><span data-stu-id="47c68-122">id</span></span>|<span data-ttu-id="47c68-123">String</span><span class="sxs-lookup"><span data-stu-id="47c68-123">String</span></span>|<span data-ttu-id="47c68-124">实体的键。</span><span class="sxs-lookup"><span data-stu-id="47c68-124">The key of the entity.</span></span>|
|<span data-ttu-id="47c68-125">content</span><span class="sxs-lookup"><span data-stu-id="47c68-125">content</span></span>|<span data-ttu-id="47c68-126">Binary</span><span class="sxs-lookup"><span data-stu-id="47c68-126">Binary</span></span>|<span data-ttu-id="47c68-127">原始数据格式的 Windows Symantec 代码签名证书。</span><span class="sxs-lookup"><span data-stu-id="47c68-127">The Windows Symantec Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="47c68-128">状态</span><span class="sxs-lookup"><span data-stu-id="47c68-128">status</span></span>|[<span data-ttu-id="47c68-129">certificateStatus</span><span class="sxs-lookup"><span data-stu-id="47c68-129">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="47c68-130">证书状态已设置或未设置。</span><span class="sxs-lookup"><span data-stu-id="47c68-130">The Cert Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="47c68-131">可取值为：`notProvisioned`、`provisioned`。</span><span class="sxs-lookup"><span data-stu-id="47c68-131">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="47c68-132">密码</span><span class="sxs-lookup"><span data-stu-id="47c68-132">password</span></span>|<span data-ttu-id="47c68-133">String</span><span class="sxs-lookup"><span data-stu-id="47c68-133">String</span></span>|<span data-ttu-id="47c68-134">.Pfx 文件所需的密码。</span><span class="sxs-lookup"><span data-stu-id="47c68-134">The Password required for .pfx file.</span></span>|
|<span data-ttu-id="47c68-135">SubjectName</span><span class="sxs-lookup"><span data-stu-id="47c68-135">subjectName</span></span>|<span data-ttu-id="47c68-136">String</span><span class="sxs-lookup"><span data-stu-id="47c68-136">String</span></span>|<span data-ttu-id="47c68-137">证书的主题名称。</span><span class="sxs-lookup"><span data-stu-id="47c68-137">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="47c68-138">subject</span><span class="sxs-lookup"><span data-stu-id="47c68-138">subject</span></span>|<span data-ttu-id="47c68-139">String</span><span class="sxs-lookup"><span data-stu-id="47c68-139">String</span></span>|<span data-ttu-id="47c68-140">证书的主题值。</span><span class="sxs-lookup"><span data-stu-id="47c68-140">The Subject value for the cert.</span></span>|
|<span data-ttu-id="47c68-141">issuerName</span><span class="sxs-lookup"><span data-stu-id="47c68-141">issuerName</span></span>|<span data-ttu-id="47c68-142">String</span><span class="sxs-lookup"><span data-stu-id="47c68-142">String</span></span>|<span data-ttu-id="47c68-143">证书的颁发者名称。</span><span class="sxs-lookup"><span data-stu-id="47c68-143">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="47c68-144">常用</span><span class="sxs-lookup"><span data-stu-id="47c68-144">issuer</span></span>|<span data-ttu-id="47c68-145">String</span><span class="sxs-lookup"><span data-stu-id="47c68-145">String</span></span>|<span data-ttu-id="47c68-146">证书的 Issuer 值。</span><span class="sxs-lookup"><span data-stu-id="47c68-146">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="47c68-147">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="47c68-147">expirationDateTime</span></span>|<span data-ttu-id="47c68-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47c68-148">DateTimeOffset</span></span>|<span data-ttu-id="47c68-149">证书到期日期。</span><span class="sxs-lookup"><span data-stu-id="47c68-149">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="47c68-150">uploadDateTime</span><span class="sxs-lookup"><span data-stu-id="47c68-150">uploadDateTime</span></span>|<span data-ttu-id="47c68-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47c68-151">DateTimeOffset</span></span>|<span data-ttu-id="47c68-152">作为 Symantec 证书的 CodeSigning 证书的类型。</span><span class="sxs-lookup"><span data-stu-id="47c68-152">The Type of the CodeSigning Cert as Symantec Cert.</span></span>|

## <a name="relationships"></a><span data-ttu-id="47c68-153">关系</span><span class="sxs-lookup"><span data-stu-id="47c68-153">Relationships</span></span>
<span data-ttu-id="47c68-154">无</span><span class="sxs-lookup"><span data-stu-id="47c68-154">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="47c68-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="47c68-155">JSON Representation</span></span>
<span data-ttu-id="47c68-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="47c68-156">Here is a JSON representation of the resource.</span></span>
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






