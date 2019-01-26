---
title: audioRoutingGroup 资源类型
description: 音频路由组存储在进行多方对话中的参与者之间的专用音频路由。 源是参与者本身而接收器是进行多方对话中的其他参与者的子集。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: fb1303e2a6f9e269faf5767093d418cdd0980463
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573016"
---
# <a name="audioroutinggroup-resource-type"></a><span data-ttu-id="d920f-104">audioRoutingGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="d920f-104">audioRoutingGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d920f-105">音频路由组存储在进行多方对话中的参与者之间的专用音频路由。</span><span class="sxs-lookup"><span data-stu-id="d920f-105">The audio routing group stores a private audio route between participants in a multiparty conversation.</span></span> <span data-ttu-id="d920f-106">源是参与者本身而接收器是进行多方对话中的其他参与者的子集。</span><span class="sxs-lookup"><span data-stu-id="d920f-106">Source is the participant itself and the receivers are a subset of other participants in the multiparty conversation.</span></span>

> <span data-ttu-id="d920f-107">**注意：**[ConfigureMixer](../api/participant-configuremixer.md)不涉及任何路由，用于整个呼叫设置源接收器组合的音量级别。</span><span class="sxs-lookup"><span data-stu-id="d920f-107">**Note:** [ConfigureMixer](../api/participant-configuremixer.md) does not involve any routes, it is for the entire call for setting the volume levels for source-receiver combinations.</span></span>

## <a name="methods"></a><span data-ttu-id="d920f-108">方法</span><span class="sxs-lookup"><span data-stu-id="d920f-108">Methods</span></span>

| <span data-ttu-id="d920f-109">方法</span><span class="sxs-lookup"><span data-stu-id="d920f-109">Method</span></span>                                                  | <span data-ttu-id="d920f-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="d920f-110">Return Type</span></span>                               | <span data-ttu-id="d920f-111">说明</span><span class="sxs-lookup"><span data-stu-id="d920f-111">Description</span></span>                                  |
|:--------------------------------------------------------|:------------------------------------------|:---------------------------------------------|
| [<span data-ttu-id="d920f-112">获取 audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="d920f-112">Get audioRoutingGroup</span></span>](../api/audioroutinggroup-get.md)| [<span data-ttu-id="d920f-113">audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="d920f-113">audioRoutingGroup</span></span>](audioroutinggroup.md) | <span data-ttu-id="d920f-114">读取属性和 audioRoutingGroup 对象的关系。</span><span class="sxs-lookup"><span data-stu-id="d920f-114">Read properties and relationships of audioRoutingGroup object.</span></span>|
| [<span data-ttu-id="d920f-115">Update</span><span class="sxs-lookup"><span data-stu-id="d920f-115">Update</span></span>](../api/audioroutinggroup-update.md)            | [<span data-ttu-id="d920f-116">audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="d920f-116">audioRoutingGroup</span></span>](audioroutinggroup.md) | <span data-ttu-id="d920f-117">更新接收器列表。</span><span class="sxs-lookup"><span data-stu-id="d920f-117">Update receivers list.</span></span>                       |
| [<span data-ttu-id="d920f-118">Delete</span><span class="sxs-lookup"><span data-stu-id="d920f-118">Delete</span></span>](../api/audioroutinggroup-delete.md)            | <span data-ttu-id="d920f-119">无</span><span class="sxs-lookup"><span data-stu-id="d920f-119">None</span></span>                                      | <span data-ttu-id="d920f-120">音频路由组中删除。</span><span class="sxs-lookup"><span data-stu-id="d920f-120">Delete the audio routing group.</span></span>              |

## <a name="properties"></a><span data-ttu-id="d920f-121">属性</span><span class="sxs-lookup"><span data-stu-id="d920f-121">Properties</span></span>

