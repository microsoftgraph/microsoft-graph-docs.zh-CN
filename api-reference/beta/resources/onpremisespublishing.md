---
title: onPremisesPublishing 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: 8531a68ad56dad0f44ef8cd55e9fabeff47a6c2e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341786"
---
# <a name="onpremisespublishing-resource-type"></a><span data-ttu-id="a1325-103">onPremisesPublishing 资源类型</span><span class="sxs-lookup"><span data-stu-id="a1325-103">onPremisesPublishing resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="a1325-104">属性</span><span class="sxs-lookup"><span data-stu-id="a1325-104">Properties</span></span>
| <span data-ttu-id="a1325-105">属性</span><span class="sxs-lookup"><span data-stu-id="a1325-105">Property</span></span>     | <span data-ttu-id="a1325-106">类型</span><span class="sxs-lookup"><span data-stu-id="a1325-106">Type</span></span>   |<span data-ttu-id="a1325-107">说明</span><span class="sxs-lookup"><span data-stu-id="a1325-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a1325-108">customDomainCertificate</span><span class="sxs-lookup"><span data-stu-id="a1325-108">customDomainCertificate</span></span>|<span data-ttu-id="a1325-109">String</span><span class="sxs-lookup"><span data-stu-id="a1325-109">String</span></span>|<span data-ttu-id="a1325-110">使用自定义域时与应用程序关联的证书的详细信息。</span><span class="sxs-lookup"><span data-stu-id="a1325-110">Details of the certificate associated with the applicaiton when a custom domain is in use.</span></span> <span data-ttu-id="a1325-111">使用默认域时为 Null。</span><span class="sxs-lookup"><span data-stu-id="a1325-111">Null when using the default domain.</span></span>|
|<span data-ttu-id="a1325-112">externalAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="a1325-112">externalAuthenticationType</span></span>|<span data-ttu-id="a1325-113">String</span><span class="sxs-lookup"><span data-stu-id="a1325-113">String</span></span>|<span data-ttu-id="a1325-114">详细说明应用程序的预身份验证设置可能的值为`passthru`: `aadPreAuthentication`、。</span><span class="sxs-lookup"><span data-stu-id="a1325-114">Details the pre-authentication setting for the application Possible values are: `passthru`, `aadPreAuthentication`.</span></span>|
|<span data-ttu-id="a1325-115">externalUrl</span><span class="sxs-lookup"><span data-stu-id="a1325-115">externalUrl</span></span>|<span data-ttu-id="a1325-116">String</span><span class="sxs-lookup"><span data-stu-id="a1325-116">String</span></span>|<span data-ttu-id="a1325-117">应用程序的已发布外部 url。</span><span class="sxs-lookup"><span data-stu-id="a1325-117">The published external url for the application.</span></span> <span data-ttu-id="a1325-118">例如https://intranet-contoso.msappproxy.net/</span><span class="sxs-lookup"><span data-stu-id="a1325-118">For example https://intranet-contoso.msappproxy.net/</span></span>  |
|<span data-ttu-id="a1325-119">internalUrl</span><span class="sxs-lookup"><span data-stu-id="a1325-119">internalUrl</span></span>|<span data-ttu-id="a1325-120">String</span><span class="sxs-lookup"><span data-stu-id="a1325-120">String</span></span>|<span data-ttu-id="a1325-121">应用程序的内部 url。</span><span class="sxs-lookup"><span data-stu-id="a1325-121">The internal url of the application.</span></span> <span data-ttu-id="a1325-122">例如https://intranet/</span><span class="sxs-lookup"><span data-stu-id="a1325-122">For example https://intranet/</span></span> |
|<span data-ttu-id="a1325-123">isOnPremPublishingEnabled</span><span class="sxs-lookup"><span data-stu-id="a1325-123">isOnPremPublishingEnabled</span></span>|<span data-ttu-id="a1325-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1325-124">Boolean</span></span>|<span data-ttu-id="a1325-125">指示应用程序当前是否正在发布。</span><span class="sxs-lookup"><span data-stu-id="a1325-125">Indicates if the application is currently being published or not.</span></span>|
|<span data-ttu-id="a1325-126">applicationServerTimeout</span><span class="sxs-lookup"><span data-stu-id="a1325-126">applicationServerTimeout</span></span>|<span data-ttu-id="a1325-127">String</span><span class="sxs-lookup"><span data-stu-id="a1325-127">String</span></span>|<span data-ttu-id="a1325-128">在关闭连接之前, 连接器将等待后端应用程序响应的持续时间。</span><span class="sxs-lookup"><span data-stu-id="a1325-128">The duration the connector will wait for a response from the backend application before closing the connection.</span></span> <span data-ttu-id="a1325-129">可能的值`default`为`long`。</span><span class="sxs-lookup"><span data-stu-id="a1325-129">Possible values are `default`, `long`.</span></span> <span data-ttu-id="a1325-130">如果`long`服务器要响应请求的时间超过60-75 秒, 请使用。</span><span class="sxs-lookup"><span data-stu-id="a1325-130">Use `long` if your server takes more than 60-75 seconds to respond to requests.</span></span> <span data-ttu-id="a1325-131">此外, `long`如果您无法访问应用程序, 并且错误状态为 "后端超时", 也会尝试。</span><span class="sxs-lookup"><span data-stu-id="a1325-131">Also try `long` if you are unable to access the application and the error status is "Backend Timeout".</span></span>|
|<span data-ttu-id="a1325-132">isTranslateHostHeaderEnabled</span><span class="sxs-lookup"><span data-stu-id="a1325-132">isTranslateHostHeaderEnabled</span></span>|<span data-ttu-id="a1325-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1325-133">Boolean</span></span>|<span data-ttu-id="a1325-134">指示应用程序是否应转换响应标头中的 url。</span><span class="sxs-lookup"><span data-stu-id="a1325-134">Indicates if the application should translate urls in the reponse headers.</span></span> <span data-ttu-id="a1325-135">这包括为 cookie 设置正确的网站。</span><span class="sxs-lookup"><span data-stu-id="a1325-135">This includes setting the correct site for cookies.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a1325-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a1325-136">JSON representation</span></span>

<span data-ttu-id="a1325-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a1325-137">Here is a JSON representation of the resource.</span></span>

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
