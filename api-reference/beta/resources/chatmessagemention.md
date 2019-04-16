---
title: chatMessageMention 资源类型
description: '表示了 chatmessage 实体中提及的项。 提及可用于用户、团队、机器人或频道。 '
localization_priority: Normal
author: nkramer
ms.openlocfilehash: 5d7304325e48c87bfd75b57bf49585f66a77b262
ms.sourcegitcommit: a39db1154a07aa0dd7e96fb6f9d7e891a812207e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2019
ms.locfileid: "31889994"
---
# <a name="chatmessagemention-resource-type"></a><span data-ttu-id="05c03-104">chatMessageMention 资源类型</span><span class="sxs-lookup"><span data-stu-id="05c03-104">chatMessageMention resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05c03-105">表示[了 chatmessage](chatmessage.md)实体中提及的项。</span><span class="sxs-lookup"><span data-stu-id="05c03-105">Represents a mention in a [chatMessage](chatmessage.md) entity.</span></span> <span data-ttu-id="05c03-106">提及可用于用户、团队、机器人或频道。</span><span class="sxs-lookup"><span data-stu-id="05c03-106">The mention can be to a user, team, bot, or channel.</span></span> 

## <a name="properties"></a><span data-ttu-id="05c03-107">属性</span><span class="sxs-lookup"><span data-stu-id="05c03-107">Properties</span></span>
| <span data-ttu-id="05c03-108">属性</span><span class="sxs-lookup"><span data-stu-id="05c03-108">Property</span></span>     | <span data-ttu-id="05c03-109">类型</span><span class="sxs-lookup"><span data-stu-id="05c03-109">Type</span></span>   |<span data-ttu-id="05c03-110">说明</span><span class="sxs-lookup"><span data-stu-id="05c03-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="05c03-111">id</span><span class="sxs-lookup"><span data-stu-id="05c03-111">id</span></span>|<span data-ttu-id="05c03-112">int</span><span class="sxs-lookup"><span data-stu-id="05c03-112">int</span></span>|<span data-ttu-id="05c03-113">提到的实体的索引。</span><span class="sxs-lookup"><span data-stu-id="05c03-113">Index of the entity being mentioned.</span></span> <span data-ttu-id="05c03-114">与邮件正文<at id="index">的标记匹配。</span><span class="sxs-lookup"><span data-stu-id="05c03-114">Matches with the <at id="index"> tag of the message body.</span></span>|
|<span data-ttu-id="05c03-115">mentionText</span><span class="sxs-lookup"><span data-stu-id="05c03-115">mentionText</span></span>|<span data-ttu-id="05c03-116">string</span><span class="sxs-lookup"><span data-stu-id="05c03-116">string</span></span>|<span data-ttu-id="05c03-117">用于表示提及的字符串。</span><span class="sxs-lookup"><span data-stu-id="05c03-117">String used to represent the mention.</span></span> <span data-ttu-id="05c03-118">例如, 用户显示名称, 工作组名称。</span><span class="sxs-lookup"><span data-stu-id="05c03-118">For example, User display name, Team name.</span></span>|
|<span data-ttu-id="05c03-119">所</span><span class="sxs-lookup"><span data-stu-id="05c03-119">mentioned</span></span>|[<span data-ttu-id="05c03-120">identitySet</span><span class="sxs-lookup"><span data-stu-id="05c03-120">identitySet</span></span>](identityset.md)|<span data-ttu-id="05c03-121">提到的实体 (用户、应用程序、团队或通道)。</span><span class="sxs-lookup"><span data-stu-id="05c03-121">The entity (user, application, team, or channel) that was mentioned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="05c03-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="05c03-122">JSON representation</span></span>

<span data-ttu-id="05c03-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="05c03-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessageMention"
}-->

```json
{
  "id": "number",
  "mentionText": "string",
  "mentioned": "microsoft.graph.identitySet"
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
  "suppressions": [
    "Error: /api-reference/beta/resources/chatmessagemention.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
