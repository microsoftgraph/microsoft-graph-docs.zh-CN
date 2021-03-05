---
title: teamworkBot 资源类型
description: Microsoft Teams 生态系统中的机器人。
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 99bdde9a4ff26945dd5aa040f2741fdf50c1273b
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50476408"
---
# <a name="teamworkbot-resource-type"></a><span data-ttu-id="02e29-103">teamworkBot 资源类型</span><span class="sxs-lookup"><span data-stu-id="02e29-103">teamworkBot resource type</span></span>

<span data-ttu-id="02e29-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02e29-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="02e29-105">表示 Microsoft Teams 生态系统中的机器人。</span><span class="sxs-lookup"><span data-stu-id="02e29-105">Represents a bot in the Microsoft Teams ecosystem.</span></span>

## <a name="methods"></a><span data-ttu-id="02e29-106">Methods</span><span class="sxs-lookup"><span data-stu-id="02e29-106">Methods</span></span>
|<span data-ttu-id="02e29-107">方法</span><span class="sxs-lookup"><span data-stu-id="02e29-107">Method</span></span>|<span data-ttu-id="02e29-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="02e29-108">Return type</span></span>|<span data-ttu-id="02e29-109">说明</span><span class="sxs-lookup"><span data-stu-id="02e29-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="02e29-110">获取自动程序</span><span class="sxs-lookup"><span data-stu-id="02e29-110">Get bot</span></span>](../api/teamworkbot-get.md)|[<span data-ttu-id="02e29-111">teamworkBot</span><span class="sxs-lookup"><span data-stu-id="02e29-111">teamworkBot</span></span>](../resources/teamworkbot.md)|<span data-ttu-id="02e29-112">读取团队合作Bot 对象 [的属性](../resources/teamworkbot.md) 和关系。</span><span class="sxs-lookup"><span data-stu-id="02e29-112">Read the properties and relationships of a [teamworkBot](../resources/teamworkbot.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="02e29-113">属性</span><span class="sxs-lookup"><span data-stu-id="02e29-113">Properties</span></span>
|<span data-ttu-id="02e29-114">属性</span><span class="sxs-lookup"><span data-stu-id="02e29-114">Property</span></span>|<span data-ttu-id="02e29-115">类型</span><span class="sxs-lookup"><span data-stu-id="02e29-115">Type</span></span>|<span data-ttu-id="02e29-116">说明</span><span class="sxs-lookup"><span data-stu-id="02e29-116">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02e29-117">id</span><span class="sxs-lookup"><span data-stu-id="02e29-117">id</span></span>|<span data-ttu-id="02e29-118">String</span><span class="sxs-lookup"><span data-stu-id="02e29-118">String</span></span>|<span data-ttu-id="02e29-119">与特定 [teamsAppDefinition](../resources/teamsappdefinition.md)相关联的机器人的 ID。</span><span class="sxs-lookup"><span data-stu-id="02e29-119">The ID of the bot associated with the specific [teamsAppDefinition](../resources/teamsappdefinition.md).</span></span> <span data-ttu-id="02e29-120">此值通常为 GUID。</span><span class="sxs-lookup"><span data-stu-id="02e29-120">This value is usually a GUID.</span></span>|

## <a name="relationships"></a><span data-ttu-id="02e29-121">关系</span><span class="sxs-lookup"><span data-stu-id="02e29-121">Relationships</span></span>
<span data-ttu-id="02e29-122">无。</span><span class="sxs-lookup"><span data-stu-id="02e29-122">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="02e29-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="02e29-123">JSON representation</span></span>
<span data-ttu-id="02e29-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="02e29-124">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamworkBot",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkBot",
  "id": "String (identifier)"
}
```

## <a name="see-also"></a><span data-ttu-id="02e29-125">另请参阅</span><span class="sxs-lookup"><span data-stu-id="02e29-125">See also</span></span>

- <span data-ttu-id="02e29-126">若要在团队中安装机器人，请参阅团队中 [列表应用的示例](../api/team-list-installedapps.md)2。</span><span class="sxs-lookup"><span data-stu-id="02e29-126">To get bots installed in a team, see example 2 in [List apps in team](../api/team-list-installedapps.md).</span></span> <!-- - To get bots installed in a chat, see example 2 in [List apps in chat](../api/chat-list-installedapps.md). -->
- <span data-ttu-id="02e29-127">若要在用户的个人范围内安装自动程序，请参阅为用户安装的列表 [应用中的示例](../api/userteamwork-list-installedapps.md)2。</span><span class="sxs-lookup"><span data-stu-id="02e29-127">To get bots installed in the personal scope of a user, see example 2 in [List apps installed for user](../api/userteamwork-list-installedapps.md).</span></span>



