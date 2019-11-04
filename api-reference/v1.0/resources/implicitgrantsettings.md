---
title: implicitGrantSettings 资源类型
description: 指定此 web 应用程序是否可以使用 OAuth 2.0 隐式流请求令牌。 在隐式流中，可以使用单独的属性来请求 ID 和访问令牌。 若要启用隐式流，下列属性中必须至少有一个设置为 true。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 52c2929d36ceaa250bd3843556073190da9d4152
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939486"
---
# <a name="implicitgrantsettings-resource-type"></a><span data-ttu-id="b54dc-105">implicitGrantSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="b54dc-105">implicitGrantSettings resource type</span></span>

<span data-ttu-id="b54dc-106">指定此 web 应用程序是否可以使用 OAuth 2.0 隐式流请求令牌。</span><span class="sxs-lookup"><span data-stu-id="b54dc-106">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span> <span data-ttu-id="b54dc-107">在隐式流中，可以使用单独的属性来请求 ID 和访问令牌。</span><span class="sxs-lookup"><span data-stu-id="b54dc-107">Separate properties are available to request ID and access tokens as part of the implicit flow.</span></span> <span data-ttu-id="b54dc-108">若要启用隐式流，下列属性中必须至少有一个设置为 true。</span><span class="sxs-lookup"><span data-stu-id="b54dc-108">To enable implicit flow, at least one of the following properties must be set to true.</span></span>

## <a name="properties"></a><span data-ttu-id="b54dc-109">属性</span><span class="sxs-lookup"><span data-stu-id="b54dc-109">Properties</span></span>

| <span data-ttu-id="b54dc-110">属性</span><span class="sxs-lookup"><span data-stu-id="b54dc-110">Property</span></span> | <span data-ttu-id="b54dc-111">类型</span><span class="sxs-lookup"><span data-stu-id="b54dc-111">Type</span></span> | <span data-ttu-id="b54dc-112">描述</span><span class="sxs-lookup"><span data-stu-id="b54dc-112">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="b54dc-113">enableIdTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="b54dc-113">enableIdTokenIssuance</span></span>| <span data-ttu-id="b54dc-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="b54dc-114">Boolean</span></span> | <span data-ttu-id="b54dc-115">指定此 web 应用程序是否可以使用 OAuth 2.0 隐式流请求 ID 令牌。</span><span class="sxs-lookup"><span data-stu-id="b54dc-115">Specifies whether this web application can request an ID token using the OAuth 2.0 implicit flow.</span></span>|
|<span data-ttu-id="b54dc-116">enableAccessTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="b54dc-116">enableAccessTokenIssuance</span></span>| <span data-ttu-id="b54dc-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="b54dc-117">Boolean</span></span> | <span data-ttu-id="b54dc-118">指定此 web 应用程序是否可以使用 OAuth 2.0 隐式流请求访问令牌。</span><span class="sxs-lookup"><span data-stu-id="b54dc-118">Specifies whether this web application can request an access token using the OAuth 2.0 implicit flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b54dc-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b54dc-119">JSON representation</span></span>
<span data-ttu-id="b54dc-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b54dc-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.implicitGrantSettings"
}-->
```json
{
  "enableIdTokenIssuance": "Boolean",
  "enableAccessTokenIssuance": "Boolean"
}

```
