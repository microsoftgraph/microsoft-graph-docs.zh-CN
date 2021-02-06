---
title: verifiedCustomDomainCertificatesMetadata 资源类型
description: 表示通过应用程序代理发布的本地应用程序的自定义证书元数据。
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: bc0f839d91147f80d41dc48ee53c0f888aa35283
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137590"
---
# <a name="verifiedcustomdomaincertificatesmetadata-resource-type"></a><span data-ttu-id="02820-103">verifiedCustomDomainCertificatesMetadata 资源类型</span><span class="sxs-lookup"><span data-stu-id="02820-103">verifiedCustomDomainCertificatesMetadata resource type</span></span>

<span data-ttu-id="02820-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02820-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02820-105">表示使用应用程序代理发布本地应用程序时 [onPremisesPublishing](onpremisespublishing.md) 资源的自定义域证书元数据。</span><span class="sxs-lookup"><span data-stu-id="02820-105">Represents the custom domain certificate metadata for the [onPremisesPublishing](onpremisespublishing.md) resource when publishing an on-premises application with Application Proxy.</span></span> <span data-ttu-id="02820-106">使用自定义域，您可以为应用程序使用自己的域名，而不是默认msappproxy.net域名。</span><span class="sxs-lookup"><span data-stu-id="02820-106">Using a custom domain allows you to use your own domain name instead of the default domain, msappproxy.net, for your application.</span></span> <span data-ttu-id="02820-107">若要了解更多信息，请参阅 [Azure AD 应用程序代理中的自定义域](/azure/active-directory/manage-apps/application-proxy-configure-custom-domain)。</span><span class="sxs-lookup"><span data-stu-id="02820-107">To learn more see, [Custom domains in Azure AD Application Proxy](/azure/active-directory/manage-apps/application-proxy-configure-custom-domain).</span></span>

## <a name="properties"></a><span data-ttu-id="02820-108">属性</span><span class="sxs-lookup"><span data-stu-id="02820-108">Properties</span></span>

| <span data-ttu-id="02820-109">属性</span><span class="sxs-lookup"><span data-stu-id="02820-109">Property</span></span>     | <span data-ttu-id="02820-110">类型</span><span class="sxs-lookup"><span data-stu-id="02820-110">Type</span></span>        | <span data-ttu-id="02820-111">说明</span><span class="sxs-lookup"><span data-stu-id="02820-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="02820-112">expiryDate</span><span class="sxs-lookup"><span data-stu-id="02820-112">expiryDate</span></span>|<span data-ttu-id="02820-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02820-113">DateTimeOffset</span></span>| <span data-ttu-id="02820-114">自定义域证书的到期日期。</span><span class="sxs-lookup"><span data-stu-id="02820-114">The expiry date of the custom domain certificate.</span></span> <span data-ttu-id="02820-115">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="02820-115">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="02820-116">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="02820-116">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> |
|<span data-ttu-id="02820-117">issueDate</span><span class="sxs-lookup"><span data-stu-id="02820-117">issueDate</span></span>|<span data-ttu-id="02820-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02820-118">DateTimeOffset</span></span>| <span data-ttu-id="02820-119">自定义域的发行日期。</span><span class="sxs-lookup"><span data-stu-id="02820-119">The issue date of the custom domain.</span></span> <span data-ttu-id="02820-120">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="02820-120">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="02820-121">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="02820-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> |
|<span data-ttu-id="02820-122">issuerName</span><span class="sxs-lookup"><span data-stu-id="02820-122">issuerName</span></span>|<span data-ttu-id="02820-123">字符串</span><span class="sxs-lookup"><span data-stu-id="02820-123">String</span></span>| <span data-ttu-id="02820-124">自定义域证书的颁发者名称。</span><span class="sxs-lookup"><span data-stu-id="02820-124">The issuer name of the custom domain certificate.</span></span> |
|<span data-ttu-id="02820-125">SubjectName</span><span class="sxs-lookup"><span data-stu-id="02820-125">subjectName</span></span>|<span data-ttu-id="02820-126">String</span><span class="sxs-lookup"><span data-stu-id="02820-126">String</span></span>| <span data-ttu-id="02820-127">自定义域证书的主题名称。</span><span class="sxs-lookup"><span data-stu-id="02820-127">The subject name of the custom domain certificate.</span></span> |
|<span data-ttu-id="02820-128">thumbprint</span><span class="sxs-lookup"><span data-stu-id="02820-128">thumbprint</span></span>|<span data-ttu-id="02820-129">字符串</span><span class="sxs-lookup"><span data-stu-id="02820-129">String</span></span>| <span data-ttu-id="02820-130">与自定义域证书关联的指纹。</span><span class="sxs-lookup"><span data-stu-id="02820-130">The thumbprint associated with the custom domain certificate.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="02820-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="02820-131">JSON representation</span></span>

<span data-ttu-id="02820-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="02820-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.verifiedCustomDomainCertificatesMetadata",
  "baseType": null
}-->

```json
{
  "expiryDate": "String (timestamp)",
  "issueDate": "String (timestamp)",
  "issuerName": "String",
  "subjectName": "String",
  "thumbprint": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "verifiedCustomDomainCertificatesMetadata resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
