---
title: teamsAppDefinition 资源类型
description: 一个版本的 teamsApp 的详细信息。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4b350c5ebe39da336dfe467bb73f5b91270dc31c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345797"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="8910f-103">teamsAppDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="8910f-103">teamsAppDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8910f-104">一个版本的[teamsApp](teamsapp.md)的详细信息。</span><span class="sxs-lookup"><span data-stu-id="8910f-104">The details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="8910f-105">属性</span><span class="sxs-lookup"><span data-stu-id="8910f-105">Properties</span></span>

| <span data-ttu-id="8910f-106">属性</span><span class="sxs-lookup"><span data-stu-id="8910f-106">Property</span></span>            | <span data-ttu-id="8910f-107">类型</span><span class="sxs-lookup"><span data-stu-id="8910f-107">Type</span></span>     | <span data-ttu-id="8910f-108">说明</span><span class="sxs-lookup"><span data-stu-id="8910f-108">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="8910f-109">id</span><span class="sxs-lookup"><span data-stu-id="8910f-109">id</span></span>                  | <span data-ttu-id="8910f-110">string</span><span class="sxs-lookup"><span data-stu-id="8910f-110">string</span></span>   | <span data-ttu-id="8910f-111">唯一 id (而不是团队 appid)。</span><span class="sxs-lookup"><span data-stu-id="8910f-111">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="8910f-112">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="8910f-112">teamsAppId</span></span>          | <span data-ttu-id="8910f-113">string</span><span class="sxs-lookup"><span data-stu-id="8910f-113">string</span></span>   | <span data-ttu-id="8910f-114">团队应用程序清单中的 id。</span><span class="sxs-lookup"><span data-stu-id="8910f-114">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="8910f-115">displayName</span><span class="sxs-lookup"><span data-stu-id="8910f-115">displayName</span></span>         | <span data-ttu-id="8910f-116">string</span><span class="sxs-lookup"><span data-stu-id="8910f-116">string</span></span>   | <span data-ttu-id="8910f-117">应用程序开发人员提供的应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="8910f-117">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="8910f-118">version</span><span class="sxs-lookup"><span data-stu-id="8910f-118">version</span></span>             | <span data-ttu-id="8910f-119">string</span><span class="sxs-lookup"><span data-stu-id="8910f-119">string</span></span>   | <span data-ttu-id="8910f-120">应用程序的版本号。</span><span class="sxs-lookup"><span data-stu-id="8910f-120">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8910f-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8910f-121">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppDefinition",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
  "teamsAppId": "string",
  "displayName": "Test App",
  "version": "1.0.0",
}
```

# <a name="see-also"></a><span data-ttu-id="8910f-122">另请参阅</span><span class="sxs-lookup"><span data-stu-id="8910f-122">See also</span></span>

- [<span data-ttu-id="8910f-123">teamsApp</span><span class="sxs-lookup"><span data-stu-id="8910f-123">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="8910f-124">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="8910f-124">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="8910f-125">teamsTab</span><span class="sxs-lookup"><span data-stu-id="8910f-125">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

