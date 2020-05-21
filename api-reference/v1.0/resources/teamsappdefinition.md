---
title: teamsAppDefinition 资源类型
description: 一个版本的 teamsApp 的详细信息。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 95f701151370a6f741e7fa97aa1792ef67ad15d3
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44334954"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="ee418-103">teamsAppDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="ee418-103">teamsAppDefinition resource type</span></span>

<span data-ttu-id="ee418-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee418-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="ee418-105">一个版本的[teamsApp](teamsapp.md)的详细信息。</span><span class="sxs-lookup"><span data-stu-id="ee418-105">The details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ee418-106">属性</span><span class="sxs-lookup"><span data-stu-id="ee418-106">Properties</span></span>

| <span data-ttu-id="ee418-107">属性</span><span class="sxs-lookup"><span data-stu-id="ee418-107">Property</span></span>            | <span data-ttu-id="ee418-108">类型</span><span class="sxs-lookup"><span data-stu-id="ee418-108">Type</span></span>     | <span data-ttu-id="ee418-109">说明</span><span class="sxs-lookup"><span data-stu-id="ee418-109">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="ee418-110">id</span><span class="sxs-lookup"><span data-stu-id="ee418-110">id</span></span>                  | <span data-ttu-id="ee418-111">string</span><span class="sxs-lookup"><span data-stu-id="ee418-111">string</span></span>   | <span data-ttu-id="ee418-112">唯一 id （而不是团队 appid）。</span><span class="sxs-lookup"><span data-stu-id="ee418-112">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="ee418-113">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="ee418-113">teamsAppId</span></span>          | <span data-ttu-id="ee418-114">string</span><span class="sxs-lookup"><span data-stu-id="ee418-114">string</span></span>   | <span data-ttu-id="ee418-115">团队应用程序清单中的 id。</span><span class="sxs-lookup"><span data-stu-id="ee418-115">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="ee418-116">displayName</span><span class="sxs-lookup"><span data-stu-id="ee418-116">displayName</span></span>         | <span data-ttu-id="ee418-117">string</span><span class="sxs-lookup"><span data-stu-id="ee418-117">string</span></span>   | <span data-ttu-id="ee418-118">应用程序开发人员提供的应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="ee418-118">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="ee418-119">version</span><span class="sxs-lookup"><span data-stu-id="ee418-119">version</span></span>             | <span data-ttu-id="ee418-120">string</span><span class="sxs-lookup"><span data-stu-id="ee418-120">string</span></span>   | <span data-ttu-id="ee418-121">应用程序的版本号。</span><span class="sxs-lookup"><span data-stu-id="ee418-121">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ee418-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ee418-122">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="ee418-123">另请参阅</span><span class="sxs-lookup"><span data-stu-id="ee418-123">See also</span></span>

- [<span data-ttu-id="ee418-124">teamsApp</span><span class="sxs-lookup"><span data-stu-id="ee418-124">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="ee418-125">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="ee418-125">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="ee418-126">teamsTab</span><span class="sxs-lookup"><span data-stu-id="ee418-126">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

