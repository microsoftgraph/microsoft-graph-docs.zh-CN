---
title: implicitGrantSettings 资源类型
description: '指定此 Web 应用程序是否可以使用 OAuth 2.0 隐式流请求令牌。 '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: fe471eefe817e48468258195dae4c93331dd6e04
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547013"
---
# <a name="implicitgrantsettings-resource-type"></a><span data-ttu-id="d4e08-103">implicitGrantSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="d4e08-103">implicitGrantSettings resource type</span></span>

<span data-ttu-id="d4e08-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4e08-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4e08-105">指定此 Web 应用程序是否可以使用 OAuth 2.0 隐式流请求令牌。</span><span class="sxs-lookup"><span data-stu-id="d4e08-105">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span> <span data-ttu-id="d4e08-106">作为隐式流的一部分，单独的属性可用于请求 ID 和访问令牌。</span><span class="sxs-lookup"><span data-stu-id="d4e08-106">Separate properties are available to request ID and access tokens as part of the implicit flow.</span></span> <span data-ttu-id="d4e08-107">若要启用隐式流，必须至少将下列属性之一设置为 true。</span><span class="sxs-lookup"><span data-stu-id="d4e08-107">To enable implicit flow, at least one of the following properties must be set to true.</span></span>

## <a name="properties"></a><span data-ttu-id="d4e08-108">属性</span><span class="sxs-lookup"><span data-stu-id="d4e08-108">Properties</span></span>

| <span data-ttu-id="d4e08-109">属性</span><span class="sxs-lookup"><span data-stu-id="d4e08-109">Property</span></span> | <span data-ttu-id="d4e08-110">类型</span><span class="sxs-lookup"><span data-stu-id="d4e08-110">Type</span></span> | <span data-ttu-id="d4e08-111">说明</span><span class="sxs-lookup"><span data-stu-id="d4e08-111">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="d4e08-112">enableIdTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="d4e08-112">enableIdTokenIssuance</span></span>| <span data-ttu-id="d4e08-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4e08-113">Boolean</span></span> | <span data-ttu-id="d4e08-114">指定此 Web 应用程序是否可以使用 OAuth 2.0 隐式流请求 ID 令牌。</span><span class="sxs-lookup"><span data-stu-id="d4e08-114">Specifies whether this web application can request an ID token using the OAuth 2.0 implicit flow.</span></span>|
|<span data-ttu-id="d4e08-115">enableAccessTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="d4e08-115">enableAccessTokenIssuance</span></span>| <span data-ttu-id="d4e08-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4e08-116">Boolean</span></span> | <span data-ttu-id="d4e08-117">指定此 Web 应用程序是否可以使用 OAuth 2.0 隐式流请求访问令牌。</span><span class="sxs-lookup"><span data-stu-id="d4e08-117">Specifies whether this web application can request an access token using the OAuth 2.0 implicit flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d4e08-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d4e08-118">JSON representation</span></span>
<span data-ttu-id="d4e08-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d4e08-119">Here is a JSON representation of the resource.</span></span>
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


