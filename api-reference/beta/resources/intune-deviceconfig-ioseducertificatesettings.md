---
title: iosEduCertificateSettings 资源类型
description: 适用于 iOS EDU 的受信任的根和 PFX 证书。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 30e7a68f76c60fafff9fc2b035a65a60307f775d
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34981466"
---
# <a name="ioseducertificatesettings-resource-type"></a><span data-ttu-id="9454e-103">iosEduCertificateSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="9454e-103">iosEduCertificateSettings resource type</span></span>

> <span data-ttu-id="9454e-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9454e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9454e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9454e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9454e-106">适用于 iOS EDU 的受信任的根和 PFX 证书。</span><span class="sxs-lookup"><span data-stu-id="9454e-106">Trusted Root and PFX certificates for iOS EDU.</span></span>

## <a name="properties"></a><span data-ttu-id="9454e-107">属性</span><span class="sxs-lookup"><span data-stu-id="9454e-107">Properties</span></span>
|<span data-ttu-id="9454e-108">属性</span><span class="sxs-lookup"><span data-stu-id="9454e-108">Property</span></span>|<span data-ttu-id="9454e-109">类型</span><span class="sxs-lookup"><span data-stu-id="9454e-109">Type</span></span>|<span data-ttu-id="9454e-110">说明</span><span class="sxs-lookup"><span data-stu-id="9454e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9454e-111">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="9454e-111">trustedRootCertificate</span></span>|<span data-ttu-id="9454e-112">Binary</span><span class="sxs-lookup"><span data-stu-id="9454e-112">Binary</span></span>|<span data-ttu-id="9454e-113">受信任的根证书。</span><span class="sxs-lookup"><span data-stu-id="9454e-113">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="9454e-114">certFileName</span><span class="sxs-lookup"><span data-stu-id="9454e-114">certFileName</span></span>|<span data-ttu-id="9454e-115">String</span><span class="sxs-lookup"><span data-stu-id="9454e-115">String</span></span>|<span data-ttu-id="9454e-116">要在 UI 中显示的文件名。</span><span class="sxs-lookup"><span data-stu-id="9454e-116">File name to display in UI.</span></span>|
|<span data-ttu-id="9454e-117">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="9454e-117">certificationAuthority</span></span>|<span data-ttu-id="9454e-118">String</span><span class="sxs-lookup"><span data-stu-id="9454e-118">String</span></span>|<span data-ttu-id="9454e-119">PKCS 证书颁发机构。</span><span class="sxs-lookup"><span data-stu-id="9454e-119">PKCS Certification Authority.</span></span>|
|<span data-ttu-id="9454e-120">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="9454e-120">certificationAuthorityName</span></span>|<span data-ttu-id="9454e-121">String</span><span class="sxs-lookup"><span data-stu-id="9454e-121">String</span></span>|<span data-ttu-id="9454e-122">PKCS 证书颁发机构名称。</span><span class="sxs-lookup"><span data-stu-id="9454e-122">PKCS Certification Authority Name.</span></span>|
|<span data-ttu-id="9454e-123">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="9454e-123">certificateTemplateName</span></span>|<span data-ttu-id="9454e-124">String</span><span class="sxs-lookup"><span data-stu-id="9454e-124">String</span></span>|<span data-ttu-id="9454e-125">PKCS 证书模板名称。</span><span class="sxs-lookup"><span data-stu-id="9454e-125">PKCS Certificate Template Name.</span></span>|
|<span data-ttu-id="9454e-126">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="9454e-126">renewalThresholdPercentage</span></span>|<span data-ttu-id="9454e-127">Int32</span><span class="sxs-lookup"><span data-stu-id="9454e-127">Int32</span></span>|<span data-ttu-id="9454e-128">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="9454e-128">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="9454e-129">有效值为1至99</span><span class="sxs-lookup"><span data-stu-id="9454e-129">Valid values 1 to 99</span></span>|
|<span data-ttu-id="9454e-130">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="9454e-130">certificateValidityPeriodValue</span></span>|<span data-ttu-id="9454e-131">Int32</span><span class="sxs-lookup"><span data-stu-id="9454e-131">Int32</span></span>|<span data-ttu-id="9454e-132">证书有效期限的值。</span><span class="sxs-lookup"><span data-stu-id="9454e-132">Value for the Certificate Validity Period.</span></span>|
|<span data-ttu-id="9454e-133">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="9454e-133">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="9454e-134">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="9454e-134">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="9454e-135">证书有效期的小数位数。</span><span class="sxs-lookup"><span data-stu-id="9454e-135">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="9454e-136">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="9454e-136">Possible values are: `days`, `months`, `years`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9454e-137">关系</span><span class="sxs-lookup"><span data-stu-id="9454e-137">Relationships</span></span>
<span data-ttu-id="9454e-138">无</span><span class="sxs-lookup"><span data-stu-id="9454e-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9454e-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9454e-139">JSON Representation</span></span>
<span data-ttu-id="9454e-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9454e-140">Here is a JSON representation of the resource.</span></span>
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





