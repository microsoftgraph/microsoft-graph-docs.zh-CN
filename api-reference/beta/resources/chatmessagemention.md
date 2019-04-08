---
title: chatMessageMention 资源类型
description: '表示了 chatmessage 实体中提及的项。 提及可用于用户、团队、机器人或频道。 '
localization_priority: Normal
ms.openlocfilehash: 45b4c60e22f727210150a64078935741dfb71640
ms.sourcegitcommit: 953895b28b6bae6e17eead938565fde289c49ef7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/05/2019
ms.locfileid: "31481368"
---
# <a name="chatmessagemention-resource-type"></a><span data-ttu-id="0136f-104">chatMessageMention 资源类型</span><span class="sxs-lookup"><span data-stu-id="0136f-104">chatMessageMention resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0136f-105">表示[了 chatmessage](chatmessage.md)实体中提及的项。</span><span class="sxs-lookup"><span data-stu-id="0136f-105">Represents a mention in a [chatMessage](chatmessage.md) entity.</span></span> <span data-ttu-id="0136f-106">提及可用于用户、团队、机器人或频道。</span><span class="sxs-lookup"><span data-stu-id="0136f-106">The mention can be to a user, team, bot or channel.</span></span> 

## <a name="properties"></a><span data-ttu-id="0136f-107">属性</span><span class="sxs-lookup"><span data-stu-id="0136f-107">Properties</span></span>
| <span data-ttu-id="0136f-108">属性</span><span class="sxs-lookup"><span data-stu-id="0136f-108">Property</span></span>     | <span data-ttu-id="0136f-109">类型</span><span class="sxs-lookup"><span data-stu-id="0136f-109">Type</span></span>   |<span data-ttu-id="0136f-110">说明</span><span class="sxs-lookup"><span data-stu-id="0136f-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0136f-111">id</span><span class="sxs-lookup"><span data-stu-id="0136f-111">id</span></span>|<span data-ttu-id="0136f-112">string</span><span class="sxs-lookup"><span data-stu-id="0136f-112">string</span></span>|<span data-ttu-id="0136f-113">提到的实体 Id</span><span class="sxs-lookup"><span data-stu-id="0136f-113">Id of the entity being mentioned</span></span>|
|<span data-ttu-id="0136f-114">mentionText</span><span class="sxs-lookup"><span data-stu-id="0136f-114">mentionText</span></span>|<span data-ttu-id="0136f-115">string</span><span class="sxs-lookup"><span data-stu-id="0136f-115">string</span></span>|<span data-ttu-id="0136f-116">用于表示提及的 Ex: 用户显示名称、团队名称等的字符串</span><span class="sxs-lookup"><span data-stu-id="0136f-116">String used to represent the mention Ex: User display name, Team name etc</span></span>|
|<span data-ttu-id="0136f-117">所</span><span class="sxs-lookup"><span data-stu-id="0136f-117">mentioned</span></span>|[<span data-ttu-id="0136f-118">identitySet</span><span class="sxs-lookup"><span data-stu-id="0136f-118">identitySet</span></span>](identityset.md)|<span data-ttu-id="0136f-119">提到的用户</span><span class="sxs-lookup"><span data-stu-id="0136f-119">The user that was mentioned</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0136f-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0136f-120">JSON representation</span></span>

<span data-ttu-id="0136f-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0136f-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessageMention"
}-->

```json
{
  "id": "string (identifier)",
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
