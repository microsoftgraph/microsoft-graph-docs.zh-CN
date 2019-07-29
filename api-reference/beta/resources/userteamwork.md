---
title: userTeamwork 资源类型
description: '可供用户使用的 Microsoft Teams 功能的容器。 '
author: clearab
doc_type: resourcePageType
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: d68ceff79856b23f2d86b2c57a6278b7c6ad7e9d
ms.sourcegitcommit: 82b73552fff79a4ef7a2ee57fc2d1b3286b5bd4c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/26/2019
ms.locfileid: "35908584"
---
# <a name="userteamwork-resource-type"></a><span data-ttu-id="36459-103">userTeamwork 资源类型</span><span class="sxs-lookup"><span data-stu-id="36459-103">userTeamwork resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36459-104">适用于租户中每个用户可用的 Microsoft Teams 功能范围的容器。</span><span class="sxs-lookup"><span data-stu-id="36459-104">A container for the range of Microsoft Teams functionalities that are available per user in the tenant.</span></span>

## <a name="properties"></a><span data-ttu-id="36459-105">属性</span><span class="sxs-lookup"><span data-stu-id="36459-105">Properties</span></span>

| <span data-ttu-id="36459-106">属性</span><span class="sxs-lookup"><span data-stu-id="36459-106">Property</span></span> | <span data-ttu-id="36459-107">类型</span><span class="sxs-lookup"><span data-stu-id="36459-107">Type</span></span> | <span data-ttu-id="36459-108">说明</span><span class="sxs-lookup"><span data-stu-id="36459-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="36459-109">id</span><span class="sxs-lookup"><span data-stu-id="36459-109">id</span></span>|<span data-ttu-id="36459-110">string</span><span class="sxs-lookup"><span data-stu-id="36459-110">string</span></span>| <span data-ttu-id="36459-111">唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="36459-111">A unique identifier for the Announcement.</span></span> |

## <a name="relationships"></a><span data-ttu-id="36459-112">关系</span><span class="sxs-lookup"><span data-stu-id="36459-112">Relationships</span></span>

| <span data-ttu-id="36459-113">关系</span><span class="sxs-lookup"><span data-stu-id="36459-113">Relationship</span></span> | <span data-ttu-id="36459-114">类型</span><span class="sxs-lookup"><span data-stu-id="36459-114">Type</span></span> | <span data-ttu-id="36459-115">说明</span><span class="sxs-lookup"><span data-stu-id="36459-115">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="36459-116">installedApps</span><span class="sxs-lookup"><span data-stu-id="36459-116">installedApps</span></span>|<span data-ttu-id="36459-117">[teamsAppInstallation](teamsappinstallation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="36459-117">[teamsAppInstallation](teamsappinstallation.md) collection</span></span>|<span data-ttu-id="36459-118">此用户的个人范围内安装的应用。</span><span class="sxs-lookup"><span data-stu-id="36459-118">The apps installed in the personal scope of this user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="36459-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="36459-119">JSON representation</span></span>

<span data-ttu-id="36459-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="36459-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userTeamwork",
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
  "description": "userteamwork resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
