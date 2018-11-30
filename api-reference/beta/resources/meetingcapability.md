---
title: meetingCapability 资源类型
description: 包含会议的功能
ms.openlocfilehash: 438193d08ab5542f07d4cbf61704520d81433e50
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044748"
---
# <a name="meetingcapability-resource-type"></a><span data-ttu-id="059cc-103">meetingCapability 资源类型</span><span class="sxs-lookup"><span data-stu-id="059cc-103">meetingCapability resource type</span></span>

> <span data-ttu-id="059cc-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="059cc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="059cc-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="059cc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="059cc-106">包含会议的功能</span><span class="sxs-lookup"><span data-stu-id="059cc-106">Contains the capabilities of a meeting</span></span>

## <a name="properties"></a><span data-ttu-id="059cc-107">属性</span><span class="sxs-lookup"><span data-stu-id="059cc-107">Properties</span></span>

| <span data-ttu-id="059cc-108">属性</span><span class="sxs-lookup"><span data-stu-id="059cc-108">Property</span></span>       | <span data-ttu-id="059cc-109">类型</span><span class="sxs-lookup"><span data-stu-id="059cc-109">Type</span></span>    | <span data-ttu-id="059cc-110">说明</span><span class="sxs-lookup"><span data-stu-id="059cc-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="059cc-111">allowAnonymousUsersToDialOut</span><span class="sxs-lookup"><span data-stu-id="059cc-111">allowAnonymousUsersToDialOut</span></span> | <span data-ttu-id="059cc-112">布尔</span><span class="sxs-lookup"><span data-stu-id="059cc-112">Boolean</span></span> | <span data-ttu-id="059cc-113">指示是否在会议中允许匿名用户拨出。</span><span class="sxs-lookup"><span data-stu-id="059cc-113">Indicates whether anonymous users dialout is allowed in a meeting.</span></span> |
| <span data-ttu-id="059cc-114">autoAdmittedUsers</span><span class="sxs-lookup"><span data-stu-id="059cc-114">autoAdmittedUsers</span></span> | <span data-ttu-id="059cc-115">String</span><span class="sxs-lookup"><span data-stu-id="059cc-115">String</span></span> | <span data-ttu-id="059cc-116">可取值为：`everyoneInCompany`、`everyone`。</span><span class="sxs-lookup"><span data-stu-id="059cc-116">Possible values are: `everyoneInCompany`, `everyone`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="059cc-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="059cc-117">JSON representation</span></span>

<span data-ttu-id="059cc-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="059cc-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingCapability"
}-->
```json
{
  "allowAnonymousUsersToDialOut": true,
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
