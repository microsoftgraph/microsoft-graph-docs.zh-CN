---
title: publicClientApplication 资源类型
description: 指定非 Web 应用程序或 Web Api 的设置。 （例如，移动或其他公共客户端，如在桌面设备上运行的已安装应用程序）
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: e25c61cc58874944017ee34dddcff75c22b134b6
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937411"
---
# <a name="publicclientapplication-resource-type"></a><span data-ttu-id="48ba4-104">publicClientApplication 资源类型</span><span class="sxs-lookup"><span data-stu-id="48ba4-104">publicClientApplication resource type</span></span>

<span data-ttu-id="48ba4-105">指定非 web 应用或非 web API 的设置（例如，移动或其他公共客户端，如在桌面设备上运行的已安装应用程序）。</span><span class="sxs-lookup"><span data-stu-id="48ba4-105">Specifies settings for non-web app or non-web API (for example, mobile or other public clients such as an installed application running on a desktop device).</span></span>

## <a name="properties"></a><span data-ttu-id="48ba4-106">属性</span><span class="sxs-lookup"><span data-stu-id="48ba4-106">Properties</span></span>

| <span data-ttu-id="48ba4-107">属性</span><span class="sxs-lookup"><span data-stu-id="48ba4-107">Property</span></span> | <span data-ttu-id="48ba4-108">类型</span><span class="sxs-lookup"><span data-stu-id="48ba4-108">Type</span></span> | <span data-ttu-id="48ba4-109">描述</span><span class="sxs-lookup"><span data-stu-id="48ba4-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="48ba4-110">redirectUris</span><span class="sxs-lookup"><span data-stu-id="48ba4-110">redirectUris</span></span>|<span data-ttu-id="48ba4-111">String collection</span><span class="sxs-lookup"><span data-stu-id="48ba4-111">String collection</span></span>| <span data-ttu-id="48ba4-112">指定向其发送用户令牌以进行登录的 Url，或用于发送 OAuth 2.0 授权代码和访问令牌的重定向 Uri。</span><span class="sxs-lookup"><span data-stu-id="48ba4-112">Specifies the URLs where user tokens are sent for sign-in, or the redirect URIs where OAuth 2.0 authorization codes and access tokens are sent.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="48ba4-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="48ba4-113">JSON representation</span></span>
<span data-ttu-id="48ba4-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="48ba4-114">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.publicClientApplication"
}-->

```json
{
  "redirectUris": ["String"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "installedClient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
