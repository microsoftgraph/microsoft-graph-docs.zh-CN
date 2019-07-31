---
title: meetingCapability 资源类型
description: 包含会议的功能
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 1de406cf0614a4cbb64749cef763a97a3723eb48
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966842"
---
# <a name="meetingcapability-resource-type"></a><span data-ttu-id="9db28-103">meetingCapability 资源类型</span><span class="sxs-lookup"><span data-stu-id="9db28-103">meetingCapability resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9db28-104">包含会议的功能</span><span class="sxs-lookup"><span data-stu-id="9db28-104">Contains the capabilities of a meeting</span></span>

## <a name="properties"></a><span data-ttu-id="9db28-105">属性</span><span class="sxs-lookup"><span data-stu-id="9db28-105">Properties</span></span>

| <span data-ttu-id="9db28-106">属性</span><span class="sxs-lookup"><span data-stu-id="9db28-106">Property</span></span>                          | <span data-ttu-id="9db28-107">类型</span><span class="sxs-lookup"><span data-stu-id="9db28-107">Type</span></span>    | <span data-ttu-id="9db28-108">说明</span><span class="sxs-lookup"><span data-stu-id="9db28-108">Description</span></span>                                                        |
|:----------------------------------|:--------|:-------------------------------------------------------------------|
| <span data-ttu-id="9db28-109">allowAnonymousUsersToDialOut</span><span class="sxs-lookup"><span data-stu-id="9db28-109">allowAnonymousUsersToDialOut</span></span>      | <span data-ttu-id="9db28-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="9db28-110">Boolean</span></span> | <span data-ttu-id="9db28-111">指示是否允许在会议中拨出匿名用户。</span><span class="sxs-lookup"><span data-stu-id="9db28-111">Indicates whether anonymous users dialout is allowed in a meeting.</span></span> |
| <span data-ttu-id="9db28-112">allowAnonymousUsersToStartMeeting</span><span class="sxs-lookup"><span data-stu-id="9db28-112">allowAnonymousUsersToStartMeeting</span></span> | <span data-ttu-id="9db28-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="9db28-113">Boolean</span></span> | <span data-ttu-id="9db28-114">指示是否允许匿名用户启动会议。</span><span class="sxs-lookup"><span data-stu-id="9db28-114">Indicates whether anonymous users are allowed to start a meeting.</span></span>  |
| <span data-ttu-id="9db28-115">autoAdmittedUsers</span><span class="sxs-lookup"><span data-stu-id="9db28-115">autoAdmittedUsers</span></span>                 | <span data-ttu-id="9db28-116">String</span><span class="sxs-lookup"><span data-stu-id="9db28-116">String</span></span>  | <span data-ttu-id="9db28-117">可取值为：`everyoneInCompany`、`everyone`。</span><span class="sxs-lookup"><span data-stu-id="9db28-117">Possible values are: `everyoneInCompany`, `everyone`.</span></span>              |

## <a name="json-representation"></a><span data-ttu-id="9db28-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9db28-118">JSON representation</span></span>

<span data-ttu-id="9db28-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9db28-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingCapability"
}-->
```json
{
  "allowAnonymousUsersToDialOut": true,
  "allowAnonymousUsersToStartMeeting": true,
  "autoAdmittedUsers": "everyoneInCompany | everyone"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingCapability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
