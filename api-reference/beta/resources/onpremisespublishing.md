---
title: onPremisesPublishing 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d1ee3b9cd98ae61bd6322ee49fede6310f78815a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966373"
---
# <a name="onpremisespublishing-resource-type"></a><span data-ttu-id="20d8a-103">onPremisesPublishing 资源类型</span><span class="sxs-lookup"><span data-stu-id="20d8a-103">onPremisesPublishing resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20d8a-104">一个**onPremisesPublishing**对象, 表示用于发布内部部署[应用程序](application.md)的属性集。</span><span class="sxs-lookup"><span data-stu-id="20d8a-104">An **onPremisesPublishing** object represents the set of properties for publishing of on-premises [application](application.md).</span></span>

## <a name="properties"></a><span data-ttu-id="20d8a-105">属性</span><span class="sxs-lookup"><span data-stu-id="20d8a-105">Properties</span></span>

| <span data-ttu-id="20d8a-106">属性</span><span class="sxs-lookup"><span data-stu-id="20d8a-106">Property</span></span>|<span data-ttu-id="20d8a-107">类型</span><span class="sxs-lookup"><span data-stu-id="20d8a-107">Type</span></span>|<span data-ttu-id="20d8a-108">说明</span><span class="sxs-lookup"><span data-stu-id="20d8a-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="20d8a-109">customDomainCertificate</span><span class="sxs-lookup"><span data-stu-id="20d8a-109">customDomainCertificate</span></span>|<span data-ttu-id="20d8a-110">String</span><span class="sxs-lookup"><span data-stu-id="20d8a-110">String</span></span>|<span data-ttu-id="20d8a-111">使用自定义域时与应用程序关联的证书的详细信息。</span><span class="sxs-lookup"><span data-stu-id="20d8a-111">Details of the certificate associated with the applicaiton when a custom domain is in use.</span></span> <span data-ttu-id="20d8a-112">使用默认域时为 Null。</span><span class="sxs-lookup"><span data-stu-id="20d8a-112">Null when using the default domain.</span></span>|
|<span data-ttu-id="20d8a-113">externalAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="20d8a-113">externalAuthenticationType</span></span>|<span data-ttu-id="20d8a-114">String</span><span class="sxs-lookup"><span data-stu-id="20d8a-114">String</span></span>|<span data-ttu-id="20d8a-115">详细说明应用程序的预身份验证设置可能的值为`passthru`: `aadPreAuthentication`、。</span><span class="sxs-lookup"><span data-stu-id="20d8a-115">Details the pre-authentication setting for the application Possible values are: `passthru`, `aadPreAuthentication`.</span></span>|
|<span data-ttu-id="20d8a-116">externalUrl</span><span class="sxs-lookup"><span data-stu-id="20d8a-116">externalUrl</span></span>|<span data-ttu-id="20d8a-117">String</span><span class="sxs-lookup"><span data-stu-id="20d8a-117">String</span></span>|<span data-ttu-id="20d8a-118">应用程序的已发布外部 url。</span><span class="sxs-lookup"><span data-stu-id="20d8a-118">The published external url for the application.</span></span> <span data-ttu-id="20d8a-119">例如https://intranet-contoso.msappproxy.net/</span><span class="sxs-lookup"><span data-stu-id="20d8a-119">For example https://intranet-contoso.msappproxy.net/</span></span>  |
|<span data-ttu-id="20d8a-120">internalUrl</span><span class="sxs-lookup"><span data-stu-id="20d8a-120">internalUrl</span></span>|<span data-ttu-id="20d8a-121">String</span><span class="sxs-lookup"><span data-stu-id="20d8a-121">String</span></span>|<span data-ttu-id="20d8a-122">应用程序的内部 url。</span><span class="sxs-lookup"><span data-stu-id="20d8a-122">The internal url of the application.</span></span> <span data-ttu-id="20d8a-123">例如https://intranet/</span><span class="sxs-lookup"><span data-stu-id="20d8a-123">For example https://intranet/</span></span> |
|<span data-ttu-id="20d8a-124">isOnPremPublishingEnabled</span><span class="sxs-lookup"><span data-stu-id="20d8a-124">isOnPremPublishingEnabled</span></span>|<span data-ttu-id="20d8a-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="20d8a-125">Boolean</span></span>|<span data-ttu-id="20d8a-126">指示应用程序当前是否正在发布。</span><span class="sxs-lookup"><span data-stu-id="20d8a-126">Indicates if the application is currently being published or not.</span></span>|
|<span data-ttu-id="20d8a-127">applicationServerTimeout</span><span class="sxs-lookup"><span data-stu-id="20d8a-127">applicationServerTimeout</span></span>|<span data-ttu-id="20d8a-128">String</span><span class="sxs-lookup"><span data-stu-id="20d8a-128">String</span></span>|<span data-ttu-id="20d8a-129">在关闭连接之前, 连接器将等待后端应用程序响应的持续时间。</span><span class="sxs-lookup"><span data-stu-id="20d8a-129">The duration the connector will wait for a response from the backend application before closing the connection.</span></span> <span data-ttu-id="20d8a-130">可能的值`default`为`long`。</span><span class="sxs-lookup"><span data-stu-id="20d8a-130">Possible values are `default`, `long`.</span></span> <span data-ttu-id="20d8a-131">如果`long`服务器要响应请求的时间超过60-75 秒, 请使用。</span><span class="sxs-lookup"><span data-stu-id="20d8a-131">Use `long` if your server takes more than 60-75 seconds to respond to requests.</span></span> <span data-ttu-id="20d8a-132">此外, `long`如果您无法访问应用程序, 并且错误状态为 "后端超时", 也会尝试。</span><span class="sxs-lookup"><span data-stu-id="20d8a-132">Also try `long` if you are unable to access the application and the error status is "Backend Timeout".</span></span>|
|<span data-ttu-id="20d8a-133">isTranslateHostHeaderEnabled</span><span class="sxs-lookup"><span data-stu-id="20d8a-133">isTranslateHostHeaderEnabled</span></span>|<span data-ttu-id="20d8a-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="20d8a-134">Boolean</span></span>|<span data-ttu-id="20d8a-135">指示应用程序是否应转换响应标头中的 url。</span><span class="sxs-lookup"><span data-stu-id="20d8a-135">Indicates if the application should translate urls in the reponse headers.</span></span> <span data-ttu-id="20d8a-136">这包括为 cookie 设置正确的网站。</span><span class="sxs-lookup"><span data-stu-id="20d8a-136">This includes setting the correct site for cookies.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="20d8a-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="20d8a-137">JSON representation</span></span>

<span data-ttu-id="20d8a-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="20d8a-138">Here is a JSON representation of the resource.</span></span>

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
