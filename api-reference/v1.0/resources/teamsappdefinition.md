---
title: teamsAppDefinition 资源类型
description: TeamsApp 的一个版本的详细信息。
author: nkramer
ms.openlocfilehash: 43bd4262008a29668739e78d4b598da1e77e3d4b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351637"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="be22c-103">teamsAppDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="be22c-103">teamsAppDefinition resource type</span></span>



<span data-ttu-id="be22c-104">[TeamsApp](teamsapp.md)的一个版本的详细信息。</span><span class="sxs-lookup"><span data-stu-id="be22c-104">The details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="be22c-105">属性</span><span class="sxs-lookup"><span data-stu-id="be22c-105">Properties</span></span>

| <span data-ttu-id="be22c-106">属性</span><span class="sxs-lookup"><span data-stu-id="be22c-106">Property</span></span>            | <span data-ttu-id="be22c-107">类型</span><span class="sxs-lookup"><span data-stu-id="be22c-107">Type</span></span>     | <span data-ttu-id="be22c-108">说明</span><span class="sxs-lookup"><span data-stu-id="be22c-108">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="be22c-109">ID</span><span class="sxs-lookup"><span data-stu-id="be22c-109">id</span></span>                  | <span data-ttu-id="be22c-110">string</span><span class="sxs-lookup"><span data-stu-id="be22c-110">string</span></span>   | <span data-ttu-id="be22c-111">唯一的 id (不团队 appid)。</span><span class="sxs-lookup"><span data-stu-id="be22c-111">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="be22c-112">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="be22c-112">teamsAppId</span></span>          | <span data-ttu-id="be22c-113">string</span><span class="sxs-lookup"><span data-stu-id="be22c-113">string</span></span>   | <span data-ttu-id="be22c-114">从工作组应用程序清单 id。</span><span class="sxs-lookup"><span data-stu-id="be22c-114">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="be22c-115">displayName</span><span class="sxs-lookup"><span data-stu-id="be22c-115">displayName</span></span>         | <span data-ttu-id="be22c-116">string</span><span class="sxs-lookup"><span data-stu-id="be22c-116">string</span></span>   | <span data-ttu-id="be22c-117">应用程序，应用程序开发人员提供的名称。</span><span class="sxs-lookup"><span data-stu-id="be22c-117">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="be22c-118">version</span><span class="sxs-lookup"><span data-stu-id="be22c-118">version</span></span>             | <span data-ttu-id="be22c-119">string</span><span class="sxs-lookup"><span data-stu-id="be22c-119">string</span></span>   | <span data-ttu-id="be22c-120">应用程序的版本号。</span><span class="sxs-lookup"><span data-stu-id="be22c-120">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="be22c-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="be22c-121">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="be22c-122">另请参阅</span><span class="sxs-lookup"><span data-stu-id="be22c-122">See also</span></span>

- [<span data-ttu-id="be22c-123">teamsApp</span><span class="sxs-lookup"><span data-stu-id="be22c-123">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="be22c-124">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="be22c-124">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="be22c-125">teamsTab</span><span class="sxs-lookup"><span data-stu-id="be22c-125">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

