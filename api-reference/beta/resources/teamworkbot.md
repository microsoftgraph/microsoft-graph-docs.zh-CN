---
title: teamworkBot 资源类型
description: Microsoft Teams 生态系统中的机器人。
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8c21e7ab3b88c2659bf055e39b931cbc6e9d2f39
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844674"
---
# <a name="teamworkbot-resource-type"></a><span data-ttu-id="fcb42-103">teamworkBot 资源类型</span><span class="sxs-lookup"><span data-stu-id="fcb42-103">teamworkBot resource type</span></span>

<span data-ttu-id="fcb42-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fcb42-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fcb42-105">表示 Microsoft Teams 生态系统中的机器人。</span><span class="sxs-lookup"><span data-stu-id="fcb42-105">Represents a bot in the Microsoft Teams ecosystem.</span></span>

## <a name="methods"></a><span data-ttu-id="fcb42-106">方法</span><span class="sxs-lookup"><span data-stu-id="fcb42-106">Methods</span></span>
|<span data-ttu-id="fcb42-107">方法</span><span class="sxs-lookup"><span data-stu-id="fcb42-107">Method</span></span>|<span data-ttu-id="fcb42-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="fcb42-108">Return type</span></span>|<span data-ttu-id="fcb42-109">说明</span><span class="sxs-lookup"><span data-stu-id="fcb42-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="fcb42-110">获取机器人</span><span class="sxs-lookup"><span data-stu-id="fcb42-110">Get bot</span></span>](../api/teamworkbot-get.md)|[<span data-ttu-id="fcb42-111">teamworkBot</span><span class="sxs-lookup"><span data-stu-id="fcb42-111">teamworkBot</span></span>](../resources/teamworkbot.md)|<span data-ttu-id="fcb42-112">读取团队合作Bot 对象 [的属性和](../resources/teamworkbot.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="fcb42-112">Read the properties and relationships of a [teamworkBot](../resources/teamworkbot.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="fcb42-113">属性</span><span class="sxs-lookup"><span data-stu-id="fcb42-113">Properties</span></span>
|<span data-ttu-id="fcb42-114">属性</span><span class="sxs-lookup"><span data-stu-id="fcb42-114">Property</span></span>|<span data-ttu-id="fcb42-115">类型</span><span class="sxs-lookup"><span data-stu-id="fcb42-115">Type</span></span>|<span data-ttu-id="fcb42-116">说明</span><span class="sxs-lookup"><span data-stu-id="fcb42-116">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fcb42-117">id</span><span class="sxs-lookup"><span data-stu-id="fcb42-117">id</span></span>|<span data-ttu-id="fcb42-118">String</span><span class="sxs-lookup"><span data-stu-id="fcb42-118">String</span></span>|<span data-ttu-id="fcb42-119">与特定 [teamsAppDefinition](../resources/teamsappdefinition.md)相关联的机器人的 ID。</span><span class="sxs-lookup"><span data-stu-id="fcb42-119">The id of the bot associated with the specific [teamsAppDefinition](../resources/teamsappdefinition.md).</span></span> <span data-ttu-id="fcb42-120">此值通常为 GUID。</span><span class="sxs-lookup"><span data-stu-id="fcb42-120">This value is usually a GUID.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fcb42-121">关系</span><span class="sxs-lookup"><span data-stu-id="fcb42-121">Relationships</span></span>
<span data-ttu-id="fcb42-122">无。</span><span class="sxs-lookup"><span data-stu-id="fcb42-122">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fcb42-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fcb42-123">JSON representation</span></span>
<span data-ttu-id="fcb42-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fcb42-124">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamworkBot",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkBot",
  "id": "String (identifier)"
}
```

## <a name="see-also"></a><span data-ttu-id="fcb42-125">另请参阅</span><span class="sxs-lookup"><span data-stu-id="fcb42-125">See also</span></span>

- <span data-ttu-id="fcb42-126">若要在团队中安装机器人，请参阅团队中的[列表应用中的示例 2。](../api/team-list-installedapps.md)</span><span class="sxs-lookup"><span data-stu-id="fcb42-126">To get bots installed in a team, see example 2 in [List apps in team](../api/team-list-installedapps.md).</span></span>
- <span data-ttu-id="fcb42-127">若要在聊天中安装聊天机器人，请参阅聊天中的 [列表应用中的示例](../api/chat-list-installedapps.md)2。</span><span class="sxs-lookup"><span data-stu-id="fcb42-127">To get bots installed in a chat, see example 2 in [List apps in chat](../api/chat-list-installedapps.md).</span></span>
- <span data-ttu-id="fcb42-128">若要在用户的个人范围内安装机器人，请参阅为用户安装 [的列表应用中的示例](../api/userteamwork-list-installedapps.md)2。</span><span class="sxs-lookup"><span data-stu-id="fcb42-128">To get bots installed in the personal scope of a user, see example 2 in [List apps installed for user](../api/userteamwork-list-installedapps.md).</span></span>



