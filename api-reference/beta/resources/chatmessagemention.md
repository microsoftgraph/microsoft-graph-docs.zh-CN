---
title: chatMessageMention 资源类型
description: '表示 chatMessage 实体中的提及。 这些提及适用于用户、团队、机器人或频道。 '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e4b6ce12589525e7ddb471f5744d68539c905f3d
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819719"
---
# <a name="chatmessagemention-resource-type"></a><span data-ttu-id="b8841-104">chatMessageMention 资源类型</span><span class="sxs-lookup"><span data-stu-id="b8841-104">chatMessageMention resource type</span></span>

<span data-ttu-id="b8841-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8841-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8841-106">表示 chatMessage 实体中的 [提及](chatmessage.md) 。</span><span class="sxs-lookup"><span data-stu-id="b8841-106">Represents a mention in a [chatMessage](chatmessage.md) entity.</span></span> <span data-ttu-id="b8841-107">提及可以是对用户[、](user.md)[团队、机](team.md)器人[或频道的](channel.md)。</span><span class="sxs-lookup"><span data-stu-id="b8841-107">The mention can be to a [user](user.md), [team](team.md), bot, or [channel](channel.md).</span></span> 

<span data-ttu-id="b8841-108">在包含 **一** 个或多个提及的 chatMessage 对象中，消息正文 **内容** 属性表示 HTML 形式的聊天消息。</span><span class="sxs-lookup"><span data-stu-id="b8841-108">In a **chatMessage** object that contains one or more mentions, the message body **content** property represents the chat message in HTML.</span></span> <span data-ttu-id="b8841-109">它将每 **提及的提及文本** 包包在 HTML 元素内 `at` ，并 `id` 具有对应于提及 id 属性 **（Property）** 的属性 （Attribute）。</span><span class="sxs-lookup"><span data-stu-id="b8841-109">It encloses the **mentionText** of each mention in an HTML `at` element, with an `id` attribute that corresponds to the **id** property of the mention.</span></span>

<span data-ttu-id="b8841-110">例如，一条聊天消息包含两个提及文字，分说明文字分为"Megan"和"Alex"。</span><span class="sxs-lookup"><span data-stu-id="b8841-110">As an example, a chat message contains two mentions, with the mention text "Megan" and "Alex" respectively.</span></span> <span data-ttu-id="b8841-111">它的 **正文** 内容属性 `at` 指定这两个提及的元素，如下所示：</span><span class="sxs-lookup"><span data-stu-id="b8841-111">Its body **content** property specifies `at` elements for the two mentions as follows:</span></span>

``` json
"body": {
    "contentType": "html",
    "content": "<div><div>Ah, <at id=\"0\">Megan</at>, <at id=\"1\">Alex</at>, I saw them in a separate folder. Thanks!</div>\n</div>"
}
```

<span data-ttu-id="b8841-112">在 content **属性中** ，第一个提及具有 HTML `id` 特性 0。</span><span class="sxs-lookup"><span data-stu-id="b8841-112">In the **content** property, the first mention has an HTML `id` attribute of 0.</span></span> <span data-ttu-id="b8841-113">此属性对应于**chatMessageMention**的第一个实例的**id**属性，也是 0。</span><span class="sxs-lookup"><span data-stu-id="b8841-113">This corresponds to the **id** property of that first instance of **chatMessageMention**, which is also 0.</span></span>

<span data-ttu-id="b8841-114">第二次提及具有 `id` 1 特性，它与第二个实例的 **id** 属性相匹配，即 1。</span><span class="sxs-lookup"><span data-stu-id="b8841-114">The second mention has an `id` attribute of 1, matching the **id** property of the second instance, which is 1.</span></span>

<span data-ttu-id="b8841-115">有关该示例的更全上下文，请参阅["列表频道消息回复"。](../api/channel-list-messagereplies.md#example)</span><span class="sxs-lookup"><span data-stu-id="b8841-115">For a fuller context of the example, see [List channel message replies](../api/channel-list-messagereplies.md#example).</span></span>

## <a name="properties"></a><span data-ttu-id="b8841-116">属性</span><span class="sxs-lookup"><span data-stu-id="b8841-116">Properties</span></span>
| <span data-ttu-id="b8841-117">属性</span><span class="sxs-lookup"><span data-stu-id="b8841-117">Property</span></span>     | <span data-ttu-id="b8841-118">类型</span><span class="sxs-lookup"><span data-stu-id="b8841-118">Type</span></span>   |<span data-ttu-id="b8841-119">说明</span><span class="sxs-lookup"><span data-stu-id="b8841-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b8841-120">id</span><span class="sxs-lookup"><span data-stu-id="b8841-120">id</span></span>|<span data-ttu-id="b8841-121">Int32</span><span class="sxs-lookup"><span data-stu-id="b8841-121">Int32</span></span>|<span data-ttu-id="b8841-122">指定 chatMessage 中提及的实体 **的索引**。</span><span class="sxs-lookup"><span data-stu-id="b8841-122">Index of an entity being mentioned in the specified **chatMessage**.</span></span> <span data-ttu-id="b8841-123">匹配邮件正文中相应标记中的 {index} `<at id="{index}">` 值。</span><span class="sxs-lookup"><span data-stu-id="b8841-123">Matches the {index} value in the corresponding `<at id="{index}">` tag in the message body.</span></span>|
|<span data-ttu-id="b8841-124">mentionText</span><span class="sxs-lookup"><span data-stu-id="b8841-124">mentionText</span></span>|<span data-ttu-id="b8841-125">string</span><span class="sxs-lookup"><span data-stu-id="b8841-125">string</span></span>|<span data-ttu-id="b8841-126">用于表示提及的字符串。</span><span class="sxs-lookup"><span data-stu-id="b8841-126">String used to represent the mention.</span></span> <span data-ttu-id="b8841-127">例如，用户的显示名称组名称。</span><span class="sxs-lookup"><span data-stu-id="b8841-127">For example, a user's display name, a team name.</span></span>|
|<span data-ttu-id="b8841-128">提及</span><span class="sxs-lookup"><span data-stu-id="b8841-128">mentioned</span></span>|[<span data-ttu-id="b8841-129">identitySet</span><span class="sxs-lookup"><span data-stu-id="b8841-129">identitySet</span></span>](identityset.md)|<span data-ttu-id="b8841-130">实体的 (提及的用户、应用程序) 团队或频道。</span><span class="sxs-lookup"><span data-stu-id="b8841-130">The entity (user, application, team, or channel) that was mentioned.</span></span>  <span data-ttu-id="b8841-131">如果是已有空的频道或 @mentioned团队，则 IdentitySet 包含 **为** 团队/频道提供 ID 的对话属性和一个 **conversationIdentityType** 属性，代表团队或频道。</span><span class="sxs-lookup"><span data-stu-id="b8841-131">If it was a channel or team that was @mentioned, the identitySet contains a **conversation** property giving the ID of the team/channel, and a **conversationIdentityType** property that represents either the team or channel.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="b8841-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b8841-132">JSON representation</span></span>

<span data-ttu-id="b8841-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b8841-133">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.chatMessageMention"
}-->

```json
{
  "id": 1024,
  "mentionText": "string",
  "mentioned": {"@odata.type": "microsoft.graph.identitySet"}
 }
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chat mention resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
