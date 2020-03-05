---
title: iosEduCertificateSettings 资源类型
description: 适用于 iOS EDU 的受信任的根和 PFX 证书。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 503d2b1d0f4fa94e95d20882b10a0c30d968680e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529928"
---
# <a name="ioseducertificatesettings-resource-type"></a><span data-ttu-id="0642b-103">iosEduCertificateSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="0642b-103">iosEduCertificateSettings resource type</span></span>

<span data-ttu-id="0642b-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="0642b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0642b-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0642b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0642b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0642b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0642b-107">适用于 iOS EDU 的受信任的根和 PFX 证书。</span><span class="sxs-lookup"><span data-stu-id="0642b-107">Trusted Root and PFX certificates for iOS EDU.</span></span>

## <a name="properties"></a><span data-ttu-id="0642b-108">属性</span><span class="sxs-lookup"><span data-stu-id="0642b-108">Properties</span></span>
|<span data-ttu-id="0642b-109">属性</span><span class="sxs-lookup"><span data-stu-id="0642b-109">Property</span></span>|<span data-ttu-id="0642b-110">类型</span><span class="sxs-lookup"><span data-stu-id="0642b-110">Type</span></span>|<span data-ttu-id="0642b-111">说明</span><span class="sxs-lookup"><span data-stu-id="0642b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0642b-112">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="0642b-112">trustedRootCertificate</span></span>|<span data-ttu-id="0642b-113">Binary</span><span class="sxs-lookup"><span data-stu-id="0642b-113">Binary</span></span>|<span data-ttu-id="0642b-114">受信任的根证书。</span><span class="sxs-lookup"><span data-stu-id="0642b-114">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="0642b-115">certFileName</span><span class="sxs-lookup"><span data-stu-id="0642b-115">certFileName</span></span>|<span data-ttu-id="0642b-116">String</span><span class="sxs-lookup"><span data-stu-id="0642b-116">String</span></span>|<span data-ttu-id="0642b-117">要在 UI 中显示的文件名。</span><span class="sxs-lookup"><span data-stu-id="0642b-117">File name to display in UI.</span></span>|
|<span data-ttu-id="0642b-118">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="0642b-118">certificationAuthority</span></span>|<span data-ttu-id="0642b-119">String</span><span class="sxs-lookup"><span data-stu-id="0642b-119">String</span></span>|<span data-ttu-id="0642b-120">PKCS 证书颁发机构。</span><span class="sxs-lookup"><span data-stu-id="0642b-120">PKCS Certification Authority.</span></span>|
|<span data-ttu-id="0642b-121">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="0642b-121">certificationAuthorityName</span></span>|<span data-ttu-id="0642b-122">String</span><span class="sxs-lookup"><span data-stu-id="0642b-122">String</span></span>|<span data-ttu-id="0642b-123">PKCS 证书颁发机构名称。</span><span class="sxs-lookup"><span data-stu-id="0642b-123">PKCS Certification Authority Name.</span></span>|
|<span data-ttu-id="0642b-124">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="0642b-124">certificateTemplateName</span></span>|<span data-ttu-id="0642b-125">String</span><span class="sxs-lookup"><span data-stu-id="0642b-125">String</span></span>|<span data-ttu-id="0642b-126">PKCS 证书模板名称。</span><span class="sxs-lookup"><span data-stu-id="0642b-126">PKCS Certificate Template Name.</span></span>|
|<span data-ttu-id="0642b-127">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="0642b-127">renewalThresholdPercentage</span></span>|<span data-ttu-id="0642b-128">Int32</span><span class="sxs-lookup"><span data-stu-id="0642b-128">Int32</span></span>|<span data-ttu-id="0642b-129">证书续订阈值百分比。</span><span class="sxs-lookup"><span data-stu-id="0642b-129">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="0642b-130">有效值为1至99</span><span class="sxs-lookup"><span data-stu-id="0642b-130">Valid values 1 to 99</span></span>|
|<span data-ttu-id="0642b-131">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="0642b-131">certificateValidityPeriodValue</span></span>|<span data-ttu-id="0642b-132">Int32</span><span class="sxs-lookup"><span data-stu-id="0642b-132">Int32</span></span>|<span data-ttu-id="0642b-133">证书有效期限的值。</span><span class="sxs-lookup"><span data-stu-id="0642b-133">Value for the Certificate Validity Period.</span></span>|
|<span data-ttu-id="0642b-134">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="0642b-134">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="0642b-135">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="0642b-135">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="0642b-136">证书有效期的小数位数。</span><span class="sxs-lookup"><span data-stu-id="0642b-136">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="0642b-137">可取值为：`days`、`months`、`years`。</span><span class="sxs-lookup"><span data-stu-id="0642b-137">Possible values are: `days`, `months`, `years`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0642b-138">关系</span><span class="sxs-lookup"><span data-stu-id="0642b-138">Relationships</span></span>
<span data-ttu-id="0642b-139">无</span><span class="sxs-lookup"><span data-stu-id="0642b-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0642b-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0642b-140">JSON Representation</span></span>
<span data-ttu-id="0642b-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0642b-141">Here is a JSON representation of the resource.</span></span>
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



