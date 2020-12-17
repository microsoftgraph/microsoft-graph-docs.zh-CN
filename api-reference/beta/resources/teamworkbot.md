---
title: teamworkBot 资源类型
description: Microsoft Teams 生态系统中的机器人。
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 383c646fdb30d082daa73e37fd227238db195b6b
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706319"
---
# <a name="teamworkbot-resource-type"></a><span data-ttu-id="2d420-103">teamworkBot 资源类型</span><span class="sxs-lookup"><span data-stu-id="2d420-103">teamworkBot resource type</span></span>

<span data-ttu-id="2d420-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d420-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2d420-105">表示 Microsoft Teams 生态系统中的机器人。</span><span class="sxs-lookup"><span data-stu-id="2d420-105">Represents a bot in the Microsoft Teams ecosystem.</span></span>

## <a name="methods"></a><span data-ttu-id="2d420-106">方法</span><span class="sxs-lookup"><span data-stu-id="2d420-106">Methods</span></span>
|<span data-ttu-id="2d420-107">方法</span><span class="sxs-lookup"><span data-stu-id="2d420-107">Method</span></span>|<span data-ttu-id="2d420-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="2d420-108">Return type</span></span>|<span data-ttu-id="2d420-109">说明</span><span class="sxs-lookup"><span data-stu-id="2d420-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2d420-110">获取自动程序</span><span class="sxs-lookup"><span data-stu-id="2d420-110">Get bot</span></span>](../api/teamworkbot-get.md)|[<span data-ttu-id="2d420-111">teamworkBot</span><span class="sxs-lookup"><span data-stu-id="2d420-111">teamworkBot</span></span>](../resources/teamworkbot.md)|<span data-ttu-id="2d420-112">读取团队合作Bot 对象 [的属性和](../resources/teamworkbot.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="2d420-112">Read the properties and relationships of a [teamworkBot](../resources/teamworkbot.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2d420-113">属性</span><span class="sxs-lookup"><span data-stu-id="2d420-113">Properties</span></span>
|<span data-ttu-id="2d420-114">属性</span><span class="sxs-lookup"><span data-stu-id="2d420-114">Property</span></span>|<span data-ttu-id="2d420-115">类型</span><span class="sxs-lookup"><span data-stu-id="2d420-115">Type</span></span>|<span data-ttu-id="2d420-116">说明</span><span class="sxs-lookup"><span data-stu-id="2d420-116">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d420-117">id</span><span class="sxs-lookup"><span data-stu-id="2d420-117">id</span></span>|<span data-ttu-id="2d420-118">字符串</span><span class="sxs-lookup"><span data-stu-id="2d420-118">String</span></span>|<span data-ttu-id="2d420-119">与特定 [teamsAppDefinition](../resources/teamsappdefinition.md)相关联的机器人的 ID。</span><span class="sxs-lookup"><span data-stu-id="2d420-119">The id of the bot associated with the specific [teamsAppDefinition](../resources/teamsappdefinition.md).</span></span> <span data-ttu-id="2d420-120">此值通常为 GUID。</span><span class="sxs-lookup"><span data-stu-id="2d420-120">This value is usually a GUID.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2d420-121">关系</span><span class="sxs-lookup"><span data-stu-id="2d420-121">Relationships</span></span>
<span data-ttu-id="2d420-122">无。</span><span class="sxs-lookup"><span data-stu-id="2d420-122">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2d420-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2d420-123">JSON representation</span></span>
<span data-ttu-id="2d420-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2d420-124">The following is a JSON representation of the resource.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="2d420-125">另请参阅</span><span class="sxs-lookup"><span data-stu-id="2d420-125">See also</span></span>

- <span data-ttu-id="2d420-126">若要在团队中安装机器人，请参阅团队 [中的列表应用中的示例](../api/team-list-installedapps.md)2。</span><span class="sxs-lookup"><span data-stu-id="2d420-126">To get bots installed in a team, see example 2 in [List apps in team](../api/team-list-installedapps.md).</span></span>
- <span data-ttu-id="2d420-127">若要在聊天中安装聊天机器人，请参阅聊天中的 [列表应用中的示例](../api/chat-list-installedapps.md)2。</span><span class="sxs-lookup"><span data-stu-id="2d420-127">To get bots installed in a chat, see example 2 in [List apps in chat](../api/chat-list-installedapps.md).</span></span>
- <span data-ttu-id="2d420-128">若要在用户的个人范围内安装机器人，请参阅为用户安装 [的列表应用中的示例](../api/userteamwork-list-installedapps.md)2。</span><span class="sxs-lookup"><span data-stu-id="2d420-128">To get bots installed in the personal scope of a user, see example 2 in [List apps installed for user](../api/userteamwork-list-installedapps.md).</span></span>



