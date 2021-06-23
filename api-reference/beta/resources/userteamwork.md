---
title: userTeamwork 资源类型
description: '可供用户使用的 Microsoft Teams 功能的容器。 '
author: akjo
doc_type: resourcePageType
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 6ef5bb1ddf0944e7d61ab5321ae50e766713326c
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060441"
---
# <a name="userteamwork-resource-type"></a><span data-ttu-id="588d5-103">userTeamwork 资源类型</span><span class="sxs-lookup"><span data-stu-id="588d5-103">userTeamwork resource type</span></span>

<span data-ttu-id="588d5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="588d5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="588d5-105">适用于租户中每个用户可用的 Microsoft Teams 功能范围的容器。</span><span class="sxs-lookup"><span data-stu-id="588d5-105">A container for the range of Microsoft Teams functionalities that are available per user in the tenant.</span></span>

## <a name="properties"></a><span data-ttu-id="588d5-106">属性</span><span class="sxs-lookup"><span data-stu-id="588d5-106">Properties</span></span>

| <span data-ttu-id="588d5-107">属性</span><span class="sxs-lookup"><span data-stu-id="588d5-107">Property</span></span> | <span data-ttu-id="588d5-108">类型</span><span class="sxs-lookup"><span data-stu-id="588d5-108">Type</span></span> | <span data-ttu-id="588d5-109">说明</span><span class="sxs-lookup"><span data-stu-id="588d5-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="588d5-110">id</span><span class="sxs-lookup"><span data-stu-id="588d5-110">id</span></span>|<span data-ttu-id="588d5-111">string</span><span class="sxs-lookup"><span data-stu-id="588d5-111">string</span></span>| <span data-ttu-id="588d5-112">唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="588d5-112">A unique identifier.</span></span> |

## <a name="relationships"></a><span data-ttu-id="588d5-113">关系</span><span class="sxs-lookup"><span data-stu-id="588d5-113">Relationships</span></span>

| <span data-ttu-id="588d5-114">关系</span><span class="sxs-lookup"><span data-stu-id="588d5-114">Relationship</span></span> | <span data-ttu-id="588d5-115">类型</span><span class="sxs-lookup"><span data-stu-id="588d5-115">Type</span></span> | <span data-ttu-id="588d5-116">说明</span><span class="sxs-lookup"><span data-stu-id="588d5-116">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="588d5-117">installedApps</span><span class="sxs-lookup"><span data-stu-id="588d5-117">installedApps</span></span>|<span data-ttu-id="588d5-118">[teamsAppInstallation](teamsappinstallation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="588d5-118">[teamsAppInstallation](teamsappinstallation.md) collection</span></span>|<span data-ttu-id="588d5-119">此用户的个人范围内安装的应用。</span><span class="sxs-lookup"><span data-stu-id="588d5-119">The apps installed in the personal scope of this user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="588d5-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="588d5-120">JSON representation</span></span>

<span data-ttu-id="588d5-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="588d5-121">The following is a JSON representation of the resource.</span></span>

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


