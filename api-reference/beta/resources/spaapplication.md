---
title: spaApplication 资源类型
description: 指定单页应用程序的设置。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 82848c5ea8427111b2d8b02c1886f3990faba79e
ms.sourcegitcommit: be09568fa07ab793cd1db500f537ca94ca9e5b4a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836941"
---
# <a name="spaapplication-resource-type"></a><span data-ttu-id="c7984-103">spaApplication 资源类型</span><span class="sxs-lookup"><span data-stu-id="c7984-103">spaApplication resource type</span></span>

<span data-ttu-id="c7984-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7984-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7984-105">指定单页应用程序的设置。</span><span class="sxs-lookup"><span data-stu-id="c7984-105">Specifies settings for a single-page application.</span></span>

## <a name="properties"></a><span data-ttu-id="c7984-106">属性</span><span class="sxs-lookup"><span data-stu-id="c7984-106">Properties</span></span>

| <span data-ttu-id="c7984-107">属性</span><span class="sxs-lookup"><span data-stu-id="c7984-107">Property</span></span> | <span data-ttu-id="c7984-108">类型</span><span class="sxs-lookup"><span data-stu-id="c7984-108">Type</span></span> | <span data-ttu-id="c7984-109">说明</span><span class="sxs-lookup"><span data-stu-id="c7984-109">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="c7984-110">redirectUris</span><span class="sxs-lookup"><span data-stu-id="c7984-110">redirectUris</span></span> | <span data-ttu-id="c7984-111">String 集合</span><span class="sxs-lookup"><span data-stu-id="c7984-111">String collection</span></span> | <span data-ttu-id="c7984-112">指定用于登录的用户令牌的 URL，或发送 OAuth 2.0 授权代码和访问令牌的重定向 URI。</span><span class="sxs-lookup"><span data-stu-id="c7984-112">Specifies the URLs where user tokens are sent for sign-in, or the redirect URIs where OAuth 2.0 authorization codes and access tokens are sent.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c7984-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c7984-113">JSON representation</span></span>
<span data-ttu-id="c7984-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c7984-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.spaApplication"
}-->

```json
{
  "redirectUris": ["String"]
}
```
