---
title: publicClient 资源类型
description: 指定非 Web 应用程序或 Web Api 设置。 （例如移动或其他公共的客户端，例如桌面设备上运行安装的应用程序）
ms.openlocfilehash: ba921fecb554a8749a9020508c538c68a7ff342e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042114"
---
# <a name="publicclient-resource-type"></a><span data-ttu-id="8d325-104">publicClient 资源类型</span><span class="sxs-lookup"><span data-stu-id="8d325-104">publicClient resource type</span></span>

> <span data-ttu-id="8d325-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8d325-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8d325-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8d325-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8d325-107">指定非 Web 应用程序或 Web Api 设置。</span><span class="sxs-lookup"><span data-stu-id="8d325-107">Specifies settings for non Web App or Web Api.</span></span> <span data-ttu-id="8d325-108">（例如移动或其他公共的客户端，例如桌面设备上运行安装的应用程序）</span><span class="sxs-lookup"><span data-stu-id="8d325-108">(e.g. Mobile or other public client such as an installed application running on a desktop device)</span></span>

## <a name="properties"></a><span data-ttu-id="8d325-109">属性</span><span class="sxs-lookup"><span data-stu-id="8d325-109">Properties</span></span>

| <span data-ttu-id="8d325-110">属性</span><span class="sxs-lookup"><span data-stu-id="8d325-110">Property</span></span> | <span data-ttu-id="8d325-111">类型</span><span class="sxs-lookup"><span data-stu-id="8d325-111">Type</span></span> | <span data-ttu-id="8d325-112">说明</span><span class="sxs-lookup"><span data-stu-id="8d325-112">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="8d325-113">redirectUris</span><span class="sxs-lookup"><span data-stu-id="8d325-113">redirectUris</span></span>|<span data-ttu-id="8d325-114">String 集合</span><span class="sxs-lookup"><span data-stu-id="8d325-114">String collection</span></span>| <span data-ttu-id="8d325-115">指定用于登录，用户令牌发送到的 Url 或 Uri 的 OAuth 2.0 授权代码和访问令牌发送到的重定向。</span><span class="sxs-lookup"><span data-stu-id="8d325-115">Specifies the URLs that user tokens are sent to for sign in, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8d325-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8d325-116">JSON representation</span></span>
<span data-ttu-id="8d325-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8d325-117">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "installedClient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->