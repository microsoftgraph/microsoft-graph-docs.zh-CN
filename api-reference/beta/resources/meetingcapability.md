---
title: meetingCapability 资源类型
description: 包含会议的功能
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 2b891a9e6d0eb90a527c79528e9fd595c2f8ca5b
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913623"
---
# <a name="meetingcapability-resource-type"></a><span data-ttu-id="479f9-103">meetingCapability 资源类型</span><span class="sxs-lookup"><span data-stu-id="479f9-103">meetingCapability resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="479f9-104">包含会议的功能</span><span class="sxs-lookup"><span data-stu-id="479f9-104">Contains the capabilities of a meeting</span></span>

## <a name="properties"></a><span data-ttu-id="479f9-105">属性</span><span class="sxs-lookup"><span data-stu-id="479f9-105">Properties</span></span>

| <span data-ttu-id="479f9-106">属性</span><span class="sxs-lookup"><span data-stu-id="479f9-106">Property</span></span>                          | <span data-ttu-id="479f9-107">类型</span><span class="sxs-lookup"><span data-stu-id="479f9-107">Type</span></span>    | <span data-ttu-id="479f9-108">说明</span><span class="sxs-lookup"><span data-stu-id="479f9-108">Description</span></span>                                                        |
|:----------------------------------|:--------|:-------------------------------------------------------------------|
| <span data-ttu-id="479f9-109">allowAnonymousUsersToDialOut</span><span class="sxs-lookup"><span data-stu-id="479f9-109">allowAnonymousUsersToDialOut</span></span>      | <span data-ttu-id="479f9-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="479f9-110">Boolean</span></span> | <span data-ttu-id="479f9-111">指示是否允许在会议中拨出匿名用户。</span><span class="sxs-lookup"><span data-stu-id="479f9-111">Indicates whether anonymous users dialout is allowed in a meeting.</span></span> |
| <span data-ttu-id="479f9-112">allowAnonymousUsersToStartMeeting</span><span class="sxs-lookup"><span data-stu-id="479f9-112">allowAnonymousUsersToStartMeeting</span></span> | <span data-ttu-id="479f9-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="479f9-113">Boolean</span></span> | <span data-ttu-id="479f9-114">指示是否允许匿名用户启动会议。</span><span class="sxs-lookup"><span data-stu-id="479f9-114">Indicates whether anonymous users are allowed to start a meeting.</span></span>  |
| <span data-ttu-id="479f9-115">autoAdmittedUsers</span><span class="sxs-lookup"><span data-stu-id="479f9-115">autoAdmittedUsers</span></span>                 | <span data-ttu-id="479f9-116">String</span><span class="sxs-lookup"><span data-stu-id="479f9-116">String</span></span>  | <span data-ttu-id="479f9-117">可取值为：`everyoneInCompany`、`everyone`。</span><span class="sxs-lookup"><span data-stu-id="479f9-117">Possible values are: `everyoneInCompany`, `everyone`.</span></span>              |

## <a name="json-representation"></a><span data-ttu-id="479f9-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="479f9-118">JSON representation</span></span>

<span data-ttu-id="479f9-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="479f9-119">The following is a JSON representation of the resource.</span></span>

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
