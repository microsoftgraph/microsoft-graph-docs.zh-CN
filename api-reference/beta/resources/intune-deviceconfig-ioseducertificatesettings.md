---
title: iosEduCertificateSettings 资源类型
description: 适用于 iOS EDU 的受信任的根和 PFX 证书。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: bf6b0da4d3ff7af562ae99e81e10f52351bd735d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822076"
---
# <a name="ioseducertificatesettings-resource-type"></a><span data-ttu-id="e1cef-103">iosEduCertificateSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="e1cef-103">iosEduCertificateSettings resource type</span></span>

> <span data-ttu-id="e1cef-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e1cef-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e1cef-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e1cef-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e1cef-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e1cef-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e1cef-107">适用于 iOS EDU 的受信任的根和 PFX 证书。</span><span class="sxs-lookup"><span data-stu-id="e1cef-107">Trusted Root and PFX certificates for iOS EDU.</span></span>
## <a name="properties"></a><span data-ttu-id="e1cef-108">属性</span><span class="sxs-lookup"><span data-stu-id="e1cef-108">Properties</span></span>
|<span data-ttu-id="e1cef-109">属性</span><span class="sxs-lookup"><span data-stu-id="e1cef-109">Property</span></span>|<span data-ttu-id="e1cef-110">类型</span><span class="sxs-lookup"><span data-stu-id="e1cef-110">Type</span></span>|<span data-ttu-id="e1cef-111">Description</span><span class="sxs-lookup"><span data-stu-id="e1cef-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1cef-112">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="e1cef-112">trustedRootCertificate</span></span>|<span data-ttu-id="e1cef-113">Binary</span><span class="sxs-lookup"><span data-stu-id="e1cef-113">Binary</span></span>|<span data-ttu-id="e1cef-114">受信任的根证书。</span><span class="sxs-lookup"><span data-stu-id="e1cef-114">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="e1cef-115">certFileName</span><span class="sxs-lookup"><span data-stu-id="e1cef-115">certFileName</span></span>|<span data-ttu-id="e1cef-116">字符串</span><span class="sxs-lookup"><span data-stu-id="e1cef-116">String</span></span>|<span data-ttu-id="e1cef-117">若要在 UI 中显示的文件名。</span><span class="sxs-lookup"><span data-stu-id="e1cef-117">File name to display in UI.</span></span>|
|<span data-ttu-id="e1cef-118">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="e1cef-118">certificationAuthority</span></span>|<span data-ttu-id="e1cef-119">字符串</span><span class="sxs-lookup"><span data-stu-id="e1cef-119">String</span></span>|<span data-ttu-id="e1cef-120">PKCS 证书颁发机构。</span><span class="sxs-lookup"><span data-stu-id="e1cef-120">PKCS Certification Authority.</span></span>|
|<span data-ttu-id="e1cef-121">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="e1cef-121">certificationAuthorityName</span></span>|<span data-ttu-id="e1cef-122">字符串</span><span class="sxs-lookup"><span data-stu-id="e1cef-122">String</span></span>|<span data-ttu-id="e1cef-123">PKCS 证书颁发机构的名称。</span><span class="sxs-lookup"><span data-stu-id="e1cef-123">PKCS Certification Authority Name.</span></span>|
|<span data-ttu-id="e1cef-124">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="e1cef-124">certificateTemplateName</span></span>|<span data-ttu-id="e1cef-125">字符串</span><span class="sxs-lookup"><span data-stu-id="e1cef-125">String</span></span>|<span data-ttu-id="e1cef-126">PKCS 证书模板名称。</span><span class="sxs-lookup"><span data-stu-id="e1cef-126">PKCS Certificate Template Name.</span></span>|
|<span data-ttu-id="e1cef-127">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="e1cef-127">renewalThresholdPercentage</span></span>|<span data-ttu-id="e1cef-128">Int32</span><span class="sxs-lookup"><span data-stu-id="e1cef-128">Int32</span></span>|<span data-ttu-id="e1cef-129">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="e1cef-129">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="e1cef-130">有效的值 1 到 99</span><span class="sxs-lookup"><span data-stu-id="e1cef-130">Valid values 1 to 99</span></span>|
|<span data-ttu-id="e1cef-131">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="e1cef-131">certificateValidityPeriodValue</span></span>|<span data-ttu-id="e1cef-132">Int32</span><span class="sxs-lookup"><span data-stu-id="e1cef-132">Int32</span></span>|<span data-ttu-id="e1cef-133">证书有效期限的值。</span><span class="sxs-lookup"><span data-stu-id="e1cef-133">Value for the Certificate Validity Period.</span></span>|
|<span data-ttu-id="e1cef-134">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="e1cef-134">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="e1cef-135">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="e1cef-135">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="e1cef-136">证书有效期限的小数位数。</span><span class="sxs-lookup"><span data-stu-id="e1cef-136">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="e1cef-137">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="e1cef-137">Possible values are: `days`, `months`, `years`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1cef-138">Relationships</span><span class="sxs-lookup"><span data-stu-id="e1cef-138">Relationships</span></span>
<span data-ttu-id="e1cef-139">无</span><span class="sxs-lookup"><span data-stu-id="e1cef-139">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e1cef-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e1cef-140">JSON Representation</span></span>
<span data-ttu-id="e1cef-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e1cef-141">Here is a JSON representation of the resource.</span></span>
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





