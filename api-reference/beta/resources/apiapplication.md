---
title: apiApplication 资源类型
description: 指定 Web API 应用程序的设置。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 85e9c5f62182b1dd7666117c6fcf42743ccc1e8e
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939157"
---
# <a name="apiapplication-resource-type"></a><span data-ttu-id="326e3-103">apiApplication 资源类型</span><span class="sxs-lookup"><span data-stu-id="326e3-103">apiApplication resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="326e3-104">指定实现 web API 的应用程序的设置。</span><span class="sxs-lookup"><span data-stu-id="326e3-104">Specifies settings for an application that implements a web API.</span></span>

## <a name="properties"></a><span data-ttu-id="326e3-105">属性</span><span class="sxs-lookup"><span data-stu-id="326e3-105">Properties</span></span>

| <span data-ttu-id="326e3-106">属性</span><span class="sxs-lookup"><span data-stu-id="326e3-106">Property</span></span> | <span data-ttu-id="326e3-107">类型</span><span class="sxs-lookup"><span data-stu-id="326e3-107">Type</span></span> | <span data-ttu-id="326e3-108">说明</span><span class="sxs-lookup"><span data-stu-id="326e3-108">Description</span></span> |
|:---------------|:--------|:----------|
|`acceptMappedClaims`| <span data-ttu-id="326e3-109">Boolean</span><span class="sxs-lookup"><span data-stu-id="326e3-109">Boolean</span></span> | <span data-ttu-id="326e3-110">如果为 true，则允许应用程序在未指定自定义签名密钥的情况下使用声明映射。</span><span class="sxs-lookup"><span data-stu-id="326e3-110">When true, allows an application to use claims mapping without specifying a custom signing key.</span></span> |
|`knownClientApplications`| <span data-ttu-id="326e3-111">Guid 集合</span><span class="sxs-lookup"><span data-stu-id="326e3-111">Guid collection</span></span> |<span data-ttu-id="326e3-112">如果您有一个包含两部分的解决方案，则可用于捆绑许可：客户端应用程序和自定义 web API 应用程序。</span><span class="sxs-lookup"><span data-stu-id="326e3-112">Used for bundling consent if you have a solution that contains two parts: a client app and a custom web API app.</span></span> <span data-ttu-id="326e3-113">如果将客户端应用程序的 appID 设置为此值，则用户仅对客户端应用程序同意一次。</span><span class="sxs-lookup"><span data-stu-id="326e3-113">If you set the appID of the client app to this value, the user only consents once to the client app.</span></span> <span data-ttu-id="326e3-114">Azure AD 知道，同意客户端表示隐式同意 web API 并同时自动为这两个 Api 设置服务主体。</span><span class="sxs-lookup"><span data-stu-id="326e3-114">Azure AD knows that consenting to the client means implicitly consenting to the web API and automatically provisions service principals for both APIs at the same time.</span></span> <span data-ttu-id="326e3-115">客户端和 web API 应用都必须在同一个租户中注册。</span><span class="sxs-lookup"><span data-stu-id="326e3-115">Both the client and the web API app must be registered in the same tenant.</span></span>|
|`oauth2PermissionScopes`| <span data-ttu-id="326e3-116">[permissionScope](permissionscope.md)集合</span><span class="sxs-lookup"><span data-stu-id="326e3-116">[permissionScope](permissionscope.md) collection</span></span> | <span data-ttu-id="326e3-117">Web API （资源）应用程序向客户端应用程序公开的 OAuth 2.0 权限范围的集合。</span><span class="sxs-lookup"><span data-stu-id="326e3-117">The collection of OAuth 2.0 permission scopes that the web API (resource) application exposes to client applications.</span></span> <span data-ttu-id="326e3-118">在同意期间，可以向客户端应用程序授予这些权限范围。</span><span class="sxs-lookup"><span data-stu-id="326e3-118">These permission scopes may be granted to client applications during consent.</span></span> |
|`preAuthorizedApplications`| <span data-ttu-id="326e3-119">[preAuthorizedApplication](preauthorizedapplication.md)集合</span><span class="sxs-lookup"><span data-stu-id="326e3-119">[preAuthorizedApplication](preauthorizedapplication.md) collection</span></span> | <span data-ttu-id="326e3-120">列出使用指定委派权限预授权的客户端应用程序，以访问此应用程序的 Api。</span><span class="sxs-lookup"><span data-stu-id="326e3-120">Lists the client applications that are pre-authorized with the specified delegated permissions to access this application's APIs.</span></span> <span data-ttu-id="326e3-121">用户无需同意任何预先授权的应用程序（针对指定的权限）。</span><span class="sxs-lookup"><span data-stu-id="326e3-121">Users are not required to consent to any pre-authorized application (for the permissions specified).</span></span> <span data-ttu-id="326e3-122">但是，preAuthorizedApplications 中未列出的任何其他权限（例如，通过增量许可请求）将需要用户同意。</span><span class="sxs-lookup"><span data-stu-id="326e3-122">However, any additional permissions not listed in preAuthorizedApplications (requested through incremental consent for example) will require user consent.</span></span> |
|`requestedAccessTokenVersion`| <span data-ttu-id="326e3-123">Int32</span><span class="sxs-lookup"><span data-stu-id="326e3-123">Int32</span></span> | <span data-ttu-id="326e3-124">指定此资源所需的访问令牌版本。</span><span class="sxs-lookup"><span data-stu-id="326e3-124">Specifies the access token version expected by this resource.</span></span> <span data-ttu-id="326e3-125">这会更改与终结点或客户端（用于请求访问令牌）独立生成的 JWT 的版本和格式。</span><span class="sxs-lookup"><span data-stu-id="326e3-125">This changes the version and format of the JWT produced independent of the endpoint or client used to request the access token.</span></span> <br><br> <span data-ttu-id="326e3-126">使用的终结点为 v1.0 或 v2.0，由客户端选择，仅影响 id_tokens 的版本。</span><span class="sxs-lookup"><span data-stu-id="326e3-126">The endpoint used, v1.0 or v2.0, is chosen by the client and only impacts the version of id_tokens.</span></span> <span data-ttu-id="326e3-127">资源需要显式配置`requestedAccessTokenVersion` ，以指示支持的访问令牌格式。</span><span class="sxs-lookup"><span data-stu-id="326e3-127">Resources need to explicitly configure `requestedAccessTokenVersion` to indicate the supported access token format.</span></span> <br><br> <span data-ttu-id="326e3-128">的可能值`requestedAccessTokenVersion`为`1`、 `2`或`null`。</span><span class="sxs-lookup"><span data-stu-id="326e3-128">Possible values for `requestedAccessTokenVersion` are `1`, `2`, or `null`.</span></span> <span data-ttu-id="326e3-129">如果值为`null`，则默认为`1`，它对应于1.0 版终结点。</span><span class="sxs-lookup"><span data-stu-id="326e3-129">If the value is `null`, this defaults to `1`, which corresponds to the v1.0 endpoint.</span></span> <br><br> <span data-ttu-id="326e3-130">如果`signInAudience`将应用程序配置为`AzureADandPersonalMicrosoftAccount`，则此属性的值必须为`2`</span><span class="sxs-lookup"><span data-stu-id="326e3-130">If `signInAudience` on the application is configured as `AzureADandPersonalMicrosoftAccount`, the value for this property must be `2`</span></span> |

## <a name="json-representation"></a><span data-ttu-id="326e3-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="326e3-131">JSON representation</span></span>
<span data-ttu-id="326e3-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="326e3-132">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.apiApplication"
}-->

```json
{
  "acceptMappedClaims": true,
  "knownClientApplications": ["Guid"],
  "oauth2PermissionScopes": [{"@odata.type": "microsoft.graph.permissionScope"}],
  "preAuthorizedApplications": [{"@odata.type": "microsoft.graph.preAuthorizedApplication"}],
  "requestedAccessTokenVersion": 2
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "api resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
