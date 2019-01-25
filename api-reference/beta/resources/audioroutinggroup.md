---
title: audioRoutingGroup 资源类型
description: 音频路由组存储在进行多方对话中的参与者之间的专用音频路由。 源是参与者本身而接收器是进行多方对话中的其他参与者的子集。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e7fc7de5b5caaa2f4079c453f9cd855a42577cb8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509621"
---
# <a name="audioroutinggroup-resource-type"></a><span data-ttu-id="9db46-104">audioRoutingGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="9db46-104">audioRoutingGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9db46-105">音频路由组存储在进行多方对话中的参与者之间的专用音频路由。</span><span class="sxs-lookup"><span data-stu-id="9db46-105">The audio routing group stores a private audio route between participants in a multiparty conversation.</span></span> <span data-ttu-id="9db46-106">源是参与者本身而接收器是进行多方对话中的其他参与者的子集。</span><span class="sxs-lookup"><span data-stu-id="9db46-106">Source is the participant itself and the receivers are a subset of other participants in the multiparty conversation.</span></span>

> <span data-ttu-id="9db46-107">**注意：**[ConfigureMixer](../api/participant-configuremixer.md)不涉及任何路由，用于整个呼叫设置源接收器组合的音量级别。</span><span class="sxs-lookup"><span data-stu-id="9db46-107">**Note:** [ConfigureMixer](../api/participant-configuremixer.md) does not involve any routes, it is for the entire call for setting the volume levels for source-receiver combinations.</span></span>

## <a name="methods"></a><span data-ttu-id="9db46-108">方法</span><span class="sxs-lookup"><span data-stu-id="9db46-108">Methods</span></span>

| <span data-ttu-id="9db46-109">方法</span><span class="sxs-lookup"><span data-stu-id="9db46-109">Method</span></span>                                                  | <span data-ttu-id="9db46-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="9db46-110">Return Type</span></span>                               | <span data-ttu-id="9db46-111">说明</span><span class="sxs-lookup"><span data-stu-id="9db46-111">Description</span></span>                                  |
|:--------------------------------------------------------|:------------------------------------------|:---------------------------------------------|
| [<span data-ttu-id="9db46-112">获取 audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="9db46-112">Get audioRoutingGroup</span></span>](../api/audioroutinggroup-get.md)| [<span data-ttu-id="9db46-113">audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="9db46-113">audioRoutingGroup</span></span>](audioroutinggroup.md) | <span data-ttu-id="9db46-114">读取属性和 audioRoutingGroup 对象的关系。</span><span class="sxs-lookup"><span data-stu-id="9db46-114">Read properties and relationships of audioRoutingGroup object.</span></span>|
| [<span data-ttu-id="9db46-115">Update</span><span class="sxs-lookup"><span data-stu-id="9db46-115">Update</span></span>](../api/audioroutinggroup-update.md)            | [<span data-ttu-id="9db46-116">audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="9db46-116">audioRoutingGroup</span></span>](audioroutinggroup.md) | <span data-ttu-id="9db46-117">更新接收器列表。</span><span class="sxs-lookup"><span data-stu-id="9db46-117">Update receivers list.</span></span>                       |
| [<span data-ttu-id="9db46-118">删除</span><span class="sxs-lookup"><span data-stu-id="9db46-118">Delete</span></span>](../api/audioroutinggroup-delete.md)            | <span data-ttu-id="9db46-119">无</span><span class="sxs-lookup"><span data-stu-id="9db46-119">None</span></span>                                      | <span data-ttu-id="9db46-120">音频路由组中删除。</span><span class="sxs-lookup"><span data-stu-id="9db46-120">Delete the audio routing group.</span></span>              |

## <a name="properties"></a><span data-ttu-id="9db46-121">属性</span><span class="sxs-lookup"><span data-stu-id="9db46-121">Properties</span></span>

