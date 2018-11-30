---
title: implicitGrantSettings 资源类型
description: 指定此 web 应用程序是否可以请求令牌使用 OAuth 2.0 隐式流。 单独属性均可用于请求 ID 和访问令牌的隐式流的一部分。 若要启用隐式流，至少一个以下属性必须设置为 true。
ms.openlocfilehash: 018cd422b56724811e1913ff0e94aea16d7c68f9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043804"
---
# <a name="implicitgrantsettings-resource-type"></a><span data-ttu-id="36d0e-105">implicitGrantSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="36d0e-105">implicitGrantSettings resource type</span></span>

> <span data-ttu-id="36d0e-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="36d0e-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="36d0e-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="36d0e-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="36d0e-108">指定此 web 应用程序是否可以请求令牌使用 OAuth 2.0 隐式流。</span><span class="sxs-lookup"><span data-stu-id="36d0e-108">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span> <span data-ttu-id="36d0e-109">单独属性均可用于请求 ID 和访问令牌的隐式流的一部分。</span><span class="sxs-lookup"><span data-stu-id="36d0e-109">Separate properties are available to request ID and access tokens as part of the implicit flow.</span></span> <span data-ttu-id="36d0e-110">若要启用隐式流，至少一个以下属性必须设置为 true。</span><span class="sxs-lookup"><span data-stu-id="36d0e-110">To enable implicit flow, at least one of the following properties must be set to true.</span></span>

## <a name="properties"></a><span data-ttu-id="36d0e-111">属性</span><span class="sxs-lookup"><span data-stu-id="36d0e-111">Properties</span></span>

| <span data-ttu-id="36d0e-112">属性</span><span class="sxs-lookup"><span data-stu-id="36d0e-112">Property</span></span> | <span data-ttu-id="36d0e-113">类型</span><span class="sxs-lookup"><span data-stu-id="36d0e-113">Type</span></span> | <span data-ttu-id="36d0e-114">说明</span><span class="sxs-lookup"><span data-stu-id="36d0e-114">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="36d0e-115">enableIdTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="36d0e-115">enableIdTokenIssuance</span></span>| <span data-ttu-id="36d0e-116">布尔</span><span class="sxs-lookup"><span data-stu-id="36d0e-116">Boolean</span></span> | <span data-ttu-id="36d0e-117">指定此 web 应用程序是否可以请求使用 OAuth 2.0 隐式流 ID 令牌。</span><span class="sxs-lookup"><span data-stu-id="36d0e-117">Specifies whether this web application can request an ID token using the OAuth 2.0 implicit flow.</span></span>|
|<span data-ttu-id="36d0e-118">enableAccessTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="36d0e-118">enableAccessTokenIssuance</span></span>| <span data-ttu-id="36d0e-119">布尔</span><span class="sxs-lookup"><span data-stu-id="36d0e-119">Boolean</span></span> | <span data-ttu-id="36d0e-120">指定此 web 应用程序是否可以请求使用 OAuth 2.0 隐式流访问令牌。</span><span class="sxs-lookup"><span data-stu-id="36d0e-120">Specifies whether this web application can request an access token using the OAuth 2.0 implicit flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="36d0e-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="36d0e-121">JSON representation</span></span>
<span data-ttu-id="36d0e-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="36d0e-122">Here is a JSON representation of the resource.</span></span>

```json
{
  "enableIdTokenIssuance": "Boolean",
  "enableAccessTokenIssuance": "Boolean"
}

```