| <span data-ttu-id="d920f-122">属性</span><span class="sxs-lookup"><span data-stu-id="d920f-122">Property</span></span>      | <span data-ttu-id="d920f-123">类型</span><span class="sxs-lookup"><span data-stu-id="d920f-123">Type</span></span>              | <span data-ttu-id="d920f-124">说明</span><span class="sxs-lookup"><span data-stu-id="d920f-124">Description</span></span>                                                          |
| :----------   | :---------------- | :--------------------------------------------------------------------|
| <span data-ttu-id="d920f-125">id</span><span class="sxs-lookup"><span data-stu-id="d920f-125">id</span></span>            | <span data-ttu-id="d920f-126">String</span><span class="sxs-lookup"><span data-stu-id="d920f-126">String</span></span>            | <span data-ttu-id="d920f-127">只读。</span><span class="sxs-lookup"><span data-stu-id="d920f-127">Read-only.</span></span> <span data-ttu-id="d920f-128">由服务器生成。</span><span class="sxs-lookup"><span data-stu-id="d920f-128">Server generated.</span></span>                                         |
| <span data-ttu-id="d920f-129">接收器</span><span class="sxs-lookup"><span data-stu-id="d920f-129">receivers</span></span>     | <span data-ttu-id="d920f-130">String 集合</span><span class="sxs-lookup"><span data-stu-id="d920f-130">String Collection</span></span> | <span data-ttu-id="d920f-131">接收参与者 id 的列表。</span><span class="sxs-lookup"><span data-stu-id="d920f-131">List of receiving participant ids.</span></span>                                   |
| <span data-ttu-id="d920f-132">routingMode</span><span class="sxs-lookup"><span data-stu-id="d920f-132">routingMode</span></span>   | <span data-ttu-id="d920f-133">String</span><span class="sxs-lookup"><span data-stu-id="d920f-133">String</span></span>            | <span data-ttu-id="d920f-134">路由组模式。</span><span class="sxs-lookup"><span data-stu-id="d920f-134">Routing group mode.</span></span>  <span data-ttu-id="d920f-135">可取值为：`oneToOne`、`multicast`。</span><span class="sxs-lookup"><span data-stu-id="d920f-135">Possible values are: `oneToOne`, `multicast`.</span></span>   |
| <span data-ttu-id="d920f-136">sources</span><span class="sxs-lookup"><span data-stu-id="d920f-136">sources</span></span>       | <span data-ttu-id="d920f-137">String 集合</span><span class="sxs-lookup"><span data-stu-id="d920f-137">String Collection</span></span> | <span data-ttu-id="d920f-138">源参与者 id 的列表。</span><span class="sxs-lookup"><span data-stu-id="d920f-138">List of source participant ids.</span></span>                                      |

> <span data-ttu-id="d920f-139">**注意：** 路由模式确定源和接收器的限制。</span><span class="sxs-lookup"><span data-stu-id="d920f-139">**Note:** Routing mode determines the restrictions on the sources and receivers.</span></span> <span data-ttu-id="d920f-140">支持以下路由组。</span><span class="sxs-lookup"><span data-stu-id="d920f-140">Only the following routing groups are supported.</span></span>
> - <span data-ttu-id="d920f-141">`oneToOne`-源和接收器具有只有一个参与者。</span><span class="sxs-lookup"><span data-stu-id="d920f-141">`oneToOne` - sources and receivers have only one participant each.</span></span>
> - <span data-ttu-id="d920f-142">`multicast`-源有一个参与者，但有多个接收器。</span><span class="sxs-lookup"><span data-stu-id="d920f-142">`multicast` - source has one participant but there are multiple receivers.</span></span> <span data-ttu-id="d920f-143">接收器列表可能会更新。</span><span class="sxs-lookup"><span data-stu-id="d920f-143">Receivers list may be updated.</span></span>

> <span data-ttu-id="d920f-144">**注意：** 如果创建许多音频路由组 （例如每个参与者自动程序），则将被转接仅顶部 4 基准扬声器的音频。</span><span class="sxs-lookup"><span data-stu-id="d920f-144">**Note:** If you create many audio routing groups (e.g. a bot per participant), only the audio of the top 4 dominant speakers is forwarded.</span></span> <span data-ttu-id="d920f-145">它与自定义音频路由组，即使意味着，如果扬声器不调节主混音器中，即使仅为此扬声器和自动程序的专用音频组他/她不能通过 bot 听到。</span><span class="sxs-lookup"><span data-stu-id="d920f-145">It means even with customized audio routing group, if the speaker is not loud enough in the main mixer, he/she cannot be heard by the bot even if there is a private audio group just for this speaker and the bot.</span></span>

## <a name="relationships"></a><span data-ttu-id="d920f-146">关系</span><span class="sxs-lookup"><span data-stu-id="d920f-146">Relationships</span></span>
<span data-ttu-id="d920f-147">无</span><span class="sxs-lookup"><span data-stu-id="d920f-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d920f-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d920f-148">JSON representation</span></span>

<span data-ttu-id="d920f-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d920f-149">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioRoutingGroup"
}-->
```json
{
  "id": "String (identifier)",
  "receivers": [ "Guid" ],
  "routingMode": "oneToOne | multicast",
  "sources": [ "Guid" ]
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
