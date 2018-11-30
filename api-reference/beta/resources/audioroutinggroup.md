---
title: audioRoutingGroup 资源类型
description: 音频路由组存储在进行多方对话中的参与者之间的专用音频路由。 源是参与者本身而接收器是进行多方对话中的其他参与者的子集。
ms.openlocfilehash: 98c58e39773567f13a2723e94c0413efd2841cd0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041830"
---
# <a name="audioroutinggroup-resource-type"></a><span data-ttu-id="b7580-104">audioRoutingGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="b7580-104">audioRoutingGroup resource type</span></span>

> <span data-ttu-id="b7580-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b7580-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b7580-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b7580-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b7580-107">音频路由组存储在进行多方对话中的参与者之间的专用音频路由。</span><span class="sxs-lookup"><span data-stu-id="b7580-107">The audio routing group stores a private audio route between participants in a multiparty conversation.</span></span> <span data-ttu-id="b7580-108">源是参与者本身而接收器是进行多方对话中的其他参与者的子集。</span><span class="sxs-lookup"><span data-stu-id="b7580-108">Source is the participant itself and the receivers are a subset of other participants in the multiparty conversation.</span></span>

> <span data-ttu-id="b7580-109">**注意：**[ConfigureMixer](../api/participant-configuremixer.md)不涉及任何路由，用于整个呼叫设置源接收器组合的音量级别。</span><span class="sxs-lookup"><span data-stu-id="b7580-109">**Note:** [ConfigureMixer](../api/participant-configuremixer.md) does not involve any routes, it is for the entire call for setting the volume levels for source-receiver combinations.</span></span>

## <a name="methods"></a><span data-ttu-id="b7580-110">方法</span><span class="sxs-lookup"><span data-stu-id="b7580-110">Methods</span></span>

| <span data-ttu-id="b7580-111">方法</span><span class="sxs-lookup"><span data-stu-id="b7580-111">Method</span></span>                                                  | <span data-ttu-id="b7580-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="b7580-112">Return Type</span></span>                               | <span data-ttu-id="b7580-113">说明</span><span class="sxs-lookup"><span data-stu-id="b7580-113">Description</span></span>                                  |
|:--------------------------------------------------------|:------------------------------------------|:---------------------------------------------|
| [<span data-ttu-id="b7580-114">获取 audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="b7580-114">Get audioRoutingGroup</span></span>](../api/audioroutinggroup-get.md)| [<span data-ttu-id="b7580-115">audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="b7580-115">audioRoutingGroup</span></span>](audioroutinggroup.md) | <span data-ttu-id="b7580-116">读取属性和 audioRoutingGroup 对象的关系。</span><span class="sxs-lookup"><span data-stu-id="b7580-116">Read properties and relationships of audioRoutingGroup object.</span></span>|
| [<span data-ttu-id="b7580-117">Update</span><span class="sxs-lookup"><span data-stu-id="b7580-117">Update</span></span>](../api/audioroutinggroup-update.md)            | [<span data-ttu-id="b7580-118">audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="b7580-118">audioRoutingGroup</span></span>](audioroutinggroup.md) | <span data-ttu-id="b7580-119">更新接收器列表。</span><span class="sxs-lookup"><span data-stu-id="b7580-119">Update receivers list.</span></span>                       |
| [<span data-ttu-id="b7580-120">删除</span><span class="sxs-lookup"><span data-stu-id="b7580-120">Delete</span></span>](../api/audioroutinggroup-delete.md)            | <span data-ttu-id="b7580-121">无</span><span class="sxs-lookup"><span data-stu-id="b7580-121">None</span></span>                                      | <span data-ttu-id="b7580-122">音频路由组中删除。</span><span class="sxs-lookup"><span data-stu-id="b7580-122">Delete the audio routing group.</span></span>              |

## <a name="properties"></a><span data-ttu-id="b7580-123">属性</span><span class="sxs-lookup"><span data-stu-id="b7580-123">Properties</span></span>

