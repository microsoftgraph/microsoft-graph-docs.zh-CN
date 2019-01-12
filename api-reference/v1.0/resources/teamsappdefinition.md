---
title: teamsAppDefinition 资源类型
description: TeamsApp 的一个版本的详细信息。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 3aed533ecca3bff48071b04adadcea6b52169f89
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951927"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="4eb3f-103">teamsAppDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="4eb3f-103">teamsAppDefinition resource type</span></span>



<span data-ttu-id="4eb3f-104">[TeamsApp](teamsapp.md)的一个版本的详细信息。</span><span class="sxs-lookup"><span data-stu-id="4eb3f-104">The details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="4eb3f-105">属性</span><span class="sxs-lookup"><span data-stu-id="4eb3f-105">Properties</span></span>

| <span data-ttu-id="4eb3f-106">属性</span><span class="sxs-lookup"><span data-stu-id="4eb3f-106">Property</span></span>            | <span data-ttu-id="4eb3f-107">类型</span><span class="sxs-lookup"><span data-stu-id="4eb3f-107">Type</span></span>     | <span data-ttu-id="4eb3f-108">说明</span><span class="sxs-lookup"><span data-stu-id="4eb3f-108">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="4eb3f-109">ID</span><span class="sxs-lookup"><span data-stu-id="4eb3f-109">id</span></span>                  | <span data-ttu-id="4eb3f-110">string</span><span class="sxs-lookup"><span data-stu-id="4eb3f-110">string</span></span>   | <span data-ttu-id="4eb3f-111">唯一的 id (不团队 appid)。</span><span class="sxs-lookup"><span data-stu-id="4eb3f-111">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="4eb3f-112">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="4eb3f-112">teamsAppId</span></span>          | <span data-ttu-id="4eb3f-113">string</span><span class="sxs-lookup"><span data-stu-id="4eb3f-113">string</span></span>   | <span data-ttu-id="4eb3f-114">从工作组应用程序清单 id。</span><span class="sxs-lookup"><span data-stu-id="4eb3f-114">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="4eb3f-115">displayName</span><span class="sxs-lookup"><span data-stu-id="4eb3f-115">displayName</span></span>         | <span data-ttu-id="4eb3f-116">string</span><span class="sxs-lookup"><span data-stu-id="4eb3f-116">string</span></span>   | <span data-ttu-id="4eb3f-117">应用程序，应用程序开发人员提供的名称。</span><span class="sxs-lookup"><span data-stu-id="4eb3f-117">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="4eb3f-118">version</span><span class="sxs-lookup"><span data-stu-id="4eb3f-118">version</span></span>             | <span data-ttu-id="4eb3f-119">string</span><span class="sxs-lookup"><span data-stu-id="4eb3f-119">string</span></span>   | <span data-ttu-id="4eb3f-120">应用程序的版本号。</span><span class="sxs-lookup"><span data-stu-id="4eb3f-120">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4eb3f-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4eb3f-121">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="4eb3f-122">另请参阅</span><span class="sxs-lookup"><span data-stu-id="4eb3f-122">See also</span></span>

- [<span data-ttu-id="4eb3f-123">teamsApp</span><span class="sxs-lookup"><span data-stu-id="4eb3f-123">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="4eb3f-124">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="4eb3f-124">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="4eb3f-125">teamsTab</span><span class="sxs-lookup"><span data-stu-id="4eb3f-125">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

