---
title: meetingCapability 资源类型
description: 包含会议的功能
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 342d264c1f4c670d159c15558c78cc896d4a9487
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931361"
---
# <a name="meetingcapability-resource-type"></a><span data-ttu-id="611d2-103">meetingCapability 资源类型</span><span class="sxs-lookup"><span data-stu-id="611d2-103">meetingCapability resource type</span></span>

> <span data-ttu-id="611d2-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="611d2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="611d2-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="611d2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="611d2-106">包含会议的功能</span><span class="sxs-lookup"><span data-stu-id="611d2-106">Contains the capabilities of a meeting</span></span>

## <a name="properties"></a><span data-ttu-id="611d2-107">属性</span><span class="sxs-lookup"><span data-stu-id="611d2-107">Properties</span></span>

| <span data-ttu-id="611d2-108">属性</span><span class="sxs-lookup"><span data-stu-id="611d2-108">Property</span></span>                          | <span data-ttu-id="611d2-109">类型</span><span class="sxs-lookup"><span data-stu-id="611d2-109">Type</span></span>    | <span data-ttu-id="611d2-110">说明</span><span class="sxs-lookup"><span data-stu-id="611d2-110">Description</span></span>                                                        |
|:----------------------------------|:--------|:-------------------------------------------------------------------|
| <span data-ttu-id="611d2-111">allowAnonymousUsersToDialOut</span><span class="sxs-lookup"><span data-stu-id="611d2-111">allowAnonymousUsersToDialOut</span></span>      | <span data-ttu-id="611d2-112">布尔</span><span class="sxs-lookup"><span data-stu-id="611d2-112">Boolean</span></span> | <span data-ttu-id="611d2-113">指示是否在会议中允许匿名用户拨出。</span><span class="sxs-lookup"><span data-stu-id="611d2-113">Indicates whether anonymous users dialout is allowed in a meeting.</span></span> |
| <span data-ttu-id="611d2-114">allowAnonymousUsersToStartMeeting</span><span class="sxs-lookup"><span data-stu-id="611d2-114">allowAnonymousUsersToStartMeeting</span></span> | <span data-ttu-id="611d2-115">布尔</span><span class="sxs-lookup"><span data-stu-id="611d2-115">Boolean</span></span> | <span data-ttu-id="611d2-116">指示是否允许匿名用户开始会议。</span><span class="sxs-lookup"><span data-stu-id="611d2-116">Indicates whether anonymous users are allowed to start a meeting.</span></span>  |
| <span data-ttu-id="611d2-117">autoAdmittedUsers</span><span class="sxs-lookup"><span data-stu-id="611d2-117">autoAdmittedUsers</span></span>                 | <span data-ttu-id="611d2-118">String</span><span class="sxs-lookup"><span data-stu-id="611d2-118">String</span></span>  | <span data-ttu-id="611d2-119">可取值为：`everyoneInCompany`、`everyone`。</span><span class="sxs-lookup"><span data-stu-id="611d2-119">Possible values are: `everyoneInCompany`, `everyone`.</span></span>              |

## <a name="json-representation"></a><span data-ttu-id="611d2-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="611d2-120">JSON representation</span></span>

<span data-ttu-id="611d2-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="611d2-121">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "meetingCapability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
