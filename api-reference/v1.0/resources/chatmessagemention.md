---
title: chatMessageMention 资源类型
description: '表示了 chatmessage 实体中提及的项。 提及可用于用户、团队、机器人或频道。 '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 05db56363acd5e7706a6a4acd8a650f0dca3c93b
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845804"
---
# <a name="chatmessagemention-resource-type"></a><span data-ttu-id="112e3-104">chatMessageMention 资源类型</span><span class="sxs-lookup"><span data-stu-id="112e3-104">chatMessageMention resource type</span></span>

<span data-ttu-id="112e3-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="112e3-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="112e3-106">表示[了 chatmessage](./chatmessage.md)实体中提及的项。</span><span class="sxs-lookup"><span data-stu-id="112e3-106">Represents a mention in a [chatMessage](./chatmessage.md) entity.</span></span> <span data-ttu-id="112e3-107">提及可用于[用户](user.md)、[团队](team.md)、机器人或[频道](channel.md)。</span><span class="sxs-lookup"><span data-stu-id="112e3-107">The mention can be to a [user](user.md), [team](team.md), bot, or [channel](channel.md).</span></span> 

<span data-ttu-id="112e3-108">在包含一个或多个提及的**了 chatmessage**对象中，邮件正文**内容**属性代表 HTML 中的聊天消息。</span><span class="sxs-lookup"><span data-stu-id="112e3-108">In a **chatMessage** object that contains one or more mentions, the message body **content** property represents the chat message in HTML.</span></span> <span data-ttu-id="112e3-109">它将每个提及的**mentionText**封装在 HTML `at` 元素中，其中包含一个与 `id` 提及的**id**属性相对应的属性。</span><span class="sxs-lookup"><span data-stu-id="112e3-109">It encloses the **mentionText** of each mention in an HTML `at` element, with an `id` attribute that corresponds to the **id** property of the mention.</span></span>

<span data-ttu-id="112e3-110">例如，聊天邮件包含两个提及，分别提及 "Megan" 和 "Alex" 文本。</span><span class="sxs-lookup"><span data-stu-id="112e3-110">As an example, a chat message contains two mentions, with the mention text "Megan" and "Alex" respectively.</span></span> <span data-ttu-id="112e3-111">其 body**内容**属性按 `at` 如下所示为两个提及指定元素：</span><span class="sxs-lookup"><span data-stu-id="112e3-111">Its body **content** property specifies `at` elements for the two mentions as follows:</span></span>

``` json
"body": {
    "contentType": "html",
    "content": "<div><div>Ah, <at id=\"0\">Megan</at>, <at id=\"1\">Alex</at>, I saw them in a separate folder. Thanks!</div>\n</div>"
}
```

<span data-ttu-id="112e3-112">在**content**属性中，第一个提及的 HTML `id` 属性为0。</span><span class="sxs-lookup"><span data-stu-id="112e3-112">In the **content** property, the first mention has an HTML `id` attribute of 0.</span></span> <span data-ttu-id="112e3-113">这对应于**chatMessageMention**的第一个实例的**id**属性，也是0。</span><span class="sxs-lookup"><span data-stu-id="112e3-113">This corresponds to the **id** property of that first instance of **chatMessageMention**, which is also 0.</span></span>

<span data-ttu-id="112e3-114">第二个提及的 `id` 属性为1，与第二个实例的**id**属性相匹配，即1。</span><span class="sxs-lookup"><span data-stu-id="112e3-114">The second mention has an `id` attribute of 1, matching the **id** property of the second instance, which is 1.</span></span>

<span data-ttu-id="112e3-115">有关此示例的更完整上下文，请参阅[列出通道邮件答复](/graph/api/channel-list-messagereplies?view=graph-rest-beta)。</span><span class="sxs-lookup"><span data-stu-id="112e3-115">For a fuller context of the example, see [List channel message replies](/graph/api/channel-list-messagereplies?view=graph-rest-beta).</span></span>

## <a name="properties"></a><span data-ttu-id="112e3-116">属性</span><span class="sxs-lookup"><span data-stu-id="112e3-116">Properties</span></span>

| <span data-ttu-id="112e3-117">属性</span><span class="sxs-lookup"><span data-stu-id="112e3-117">Property</span></span>| <span data-ttu-id="112e3-118">类型</span><span class="sxs-lookup"><span data-stu-id="112e3-118">Type</span></span>|<span data-ttu-id="112e3-119">说明</span><span class="sxs-lookup"><span data-stu-id="112e3-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="112e3-120">id</span><span class="sxs-lookup"><span data-stu-id="112e3-120">id</span></span>|<span data-ttu-id="112e3-121">Int32</span><span class="sxs-lookup"><span data-stu-id="112e3-121">Int32</span></span>|<span data-ttu-id="112e3-122">在指定的**了 chatmessage**中提到的实体的索引。</span><span class="sxs-lookup"><span data-stu-id="112e3-122">Index of an entity being mentioned in the specified **chatMessage**.</span></span> <span data-ttu-id="112e3-123">与邮件正文中对应的标记中的 {index} 值相匹配 `<at id="{index}">` 。</span><span class="sxs-lookup"><span data-stu-id="112e3-123">Matches the {index} value in the corresponding `<at id="{index}">` tag in the message body.</span></span>|
|<span data-ttu-id="112e3-124">mentionText</span><span class="sxs-lookup"><span data-stu-id="112e3-124">mentionText</span></span>|<span data-ttu-id="112e3-125">字符串</span><span class="sxs-lookup"><span data-stu-id="112e3-125">string</span></span>|<span data-ttu-id="112e3-126">用于表示提及的字符串。</span><span class="sxs-lookup"><span data-stu-id="112e3-126">String used to represent the mention.</span></span> <span data-ttu-id="112e3-127">例如，用户的显示名称（团队名称）。</span><span class="sxs-lookup"><span data-stu-id="112e3-127">For example, a user's display name, a team name.</span></span>|
|<span data-ttu-id="112e3-128">所</span><span class="sxs-lookup"><span data-stu-id="112e3-128">mentioned</span></span>|[<span data-ttu-id="112e3-129">identitySet</span><span class="sxs-lookup"><span data-stu-id="112e3-129">identitySet</span></span>](identityset.md)|<span data-ttu-id="112e3-130">提到的实体（用户、应用程序、团队或通道）。</span><span class="sxs-lookup"><span data-stu-id="112e3-130">The entity (user, application, team, or channel) that was mentioned.</span></span>  <span data-ttu-id="112e3-131">如果它是 @mentioned 的频道或团队，则了解 identityset 包含一个**会话**属性，该属性提供团队/通道的 ID 和代表团队或频道的**conversationIdentityType**属性。</span><span class="sxs-lookup"><span data-stu-id="112e3-131">If it was a channel or team that was @mentioned, the identitySet contains a **conversation** property giving the ID of the team/channel, and a **conversationIdentityType** property that represents either the team or channel.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="112e3-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="112e3-132">JSON representation</span></span>

<span data-ttu-id="112e3-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="112e3-133">The following is a JSON representation of the resource.</span></span>

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
