---
title: apiApplication 资源类型
description: 指定 Web API 应用程序的设置。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 81d0431a21ca230d96de0dd8f826a166fa16bace
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135000"
---
# <a name="apiapplication-resource-type"></a><span data-ttu-id="0306e-103">apiApplication 资源类型</span><span class="sxs-lookup"><span data-stu-id="0306e-103">apiApplication resource type</span></span>

<span data-ttu-id="0306e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0306e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0306e-105">指定实现 Web API 的应用程序的设置。</span><span class="sxs-lookup"><span data-stu-id="0306e-105">Specifies settings for an application that implements a web API.</span></span>

## <a name="properties"></a><span data-ttu-id="0306e-106">属性</span><span class="sxs-lookup"><span data-stu-id="0306e-106">Properties</span></span>

| <span data-ttu-id="0306e-107">属性</span><span class="sxs-lookup"><span data-stu-id="0306e-107">Property</span></span> | <span data-ttu-id="0306e-108">类型</span><span class="sxs-lookup"><span data-stu-id="0306e-108">Type</span></span> | <span data-ttu-id="0306e-109">说明</span><span class="sxs-lookup"><span data-stu-id="0306e-109">Description</span></span> |
|:---------------|:--------|:----------|
|`acceptMappedClaims`| <span data-ttu-id="0306e-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="0306e-110">Boolean</span></span> | <span data-ttu-id="0306e-111">如果为 true，则允许应用程序使用声明映射，而不指定自定义签名密钥。</span><span class="sxs-lookup"><span data-stu-id="0306e-111">When true, allows an application to use claims mapping without specifying a custom signing key.</span></span> |
|`knownClientApplications`| <span data-ttu-id="0306e-112">Guid 集合</span><span class="sxs-lookup"><span data-stu-id="0306e-112">Guid collection</span></span> |<span data-ttu-id="0306e-113">如果你的解决方案包含两个部分：客户端应用和自定义 Web API 应用，用于捆绑许可。</span><span class="sxs-lookup"><span data-stu-id="0306e-113">Used for bundling consent if you have a solution that contains two parts: a client app and a custom web API app.</span></span> <span data-ttu-id="0306e-114">如果将客户端应用的 appID 设置为此值，则用户仅同意客户端应用一次。</span><span class="sxs-lookup"><span data-stu-id="0306e-114">If you set the appID of the client app to this value, the user only consents once to the client app.</span></span> <span data-ttu-id="0306e-115">Azure AD 知道，同意客户端意味着隐式同意 Web API，并同时自动为两个 API 设置服务主体。</span><span class="sxs-lookup"><span data-stu-id="0306e-115">Azure AD knows that consenting to the client means implicitly consenting to the web API and automatically provisions service principals for both APIs at the same time.</span></span> <span data-ttu-id="0306e-116">客户端和 Web API 应用都必须在同一租户中注册。</span><span class="sxs-lookup"><span data-stu-id="0306e-116">Both the client and the web API app must be registered in the same tenant.</span></span>|
|`oauth2PermissionScopes`| <span data-ttu-id="0306e-117">[permissionScope](permissionscope.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0306e-117">[permissionScope](permissionscope.md) collection</span></span> | <span data-ttu-id="0306e-118">由此应用程序注册表示的 Web API 公开的委派权限的定义。</span><span class="sxs-lookup"><span data-stu-id="0306e-118">The definition of the delegated permissions exposed by the web API represented by this application registration.</span></span> <span data-ttu-id="0306e-119">这些委派权限可能由客户端应用程序请求，并且可能由用户或管理员在同意期间授予。</span><span class="sxs-lookup"><span data-stu-id="0306e-119">These delegated permissions may be requested by a client application, and may be granted by users or administrators during consent.</span></span> <span data-ttu-id="0306e-120">委派的权限有时称为 OAuth 2.0 范围。</span><span class="sxs-lookup"><span data-stu-id="0306e-120">Delegated permissions are sometimes referred to as OAuth 2.0 scopes.</span></span> |
|`preAuthorizedApplications`| <span data-ttu-id="0306e-121">[preAuthorizedApplication](preauthorizedapplication.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0306e-121">[preAuthorizedApplication](preauthorizedapplication.md) collection</span></span> | <span data-ttu-id="0306e-122">列出具有访问此应用程序 API 的指定委派权限的预授权客户端应用程序。</span><span class="sxs-lookup"><span data-stu-id="0306e-122">Lists the client applications that are pre-authorized with the specified delegated permissions to access this application's APIs.</span></span> <span data-ttu-id="0306e-123">对于用户指定的权限，用户无需同意 (授权的应用程序) 。</span><span class="sxs-lookup"><span data-stu-id="0306e-123">Users are not required to consent to any pre-authorized application (for the permissions specified).</span></span> <span data-ttu-id="0306e-124">但是，通过增量同意（例如 (请求获取的 preAuthorizedApplications 中未) 权限将需要用户同意。</span><span class="sxs-lookup"><span data-stu-id="0306e-124">However, any additional permissions not listed in preAuthorizedApplications (requested through incremental consent for example) will require user consent.</span></span> |
|`requestedAccessTokenVersion`| <span data-ttu-id="0306e-125">Int32</span><span class="sxs-lookup"><span data-stu-id="0306e-125">Int32</span></span> | <span data-ttu-id="0306e-126">指定此资源预期的访问令牌版本。</span><span class="sxs-lookup"><span data-stu-id="0306e-126">Specifies the access token version expected by this resource.</span></span> <span data-ttu-id="0306e-127">这将更改独立于用于请求访问令牌的终结点或客户端生成的 JWT 的版本和格式。</span><span class="sxs-lookup"><span data-stu-id="0306e-127">This changes the version and format of the JWT produced independent of the endpoint or client used to request the access token.</span></span> <br><br> <span data-ttu-id="0306e-128">使用的终结点 v1.0 或 v2.0 由客户端选择，并且仅影响 id_tokens。</span><span class="sxs-lookup"><span data-stu-id="0306e-128">The endpoint used, v1.0 or v2.0, is chosen by the client and only impacts the version of id_tokens.</span></span> <span data-ttu-id="0306e-129">资源需要显式配置 `requestedAccessTokenVersion` 以指示受支持的访问令牌格式。</span><span class="sxs-lookup"><span data-stu-id="0306e-129">Resources need to explicitly configure `requestedAccessTokenVersion` to indicate the supported access token format.</span></span> <br><br> <span data-ttu-id="0306e-130">可能的值为 `requestedAccessTokenVersion` `1` ， `2` 或 `null` 。</span><span class="sxs-lookup"><span data-stu-id="0306e-130">Possible values for `requestedAccessTokenVersion` are `1`, `2`, or `null`.</span></span> <span data-ttu-id="0306e-131">如果值为 `null` ，则默认值为 `1` ，对应于 v1.0 终结点。</span><span class="sxs-lookup"><span data-stu-id="0306e-131">If the value is `null`, this defaults to `1`, which corresponds to the v1.0 endpoint.</span></span> <br><br> <span data-ttu-id="0306e-132">如果 `signInAudience` 应用程序配置为，则 `AzureADandPersonalMicrosoftAccount` 此属性的值必须为 `2`</span><span class="sxs-lookup"><span data-stu-id="0306e-132">If `signInAudience` on the application is configured as `AzureADandPersonalMicrosoftAccount`, the value for this property must be `2`</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0306e-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0306e-133">JSON representation</span></span>

<span data-ttu-id="0306e-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0306e-134">Here is a JSON representation of the resource.</span></span>

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

