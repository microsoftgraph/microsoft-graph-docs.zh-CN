---
title: onPremisesPublishing 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: fd216d52ba212e739f1d7c087a99a4379682010e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508179"
---
# <a name="onpremisespublishing-resource-type"></a><span data-ttu-id="b4cfa-103">onPremisesPublishing 资源类型</span><span class="sxs-lookup"><span data-stu-id="b4cfa-103">onPremisesPublishing resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="b4cfa-104">属性</span><span class="sxs-lookup"><span data-stu-id="b4cfa-104">Properties</span></span>
| <span data-ttu-id="b4cfa-105">属性</span><span class="sxs-lookup"><span data-stu-id="b4cfa-105">Property</span></span>     | <span data-ttu-id="b4cfa-106">类型</span><span class="sxs-lookup"><span data-stu-id="b4cfa-106">Type</span></span>   |<span data-ttu-id="b4cfa-107">说明</span><span class="sxs-lookup"><span data-stu-id="b4cfa-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b4cfa-108">customDomainCertificate</span><span class="sxs-lookup"><span data-stu-id="b4cfa-108">customDomainCertificate</span></span>|<span data-ttu-id="b4cfa-109">String</span><span class="sxs-lookup"><span data-stu-id="b4cfa-109">String</span></span>|<span data-ttu-id="b4cfa-110">当正在使用中的自定义域名与应用程序关联的证书的详细信息。</span><span class="sxs-lookup"><span data-stu-id="b4cfa-110">Details of the certificate associated with the applicaiton when a custom domain is in use.</span></span> <span data-ttu-id="b4cfa-111">为空时使用的默认域。</span><span class="sxs-lookup"><span data-stu-id="b4cfa-111">Null when using the default domain.</span></span>|
|<span data-ttu-id="b4cfa-112">externalAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="b4cfa-112">externalAuthenticationType</span></span>|<span data-ttu-id="b4cfa-113">String</span><span class="sxs-lookup"><span data-stu-id="b4cfa-113">String</span></span>|<span data-ttu-id="b4cfa-114">详细预身份验证设置的应用程序可能的值为： `passthru`， `aadPreAuthentication`。</span><span class="sxs-lookup"><span data-stu-id="b4cfa-114">Details the pre-authentication setting for the application Possible values are: `passthru`, `aadPreAuthentication`.</span></span>|
|<span data-ttu-id="b4cfa-115">externalUrl</span><span class="sxs-lookup"><span data-stu-id="b4cfa-115">externalUrl</span></span>|<span data-ttu-id="b4cfa-116">String</span><span class="sxs-lookup"><span data-stu-id="b4cfa-116">String</span></span>|<span data-ttu-id="b4cfa-117">应用程序的已发布外部 url。</span><span class="sxs-lookup"><span data-stu-id="b4cfa-117">The published external url for the application.</span></span> <span data-ttu-id="b4cfa-118">例如：</span><span class="sxs-lookup"><span data-stu-id="b4cfa-118">For example https://intranet-contoso.msappproxy.net/</span></span>  |
|<span data-ttu-id="b4cfa-119">internalUrl</span><span class="sxs-lookup"><span data-stu-id="b4cfa-119">internalUrl</span></span>|<span data-ttu-id="b4cfa-120">String</span><span class="sxs-lookup"><span data-stu-id="b4cfa-120">String</span></span>|<span data-ttu-id="b4cfa-121">应用程序的内部 url。</span><span class="sxs-lookup"><span data-stu-id="b4cfa-121">The internal url of the application.</span></span> <span data-ttu-id="b4cfa-122">例如：</span><span class="sxs-lookup"><span data-stu-id="b4cfa-122">For example https://intranet/</span></span> |
|<span data-ttu-id="b4cfa-123">isOnPremPublishingEnabled</span><span class="sxs-lookup"><span data-stu-id="b4cfa-123">isOnPremPublishingEnabled</span></span>|<span data-ttu-id="b4cfa-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4cfa-124">Boolean</span></span>|<span data-ttu-id="b4cfa-125">指示是否或不当前正在发布应用程序。</span><span class="sxs-lookup"><span data-stu-id="b4cfa-125">Indicates if the application is currently being published or not.</span></span>|
|<span data-ttu-id="b4cfa-126">applicationServerTimeout</span><span class="sxs-lookup"><span data-stu-id="b4cfa-126">applicationServerTimeout</span></span>|<span data-ttu-id="b4cfa-127">String</span><span class="sxs-lookup"><span data-stu-id="b4cfa-127">String</span></span>|<span data-ttu-id="b4cfa-128">连接器将等待响应之前关闭该连接的后端应用程序持续时间。</span><span class="sxs-lookup"><span data-stu-id="b4cfa-128">The duration the connector will wait for a response from the backend application before closing the connection.</span></span> <span data-ttu-id="b4cfa-129">可取值为：`default`、`long`。</span><span class="sxs-lookup"><span data-stu-id="b4cfa-129">Possible values are `default`, `long`.</span></span> <span data-ttu-id="b4cfa-130">使用`long`如果您的服务器所需超过 60 75 秒来响应请求。</span><span class="sxs-lookup"><span data-stu-id="b4cfa-130">Use `long` if your server takes more than 60-75 seconds to respond to requests.</span></span> <span data-ttu-id="b4cfa-131">此外尝试`long`如果您不能访问应用程序，并且错误状态为"后端超时"。</span><span class="sxs-lookup"><span data-stu-id="b4cfa-131">Also try `long` if you are unable to access the application and the error status is "Backend Timeout".</span></span>|
|<span data-ttu-id="b4cfa-132">isTranslateHostHeaderEnabled</span><span class="sxs-lookup"><span data-stu-id="b4cfa-132">isTranslateHostHeaderEnabled</span></span>|<span data-ttu-id="b4cfa-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4cfa-133">Boolean</span></span>|<span data-ttu-id="b4cfa-134">指示应用程序应翻译响应头中的 url。</span><span class="sxs-lookup"><span data-stu-id="b4cfa-134">Indicates if the application should translate urls in the reponse headers.</span></span> <span data-ttu-id="b4cfa-135">这包括设置正确的站点的 cookie。</span><span class="sxs-lookup"><span data-stu-id="b4cfa-135">This includes setting the correct site for cookies.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b4cfa-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b4cfa-136">JSON representation</span></span>

<span data-ttu-id="b4cfa-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b4cfa-137">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/onpremisespublishing.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
