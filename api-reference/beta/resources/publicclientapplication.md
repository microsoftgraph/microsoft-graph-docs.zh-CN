---
title: publicClientApplication 资源类型
description: 指定非 Web 应用程序或 Web Api 的设置。 (例如, 移动或其他公共客户端, 如在桌面设备上运行的已安装应用程序)
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 4503e65777b41fc2f864cd818697b048e3c8e435
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965542"
---
# <a name="publicclientapplication-resource-type"></a><span data-ttu-id="6467c-104">publicClientApplication 资源类型</span><span class="sxs-lookup"><span data-stu-id="6467c-104">publicClientApplication resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6467c-105">指定非 Web 应用程序或 Web Api 的设置。</span><span class="sxs-lookup"><span data-stu-id="6467c-105">Specifies settings for non Web App or Web Api.</span></span> <span data-ttu-id="6467c-106">(例如, 移动或其他公共客户端, 如在桌面设备上运行的已安装应用程序)</span><span class="sxs-lookup"><span data-stu-id="6467c-106">(e.g. Mobile or other public client such as an installed application running on a desktop device)</span></span>

## <a name="properties"></a><span data-ttu-id="6467c-107">属性</span><span class="sxs-lookup"><span data-stu-id="6467c-107">Properties</span></span>

| <span data-ttu-id="6467c-108">属性</span><span class="sxs-lookup"><span data-stu-id="6467c-108">Property</span></span> | <span data-ttu-id="6467c-109">类型</span><span class="sxs-lookup"><span data-stu-id="6467c-109">Type</span></span> | <span data-ttu-id="6467c-110">说明</span><span class="sxs-lookup"><span data-stu-id="6467c-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="6467c-111">redirectUris</span><span class="sxs-lookup"><span data-stu-id="6467c-111">redirectUris</span></span>|<span data-ttu-id="6467c-112">String collection</span><span class="sxs-lookup"><span data-stu-id="6467c-112">String collection</span></span>| <span data-ttu-id="6467c-113">指定向其发送用户令牌以进行登录的 Url, 或向其发送 OAuth 2.0 授权代码和访问令牌的重定向 Uri。</span><span class="sxs-lookup"><span data-stu-id="6467c-113">Specifies the URLs that user tokens are sent to for sign in, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6467c-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6467c-114">JSON representation</span></span>
<span data-ttu-id="6467c-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6467c-115">Here is a JSON representation of the resource.</span></span>

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
