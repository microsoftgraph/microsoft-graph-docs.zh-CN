---
title: teamsAppDefinition 资源类型
description: 表示 teamsApp 的一个版本的详细信息。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8a43083e1f7fb717e2d54caef4017aeae97d9392
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50625931"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="05fc6-103">teamsAppDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="05fc6-103">teamsAppDefinition resource type</span></span>

<span data-ttu-id="05fc6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05fc6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="05fc6-105">表示 [teamsApp](teamsapp.md)版本的详细信息。</span><span class="sxs-lookup"><span data-stu-id="05fc6-105">Represents the details of a version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="05fc6-106">属性</span><span class="sxs-lookup"><span data-stu-id="05fc6-106">Properties</span></span>

| <span data-ttu-id="05fc6-107">属性</span><span class="sxs-lookup"><span data-stu-id="05fc6-107">Property</span></span>            | <span data-ttu-id="05fc6-108">类型</span><span class="sxs-lookup"><span data-stu-id="05fc6-108">Type</span></span>     | <span data-ttu-id="05fc6-109">说明</span><span class="sxs-lookup"><span data-stu-id="05fc6-109">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="05fc6-110">id</span><span class="sxs-lookup"><span data-stu-id="05fc6-110">id</span></span>                  | <span data-ttu-id="05fc6-111">string</span><span class="sxs-lookup"><span data-stu-id="05fc6-111">string</span></span>   | <span data-ttu-id="05fc6-112">唯一 ID (Teams 应用 ID) 。</span><span class="sxs-lookup"><span data-stu-id="05fc6-112">A unique ID (not the Teams app ID).</span></span> |
| <span data-ttu-id="05fc6-113">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="05fc6-113">teamsAppId</span></span>          | <span data-ttu-id="05fc6-114">string</span><span class="sxs-lookup"><span data-stu-id="05fc6-114">string</span></span>   | <span data-ttu-id="05fc6-115">Teams 应用清单中的 ID。</span><span class="sxs-lookup"><span data-stu-id="05fc6-115">The ID from the Teams app manifest.</span></span> |
| <span data-ttu-id="05fc6-116">publishingState</span><span class="sxs-lookup"><span data-stu-id="05fc6-116">publishingState</span></span>| <span data-ttu-id="05fc6-117">string</span><span class="sxs-lookup"><span data-stu-id="05fc6-117">string</span></span>|<span data-ttu-id="05fc6-118">特定版本的 Teams 应用的已发布状态。</span><span class="sxs-lookup"><span data-stu-id="05fc6-118">The published status of a specific version of a Teams app.</span></span> <span data-ttu-id="05fc6-119">可能的值是：</span><span class="sxs-lookup"><span data-stu-id="05fc6-119">Possible values are:</span></span></br><span data-ttu-id="05fc6-120">`submitted` — Teams 应用的特定版本已提交，正在审查中。</span><span class="sxs-lookup"><span data-stu-id="05fc6-120">`submitted` — The specific version of the Teams app has been submitted and is under review.</span></span> </br><span data-ttu-id="05fc6-121">`published`  — 发布特定版本的 Teams 应用的请求已由管理员批准，并且该应用已发布。</span><span class="sxs-lookup"><span data-stu-id="05fc6-121">`published`  — The request to publish the specific version of the Teams app has been approved by the admin and the app is published.</span></span> </br> <span data-ttu-id="05fc6-122">`rejected` — 管理员拒绝了发布特定版本的 Teams 应用的请求。</span><span class="sxs-lookup"><span data-stu-id="05fc6-122">`rejected` — The request to publish the specific version of the Teams app was rejected by the admin.</span></span> |
| <span data-ttu-id="05fc6-123">displayName</span><span class="sxs-lookup"><span data-stu-id="05fc6-123">displayName</span></span>         | <span data-ttu-id="05fc6-124">string</span><span class="sxs-lookup"><span data-stu-id="05fc6-124">string</span></span>   | <span data-ttu-id="05fc6-125">应用开发人员提供的应用的名称。</span><span class="sxs-lookup"><span data-stu-id="05fc6-125">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="05fc6-126">version</span><span class="sxs-lookup"><span data-stu-id="05fc6-126">version</span></span>             | <span data-ttu-id="05fc6-127">string</span><span class="sxs-lookup"><span data-stu-id="05fc6-127">string</span></span>   | <span data-ttu-id="05fc6-128">应用程序的版本号。</span><span class="sxs-lookup"><span data-stu-id="05fc6-128">The version number of the application.</span></span> |
| <span data-ttu-id="05fc6-129">shortDescription</span><span class="sxs-lookup"><span data-stu-id="05fc6-129">shortDescription</span></span>    | <span data-ttu-id="05fc6-130">string</span><span class="sxs-lookup"><span data-stu-id="05fc6-130">string</span></span>   | <span data-ttu-id="05fc6-131">应用程序的简短说明。</span><span class="sxs-lookup"><span data-stu-id="05fc6-131">Short description of the application.</span></span> |
| <span data-ttu-id="05fc6-132">说明</span><span class="sxs-lookup"><span data-stu-id="05fc6-132">description</span></span>         | <span data-ttu-id="05fc6-133">string</span><span class="sxs-lookup"><span data-stu-id="05fc6-133">string</span></span>   | <span data-ttu-id="05fc6-134">应用程序的详细说明。</span><span class="sxs-lookup"><span data-stu-id="05fc6-134">Verbose description of the application.</span></span> |

## <a name="relationships"></a><span data-ttu-id="05fc6-135">关系</span><span class="sxs-lookup"><span data-stu-id="05fc6-135">Relationships</span></span>

| <span data-ttu-id="05fc6-136">关系</span><span class="sxs-lookup"><span data-stu-id="05fc6-136">Relationship</span></span> | <span data-ttu-id="05fc6-137">类型</span><span class="sxs-lookup"><span data-stu-id="05fc6-137">Type</span></span>   | <span data-ttu-id="05fc6-138">说明</span><span class="sxs-lookup"><span data-stu-id="05fc6-138">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="05fc6-139">bot</span><span class="sxs-lookup"><span data-stu-id="05fc6-139">bot</span></span>|[<span data-ttu-id="05fc6-140">teamworkBot</span><span class="sxs-lookup"><span data-stu-id="05fc6-140">teamworkBot</span></span>](teamworkbot.md) | <span data-ttu-id="05fc6-141">Teams 应用清单中指定的自动程序的详细信息。</span><span class="sxs-lookup"><span data-stu-id="05fc6-141">The details of the bot specified in the Teams app manifest.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="05fc6-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="05fc6-142">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppDefinition",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
  "teamsAppId": "string",
  "displayName": "string",
  "version": "string"
}
```

## <a name="see-also"></a><span data-ttu-id="05fc6-143">另请参阅</span><span class="sxs-lookup"><span data-stu-id="05fc6-143">See also</span></span>

- [<span data-ttu-id="05fc6-144">teamsApp</span><span class="sxs-lookup"><span data-stu-id="05fc6-144">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="05fc6-145">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="05fc6-145">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="05fc6-146">teamsTab</span><span class="sxs-lookup"><span data-stu-id="05fc6-146">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

