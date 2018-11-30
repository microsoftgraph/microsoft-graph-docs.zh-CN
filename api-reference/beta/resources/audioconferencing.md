---
title: audioConferencing 资源类型
description: 代表 onlineMeeting 电话访问信息。
ms.openlocfilehash: dd23c6ade282e081482a8c079491644c663b4054
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043800"
---
# <a name="audioconferencing-resource-type"></a><span data-ttu-id="2365e-103">audioConferencing 资源类型</span><span class="sxs-lookup"><span data-stu-id="2365e-103">audioConferencing resource type</span></span>

> <span data-ttu-id="2365e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2365e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2365e-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2365e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2365e-106">代表[onlineMeeting](onlinemeeting.md)电话访问信息。</span><span class="sxs-lookup"><span data-stu-id="2365e-106">Represents phone access information for an [onlineMeeting](onlinemeeting.md).</span></span>

## <a name="properties"></a><span data-ttu-id="2365e-107">属性</span><span class="sxs-lookup"><span data-stu-id="2365e-107">Properties</span></span>

| <span data-ttu-id="2365e-108">属性</span><span class="sxs-lookup"><span data-stu-id="2365e-108">Property</span></span>            | <span data-ttu-id="2365e-109">类型</span><span class="sxs-lookup"><span data-stu-id="2365e-109">Type</span></span>    | <span data-ttu-id="2365e-110">说明</span><span class="sxs-lookup"><span data-stu-id="2365e-110">Description</span></span>                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="2365e-111">dialinUrl</span><span class="sxs-lookup"><span data-stu-id="2365e-111">dialinUrl</span></span>           | <span data-ttu-id="2365e-112">字符串</span><span class="sxs-lookup"><span data-stu-id="2365e-112">String</span></span>  | <span data-ttu-id="2365e-113">指向包含拨入信息的可从外部访问网页的 URL。</span><span class="sxs-lookup"><span data-stu-id="2365e-113">A URL to the externally-accessible web page that contains dial-in information.</span></span> |
| <span data-ttu-id="2365e-114">leaderPasscode</span><span class="sxs-lookup"><span data-stu-id="2365e-114">leaderPasscode</span></span>      | <span data-ttu-id="2365e-115">字符串</span><span class="sxs-lookup"><span data-stu-id="2365e-115">String</span></span>  | <span data-ttu-id="2365e-116">连接到音频会议提供商所需的主持人密码。</span><span class="sxs-lookup"><span data-stu-id="2365e-116">The leader password required to connect to the Audio Conference Provider.</span></span>      |
| <span data-ttu-id="2365e-117">participantPasscode</span><span class="sxs-lookup"><span data-stu-id="2365e-117">participantPasscode</span></span> | <span data-ttu-id="2365e-118">字符串</span><span class="sxs-lookup"><span data-stu-id="2365e-118">String</span></span>  | <span data-ttu-id="2365e-119">连接到音频会议提供商所需的参与者密码。</span><span class="sxs-lookup"><span data-stu-id="2365e-119">The participant password required to connect to the Audio Conference Provider.</span></span> |
| <span data-ttu-id="2365e-120">tollFreeNumber</span><span class="sxs-lookup"><span data-stu-id="2365e-120">tollFreeNumber</span></span>      | <span data-ttu-id="2365e-121">字符串</span><span class="sxs-lookup"><span data-stu-id="2365e-121">String</span></span>  | <span data-ttu-id="2365e-122">要连接到音频会议提供商的免费电话号码。</span><span class="sxs-lookup"><span data-stu-id="2365e-122">The toll-free number to connect to the Audio Conference Provider.</span></span>              |
| <span data-ttu-id="2365e-123">tollNumber</span><span class="sxs-lookup"><span data-stu-id="2365e-123">tollNumber</span></span>          | <span data-ttu-id="2365e-124">字符串</span><span class="sxs-lookup"><span data-stu-id="2365e-124">String</span></span>  | <span data-ttu-id="2365e-125">要连接到音频会议提供商的收费电话号码。</span><span class="sxs-lookup"><span data-stu-id="2365e-125">The toll number to connect to the Audio Conference Provider.</span></span>                   |

## <a name="json-representation"></a><span data-ttu-id="2365e-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2365e-126">JSON representation</span></span>

<span data-ttu-id="2365e-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2365e-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioConferencing"
}-->
```json
{
  "dialinUrl": "String",
  "leaderPasscode": "String",
  "participantPasscode": "String",
  "tollFreeNumber": "String",
  "tollNumber": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "audioConferencing resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
