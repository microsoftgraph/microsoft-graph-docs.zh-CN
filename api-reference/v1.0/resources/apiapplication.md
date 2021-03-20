---
title: apiApplication 资源类型
description: 指定 Web API 应用程序的设置。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 1a01418fad74d48a1697bace91833d880a94f467
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955964"
---
# <a name="apiapplication-resource-type"></a><span data-ttu-id="a93bc-103">apiApplication 资源类型</span><span class="sxs-lookup"><span data-stu-id="a93bc-103">apiApplication resource type</span></span>

<span data-ttu-id="a93bc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a93bc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a93bc-105">指定实现 Web API 的应用程序的设置。</span><span class="sxs-lookup"><span data-stu-id="a93bc-105">Specifies settings for an application that implements a web API.</span></span>

## <a name="properties"></a><span data-ttu-id="a93bc-106">属性</span><span class="sxs-lookup"><span data-stu-id="a93bc-106">Properties</span></span>

| <span data-ttu-id="a93bc-107">属性</span><span class="sxs-lookup"><span data-stu-id="a93bc-107">Property</span></span> | <span data-ttu-id="a93bc-108">类型</span><span class="sxs-lookup"><span data-stu-id="a93bc-108">Type</span></span> | <span data-ttu-id="a93bc-109">说明</span><span class="sxs-lookup"><span data-stu-id="a93bc-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a93bc-110">acceptMappedClaims</span><span class="sxs-lookup"><span data-stu-id="a93bc-110">acceptMappedClaims</span></span>| <span data-ttu-id="a93bc-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="a93bc-111">Boolean</span></span> | <span data-ttu-id="a93bc-112">如果 `true` 为 ，则允许应用程序使用声明映射，而无需指定自定义签名密钥。</span><span class="sxs-lookup"><span data-stu-id="a93bc-112">When `true`, allows an application to use claims mapping without specifying a custom signing key.</span></span> |
|<span data-ttu-id="a93bc-113">knownClientApplications</span><span class="sxs-lookup"><span data-stu-id="a93bc-113">knownClientApplications</span></span>| <span data-ttu-id="a93bc-114">Guid 集合</span><span class="sxs-lookup"><span data-stu-id="a93bc-114">Guid collection</span></span> |<span data-ttu-id="a93bc-115">如果你的解决方案包含两个部分：客户端应用和自定义 Web API 应用，用于捆绑许可。</span><span class="sxs-lookup"><span data-stu-id="a93bc-115">Used for bundling consent if you have a solution that contains two parts: a client app and a custom web API app.</span></span> <span data-ttu-id="a93bc-116">如果将客户端应用的 appID 设置为此值，则用户仅同意客户端应用一次。</span><span class="sxs-lookup"><span data-stu-id="a93bc-116">If you set the appID of the client app to this value, the user only consents once to the client app.</span></span> <span data-ttu-id="a93bc-117">Azure AD 知道，同意客户端意味着隐式同意 Web API 并同时自动为两个 API 设置服务主体。</span><span class="sxs-lookup"><span data-stu-id="a93bc-117">Azure AD knows that consenting to the client means implicitly consenting to the web API and automatically provisions service principals for both APIs at the same time.</span></span> <span data-ttu-id="a93bc-118">客户端和 Web API 应用都必须在同一租户中注册。</span><span class="sxs-lookup"><span data-stu-id="a93bc-118">Both the client and the web API app must be registered in the same tenant.</span></span>|
|<span data-ttu-id="a93bc-119">oauth2PermissionScopes</span><span class="sxs-lookup"><span data-stu-id="a93bc-119">oauth2PermissionScopes</span></span>| <span data-ttu-id="a93bc-120">[permissionScope](permissionscope.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a93bc-120">[permissionScope](permissionscope.md) collection</span></span> | <span data-ttu-id="a93bc-121">由此应用程序注册表示的 Web API 公开的委派权限的定义。</span><span class="sxs-lookup"><span data-stu-id="a93bc-121">The definition of the delegated permissions exposed by the web API represented by this application registration.</span></span> <span data-ttu-id="a93bc-122">这些委派权限可能由客户端应用程序请求，并且可能由用户或管理员在同意期间授予。</span><span class="sxs-lookup"><span data-stu-id="a93bc-122">These delegated permissions may be requested by a client application, and may be granted by users or administrators during consent.</span></span> <span data-ttu-id="a93bc-123">委派的权限有时称为 OAuth 2.0 范围。</span><span class="sxs-lookup"><span data-stu-id="a93bc-123">Delegated permissions are sometimes referred to as OAuth 2.0 scopes.</span></span> |
|<span data-ttu-id="a93bc-124">preAuthorizedApplications</span><span class="sxs-lookup"><span data-stu-id="a93bc-124">preAuthorizedApplications</span></span>| <span data-ttu-id="a93bc-125">[preAuthorizedApplication](preauthorizedapplication.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a93bc-125">[preAuthorizedApplication](preauthorizedapplication.md) collection</span></span> | <span data-ttu-id="a93bc-126">列出使用指定委派权限预授权的客户端应用程序，以访问此应用程序的 API。</span><span class="sxs-lookup"><span data-stu-id="a93bc-126">Lists the client applications that are pre-authorized with the specified delegated permissions to access this application's APIs.</span></span> <span data-ttu-id="a93bc-127">对于用户指定的权限，用户无需同意任何 (应用程序) 。</span><span class="sxs-lookup"><span data-stu-id="a93bc-127">Users are not required to consent to any pre-authorized application (for the permissions specified).</span></span> <span data-ttu-id="a93bc-128">但是，未在预AuthorizedApplications中 (增量许可请求的其他权限（例如) ）将需要用户同意。</span><span class="sxs-lookup"><span data-stu-id="a93bc-128">However, any additional permissions not listed in preAuthorizedApplications (requested through incremental consent for example) will require user consent.</span></span> |
|<span data-ttu-id="a93bc-129">requestedAccessTokenVersion</span><span class="sxs-lookup"><span data-stu-id="a93bc-129">requestedAccessTokenVersion</span></span>| <span data-ttu-id="a93bc-130">Int32</span><span class="sxs-lookup"><span data-stu-id="a93bc-130">Int32</span></span> | <span data-ttu-id="a93bc-131">指定此资源预期的访问令牌版本。</span><span class="sxs-lookup"><span data-stu-id="a93bc-131">Specifies the access token version expected by this resource.</span></span> <span data-ttu-id="a93bc-132">这将更改独立于用于请求访问令牌的终结点或客户端生成的 JWT 的版本和格式。</span><span class="sxs-lookup"><span data-stu-id="a93bc-132">This changes the version and format of the JWT produced independent of the endpoint or client used to request the access token.</span></span> <br><br> <span data-ttu-id="a93bc-133">使用的终结点 v1.0 或 v2.0 由客户端选择，并且仅影响 id_tokens。</span><span class="sxs-lookup"><span data-stu-id="a93bc-133">The endpoint used, v1.0 or v2.0, is chosen by the client and only impacts the version of id_tokens.</span></span> <span data-ttu-id="a93bc-134">资源需要显式配置 **requestedAccessTokenVersion** 以指示受支持的访问令牌格式。</span><span class="sxs-lookup"><span data-stu-id="a93bc-134">Resources need to explicitly configure **requestedAccessTokenVersion** to indicate the supported access token format.</span></span> <br><br> <span data-ttu-id="a93bc-135">**requestedAccessTokenVersion** 的可能值为 `1` 、 `2` 或 `null` 。</span><span class="sxs-lookup"><span data-stu-id="a93bc-135">Possible values for **requestedAccessTokenVersion** are `1`, `2`, or `null`.</span></span> <span data-ttu-id="a93bc-136">如果值为 `null` ，则默认为 `1` ，它对应于 v1.0 终结点。</span><span class="sxs-lookup"><span data-stu-id="a93bc-136">If the value is `null`, this defaults to `1`, which corresponds to the v1.0 endpoint.</span></span> <br><br> <span data-ttu-id="a93bc-137">如果 **应用程序上的 signInAudience** 配置为 `AzureADandPersonalMicrosoftAccount` ，则此属性的值必须为 `2`</span><span class="sxs-lookup"><span data-stu-id="a93bc-137">If **signInAudience** on the application is configured as `AzureADandPersonalMicrosoftAccount`, the value for this property must be `2`</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a93bc-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a93bc-138">JSON representation</span></span>

<span data-ttu-id="a93bc-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a93bc-139">Here is a JSON representation of the resource.</span></span>

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

