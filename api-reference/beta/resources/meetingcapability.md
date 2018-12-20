---
title: meetingCapability 资源类型
description: 包含会议的功能
author: VinodRavichandran
ms.openlocfilehash: 1a6f172922c0efbc9ad93e32141e364e2d0fc711
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380245"
---
# <a name="meetingcapability-resource-type"></a><span data-ttu-id="f37bd-103">meetingCapability 资源类型</span><span class="sxs-lookup"><span data-stu-id="f37bd-103">meetingCapability resource type</span></span>

> <span data-ttu-id="f37bd-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f37bd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f37bd-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f37bd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f37bd-106">包含会议的功能</span><span class="sxs-lookup"><span data-stu-id="f37bd-106">Contains the capabilities of a meeting</span></span>

## <a name="properties"></a><span data-ttu-id="f37bd-107">属性</span><span class="sxs-lookup"><span data-stu-id="f37bd-107">Properties</span></span>

| <span data-ttu-id="f37bd-108">属性</span><span class="sxs-lookup"><span data-stu-id="f37bd-108">Property</span></span>                          | <span data-ttu-id="f37bd-109">类型</span><span class="sxs-lookup"><span data-stu-id="f37bd-109">Type</span></span>    | <span data-ttu-id="f37bd-110">说明</span><span class="sxs-lookup"><span data-stu-id="f37bd-110">Description</span></span>                                                        |
|:----------------------------------|:--------|:-------------------------------------------------------------------|
| <span data-ttu-id="f37bd-111">allowAnonymousUsersToDialOut</span><span class="sxs-lookup"><span data-stu-id="f37bd-111">allowAnonymousUsersToDialOut</span></span>      | <span data-ttu-id="f37bd-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="f37bd-112">Boolean</span></span> | <span data-ttu-id="f37bd-113">指示是否在会议中允许匿名用户拨出。</span><span class="sxs-lookup"><span data-stu-id="f37bd-113">Indicates whether anonymous users dialout is allowed in a meeting.</span></span> |
| <span data-ttu-id="f37bd-114">allowAnonymousUsersToStartMeeting</span><span class="sxs-lookup"><span data-stu-id="f37bd-114">allowAnonymousUsersToStartMeeting</span></span> | <span data-ttu-id="f37bd-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="f37bd-115">Boolean</span></span> | <span data-ttu-id="f37bd-116">指示是否允许匿名用户开始会议。</span><span class="sxs-lookup"><span data-stu-id="f37bd-116">Indicates whether anonymous users are allowed to start a meeting.</span></span>  |
| <span data-ttu-id="f37bd-117">autoAdmittedUsers</span><span class="sxs-lookup"><span data-stu-id="f37bd-117">autoAdmittedUsers</span></span>                 | <span data-ttu-id="f37bd-118">String</span><span class="sxs-lookup"><span data-stu-id="f37bd-118">String</span></span>  | <span data-ttu-id="f37bd-119">可取值为：`everyoneInCompany`、`everyone`。</span><span class="sxs-lookup"><span data-stu-id="f37bd-119">Possible values are: `everyoneInCompany`, `everyone`.</span></span>              |

## <a name="json-representation"></a><span data-ttu-id="f37bd-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f37bd-120">JSON representation</span></span>

<span data-ttu-id="f37bd-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f37bd-121">The following is a JSON representation of the resource.</span></span>

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
