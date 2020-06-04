---
title: verifiedCustomDomainCertificatesMetadata 资源类型
description: 表示通过应用程序代理发布的本地应用程序的自定义证书元数据。
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4268c7d9faba8e744f7a6bd6a674ff680cb24346
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556390"
---
# <a name="verifiedcustomdomaincertificatesmetadata-resource-type"></a><span data-ttu-id="1ab77-103">verifiedCustomDomainCertificatesMetadata 资源类型</span><span class="sxs-lookup"><span data-stu-id="1ab77-103">verifiedCustomDomainCertificatesMetadata resource type</span></span>

<span data-ttu-id="1ab77-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ab77-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ab77-105">表示在使用应用程序代理发布本地应用程序时， [onPremisesPublishing](onpremisespublishing.md)资源的自定义域证书元数据。</span><span class="sxs-lookup"><span data-stu-id="1ab77-105">Represents the custom domain certificate metadata for the [onPremisesPublishing](onpremisespublishing.md) resource when publishing an on-premises application with Application Proxy.</span></span> <span data-ttu-id="1ab77-106">使用自定义域允许您为应用程序使用自己的域名，而不是默认域 msappproxy.net。</span><span class="sxs-lookup"><span data-stu-id="1ab77-106">Using a custom domain allows you to use your own domain name instead of the default domain, msappproxy.net, for your application.</span></span> <span data-ttu-id="1ab77-107">若要了解详细信息，请参阅[AZURE AD 应用程序代理中的自定义域](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-custom-domain)。</span><span class="sxs-lookup"><span data-stu-id="1ab77-107">To learn more see, [Custom domains in Azure AD Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-custom-domain).</span></span>

## <a name="properties"></a><span data-ttu-id="1ab77-108">属性</span><span class="sxs-lookup"><span data-stu-id="1ab77-108">Properties</span></span>

| <span data-ttu-id="1ab77-109">属性</span><span class="sxs-lookup"><span data-stu-id="1ab77-109">Property</span></span>     | <span data-ttu-id="1ab77-110">类型</span><span class="sxs-lookup"><span data-stu-id="1ab77-110">Type</span></span>        | <span data-ttu-id="1ab77-111">说明</span><span class="sxs-lookup"><span data-stu-id="1ab77-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1ab77-112">expiryDate</span><span class="sxs-lookup"><span data-stu-id="1ab77-112">expiryDate</span></span>|<span data-ttu-id="1ab77-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ab77-113">DateTimeOffset</span></span>| <span data-ttu-id="1ab77-114">自定义域证书的到期日期。</span><span class="sxs-lookup"><span data-stu-id="1ab77-114">The expiry date of the custom domain certificate.</span></span> <span data-ttu-id="1ab77-115">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="1ab77-115">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1ab77-116">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="1ab77-116">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> |
|<span data-ttu-id="1ab77-117">issueDate</span><span class="sxs-lookup"><span data-stu-id="1ab77-117">issueDate</span></span>|<span data-ttu-id="1ab77-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ab77-118">DateTimeOffset</span></span>| <span data-ttu-id="1ab77-119">自定义域的签发日期。</span><span class="sxs-lookup"><span data-stu-id="1ab77-119">The issue date of the custom domain.</span></span> <span data-ttu-id="1ab77-120">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="1ab77-120">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1ab77-121">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="1ab77-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> |
|<span data-ttu-id="1ab77-122">issuerName</span><span class="sxs-lookup"><span data-stu-id="1ab77-122">issuerName</span></span>|<span data-ttu-id="1ab77-123">String</span><span class="sxs-lookup"><span data-stu-id="1ab77-123">String</span></span>| <span data-ttu-id="1ab77-124">自定义域证书的颁发者名称。</span><span class="sxs-lookup"><span data-stu-id="1ab77-124">The issuer name of the custom domain certificate.</span></span> |
|<span data-ttu-id="1ab77-125">SubjectName</span><span class="sxs-lookup"><span data-stu-id="1ab77-125">subjectName</span></span>|<span data-ttu-id="1ab77-126">String</span><span class="sxs-lookup"><span data-stu-id="1ab77-126">String</span></span>| <span data-ttu-id="1ab77-127">自定义域证书的主题名称。</span><span class="sxs-lookup"><span data-stu-id="1ab77-127">The subject name of the custom domain certificate.</span></span> |
|<span data-ttu-id="1ab77-128">为</span><span class="sxs-lookup"><span data-stu-id="1ab77-128">thumbprint</span></span>|<span data-ttu-id="1ab77-129">String</span><span class="sxs-lookup"><span data-stu-id="1ab77-129">String</span></span>| <span data-ttu-id="1ab77-130">与自定义域证书关联的指纹。</span><span class="sxs-lookup"><span data-stu-id="1ab77-130">The thumbprint associated with the custom domain certificate.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1ab77-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1ab77-131">JSON representation</span></span>

<span data-ttu-id="1ab77-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1ab77-132">The following is a JSON representation of the resource.</span></span>

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