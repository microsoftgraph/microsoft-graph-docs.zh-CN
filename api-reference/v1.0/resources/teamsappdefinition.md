---
title: teamsAppDefinition 资源类型
description: 一个版本的 teamsApp 的详细信息。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 3aed533ecca3bff48071b04adadcea6b52169f89
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462317"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="8ecdd-103">teamsAppDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="8ecdd-103">teamsAppDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ecdd-104">一个版本的[teamsApp](teamsapp.md)的详细信息。</span><span class="sxs-lookup"><span data-stu-id="8ecdd-104">The details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="8ecdd-105">属性</span><span class="sxs-lookup"><span data-stu-id="8ecdd-105">Properties</span></span>

| <span data-ttu-id="8ecdd-106">属性</span><span class="sxs-lookup"><span data-stu-id="8ecdd-106">Property</span></span>            | <span data-ttu-id="8ecdd-107">类型</span><span class="sxs-lookup"><span data-stu-id="8ecdd-107">Type</span></span>     | <span data-ttu-id="8ecdd-108">说明</span><span class="sxs-lookup"><span data-stu-id="8ecdd-108">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="8ecdd-109">id</span><span class="sxs-lookup"><span data-stu-id="8ecdd-109">id</span></span>                  | <span data-ttu-id="8ecdd-110">string</span><span class="sxs-lookup"><span data-stu-id="8ecdd-110">string</span></span>   | <span data-ttu-id="8ecdd-111">唯一 id (而不是团队 appid)。</span><span class="sxs-lookup"><span data-stu-id="8ecdd-111">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="8ecdd-112">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="8ecdd-112">teamsAppId</span></span>          | <span data-ttu-id="8ecdd-113">字符串</span><span class="sxs-lookup"><span data-stu-id="8ecdd-113">string</span></span>   | <span data-ttu-id="8ecdd-114">团队应用程序清单中的 id。</span><span class="sxs-lookup"><span data-stu-id="8ecdd-114">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="8ecdd-115">displayName</span><span class="sxs-lookup"><span data-stu-id="8ecdd-115">displayName</span></span>         | <span data-ttu-id="8ecdd-116">string</span><span class="sxs-lookup"><span data-stu-id="8ecdd-116">string</span></span>   | <span data-ttu-id="8ecdd-117">应用程序开发人员提供的应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="8ecdd-117">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="8ecdd-118">version</span><span class="sxs-lookup"><span data-stu-id="8ecdd-118">version</span></span>             | <span data-ttu-id="8ecdd-119">字符串</span><span class="sxs-lookup"><span data-stu-id="8ecdd-119">string</span></span>   | <span data-ttu-id="8ecdd-120">应用程序的版本号。</span><span class="sxs-lookup"><span data-stu-id="8ecdd-120">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8ecdd-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8ecdd-121">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="8ecdd-122">另请参阅</span><span class="sxs-lookup"><span data-stu-id="8ecdd-122">See also</span></span>

- [<span data-ttu-id="8ecdd-123">teamsApp</span><span class="sxs-lookup"><span data-stu-id="8ecdd-123">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="8ecdd-124">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="8ecdd-124">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="8ecdd-125">teamsTab</span><span class="sxs-lookup"><span data-stu-id="8ecdd-125">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsappdefinition.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

