---
title: onPremisesPublishing 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: 8dba505347fc12d3c4a8521ebe32551d738dc4a2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045356"
---
# <a name="onpremisespublishing-resource-type"></a><span data-ttu-id="bdedf-103">onPremisesPublishing 资源类型</span><span class="sxs-lookup"><span data-stu-id="bdedf-103">onPremisesPublishing resource type</span></span>

> <span data-ttu-id="bdedf-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="bdedf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bdedf-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bdedf-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="properties"></a><span data-ttu-id="bdedf-106">属性</span><span class="sxs-lookup"><span data-stu-id="bdedf-106">Properties</span></span>
| <span data-ttu-id="bdedf-107">属性</span><span class="sxs-lookup"><span data-stu-id="bdedf-107">Property</span></span>     | <span data-ttu-id="bdedf-108">类型</span><span class="sxs-lookup"><span data-stu-id="bdedf-108">Type</span></span>   |<span data-ttu-id="bdedf-109">说明</span><span class="sxs-lookup"><span data-stu-id="bdedf-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bdedf-110">customDomainCertificate</span><span class="sxs-lookup"><span data-stu-id="bdedf-110">customDomainCertificate</span></span>|<span data-ttu-id="bdedf-111">字符串</span><span class="sxs-lookup"><span data-stu-id="bdedf-111">String</span></span>|<span data-ttu-id="bdedf-112">当正在使用中的自定义域名与应用程序关联的证书的详细信息。</span><span class="sxs-lookup"><span data-stu-id="bdedf-112">Details of the certificate associated with the applicaiton when a custom domain is in use.</span></span> <span data-ttu-id="bdedf-113">为空时使用的默认域。</span><span class="sxs-lookup"><span data-stu-id="bdedf-113">Null when using the default domain.</span></span>|
|<span data-ttu-id="bdedf-114">externalAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="bdedf-114">externalAuthenticationType</span></span>|<span data-ttu-id="bdedf-115">字符串</span><span class="sxs-lookup"><span data-stu-id="bdedf-115">String</span></span>|<span data-ttu-id="bdedf-116">详细预身份验证设置的应用程序可能的值为： `passthru`， `aadPreAuthentication`。</span><span class="sxs-lookup"><span data-stu-id="bdedf-116">Details the pre-authentication setting for the application Possible values are: `passthru`, `aadPreAuthentication`.</span></span>|
|<span data-ttu-id="bdedf-117">externalUrl</span><span class="sxs-lookup"><span data-stu-id="bdedf-117">externalUrl</span></span>|<span data-ttu-id="bdedf-118">字符串</span><span class="sxs-lookup"><span data-stu-id="bdedf-118">String</span></span>|<span data-ttu-id="bdedf-119">应用程序的已发布外部 url。</span><span class="sxs-lookup"><span data-stu-id="bdedf-119">The published external url for the application.</span></span> <span data-ttu-id="bdedf-120">例如https://intranet-contoso.msappproxy.net/</span><span class="sxs-lookup"><span data-stu-id="bdedf-120">For example https://intranet-contoso.msappproxy.net/</span></span>  |
|<span data-ttu-id="bdedf-121">internalUrl</span><span class="sxs-lookup"><span data-stu-id="bdedf-121">internalUrl</span></span>|<span data-ttu-id="bdedf-122">字符串</span><span class="sxs-lookup"><span data-stu-id="bdedf-122">String</span></span>|<span data-ttu-id="bdedf-123">应用程序的内部 url。</span><span class="sxs-lookup"><span data-stu-id="bdedf-123">The internal url of the application.</span></span> <span data-ttu-id="bdedf-124">例如https://intranet/</span><span class="sxs-lookup"><span data-stu-id="bdedf-124">For example https://intranet/</span></span> |
|<span data-ttu-id="bdedf-125">isOnPremPublishingEnabled</span><span class="sxs-lookup"><span data-stu-id="bdedf-125">isOnPremPublishingEnabled</span></span>|<span data-ttu-id="bdedf-126">布尔</span><span class="sxs-lookup"><span data-stu-id="bdedf-126">Boolean</span></span>|<span data-ttu-id="bdedf-127">指示是否或不当前正在发布应用程序。</span><span class="sxs-lookup"><span data-stu-id="bdedf-127">Indicates if the application is currently being published or not.</span></span>|
|<span data-ttu-id="bdedf-128">applicationServerTimeout</span><span class="sxs-lookup"><span data-stu-id="bdedf-128">applicationServerTimeout</span></span>|<span data-ttu-id="bdedf-129">字符串</span><span class="sxs-lookup"><span data-stu-id="bdedf-129">String</span></span>|<span data-ttu-id="bdedf-130">连接器将等待响应之前关闭该连接的后端应用程序持续时间。</span><span class="sxs-lookup"><span data-stu-id="bdedf-130">The duration the connector will wait for a response from the backend application before closing the connection.</span></span> <span data-ttu-id="bdedf-131">可能的值为`default`， `long`。</span><span class="sxs-lookup"><span data-stu-id="bdedf-131">Possible values are `default`, `long`.</span></span> <span data-ttu-id="bdedf-132">使用`long`如果您的服务器所需超过 60 75 秒来响应请求。</span><span class="sxs-lookup"><span data-stu-id="bdedf-132">Use `long` if your server takes more than 60-75 seconds to respond to requests.</span></span> <span data-ttu-id="bdedf-133">此外尝试`long`如果您不能访问应用程序，并且错误状态为"后端超时"。</span><span class="sxs-lookup"><span data-stu-id="bdedf-133">Also try `long` if you are unable to access the application and the error status is "Backend Timeout".</span></span>|
|<span data-ttu-id="bdedf-134">isTranslateHostHeaderEnabled</span><span class="sxs-lookup"><span data-stu-id="bdedf-134">isTranslateHostHeaderEnabled</span></span>|<span data-ttu-id="bdedf-135">布尔</span><span class="sxs-lookup"><span data-stu-id="bdedf-135">Boolean</span></span>|<span data-ttu-id="bdedf-136">指示应用程序应翻译响应头中的 url。</span><span class="sxs-lookup"><span data-stu-id="bdedf-136">Indicates if the application should translate urls in the reponse headers.</span></span> <span data-ttu-id="bdedf-137">这包括设置正确的站点的 cookie。</span><span class="sxs-lookup"><span data-stu-id="bdedf-137">This includes setting the correct site for cookies.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bdedf-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bdedf-138">JSON representation</span></span>

<span data-ttu-id="bdedf-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bdedf-139">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesPublishing"
}-->

```json
{
  "customDomainCertificate": "String",
  "externalAuthenticationType": "String",
  "externalUrl": "String",
  "internalUrl": "String",
  "isOnPremPublishingEnabled": true,
  "applicationServerTimeout": "String",
  "isTranslateHostHeaderEnabled": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesPublishing resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