| <span data-ttu-id="9db46-122">属性</span><span class="sxs-lookup"><span data-stu-id="9db46-122">Property</span></span>      | <span data-ttu-id="9db46-123">类型</span><span class="sxs-lookup"><span data-stu-id="9db46-123">Type</span></span>              | <span data-ttu-id="9db46-124">说明</span><span class="sxs-lookup"><span data-stu-id="9db46-124">Description</span></span>                                                          |
| :----------   | :---------------- | :--------------------------------------------------------------------|
| <span data-ttu-id="9db46-125">id</span><span class="sxs-lookup"><span data-stu-id="9db46-125">id</span></span>            | <span data-ttu-id="9db46-126">String</span><span class="sxs-lookup"><span data-stu-id="9db46-126">String</span></span>            | <span data-ttu-id="9db46-127">只读。</span><span class="sxs-lookup"><span data-stu-id="9db46-127">Read-only.</span></span> <span data-ttu-id="9db46-128">生成的服务器。</span><span class="sxs-lookup"><span data-stu-id="9db46-128">Server generated.</span></span>                                         |
| <span data-ttu-id="9db46-129">接收器</span><span class="sxs-lookup"><span data-stu-id="9db46-129">receivers</span></span>     | <span data-ttu-id="9db46-130">字符串集合</span><span class="sxs-lookup"><span data-stu-id="9db46-130">String Collection</span></span> | <span data-ttu-id="9db46-131">接收参与者 id 的列表。</span><span class="sxs-lookup"><span data-stu-id="9db46-131">List of receiving participant ids.</span></span>                                   |
| <span data-ttu-id="9db46-132">routingMode</span><span class="sxs-lookup"><span data-stu-id="9db46-132">routingMode</span></span>   | <span data-ttu-id="9db46-133">String</span><span class="sxs-lookup"><span data-stu-id="9db46-133">String</span></span>            | <span data-ttu-id="9db46-134">路由组模式。</span><span class="sxs-lookup"><span data-stu-id="9db46-134">Routing group mode.</span></span>  <span data-ttu-id="9db46-135">可取值为：`oneToOne`、`multicast`。</span><span class="sxs-lookup"><span data-stu-id="9db46-135">Possible values are: `oneToOne`, `multicast`.</span></span>   |
| <span data-ttu-id="9db46-136">sources</span><span class="sxs-lookup"><span data-stu-id="9db46-136">sources</span></span>       | <span data-ttu-id="9db46-137">字符串集合</span><span class="sxs-lookup"><span data-stu-id="9db46-137">String Collection</span></span> | <span data-ttu-id="9db46-138">源参与者 id 的列表。</span><span class="sxs-lookup"><span data-stu-id="9db46-138">List of source participant ids.</span></span>                                      |

> <span data-ttu-id="9db46-139">**注意：** 路由模式确定源和接收器的限制。</span><span class="sxs-lookup"><span data-stu-id="9db46-139">**Note:** Routing mode determines the restrictions on the sources and receivers.</span></span> <span data-ttu-id="9db46-140">支持以下路由组。</span><span class="sxs-lookup"><span data-stu-id="9db46-140">Only the following routing groups are supported.</span></span>
> - <span data-ttu-id="9db46-141">`oneToOne`-源和接收器具有只有一个参与者。</span><span class="sxs-lookup"><span data-stu-id="9db46-141">`oneToOne` - sources and receivers have only one participant each.</span></span>
> - <span data-ttu-id="9db46-142">`multicast`-源有一个参与者，但有多个接收器。</span><span class="sxs-lookup"><span data-stu-id="9db46-142">`multicast` - source has one participant but there are multiple receivers.</span></span> <span data-ttu-id="9db46-143">接收器列表可能会更新。</span><span class="sxs-lookup"><span data-stu-id="9db46-143">Receivers list may be updated.</span></span>

> <span data-ttu-id="9db46-144">**注意：** 如果创建许多音频路由组 （例如每个参与者自动程序），则将被转接仅顶部 4 基准扬声器的音频。</span><span class="sxs-lookup"><span data-stu-id="9db46-144">**Note:** If you create many audio routing groups (e.g. a bot per participant), only the audio of the top 4 dominant speakers is forwarded.</span></span> <span data-ttu-id="9db46-145">它与自定义音频路由组，即使意味着，如果扬声器不调节主混音器中，即使仅为此扬声器和自动程序的专用音频组他/她不能通过 bot 听到。</span><span class="sxs-lookup"><span data-stu-id="9db46-145">It means even with customized audio routing group, if the speaker is not loud enough in the main mixer, he/she cannot be heard by the bot even if there is a private audio group just for this speaker and the bot.</span></span>

## <a name="relationships"></a><span data-ttu-id="9db46-146">关系</span><span class="sxs-lookup"><span data-stu-id="9db46-146">Relationships</span></span>
<span data-ttu-id="9db46-147">无</span><span class="sxs-lookup"><span data-stu-id="9db46-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9db46-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9db46-148">JSON representation</span></span>

<span data-ttu-id="9db46-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9db46-149">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioRoutingGroup"
}-->
```json
{
  "id": "String (identifier)",
  "receivers": [ "String" ],
  "routingMode": "oneToOne | multicast",
  "sources": [ "String" ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "audioRoutingGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/audioroutinggroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
