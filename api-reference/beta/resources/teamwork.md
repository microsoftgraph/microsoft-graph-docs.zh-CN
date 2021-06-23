---
title: teamwork 资源类型
description: 可供组织使用的 Microsoft Teams 功能的容器。
author: akjo
doc_type: resourcePageType
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 439a4c5234d6442c2394dc8154b08d7cce2e5c69
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060445"
---
# <a name="teamwork-resource-type"></a><span data-ttu-id="36514-103">teamwork 资源类型</span><span class="sxs-lookup"><span data-stu-id="36514-103">teamwork resource type</span></span>

<span data-ttu-id="36514-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36514-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36514-105">可供组织使用的 Microsoft Teams 功能范围的容器。</span><span class="sxs-lookup"><span data-stu-id="36514-105">A container for the range of Microsoft Teams functionalities that are available for the organization.</span></span>

## <a name="properties"></a><span data-ttu-id="36514-106">属性</span><span class="sxs-lookup"><span data-stu-id="36514-106">Properties</span></span>

| <span data-ttu-id="36514-107">属性</span><span class="sxs-lookup"><span data-stu-id="36514-107">Property</span></span> | <span data-ttu-id="36514-108">类型</span><span class="sxs-lookup"><span data-stu-id="36514-108">Type</span></span> | <span data-ttu-id="36514-109">说明</span><span class="sxs-lookup"><span data-stu-id="36514-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="36514-110">id</span><span class="sxs-lookup"><span data-stu-id="36514-110">id</span></span>|<span data-ttu-id="36514-111">string</span><span class="sxs-lookup"><span data-stu-id="36514-111">string</span></span>| <span data-ttu-id="36514-112">唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="36514-112">A unique identifier.</span></span> |

## <a name="relationships"></a><span data-ttu-id="36514-113">关系</span><span class="sxs-lookup"><span data-stu-id="36514-113">Relationships</span></span>

| <span data-ttu-id="36514-114">关系</span><span class="sxs-lookup"><span data-stu-id="36514-114">Relationship</span></span> | <span data-ttu-id="36514-115">类型</span><span class="sxs-lookup"><span data-stu-id="36514-115">Type</span></span> | <span data-ttu-id="36514-116">说明</span><span class="sxs-lookup"><span data-stu-id="36514-116">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="36514-117">installedApps</span><span class="sxs-lookup"><span data-stu-id="36514-117">installedApps</span></span>|<span data-ttu-id="36514-118">[teamsAppInstallation](teamsappinstallation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="36514-118">[teamsAppInstallation](teamsappinstallation.md) collection</span></span>|<span data-ttu-id="36514-119">此用户的个人范围内安装的应用。</span><span class="sxs-lookup"><span data-stu-id="36514-119">The apps installed in the personal scope of this user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="36514-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="36514-120">JSON representation</span></span>

<span data-ttu-id="36514-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="36514-121">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="36514-122">另请参阅</span><span class="sxs-lookup"><span data-stu-id="36514-122">See Also</span></span>

- [<span data-ttu-id="36514-123">userTeamwork 资源类型</span><span class="sxs-lookup"><span data-stu-id="36514-123">userTeamwork resource</span></span>](userteamwork.md)


