---
title: publicClientApplication 资源类型
description: '指定非 Web 应用或 Web Api 的设置。  (，例如移动或其他公共客户端，如在桌面设备上运行的已安装) '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: a15f0ea159ab12403186465783200a9e374562bc
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137513"
---
# <a name="publicclientapplication-resource-type"></a><span data-ttu-id="aeda4-104">publicClientApplication 资源类型</span><span class="sxs-lookup"><span data-stu-id="aeda4-104">publicClientApplication resource type</span></span>

<span data-ttu-id="aeda4-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aeda4-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="aeda4-106">指定非 Web 应用或非 Web API (例如移动或其他公共客户端（如桌面设备上运行的已安装应用程序）的设置) 。</span><span class="sxs-lookup"><span data-stu-id="aeda4-106">Specifies settings for non-web app or non-web API (for example, mobile or other public clients such as an installed application running on a desktop device).</span></span>

## <a name="properties"></a><span data-ttu-id="aeda4-107">属性</span><span class="sxs-lookup"><span data-stu-id="aeda4-107">Properties</span></span>

| <span data-ttu-id="aeda4-108">属性</span><span class="sxs-lookup"><span data-stu-id="aeda4-108">Property</span></span> | <span data-ttu-id="aeda4-109">类型</span><span class="sxs-lookup"><span data-stu-id="aeda4-109">Type</span></span> | <span data-ttu-id="aeda4-110">说明</span><span class="sxs-lookup"><span data-stu-id="aeda4-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="aeda4-111">redirectUris</span><span class="sxs-lookup"><span data-stu-id="aeda4-111">redirectUris</span></span>|<span data-ttu-id="aeda4-112">String collection</span><span class="sxs-lookup"><span data-stu-id="aeda4-112">String collection</span></span>| <span data-ttu-id="aeda4-113">指定用于登录的用户令牌的发送 URL，或发送 OAuth 2.0 授权代码和访问令牌的重定向 URI。</span><span class="sxs-lookup"><span data-stu-id="aeda4-113">Specifies the URLs where user tokens are sent for sign-in, or the redirect URIs where OAuth 2.0 authorization codes and access tokens are sent.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="aeda4-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aeda4-114">JSON representation</span></span>
<span data-ttu-id="aeda4-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aeda4-115">Here is a JSON representation of the resource.</span></span>

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

