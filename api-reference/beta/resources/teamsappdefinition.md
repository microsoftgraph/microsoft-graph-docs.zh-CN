---
title: teamsAppDefinition 资源类型
description: TeamsApp 的一个版本的详细信息。
author: nkramer
ms.openlocfilehash: 71a1783131661aed120f375f7cc58d55fb0ca0d2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336832"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="5bf59-103">teamsAppDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="5bf59-103">teamsAppDefinition resource type</span></span>

> <span data-ttu-id="5bf59-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5bf59-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5bf59-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5bf59-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5bf59-106">[TeamsApp](teamsapp.md)的一个版本的详细信息。</span><span class="sxs-lookup"><span data-stu-id="5bf59-106">The details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5bf59-107">属性</span><span class="sxs-lookup"><span data-stu-id="5bf59-107">Properties</span></span>

| <span data-ttu-id="5bf59-108">属性</span><span class="sxs-lookup"><span data-stu-id="5bf59-108">Property</span></span>            | <span data-ttu-id="5bf59-109">类型</span><span class="sxs-lookup"><span data-stu-id="5bf59-109">Type</span></span>     | <span data-ttu-id="5bf59-110">说明</span><span class="sxs-lookup"><span data-stu-id="5bf59-110">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="5bf59-111">ID</span><span class="sxs-lookup"><span data-stu-id="5bf59-111">id</span></span>                  | <span data-ttu-id="5bf59-112">string</span><span class="sxs-lookup"><span data-stu-id="5bf59-112">string</span></span>   | <span data-ttu-id="5bf59-113">唯一的 id (不团队 appid)。</span><span class="sxs-lookup"><span data-stu-id="5bf59-113">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="5bf59-114">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="5bf59-114">teamsAppId</span></span>          | <span data-ttu-id="5bf59-115">string</span><span class="sxs-lookup"><span data-stu-id="5bf59-115">string</span></span>   | <span data-ttu-id="5bf59-116">从工作组应用程序清单 id。</span><span class="sxs-lookup"><span data-stu-id="5bf59-116">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="5bf59-117">displayName</span><span class="sxs-lookup"><span data-stu-id="5bf59-117">displayName</span></span>         | <span data-ttu-id="5bf59-118">string</span><span class="sxs-lookup"><span data-stu-id="5bf59-118">string</span></span>   | <span data-ttu-id="5bf59-119">应用程序，应用程序开发人员提供的名称。</span><span class="sxs-lookup"><span data-stu-id="5bf59-119">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="5bf59-120">version</span><span class="sxs-lookup"><span data-stu-id="5bf59-120">version</span></span>             | <span data-ttu-id="5bf59-121">string</span><span class="sxs-lookup"><span data-stu-id="5bf59-121">string</span></span>   | <span data-ttu-id="5bf59-122">应用程序的版本号。</span><span class="sxs-lookup"><span data-stu-id="5bf59-122">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5bf59-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5bf59-123">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="5bf59-124">另请参阅</span><span class="sxs-lookup"><span data-stu-id="5bf59-124">See also</span></span>

- [<span data-ttu-id="5bf59-125">teamsApp</span><span class="sxs-lookup"><span data-stu-id="5bf59-125">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="5bf59-126">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="5bf59-126">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="5bf59-127">teamsTab</span><span class="sxs-lookup"><span data-stu-id="5bf59-127">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