| <span data-ttu-id="b7580-124">属性</span><span class="sxs-lookup"><span data-stu-id="b7580-124">Property</span></span>      | <span data-ttu-id="b7580-125">类型</span><span class="sxs-lookup"><span data-stu-id="b7580-125">Type</span></span>              | <span data-ttu-id="b7580-126">说明</span><span class="sxs-lookup"><span data-stu-id="b7580-126">Description</span></span>                                                          |
| :----------   | :---------------- | :--------------------------------------------------------------------|
| <span data-ttu-id="b7580-127">id</span><span class="sxs-lookup"><span data-stu-id="b7580-127">id</span></span>            | <span data-ttu-id="b7580-128">String</span><span class="sxs-lookup"><span data-stu-id="b7580-128">String</span></span>            | <span data-ttu-id="b7580-129">只读。</span><span class="sxs-lookup"><span data-stu-id="b7580-129">Read-only.</span></span> <span data-ttu-id="b7580-130">生成的服务器。</span><span class="sxs-lookup"><span data-stu-id="b7580-130">Server generated.</span></span>                                         |
| <span data-ttu-id="b7580-131">接收器</span><span class="sxs-lookup"><span data-stu-id="b7580-131">receivers</span></span>     | <span data-ttu-id="b7580-132">字符串集合</span><span class="sxs-lookup"><span data-stu-id="b7580-132">String Collection</span></span> | <span data-ttu-id="b7580-133">接收参与者 id 的列表。</span><span class="sxs-lookup"><span data-stu-id="b7580-133">List of receiving participant ids.</span></span>                                   |
| <span data-ttu-id="b7580-134">routingMode</span><span class="sxs-lookup"><span data-stu-id="b7580-134">routingMode</span></span>   | <span data-ttu-id="b7580-135">字符串</span><span class="sxs-lookup"><span data-stu-id="b7580-135">String</span></span>            | <span data-ttu-id="b7580-136">路由组模式。</span><span class="sxs-lookup"><span data-stu-id="b7580-136">Routing group mode.</span></span>  <span data-ttu-id="b7580-137">可取值为：`oneToOne`、`multicast`。</span><span class="sxs-lookup"><span data-stu-id="b7580-137">Possible values are: `oneToOne`, `multicast`.</span></span>   |
| <span data-ttu-id="b7580-138">sources</span><span class="sxs-lookup"><span data-stu-id="b7580-138">sources</span></span>       | <span data-ttu-id="b7580-139">字符串集合</span><span class="sxs-lookup"><span data-stu-id="b7580-139">String Collection</span></span> | <span data-ttu-id="b7580-140">源参与者 id 的列表。</span><span class="sxs-lookup"><span data-stu-id="b7580-140">List of source participant ids.</span></span>                                      |

> <span data-ttu-id="b7580-141">**注意：** 路由模式确定源和接收器的限制。</span><span class="sxs-lookup"><span data-stu-id="b7580-141">**Note:** Routing mode determines the restrictions on the sources and receivers.</span></span> <span data-ttu-id="b7580-142">支持以下路由组。</span><span class="sxs-lookup"><span data-stu-id="b7580-142">Only the following routing groups are supported.</span></span>
> - <span data-ttu-id="b7580-143">`oneToOne`-源和接收器具有只有一个参与者。</span><span class="sxs-lookup"><span data-stu-id="b7580-143">`oneToOne` - sources and receivers have only one participant each.</span></span>
> - <span data-ttu-id="b7580-144">`multicast`-源有一个参与者，但有多个接收器。</span><span class="sxs-lookup"><span data-stu-id="b7580-144">`multicast` - source has one participant but there are multiple receivers.</span></span> <span data-ttu-id="b7580-145">接收器列表可能会更新。</span><span class="sxs-lookup"><span data-stu-id="b7580-145">Receivers list may be updated.</span></span>

> <span data-ttu-id="b7580-146">**注意：** 如果创建许多音频路由组 （例如每个参与者自动程序），则将被转接仅顶部 4 基准扬声器的音频。</span><span class="sxs-lookup"><span data-stu-id="b7580-146">**Note:** If you create many audio routing groups (e.g. a bot per participant), only the audio of the top 4 dominant speakers is forwarded.</span></span> <span data-ttu-id="b7580-147">它与自定义音频路由组，即使意味着，如果扬声器不调节主混音器中，即使仅为此扬声器和自动程序的专用音频组他/她不能通过 bot 听到。</span><span class="sxs-lookup"><span data-stu-id="b7580-147">It means even with customized audio routing group, if the speaker is not loud enough in the main mixer, he/she cannot be heard by the bot even if there is a private audio group just for this speaker and the bot.</span></span>

## <a name="relationships"></a><span data-ttu-id="b7580-148">Relationships</span><span class="sxs-lookup"><span data-stu-id="b7580-148">Relationships</span></span>
<span data-ttu-id="b7580-149">无</span><span class="sxs-lookup"><span data-stu-id="b7580-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b7580-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b7580-150">JSON representation</span></span>

<span data-ttu-id="b7580-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b7580-151">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "audioRoutingGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
