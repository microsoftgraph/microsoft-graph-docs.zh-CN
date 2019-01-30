---
title: publicClient 资源类型
description: 指定非 Web 应用程序或 Web Api 设置。 （例如移动或其他公共的客户端，例如桌面设备上运行安装的应用程序）
localization_priority: Normal
ms.openlocfilehash: ff1d77709293a7167868451671e1660196c9a4db
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29644054"
---
# <a name="publicclient-resource-type"></a><span data-ttu-id="4b342-104">publicClient 资源类型</span><span class="sxs-lookup"><span data-stu-id="4b342-104">publicClient resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b342-105">指定非 Web 应用程序或 Web Api 设置。</span><span class="sxs-lookup"><span data-stu-id="4b342-105">Specifies settings for non Web App or Web Api.</span></span> <span data-ttu-id="4b342-106">（例如移动或其他公共的客户端，例如桌面设备上运行安装的应用程序）</span><span class="sxs-lookup"><span data-stu-id="4b342-106">(e.g. Mobile or other public client such as an installed application running on a desktop device)</span></span>

## <a name="properties"></a><span data-ttu-id="4b342-107">属性</span><span class="sxs-lookup"><span data-stu-id="4b342-107">Properties</span></span>

| <span data-ttu-id="4b342-108">属性</span><span class="sxs-lookup"><span data-stu-id="4b342-108">Property</span></span> | <span data-ttu-id="4b342-109">类型</span><span class="sxs-lookup"><span data-stu-id="4b342-109">Type</span></span> | <span data-ttu-id="4b342-110">说明</span><span class="sxs-lookup"><span data-stu-id="4b342-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="4b342-111">redirectUris</span><span class="sxs-lookup"><span data-stu-id="4b342-111">redirectUris</span></span>|<span data-ttu-id="4b342-112">String collection</span><span class="sxs-lookup"><span data-stu-id="4b342-112">String collection</span></span>| <span data-ttu-id="4b342-113">指定用于登录，用户令牌发送到的 Url 或 Uri 的 OAuth 2.0 授权代码和访问令牌发送到的重定向。</span><span class="sxs-lookup"><span data-stu-id="4b342-113">Specifies the URLs that user tokens are sent to for sign in, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4b342-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4b342-114">JSON representation</span></span>
<span data-ttu-id="4b342-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4b342-115">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.installedClient"
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
  "suppressions": [
    "Error: /api-reference/beta/resources/publicclient.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
