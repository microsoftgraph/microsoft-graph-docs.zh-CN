---
title: teamsAppDefinition 资源类型
description: 一个版本的 teamsApp 的详细信息。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b71fb575eeb22f76419a88c7a56837bf34a31770
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533506"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="72855-103">teamsAppDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="72855-103">teamsAppDefinition resource type</span></span>

<span data-ttu-id="72855-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72855-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="72855-105">一个版本的[teamsApp](teamsapp.md)的详细信息。</span><span class="sxs-lookup"><span data-stu-id="72855-105">The details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="72855-106">属性</span><span class="sxs-lookup"><span data-stu-id="72855-106">Properties</span></span>

| <span data-ttu-id="72855-107">属性</span><span class="sxs-lookup"><span data-stu-id="72855-107">Property</span></span>            | <span data-ttu-id="72855-108">类型</span><span class="sxs-lookup"><span data-stu-id="72855-108">Type</span></span>     | <span data-ttu-id="72855-109">说明</span><span class="sxs-lookup"><span data-stu-id="72855-109">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="72855-110">id</span><span class="sxs-lookup"><span data-stu-id="72855-110">id</span></span>                  | <span data-ttu-id="72855-111">string</span><span class="sxs-lookup"><span data-stu-id="72855-111">string</span></span>   | <span data-ttu-id="72855-112">唯一 id （而不是团队 appid）。</span><span class="sxs-lookup"><span data-stu-id="72855-112">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="72855-113">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="72855-113">teamsAppId</span></span>          | <span data-ttu-id="72855-114">字符串</span><span class="sxs-lookup"><span data-stu-id="72855-114">string</span></span>   | <span data-ttu-id="72855-115">团队应用程序清单中的 id。</span><span class="sxs-lookup"><span data-stu-id="72855-115">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="72855-116">displayName</span><span class="sxs-lookup"><span data-stu-id="72855-116">displayName</span></span>         | <span data-ttu-id="72855-117">string</span><span class="sxs-lookup"><span data-stu-id="72855-117">string</span></span>   | <span data-ttu-id="72855-118">应用程序开发人员提供的应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="72855-118">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="72855-119">version</span><span class="sxs-lookup"><span data-stu-id="72855-119">version</span></span>             | <span data-ttu-id="72855-120">字符串</span><span class="sxs-lookup"><span data-stu-id="72855-120">string</span></span>   | <span data-ttu-id="72855-121">应用程序的版本号。</span><span class="sxs-lookup"><span data-stu-id="72855-121">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="72855-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="72855-122">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="72855-123">另请参阅</span><span class="sxs-lookup"><span data-stu-id="72855-123">See also</span></span>

- [<span data-ttu-id="72855-124">teamsApp</span><span class="sxs-lookup"><span data-stu-id="72855-124">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="72855-125">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="72855-125">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="72855-126">teamsTab</span><span class="sxs-lookup"><span data-stu-id="72855-126">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

