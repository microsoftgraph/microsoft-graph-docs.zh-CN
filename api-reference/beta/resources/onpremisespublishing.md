---
title: onPremisesPublishing 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9395a2d51628ed6ffc8ed0049f73595e2c98ba7a
ms.sourcegitcommit: ee41ba9ec6001716f1a9d575741bbeef577e2473
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/09/2020
ms.locfileid: "43200052"
---
# <a name="onpremisespublishing-resource-type"></a><span data-ttu-id="65c5e-103">onPremisesPublishing 资源类型</span><span class="sxs-lookup"><span data-stu-id="65c5e-103">onPremisesPublishing resource type</span></span>

<span data-ttu-id="65c5e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65c5e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65c5e-105">一个**onPremisesPublishing**对象，表示用于发布内部部署[应用程序](application.md)的属性集。</span><span class="sxs-lookup"><span data-stu-id="65c5e-105">An **onPremisesPublishing** object represents the set of properties for publishing of on-premises [application](application.md).</span></span>

## <a name="properties"></a><span data-ttu-id="65c5e-106">属性</span><span class="sxs-lookup"><span data-stu-id="65c5e-106">Properties</span></span>

| <span data-ttu-id="65c5e-107">属性</span><span class="sxs-lookup"><span data-stu-id="65c5e-107">Property</span></span>|<span data-ttu-id="65c5e-108">类型</span><span class="sxs-lookup"><span data-stu-id="65c5e-108">Type</span></span>|<span data-ttu-id="65c5e-109">说明</span><span class="sxs-lookup"><span data-stu-id="65c5e-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="65c5e-110">customDomainCertificate</span><span class="sxs-lookup"><span data-stu-id="65c5e-110">customDomainCertificate</span></span>|<span data-ttu-id="65c5e-111">字符串</span><span class="sxs-lookup"><span data-stu-id="65c5e-111">String</span></span>|<span data-ttu-id="65c5e-112">使用自定义域时与应用程序关联的证书的详细信息。</span><span class="sxs-lookup"><span data-stu-id="65c5e-112">Details of the certificate associated with the applicaiton when a custom domain is in use.</span></span> <span data-ttu-id="65c5e-113">使用默认域时为 Null。</span><span class="sxs-lookup"><span data-stu-id="65c5e-113">Null when using the default domain.</span></span>|
|<span data-ttu-id="65c5e-114">externalAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="65c5e-114">externalAuthenticationType</span></span>|<span data-ttu-id="65c5e-115">字符串</span><span class="sxs-lookup"><span data-stu-id="65c5e-115">String</span></span>|<span data-ttu-id="65c5e-116">详细说明应用程序的预身份验证设置可能的值为`passthru`： `aadPreAuthentication`、。</span><span class="sxs-lookup"><span data-stu-id="65c5e-116">Details the pre-authentication setting for the application Possible values are: `passthru`, `aadPreAuthentication`.</span></span>|
|<span data-ttu-id="65c5e-117">externalUrl</span><span class="sxs-lookup"><span data-stu-id="65c5e-117">externalUrl</span></span>|<span data-ttu-id="65c5e-118">字符串</span><span class="sxs-lookup"><span data-stu-id="65c5e-118">String</span></span>|<span data-ttu-id="65c5e-119">应用程序的已发布外部 url。</span><span class="sxs-lookup"><span data-stu-id="65c5e-119">The published external url for the application.</span></span> <span data-ttu-id="65c5e-120">例如https://intranet-contoso.msappproxy.net/</span><span class="sxs-lookup"><span data-stu-id="65c5e-120">For example https://intranet-contoso.msappproxy.net/</span></span>  |
|<span data-ttu-id="65c5e-121">internalUrl</span><span class="sxs-lookup"><span data-stu-id="65c5e-121">internalUrl</span></span>|<span data-ttu-id="65c5e-122">字符串</span><span class="sxs-lookup"><span data-stu-id="65c5e-122">String</span></span>|<span data-ttu-id="65c5e-123">应用程序的内部 url。</span><span class="sxs-lookup"><span data-stu-id="65c5e-123">The internal url of the application.</span></span> <span data-ttu-id="65c5e-124">例如https://intranet/</span><span class="sxs-lookup"><span data-stu-id="65c5e-124">For example https://intranet/</span></span> |
|<span data-ttu-id="65c5e-125">isOnPremPublishingEnabled</span><span class="sxs-lookup"><span data-stu-id="65c5e-125">isOnPremPublishingEnabled</span></span>|<span data-ttu-id="65c5e-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="65c5e-126">Boolean</span></span>|<span data-ttu-id="65c5e-127">指示应用程序当前是否正在发布。</span><span class="sxs-lookup"><span data-stu-id="65c5e-127">Indicates if the application is currently being published or not.</span></span>|
|<span data-ttu-id="65c5e-128">applicationServerTimeout</span><span class="sxs-lookup"><span data-stu-id="65c5e-128">applicationServerTimeout</span></span>|<span data-ttu-id="65c5e-129">字符串</span><span class="sxs-lookup"><span data-stu-id="65c5e-129">String</span></span>|<span data-ttu-id="65c5e-130">在关闭连接之前，连接器将等待后端应用程序响应的持续时间。</span><span class="sxs-lookup"><span data-stu-id="65c5e-130">The duration the connector will wait for a response from the backend application before closing the connection.</span></span> <span data-ttu-id="65c5e-131">可能的值`default`为`long`。</span><span class="sxs-lookup"><span data-stu-id="65c5e-131">Possible values are `default`, `long`.</span></span> <span data-ttu-id="65c5e-132">如果`long`服务器要响应请求的时间超过60-75 秒，请使用。</span><span class="sxs-lookup"><span data-stu-id="65c5e-132">Use `long` if your server takes more than 60-75 seconds to respond to requests.</span></span> <span data-ttu-id="65c5e-133">此外， `long`如果您无法访问应用程序，并且错误状态为 "后端超时"，也会尝试。</span><span class="sxs-lookup"><span data-stu-id="65c5e-133">Also try `long` if you are unable to access the application and the error status is "Backend Timeout".</span></span>|
|<span data-ttu-id="65c5e-134">isTranslateHostHeaderEnabled</span><span class="sxs-lookup"><span data-stu-id="65c5e-134">isTranslateHostHeaderEnabled</span></span>|<span data-ttu-id="65c5e-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="65c5e-135">Boolean</span></span>|<span data-ttu-id="65c5e-136">指示应用程序是否应转换响应标头中的 url。</span><span class="sxs-lookup"><span data-stu-id="65c5e-136">Indicates if the application should translate urls in the reponse headers.</span></span> <span data-ttu-id="65c5e-137">这包括为 cookie 设置正确的网站。</span><span class="sxs-lookup"><span data-stu-id="65c5e-137">This includes setting the correct site for cookies.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="65c5e-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="65c5e-138">JSON representation</span></span>

<span data-ttu-id="65c5e-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="65c5e-139">Here is a JSON representation of the resource.</span></span>

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
2019-02-04 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onPremisesPublishing resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
