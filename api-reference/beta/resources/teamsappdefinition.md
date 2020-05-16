---
title: teamsAppDefinition 资源类型
description: 一个版本的 teamsApp 的详细信息。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b8dd3e7b3e50ed5642aeb23076705f4995e27759
ms.sourcegitcommit: 62c900af626e46439d949462f09061cc5c41d6ff
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/16/2020
ms.locfileid: "44272708"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="d5e45-103">teamsAppDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="d5e45-103">teamsAppDefinition resource type</span></span>

<span data-ttu-id="d5e45-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5e45-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5e45-105">一个版本的[teamsApp](teamsapp.md)的详细信息。</span><span class="sxs-lookup"><span data-stu-id="d5e45-105">The details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d5e45-106">属性</span><span class="sxs-lookup"><span data-stu-id="d5e45-106">Properties</span></span>

| <span data-ttu-id="d5e45-107">属性</span><span class="sxs-lookup"><span data-stu-id="d5e45-107">Property</span></span>            | <span data-ttu-id="d5e45-108">类型</span><span class="sxs-lookup"><span data-stu-id="d5e45-108">Type</span></span>     | <span data-ttu-id="d5e45-109">说明</span><span class="sxs-lookup"><span data-stu-id="d5e45-109">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="d5e45-110">id</span><span class="sxs-lookup"><span data-stu-id="d5e45-110">id</span></span>                  | <span data-ttu-id="d5e45-111">string</span><span class="sxs-lookup"><span data-stu-id="d5e45-111">string</span></span>   | <span data-ttu-id="d5e45-112">唯一 id （而不是团队 appid）。</span><span class="sxs-lookup"><span data-stu-id="d5e45-112">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="d5e45-113">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="d5e45-113">teamsAppId</span></span>          | <span data-ttu-id="d5e45-114">string</span><span class="sxs-lookup"><span data-stu-id="d5e45-114">string</span></span>   | <span data-ttu-id="d5e45-115">团队应用程序清单中的 id。</span><span class="sxs-lookup"><span data-stu-id="d5e45-115">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="d5e45-116">azureADAppId</span><span class="sxs-lookup"><span data-stu-id="d5e45-116">azureADAppId</span></span>        | <span data-ttu-id="d5e45-117">string</span><span class="sxs-lookup"><span data-stu-id="d5e45-117">string</span></span>   | <span data-ttu-id="d5e45-118">来自团队应用程序清单的 WebApplicationInfo.id。</span><span class="sxs-lookup"><span data-stu-id="d5e45-118">The WebApplicationInfo.id from the Teams App manifest.</span></span> |
| <span data-ttu-id="d5e45-119">displayName</span><span class="sxs-lookup"><span data-stu-id="d5e45-119">displayName</span></span>         | <span data-ttu-id="d5e45-120">string</span><span class="sxs-lookup"><span data-stu-id="d5e45-120">string</span></span>   | <span data-ttu-id="d5e45-121">应用程序开发人员提供的应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="d5e45-121">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="d5e45-122">version</span><span class="sxs-lookup"><span data-stu-id="d5e45-122">version</span></span>             | <span data-ttu-id="d5e45-123">string</span><span class="sxs-lookup"><span data-stu-id="d5e45-123">string</span></span>   | <span data-ttu-id="d5e45-124">应用程序的版本号。</span><span class="sxs-lookup"><span data-stu-id="d5e45-124">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d5e45-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d5e45-125">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="d5e45-126">另请参阅</span><span class="sxs-lookup"><span data-stu-id="d5e45-126">See also</span></span>

- [<span data-ttu-id="d5e45-127">teamsApp</span><span class="sxs-lookup"><span data-stu-id="d5e45-127">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="d5e45-128">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="d5e45-128">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="d5e45-129">teamsTab</span><span class="sxs-lookup"><span data-stu-id="d5e45-129">teamsTab</span></span>](../resources/teamstab.md)

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

