---
title: teamsAppDefinition 资源类型
description: teamsApp 的一个版本的详细信息。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 6b5fd771d1fb38de5354c74778f5eae798ccc91e
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706113"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="7347e-103">teamsAppDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="7347e-103">teamsAppDefinition resource type</span></span>

<span data-ttu-id="7347e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7347e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7347e-105">teamsApp 版本 [的详细信息](teamsapp.md)。</span><span class="sxs-lookup"><span data-stu-id="7347e-105">The details of a version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="7347e-106">属性</span><span class="sxs-lookup"><span data-stu-id="7347e-106">Properties</span></span>

| <span data-ttu-id="7347e-107">属性</span><span class="sxs-lookup"><span data-stu-id="7347e-107">Property</span></span>            | <span data-ttu-id="7347e-108">类型</span><span class="sxs-lookup"><span data-stu-id="7347e-108">Type</span></span>     | <span data-ttu-id="7347e-109">说明</span><span class="sxs-lookup"><span data-stu-id="7347e-109">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="7347e-110">id</span><span class="sxs-lookup"><span data-stu-id="7347e-110">id</span></span>                  | <span data-ttu-id="7347e-111">string</span><span class="sxs-lookup"><span data-stu-id="7347e-111">string</span></span>   | <span data-ttu-id="7347e-112">唯一 id (不是 teams appid) 。</span><span class="sxs-lookup"><span data-stu-id="7347e-112">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="7347e-113">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="7347e-113">teamsAppId</span></span>          | <span data-ttu-id="7347e-114">string</span><span class="sxs-lookup"><span data-stu-id="7347e-114">string</span></span>   | <span data-ttu-id="7347e-115">Teams 应用清单中的 ID。</span><span class="sxs-lookup"><span data-stu-id="7347e-115">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="7347e-116">publishingState</span><span class="sxs-lookup"><span data-stu-id="7347e-116">publishingState</span></span>| <span data-ttu-id="7347e-117">string</span><span class="sxs-lookup"><span data-stu-id="7347e-117">string</span></span>|<span data-ttu-id="7347e-118">特定版本的 Teams 应用的已发布状态。</span><span class="sxs-lookup"><span data-stu-id="7347e-118">The published status of a specific version of a Teams app.</span></span> <span data-ttu-id="7347e-119">可能的值是：</span><span class="sxs-lookup"><span data-stu-id="7347e-119">Possible values are:</span></span></br><span data-ttu-id="7347e-120">`submitted` — Teams 应用的特定版本已提交，正在审查中。</span><span class="sxs-lookup"><span data-stu-id="7347e-120">`submitted` — The specific version of the Teams app has been submitted and is under review.</span></span> </br><span data-ttu-id="7347e-121">`published`  — 发布特定版本的 Teams 应用的请求已由管理员批准并发布。</span><span class="sxs-lookup"><span data-stu-id="7347e-121">`published`  — The request to publish the specific version of the Teams app has been approved by the admin and the app is published.</span></span> </br> <span data-ttu-id="7347e-122">`rejected` — 管理员拒绝了发布特定版本的 Teams 应用的请求。</span><span class="sxs-lookup"><span data-stu-id="7347e-122">`rejected` — The request to publish the specific version of the Teams app was rejected by the admin.</span></span> |
| <span data-ttu-id="7347e-123">azureADAppId</span><span class="sxs-lookup"><span data-stu-id="7347e-123">azureADAppId</span></span>        | <span data-ttu-id="7347e-124">string</span><span class="sxs-lookup"><span data-stu-id="7347e-124">string</span></span>   | <span data-ttu-id="7347e-125">Teams WebApplicationInfo.id清单中的设置。</span><span class="sxs-lookup"><span data-stu-id="7347e-125">The WebApplicationInfo.id from the Teams App manifest.</span></span> |
| <span data-ttu-id="7347e-126">displayName</span><span class="sxs-lookup"><span data-stu-id="7347e-126">displayName</span></span>         | <span data-ttu-id="7347e-127">string</span><span class="sxs-lookup"><span data-stu-id="7347e-127">string</span></span>   | <span data-ttu-id="7347e-128">应用开发人员提供的应用的名称。</span><span class="sxs-lookup"><span data-stu-id="7347e-128">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="7347e-129">version</span><span class="sxs-lookup"><span data-stu-id="7347e-129">version</span></span>             | <span data-ttu-id="7347e-130">string</span><span class="sxs-lookup"><span data-stu-id="7347e-130">string</span></span>   | <span data-ttu-id="7347e-131">应用程序的版本号。</span><span class="sxs-lookup"><span data-stu-id="7347e-131">The version number of the application.</span></span> |

## <a name="relationships"></a><span data-ttu-id="7347e-132">关系</span><span class="sxs-lookup"><span data-stu-id="7347e-132">Relationships</span></span>

| <span data-ttu-id="7347e-133">关系</span><span class="sxs-lookup"><span data-stu-id="7347e-133">Relationship</span></span> | <span data-ttu-id="7347e-134">类型</span><span class="sxs-lookup"><span data-stu-id="7347e-134">Type</span></span>   | <span data-ttu-id="7347e-135">说明</span><span class="sxs-lookup"><span data-stu-id="7347e-135">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="7347e-136">bot</span><span class="sxs-lookup"><span data-stu-id="7347e-136">bot</span></span>|[<span data-ttu-id="7347e-137">teamworkBot</span><span class="sxs-lookup"><span data-stu-id="7347e-137">teamworkBot</span></span>](teamworkbot.md) | <span data-ttu-id="7347e-138">Teams 应用清单中指定的自动程序的详细信息。</span><span class="sxs-lookup"><span data-stu-id="7347e-138">The details of the bot specified in the Teams App manifest.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7347e-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7347e-139">JSON representation</span></span>

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
  "version": "1.0.0"
}
```

## <a name="see-also"></a><span data-ttu-id="7347e-140">另请参阅</span><span class="sxs-lookup"><span data-stu-id="7347e-140">See also</span></span>

- [<span data-ttu-id="7347e-141">teamsApp</span><span class="sxs-lookup"><span data-stu-id="7347e-141">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="7347e-142">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="7347e-142">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="7347e-143">teamsTab</span><span class="sxs-lookup"><span data-stu-id="7347e-143">teamsTab</span></span>](../resources/teamstab.md)

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


