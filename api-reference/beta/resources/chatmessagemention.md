---
title: chatMessageMention 资源类型
description: '表示 chatMessage 实体中的提及。 提及内容可以提及用户、团队、机器人或频道。 '
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: fefa80cf6fa66b61a3db8457f5b7f8809b07e2f3
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207005"
---
# <a name="chatmessagemention-resource-type"></a><span data-ttu-id="b6ce4-104">chatMessageMention 资源类型</span><span class="sxs-lookup"><span data-stu-id="b6ce4-104">chatMessageMention resource type</span></span>

<span data-ttu-id="b6ce4-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6ce4-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6ce4-106">表示 [chatMessage 实体中的](chatmessage.md) 提及。</span><span class="sxs-lookup"><span data-stu-id="b6ce4-106">Represents a mention in a [chatMessage](chatmessage.md) entity.</span></span> <span data-ttu-id="b6ce4-107">提及的内容可以是用户[、](user.md)[团队、](team.md)机器人或[频道](channel.md)。</span><span class="sxs-lookup"><span data-stu-id="b6ce4-107">The mention can be to a [user](user.md), [team](team.md), bot, or [channel](channel.md).</span></span> 

<span data-ttu-id="b6ce4-108">在包含 **一个或多个提及内容的 chatMessage** 对象中，消息正文 **内容** 属性表示 HTML 格式的聊天消息。</span><span class="sxs-lookup"><span data-stu-id="b6ce4-108">In a **chatMessage** object that contains one or more mentions, the message body **content** property represents the chat message in HTML.</span></span> <span data-ttu-id="b6ce4-109">它将每个 **提及的内容的 mentionText** 包含在 HTML 元素中，并包含对应于提及项 `at` 的 `id` **id** 属性的属性。</span><span class="sxs-lookup"><span data-stu-id="b6ce4-109">It encloses the **mentionText** of each mention in an HTML `at` element, with an `id` attribute that corresponds to the **id** property of the mention.</span></span>

<span data-ttu-id="b6ce4-110">例如，聊天消息包含两个提及内容，分别包含提及文本"Megan"和"Alex"。</span><span class="sxs-lookup"><span data-stu-id="b6ce4-110">As an example, a chat message contains two mentions, with the mention text "Megan" and "Alex" respectively.</span></span> <span data-ttu-id="b6ce4-111">其 body **content** 属性 `at` 指定两个提及项的元素，如下所示：</span><span class="sxs-lookup"><span data-stu-id="b6ce4-111">Its body **content** property specifies `at` elements for the two mentions as follows:</span></span>

``` json
"body": {
    "contentType": "html",
    "content": "<div><div>Ah, <at id=\"0\">Megan</at>, <at id=\"1\">Alex</at>, I saw them in a separate folder. Thanks!</div>\n</div>"
}
```

<span data-ttu-id="b6ce4-112">在 **content** 属性中，第一个提及具有 HTML `id` 属性 0。</span><span class="sxs-lookup"><span data-stu-id="b6ce4-112">In the **content** property, the first mention has an HTML `id` attribute of 0.</span></span> <span data-ttu-id="b6ce4-113">这对应于 **chatMessageMention** 的第一个实例的 **id** 属性，这也是 0。</span><span class="sxs-lookup"><span data-stu-id="b6ce4-113">This corresponds to the **id** property of that first instance of **chatMessageMention**, which is also 0.</span></span>

<span data-ttu-id="b6ce4-114">第二个提及具有与第二个实例的 id 属性匹配的属性 `id` 1，即 1。 </span><span class="sxs-lookup"><span data-stu-id="b6ce4-114">The second mention has an `id` attribute of 1, matching the **id** property of the second instance, which is 1.</span></span>

<span data-ttu-id="b6ce4-115">有关示例的更完整上下文，请参阅 [列表频道消息回复](../api/chatmessage-list-replies.md#example)。</span><span class="sxs-lookup"><span data-stu-id="b6ce4-115">For a fuller context of the example, see [List channel message replies](../api/chatmessage-list-replies.md#example).</span></span>

## <a name="properties"></a><span data-ttu-id="b6ce4-116">属性</span><span class="sxs-lookup"><span data-stu-id="b6ce4-116">Properties</span></span>
| <span data-ttu-id="b6ce4-117">属性</span><span class="sxs-lookup"><span data-stu-id="b6ce4-117">Property</span></span>     | <span data-ttu-id="b6ce4-118">类型</span><span class="sxs-lookup"><span data-stu-id="b6ce4-118">Type</span></span>   |<span data-ttu-id="b6ce4-119">说明</span><span class="sxs-lookup"><span data-stu-id="b6ce4-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b6ce4-120">id</span><span class="sxs-lookup"><span data-stu-id="b6ce4-120">id</span></span>|<span data-ttu-id="b6ce4-121">Int32</span><span class="sxs-lookup"><span data-stu-id="b6ce4-121">Int32</span></span>|<span data-ttu-id="b6ce4-122">指定的 **chatMessage** 中提及的实体的索引。</span><span class="sxs-lookup"><span data-stu-id="b6ce4-122">Index of an entity being mentioned in the specified **chatMessage**.</span></span> <span data-ttu-id="b6ce4-123">匹配邮件正文中相应标记中的 `<at id="{index}">` {index} 值。</span><span class="sxs-lookup"><span data-stu-id="b6ce4-123">Matches the {index} value in the corresponding `<at id="{index}">` tag in the message body.</span></span>|
|<span data-ttu-id="b6ce4-124">mentionText</span><span class="sxs-lookup"><span data-stu-id="b6ce4-124">mentionText</span></span>|<span data-ttu-id="b6ce4-125">字符串</span><span class="sxs-lookup"><span data-stu-id="b6ce4-125">string</span></span>|<span data-ttu-id="b6ce4-126">用于表示提及的字符串。</span><span class="sxs-lookup"><span data-stu-id="b6ce4-126">String used to represent the mention.</span></span> <span data-ttu-id="b6ce4-127">例如，用户的显示名称，一个团队名称。</span><span class="sxs-lookup"><span data-stu-id="b6ce4-127">For example, a user's display name, a team name.</span></span>|
|<span data-ttu-id="b6ce4-128">提及</span><span class="sxs-lookup"><span data-stu-id="b6ce4-128">mentioned</span></span>|[<span data-ttu-id="b6ce4-129">chatMessageIdentitySet</span><span class="sxs-lookup"><span data-stu-id="b6ce4-129">chatMessageMentionedIdentitySet</span></span>](chatmessagementionedidentityset.md)|<span data-ttu-id="b6ce4-130">包含 (用户、应用程序、团队或频道) 实体@mentioned。</span><span class="sxs-lookup"><span data-stu-id="b6ce4-130">The entity (user, application, team, or channel) that was @mentioned.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="b6ce4-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b6ce4-131">JSON representation</span></span>

<span data-ttu-id="b6ce4-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b6ce4-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.chatMessageMention"
}-->

```json
{
  "id": 1024,
  "mentionText": "string",
  "mentioned": {"@odata.type": "microsoft.graph.chatMessageMentionedIdentitySet"}
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


