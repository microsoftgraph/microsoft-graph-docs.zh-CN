---
title: iosEduCertificateSettings 资源类型
description: 适用于 iOS EDU 的受信任的根和 PFX 证书。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d23b379dea7a75e4ae79029845cd6e9f956503c0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423550"
---
# <a name="ioseducertificatesettings-resource-type"></a><span data-ttu-id="d04b3-103">iosEduCertificateSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="d04b3-103">iosEduCertificateSettings resource type</span></span>

> <span data-ttu-id="d04b3-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="d04b3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d04b3-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d04b3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d04b3-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d04b3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d04b3-107">适用于 iOS EDU 的受信任的根和 PFX 证书。</span><span class="sxs-lookup"><span data-stu-id="d04b3-107">Trusted Root and PFX certificates for iOS EDU.</span></span>

## <a name="properties"></a><span data-ttu-id="d04b3-108">属性</span><span class="sxs-lookup"><span data-stu-id="d04b3-108">Properties</span></span>
|<span data-ttu-id="d04b3-109">属性</span><span class="sxs-lookup"><span data-stu-id="d04b3-109">Property</span></span>|<span data-ttu-id="d04b3-110">类型</span><span class="sxs-lookup"><span data-stu-id="d04b3-110">Type</span></span>|<span data-ttu-id="d04b3-111">说明</span><span class="sxs-lookup"><span data-stu-id="d04b3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d04b3-112">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="d04b3-112">trustedRootCertificate</span></span>|<span data-ttu-id="d04b3-113">Binary</span><span class="sxs-lookup"><span data-stu-id="d04b3-113">Binary</span></span>|<span data-ttu-id="d04b3-114">受信任的根证书。</span><span class="sxs-lookup"><span data-stu-id="d04b3-114">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="d04b3-115">certFileName</span><span class="sxs-lookup"><span data-stu-id="d04b3-115">certFileName</span></span>|<span data-ttu-id="d04b3-116">String</span><span class="sxs-lookup"><span data-stu-id="d04b3-116">String</span></span>|<span data-ttu-id="d04b3-117">若要在 UI 中显示的文件名。</span><span class="sxs-lookup"><span data-stu-id="d04b3-117">File name to display in UI.</span></span>|
|<span data-ttu-id="d04b3-118">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="d04b3-118">certificationAuthority</span></span>|<span data-ttu-id="d04b3-119">String</span><span class="sxs-lookup"><span data-stu-id="d04b3-119">String</span></span>|<span data-ttu-id="d04b3-120">PKCS 证书颁发机构。</span><span class="sxs-lookup"><span data-stu-id="d04b3-120">PKCS Certification Authority.</span></span>|
|<span data-ttu-id="d04b3-121">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="d04b3-121">certificationAuthorityName</span></span>|<span data-ttu-id="d04b3-122">String</span><span class="sxs-lookup"><span data-stu-id="d04b3-122">String</span></span>|<span data-ttu-id="d04b3-123">PKCS 证书颁发机构的名称。</span><span class="sxs-lookup"><span data-stu-id="d04b3-123">PKCS Certification Authority Name.</span></span>|
|<span data-ttu-id="d04b3-124">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="d04b3-124">certificateTemplateName</span></span>|<span data-ttu-id="d04b3-125">String</span><span class="sxs-lookup"><span data-stu-id="d04b3-125">String</span></span>|<span data-ttu-id="d04b3-126">PKCS 证书模板名称。</span><span class="sxs-lookup"><span data-stu-id="d04b3-126">PKCS Certificate Template Name.</span></span>|
|<span data-ttu-id="d04b3-127">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="d04b3-127">renewalThresholdPercentage</span></span>|<span data-ttu-id="d04b3-128">Int32</span><span class="sxs-lookup"><span data-stu-id="d04b3-128">Int32</span></span>|<span data-ttu-id="d04b3-129">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="d04b3-129">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="d04b3-130">有效的值 1 到 99</span><span class="sxs-lookup"><span data-stu-id="d04b3-130">Valid values 1 to 99</span></span>|
|<span data-ttu-id="d04b3-131">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="d04b3-131">certificateValidityPeriodValue</span></span>|<span data-ttu-id="d04b3-132">Int32</span><span class="sxs-lookup"><span data-stu-id="d04b3-132">Int32</span></span>|<span data-ttu-id="d04b3-133">证书有效期限的值。</span><span class="sxs-lookup"><span data-stu-id="d04b3-133">Value for the Certificate Validity Period.</span></span>|
|<span data-ttu-id="d04b3-134">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="d04b3-134">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="d04b3-135">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="d04b3-135">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="d04b3-136">证书有效期限的小数位数。</span><span class="sxs-lookup"><span data-stu-id="d04b3-136">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="d04b3-137">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="d04b3-137">Possible values are: `days`, `months`, `years`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d04b3-138">Relationships</span><span class="sxs-lookup"><span data-stu-id="d04b3-138">Relationships</span></span>
<span data-ttu-id="d04b3-139">无</span><span class="sxs-lookup"><span data-stu-id="d04b3-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d04b3-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d04b3-140">JSON Representation</span></span>
<span data-ttu-id="d04b3-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d04b3-141">Here is a JSON representation of the resource.</span></span>
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




