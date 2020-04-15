---
title: publicClientApplication 资源类型
description: 指定非 Web 应用程序或 Web Api 的设置。 （例如，移动或其他公共客户端，如在桌面设备上运行的已安装应用程序）
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: be86fd4601c31b7431a7a4994e7a2df081bbc363
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43461814"
---
# <a name="publicclientapplication-resource-type"></a><span data-ttu-id="8646f-104">publicClientApplication 资源类型</span><span class="sxs-lookup"><span data-stu-id="8646f-104">publicClientApplication resource type</span></span>

<span data-ttu-id="8646f-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8646f-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8646f-106">指定非 web 应用或非 web API 的设置（例如，移动或其他公共客户端，如在桌面设备上运行的已安装应用程序）。</span><span class="sxs-lookup"><span data-stu-id="8646f-106">Specifies settings for non-web app or non-web API (for example, mobile or other public clients such as an installed application running on a desktop device).</span></span>

## <a name="properties"></a><span data-ttu-id="8646f-107">属性</span><span class="sxs-lookup"><span data-stu-id="8646f-107">Properties</span></span>

| <span data-ttu-id="8646f-108">属性</span><span class="sxs-lookup"><span data-stu-id="8646f-108">Property</span></span> | <span data-ttu-id="8646f-109">类型</span><span class="sxs-lookup"><span data-stu-id="8646f-109">Type</span></span> | <span data-ttu-id="8646f-110">说明</span><span class="sxs-lookup"><span data-stu-id="8646f-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="8646f-111">redirectUris</span><span class="sxs-lookup"><span data-stu-id="8646f-111">redirectUris</span></span>|<span data-ttu-id="8646f-112">String 集合</span><span class="sxs-lookup"><span data-stu-id="8646f-112">String collection</span></span>| <span data-ttu-id="8646f-113">指定向其发送用户令牌以进行登录的 Url，或用于发送 OAuth 2.0 授权代码和访问令牌的重定向 Uri。</span><span class="sxs-lookup"><span data-stu-id="8646f-113">Specifies the URLs where user tokens are sent for sign-in, or the redirect URIs where OAuth 2.0 authorization codes and access tokens are sent.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8646f-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8646f-114">JSON representation</span></span>
<span data-ttu-id="8646f-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8646f-115">Here is a JSON representation of the resource.</span></span>

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
