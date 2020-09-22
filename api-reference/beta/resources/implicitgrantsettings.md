---
title: implicitGrantSettings 资源类型
description: 指定此 web 应用程序是否可以使用 OAuth 2.0 隐式流请求令牌。 在隐式流中，可以使用单独的属性来请求 ID 和访问令牌。 若要启用隐式流，下列属性中必须至少有一个设置为 true。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microasoft-identity-platform
author: sureshja
ms.openlocfilehash: 80ff94c4d7488b583fffd6c2710e48fc06dc26fa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016623"
---
# <a name="implicitgrantsettings-resource-type"></a><span data-ttu-id="320ff-105">implicitGrantSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="320ff-105">implicitGrantSettings resource type</span></span>

<span data-ttu-id="320ff-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="320ff-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="320ff-107">指定此 web 应用程序是否可以使用 OAuth 2.0 隐式流请求令牌。</span><span class="sxs-lookup"><span data-stu-id="320ff-107">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span> <span data-ttu-id="320ff-108">在隐式流中，可以使用单独的属性来请求 ID 和访问令牌。</span><span class="sxs-lookup"><span data-stu-id="320ff-108">Separate properties are available to request ID and access tokens as part of the implicit flow.</span></span> <span data-ttu-id="320ff-109">若要启用隐式流，下列属性中必须至少有一个设置为 true。</span><span class="sxs-lookup"><span data-stu-id="320ff-109">To enable implicit flow, at least one of the following properties must be set to true.</span></span>

## <a name="properties"></a><span data-ttu-id="320ff-110">属性</span><span class="sxs-lookup"><span data-stu-id="320ff-110">Properties</span></span>

| <span data-ttu-id="320ff-111">属性</span><span class="sxs-lookup"><span data-stu-id="320ff-111">Property</span></span> | <span data-ttu-id="320ff-112">类型</span><span class="sxs-lookup"><span data-stu-id="320ff-112">Type</span></span> | <span data-ttu-id="320ff-113">说明</span><span class="sxs-lookup"><span data-stu-id="320ff-113">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="320ff-114">enableIdTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="320ff-114">enableIdTokenIssuance</span></span>| <span data-ttu-id="320ff-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="320ff-115">Boolean</span></span> | <span data-ttu-id="320ff-116">指定此 web 应用程序是否可以使用 OAuth 2.0 隐式流请求 ID 令牌。</span><span class="sxs-lookup"><span data-stu-id="320ff-116">Specifies whether this web application can request an ID token using the OAuth 2.0 implicit flow.</span></span>|
|<span data-ttu-id="320ff-117">enableAccessTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="320ff-117">enableAccessTokenIssuance</span></span>| <span data-ttu-id="320ff-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="320ff-118">Boolean</span></span> | <span data-ttu-id="320ff-119">指定此 web 应用程序是否可以使用 OAuth 2.0 隐式流请求访问令牌。</span><span class="sxs-lookup"><span data-stu-id="320ff-119">Specifies whether this web application can request an access token using the OAuth 2.0 implicit flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="320ff-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="320ff-120">JSON representation</span></span>
<span data-ttu-id="320ff-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="320ff-121">Here is a JSON representation of the resource.</span></span>
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


