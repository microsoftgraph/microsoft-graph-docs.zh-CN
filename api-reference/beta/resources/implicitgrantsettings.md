---
title: implicitGrantSettings 资源类型
description: 指定此 web 应用程序是否可以使用 OAuth 2.0 隐式流请求令牌。 在隐式流中，可以使用单独的属性来请求 ID 和访问令牌。 若要启用隐式流，下列属性中必须至少有一个设置为 true。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 97824f704d855d7a2c9b1af84af577a738c3b87a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42496479"
---
# <a name="implicitgrantsettings-resource-type"></a><span data-ttu-id="ca8a2-105">implicitGrantSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="ca8a2-105">implicitGrantSettings resource type</span></span>

<span data-ttu-id="ca8a2-106">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="ca8a2-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca8a2-107">指定此 web 应用程序是否可以使用 OAuth 2.0 隐式流请求令牌。</span><span class="sxs-lookup"><span data-stu-id="ca8a2-107">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span> <span data-ttu-id="ca8a2-108">在隐式流中，可以使用单独的属性来请求 ID 和访问令牌。</span><span class="sxs-lookup"><span data-stu-id="ca8a2-108">Separate properties are available to request ID and access tokens as part of the implicit flow.</span></span> <span data-ttu-id="ca8a2-109">若要启用隐式流，下列属性中必须至少有一个设置为 true。</span><span class="sxs-lookup"><span data-stu-id="ca8a2-109">To enable implicit flow, at least one of the following properties must be set to true.</span></span>

## <a name="properties"></a><span data-ttu-id="ca8a2-110">属性</span><span class="sxs-lookup"><span data-stu-id="ca8a2-110">Properties</span></span>

| <span data-ttu-id="ca8a2-111">属性</span><span class="sxs-lookup"><span data-stu-id="ca8a2-111">Property</span></span> | <span data-ttu-id="ca8a2-112">类型</span><span class="sxs-lookup"><span data-stu-id="ca8a2-112">Type</span></span> | <span data-ttu-id="ca8a2-113">说明</span><span class="sxs-lookup"><span data-stu-id="ca8a2-113">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="ca8a2-114">enableIdTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="ca8a2-114">enableIdTokenIssuance</span></span>| <span data-ttu-id="ca8a2-115">布尔</span><span class="sxs-lookup"><span data-stu-id="ca8a2-115">Boolean</span></span> | <span data-ttu-id="ca8a2-116">指定此 web 应用程序是否可以使用 OAuth 2.0 隐式流请求 ID 令牌。</span><span class="sxs-lookup"><span data-stu-id="ca8a2-116">Specifies whether this web application can request an ID token using the OAuth 2.0 implicit flow.</span></span>|
|<span data-ttu-id="ca8a2-117">enableAccessTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="ca8a2-117">enableAccessTokenIssuance</span></span>| <span data-ttu-id="ca8a2-118">布尔</span><span class="sxs-lookup"><span data-stu-id="ca8a2-118">Boolean</span></span> | <span data-ttu-id="ca8a2-119">指定此 web 应用程序是否可以使用 OAuth 2.0 隐式流请求访问令牌。</span><span class="sxs-lookup"><span data-stu-id="ca8a2-119">Specifies whether this web application can request an access token using the OAuth 2.0 implicit flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ca8a2-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ca8a2-120">JSON representation</span></span>
<span data-ttu-id="ca8a2-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ca8a2-121">Here is a JSON representation of the resource.</span></span>
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
