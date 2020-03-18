---
title: iosEduCertificateSettings 资源类型
description: 适用于 iOS EDU 的受信任的根和 PFX 证书。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f772ee8f484b2b8bc42a6ed48298dc5a17016afc
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42791616"
---
# <a name="ioseducertificatesettings-resource-type"></a><span data-ttu-id="ed561-103">iosEduCertificateSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="ed561-103">iosEduCertificateSettings resource type</span></span>

> <span data-ttu-id="ed561-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ed561-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ed561-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ed561-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed561-106">适用于 iOS EDU 的受信任的根和 PFX 证书。</span><span class="sxs-lookup"><span data-stu-id="ed561-106">Trusted Root and PFX certificates for iOS EDU.</span></span>

## <a name="properties"></a><span data-ttu-id="ed561-107">属性</span><span class="sxs-lookup"><span data-stu-id="ed561-107">Properties</span></span>
|<span data-ttu-id="ed561-108">属性</span><span class="sxs-lookup"><span data-stu-id="ed561-108">Property</span></span>|<span data-ttu-id="ed561-109">类型</span><span class="sxs-lookup"><span data-stu-id="ed561-109">Type</span></span>|<span data-ttu-id="ed561-110">说明</span><span class="sxs-lookup"><span data-stu-id="ed561-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed561-111">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="ed561-111">trustedRootCertificate</span></span>|<span data-ttu-id="ed561-112">Binary</span><span class="sxs-lookup"><span data-stu-id="ed561-112">Binary</span></span>|<span data-ttu-id="ed561-113">受信任的根证书。</span><span class="sxs-lookup"><span data-stu-id="ed561-113">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="ed561-114">certFileName</span><span class="sxs-lookup"><span data-stu-id="ed561-114">certFileName</span></span>|<span data-ttu-id="ed561-115">String</span><span class="sxs-lookup"><span data-stu-id="ed561-115">String</span></span>|<span data-ttu-id="ed561-116">要在 UI 中显示的文件名。</span><span class="sxs-lookup"><span data-stu-id="ed561-116">File name to display in UI.</span></span>|
|<span data-ttu-id="ed561-117">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="ed561-117">certificationAuthority</span></span>|<span data-ttu-id="ed561-118">String</span><span class="sxs-lookup"><span data-stu-id="ed561-118">String</span></span>|<span data-ttu-id="ed561-119">PKCS 证书颁发机构。</span><span class="sxs-lookup"><span data-stu-id="ed561-119">PKCS Certification Authority.</span></span>|
|<span data-ttu-id="ed561-120">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="ed561-120">certificationAuthorityName</span></span>|<span data-ttu-id="ed561-121">String</span><span class="sxs-lookup"><span data-stu-id="ed561-121">String</span></span>|<span data-ttu-id="ed561-122">PKCS 证书颁发机构名称。</span><span class="sxs-lookup"><span data-stu-id="ed561-122">PKCS Certification Authority Name.</span></span>|
|<span data-ttu-id="ed561-123">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="ed561-123">certificateTemplateName</span></span>|<span data-ttu-id="ed561-124">String</span><span class="sxs-lookup"><span data-stu-id="ed561-124">String</span></span>|<span data-ttu-id="ed561-125">PKCS 证书模板名称。</span><span class="sxs-lookup"><span data-stu-id="ed561-125">PKCS Certificate Template Name.</span></span>|
|<span data-ttu-id="ed561-126">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="ed561-126">renewalThresholdPercentage</span></span>|<span data-ttu-id="ed561-127">Int32</span><span class="sxs-lookup"><span data-stu-id="ed561-127">Int32</span></span>|<span data-ttu-id="ed561-128">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="ed561-128">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="ed561-129">有效值为1至99</span><span class="sxs-lookup"><span data-stu-id="ed561-129">Valid values 1 to 99</span></span>|
|<span data-ttu-id="ed561-130">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="ed561-130">certificateValidityPeriodValue</span></span>|<span data-ttu-id="ed561-131">Int32</span><span class="sxs-lookup"><span data-stu-id="ed561-131">Int32</span></span>|<span data-ttu-id="ed561-132">证书有效期限的值。</span><span class="sxs-lookup"><span data-stu-id="ed561-132">Value for the Certificate Validity Period.</span></span>|
|<span data-ttu-id="ed561-133">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="ed561-133">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="ed561-134">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="ed561-134">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="ed561-135">证书有效期的小数位数。</span><span class="sxs-lookup"><span data-stu-id="ed561-135">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="ed561-136">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="ed561-136">Possible values are: `days`, `months`, `years`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ed561-137">关系</span><span class="sxs-lookup"><span data-stu-id="ed561-137">Relationships</span></span>
<span data-ttu-id="ed561-138">无</span><span class="sxs-lookup"><span data-stu-id="ed561-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ed561-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ed561-139">JSON Representation</span></span>
<span data-ttu-id="ed561-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ed561-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosEduCertificateSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosEduCertificateSettings",
  "trustedRootCertificate": "binary",
  "certFileName": "String",
  "certificationAuthority": "String",
  "certificationAuthorityName": "String",
  "certificateTemplateName": "String",
  "renewalThresholdPercentage": 1024,
  "certificateValidityPeriodValue": 1024,
  "certificateValidityPeriodScale": "String"
}
```



