---
title: publicClient 资源类型
description: 指定非 Web 应用程序或 Web Api 设置。 （例如移动或其他公共的客户端，例如桌面设备上运行安装的应用程序）
localization_priority: Normal
ms.openlocfilehash: 866e27b4ea3e1386b7cc69f967635d38641f121c
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571840"
---
# <a name="publicclient-resource-type"></a><span data-ttu-id="b2253-104">publicClient 资源类型</span><span class="sxs-lookup"><span data-stu-id="b2253-104">publicClient resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2253-105">指定非 Web 应用程序或 Web Api 设置。</span><span class="sxs-lookup"><span data-stu-id="b2253-105">Specifies settings for non Web App or Web Api.</span></span> <span data-ttu-id="b2253-106">（例如移动或其他公共的客户端，例如桌面设备上运行安装的应用程序）</span><span class="sxs-lookup"><span data-stu-id="b2253-106">(e.g. Mobile or other public client such as an installed application running on a desktop device)</span></span>

## <a name="properties"></a><span data-ttu-id="b2253-107">属性</span><span class="sxs-lookup"><span data-stu-id="b2253-107">Properties</span></span>

| <span data-ttu-id="b2253-108">属性</span><span class="sxs-lookup"><span data-stu-id="b2253-108">Property</span></span> | <span data-ttu-id="b2253-109">类型</span><span class="sxs-lookup"><span data-stu-id="b2253-109">Type</span></span> | <span data-ttu-id="b2253-110">说明</span><span class="sxs-lookup"><span data-stu-id="b2253-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="b2253-111">redirectUris</span><span class="sxs-lookup"><span data-stu-id="b2253-111">redirectUris</span></span>|<span data-ttu-id="b2253-112">String 集合</span><span class="sxs-lookup"><span data-stu-id="b2253-112">String collection</span></span>| <span data-ttu-id="b2253-113">指定用于登录，用户令牌发送到的 Url 或 Uri 的 OAuth 2.0 授权代码和访问令牌发送到的重定向。</span><span class="sxs-lookup"><span data-stu-id="b2253-113">Specifies the URLs that user tokens are sent to for sign in, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b2253-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b2253-114">JSON representation</span></span>
<span data-ttu-id="b2253-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b2253-115">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/publicclient.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
