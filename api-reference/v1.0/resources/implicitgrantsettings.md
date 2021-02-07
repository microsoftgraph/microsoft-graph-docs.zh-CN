---
title: implicitGrantSettings 资源类型
description: 指定此 Web 应用程序是否可以使用 OAuth 2.0 隐式流请求令牌。 单独的属性可用于请求 ID 和访问令牌作为隐式流的一部分。 若要启用隐式流，必须至少将以下属性之一设置为 true。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 58509ff0f0264a683aaae9c83d60e0f041ef0af7
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133278"
---
# <a name="implicitgrantsettings-resource-type"></a><span data-ttu-id="2b7f9-105">implicitGrantSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="2b7f9-105">implicitGrantSettings resource type</span></span>

<span data-ttu-id="2b7f9-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b7f9-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2b7f9-107">指定此 Web 应用程序是否可以使用 OAuth 2.0 隐式流请求令牌。</span><span class="sxs-lookup"><span data-stu-id="2b7f9-107">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span> <span data-ttu-id="2b7f9-108">单独的属性可用于请求 ID 和访问令牌作为隐式流的一部分。</span><span class="sxs-lookup"><span data-stu-id="2b7f9-108">Separate properties are available to request ID and access tokens as part of the implicit flow.</span></span> <span data-ttu-id="2b7f9-109">若要启用隐式流，必须至少将以下属性之一设置为 true。</span><span class="sxs-lookup"><span data-stu-id="2b7f9-109">To enable implicit flow, at least one of the following properties must be set to true.</span></span>

## <a name="properties"></a><span data-ttu-id="2b7f9-110">属性</span><span class="sxs-lookup"><span data-stu-id="2b7f9-110">Properties</span></span>

| <span data-ttu-id="2b7f9-111">属性</span><span class="sxs-lookup"><span data-stu-id="2b7f9-111">Property</span></span> | <span data-ttu-id="2b7f9-112">类型</span><span class="sxs-lookup"><span data-stu-id="2b7f9-112">Type</span></span> | <span data-ttu-id="2b7f9-113">说明</span><span class="sxs-lookup"><span data-stu-id="2b7f9-113">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="2b7f9-114">enableIdTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="2b7f9-114">enableIdTokenIssuance</span></span>| <span data-ttu-id="2b7f9-115">布尔</span><span class="sxs-lookup"><span data-stu-id="2b7f9-115">Boolean</span></span> | <span data-ttu-id="2b7f9-116">指定此 Web 应用程序是否可以使用 OAuth 2.0 隐式流请求 ID 令牌。</span><span class="sxs-lookup"><span data-stu-id="2b7f9-116">Specifies whether this web application can request an ID token using the OAuth 2.0 implicit flow.</span></span>|
|<span data-ttu-id="2b7f9-117">enableAccessTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="2b7f9-117">enableAccessTokenIssuance</span></span>| <span data-ttu-id="2b7f9-118">布尔</span><span class="sxs-lookup"><span data-stu-id="2b7f9-118">Boolean</span></span> | <span data-ttu-id="2b7f9-119">指定此 Web 应用程序是否可以使用 OAuth 2.0 隐式流请求访问令牌。</span><span class="sxs-lookup"><span data-stu-id="2b7f9-119">Specifies whether this web application can request an access token using the OAuth 2.0 implicit flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2b7f9-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2b7f9-120">JSON representation</span></span>
<span data-ttu-id="2b7f9-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2b7f9-121">Here is a JSON representation of the resource.</span></span>
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

