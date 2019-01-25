---
title: chatMessageMention 资源类型
description: '代表 chatMessage 实体中的某个提及。 提及的可向用户、 团队、 自动程序或通道。 '
localization_priority: Normal
ms.openlocfilehash: f37374a9793000ba641ed772e5dbfca5c0f1bd30
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515347"
---
# <a name="chatmessagemention-resource-type"></a><span data-ttu-id="6ed24-104">chatMessageMention 资源类型</span><span class="sxs-lookup"><span data-stu-id="6ed24-104">chatMessageMention resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ed24-105">代表[chatMessage](chatmessage.md)实体中的某个提及。</span><span class="sxs-lookup"><span data-stu-id="6ed24-105">Represents a mention in a [chatMessage](chatmessage.md) entity.</span></span> <span data-ttu-id="6ed24-106">提及的可向用户、 团队、 自动程序或通道。</span><span class="sxs-lookup"><span data-stu-id="6ed24-106">The mention can be to a user, team, bot or channel.</span></span> 

## <a name="properties"></a><span data-ttu-id="6ed24-107">属性</span><span class="sxs-lookup"><span data-stu-id="6ed24-107">Properties</span></span>
| <span data-ttu-id="6ed24-108">属性</span><span class="sxs-lookup"><span data-stu-id="6ed24-108">Property</span></span>     | <span data-ttu-id="6ed24-109">类型</span><span class="sxs-lookup"><span data-stu-id="6ed24-109">Type</span></span>   |<span data-ttu-id="6ed24-110">说明</span><span class="sxs-lookup"><span data-stu-id="6ed24-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6ed24-111">id</span><span class="sxs-lookup"><span data-stu-id="6ed24-111">id</span></span>|<span data-ttu-id="6ed24-112">string</span><span class="sxs-lookup"><span data-stu-id="6ed24-112">string</span></span>|<span data-ttu-id="6ed24-113">正在提到的实体的 id</span><span class="sxs-lookup"><span data-stu-id="6ed24-113">Id of the entity being mentioned</span></span>|
|<span data-ttu-id="6ed24-114">mentionText</span><span class="sxs-lookup"><span data-stu-id="6ed24-114">mentionText</span></span>|<span data-ttu-id="6ed24-115">string</span><span class="sxs-lookup"><span data-stu-id="6ed24-115">string</span></span>|<span data-ttu-id="6ed24-116">用来表示 Ex 提及的字符串： 用户的显示名称、 工作组名称等</span><span class="sxs-lookup"><span data-stu-id="6ed24-116">String used to represent the mention Ex: User display name, Team name etc</span></span>|
|<span data-ttu-id="6ed24-117">提到</span><span class="sxs-lookup"><span data-stu-id="6ed24-117">mentioned</span></span>|[<span data-ttu-id="6ed24-118">identitySet</span><span class="sxs-lookup"><span data-stu-id="6ed24-118">identitySet</span></span>](identityset.md)|<span data-ttu-id="6ed24-119">已提及用户</span><span class="sxs-lookup"><span data-stu-id="6ed24-119">The user that was mentioned</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6ed24-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6ed24-120">JSON representation</span></span>

<span data-ttu-id="6ed24-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6ed24-121">The following is a JSON representation of the resource.</span></span>

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
    "Error: /api-reference/beta/resources/chatMention.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
