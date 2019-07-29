---
title: teamwork 资源类型
description: 可供组织使用的 Microsoft Teams 功能的容器。
author: clearab
doc_type: resourcePageType
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 7a72e34fc3d9d02a36e34295f7d4469536506df3
ms.sourcegitcommit: 82b73552fff79a4ef7a2ee57fc2d1b3286b5bd4c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/26/2019
ms.locfileid: "35908591"
---
# <a name="teamwork-resource-type"></a><span data-ttu-id="9a233-103">teamwork 资源类型</span><span class="sxs-lookup"><span data-stu-id="9a233-103">teamwork resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a233-104">可供组织使用的 Microsoft Teams 功能范围的容器。</span><span class="sxs-lookup"><span data-stu-id="9a233-104">A container for the range of Microsoft Teams functionalities that are available for the organization.</span></span>

## <a name="properties"></a><span data-ttu-id="9a233-105">属性</span><span class="sxs-lookup"><span data-stu-id="9a233-105">Properties</span></span>

| <span data-ttu-id="9a233-106">属性</span><span class="sxs-lookup"><span data-stu-id="9a233-106">Property</span></span> | <span data-ttu-id="9a233-107">类型</span><span class="sxs-lookup"><span data-stu-id="9a233-107">Type</span></span> | <span data-ttu-id="9a233-108">说明</span><span class="sxs-lookup"><span data-stu-id="9a233-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="9a233-109">id</span><span class="sxs-lookup"><span data-stu-id="9a233-109">id</span></span>|<span data-ttu-id="9a233-110">string</span><span class="sxs-lookup"><span data-stu-id="9a233-110">string</span></span>| <span data-ttu-id="9a233-111">唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="9a233-111">A unique identifier for the Announcement.</span></span> |

## <a name="relationships"></a><span data-ttu-id="9a233-112">关系</span><span class="sxs-lookup"><span data-stu-id="9a233-112">Relationships</span></span>

| <span data-ttu-id="9a233-113">关系</span><span class="sxs-lookup"><span data-stu-id="9a233-113">Relationship</span></span> | <span data-ttu-id="9a233-114">类型</span><span class="sxs-lookup"><span data-stu-id="9a233-114">Type</span></span> | <span data-ttu-id="9a233-115">说明</span><span class="sxs-lookup"><span data-stu-id="9a233-115">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="9a233-116">installedApps</span><span class="sxs-lookup"><span data-stu-id="9a233-116">installedApps</span></span>|<span data-ttu-id="9a233-117">[teamsAppInstallation](teamsappinstallation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9a233-117">[teamsAppInstallation](teamsappinstallation.md) collection</span></span>|<span data-ttu-id="9a233-118">此用户的个人范围内安装的应用。</span><span class="sxs-lookup"><span data-stu-id="9a233-118">The apps installed in the personal scope of this user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9a233-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9a233-119">JSON representation</span></span>

<span data-ttu-id="9a233-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9a233-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamwork",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teamwork resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

## <a name="see-also"></a><span data-ttu-id="9a233-121">另请参阅</span><span class="sxs-lookup"><span data-stu-id="9a233-121">See Also</span></span>

- [<span data-ttu-id="9a233-122">userTeamwork 资源类型</span><span class="sxs-lookup"><span data-stu-id="9a233-122">userTeamwork resource</span></span>](userteamwork.md)
