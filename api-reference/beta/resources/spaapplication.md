---
title: spaApplication 资源类型
description: 指定单个页面应用程序的设置。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: hamiltonha
ms.openlocfilehash: dd5e2c6419acd66cb482f2ccff2914b1bf0245dc
ms.sourcegitcommit: 40b0e58312819b69567f35ab894ee0d2989837ab
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/13/2020
ms.locfileid: "49031901"
---
# <a name="spaapplication-resource-type"></a><span data-ttu-id="cd10e-103">spaApplication 资源类型</span><span class="sxs-lookup"><span data-stu-id="cd10e-103">spaApplication resource type</span></span>

<span data-ttu-id="cd10e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd10e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cd10e-105">指定单个页面应用程序的设置。</span><span class="sxs-lookup"><span data-stu-id="cd10e-105">Specifies settings for a single-page application.</span></span>

## <a name="properties"></a><span data-ttu-id="cd10e-106">属性</span><span class="sxs-lookup"><span data-stu-id="cd10e-106">Properties</span></span>

| <span data-ttu-id="cd10e-107">属性</span><span class="sxs-lookup"><span data-stu-id="cd10e-107">Property</span></span> | <span data-ttu-id="cd10e-108">类型</span><span class="sxs-lookup"><span data-stu-id="cd10e-108">Type</span></span> | <span data-ttu-id="cd10e-109">Description</span><span class="sxs-lookup"><span data-stu-id="cd10e-109">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="cd10e-110">redirectUris</span><span class="sxs-lookup"><span data-stu-id="cd10e-110">redirectUris</span></span> | <span data-ttu-id="cd10e-111">String collection</span><span class="sxs-lookup"><span data-stu-id="cd10e-111">String collection</span></span> | <span data-ttu-id="cd10e-112">指定向其发送用户令牌以进行登录的 Url，或用于发送 OAuth 2.0 授权代码和访问令牌的重定向 Uri。</span><span class="sxs-lookup"><span data-stu-id="cd10e-112">Specifies the URLs where user tokens are sent for sign-in, or the redirect URIs where OAuth 2.0 authorization codes and access tokens are sent.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="cd10e-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cd10e-113">JSON representation</span></span>
<span data-ttu-id="cd10e-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cd10e-114">The following is a JSON representation of the resource.</span></span>

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
