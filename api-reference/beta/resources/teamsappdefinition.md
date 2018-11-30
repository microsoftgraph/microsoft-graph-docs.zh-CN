---
title: teamsAppDefinition 资源类型
description: TeamsApp 的一个版本的详细信息。
ms.openlocfilehash: b2a5b86de67fa1a4ecf673434b13d09c64ebe678
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048019"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="481f3-103">teamsAppDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="481f3-103">teamsAppDefinition resource type</span></span>

> <span data-ttu-id="481f3-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="481f3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="481f3-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="481f3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="481f3-106">[TeamsApp](teamsapp.md)的一个版本的详细信息。</span><span class="sxs-lookup"><span data-stu-id="481f3-106">The details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="481f3-107">属性</span><span class="sxs-lookup"><span data-stu-id="481f3-107">Properties</span></span>

| <span data-ttu-id="481f3-108">属性</span><span class="sxs-lookup"><span data-stu-id="481f3-108">Property</span></span>            | <span data-ttu-id="481f3-109">类型</span><span class="sxs-lookup"><span data-stu-id="481f3-109">Type</span></span>     | <span data-ttu-id="481f3-110">说明</span><span class="sxs-lookup"><span data-stu-id="481f3-110">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="481f3-111">ID</span><span class="sxs-lookup"><span data-stu-id="481f3-111">id</span></span>                  | <span data-ttu-id="481f3-112">string</span><span class="sxs-lookup"><span data-stu-id="481f3-112">string</span></span>   | <span data-ttu-id="481f3-113">唯一的 id (不团队 appid)。</span><span class="sxs-lookup"><span data-stu-id="481f3-113">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="481f3-114">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="481f3-114">teamsAppId</span></span>          | <span data-ttu-id="481f3-115">string</span><span class="sxs-lookup"><span data-stu-id="481f3-115">string</span></span>   | <span data-ttu-id="481f3-116">从工作组应用程序清单 id。</span><span class="sxs-lookup"><span data-stu-id="481f3-116">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="481f3-117">displayName</span><span class="sxs-lookup"><span data-stu-id="481f3-117">displayName</span></span>         | <span data-ttu-id="481f3-118">string</span><span class="sxs-lookup"><span data-stu-id="481f3-118">string</span></span>   | <span data-ttu-id="481f3-119">应用程序，应用程序开发人员提供的名称。</span><span class="sxs-lookup"><span data-stu-id="481f3-119">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="481f3-120">version</span><span class="sxs-lookup"><span data-stu-id="481f3-120">version</span></span>             | <span data-ttu-id="481f3-121">string</span><span class="sxs-lookup"><span data-stu-id="481f3-121">string</span></span>   | <span data-ttu-id="481f3-122">应用程序的版本号。</span><span class="sxs-lookup"><span data-stu-id="481f3-122">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="481f3-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="481f3-123">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="481f3-124">另请参阅</span><span class="sxs-lookup"><span data-stu-id="481f3-124">See also</span></span>

- [<span data-ttu-id="481f3-125">teamsApp</span><span class="sxs-lookup"><span data-stu-id="481f3-125">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="481f3-126">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="481f3-126">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="481f3-127">teamsTab</span><span class="sxs-lookup"><span data-stu-id="481f3-127">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

