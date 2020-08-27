---
title: teamsAppDefinition 资源类型
description: 一个版本的 teamsApp 的详细信息。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 6f8cb1f316bf9051dba0fe0ac138d75faf95c8d7
ms.sourcegitcommit: c4366ac71cf496242c8ff435bc8d8b3816bdc1aa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2020
ms.locfileid: "47287489"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="1c5c4-103">teamsAppDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="1c5c4-103">teamsAppDefinition resource type</span></span>

<span data-ttu-id="1c5c4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c5c4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c5c4-105">一个版本的 [teamsApp](teamsapp.md)的详细信息。</span><span class="sxs-lookup"><span data-stu-id="1c5c4-105">The details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="1c5c4-106">属性</span><span class="sxs-lookup"><span data-stu-id="1c5c4-106">Properties</span></span>

| <span data-ttu-id="1c5c4-107">属性</span><span class="sxs-lookup"><span data-stu-id="1c5c4-107">Property</span></span>            | <span data-ttu-id="1c5c4-108">类型</span><span class="sxs-lookup"><span data-stu-id="1c5c4-108">Type</span></span>     | <span data-ttu-id="1c5c4-109">说明</span><span class="sxs-lookup"><span data-stu-id="1c5c4-109">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="1c5c4-110">id</span><span class="sxs-lookup"><span data-stu-id="1c5c4-110">id</span></span>                  | <span data-ttu-id="1c5c4-111">string</span><span class="sxs-lookup"><span data-stu-id="1c5c4-111">string</span></span>   | <span data-ttu-id="1c5c4-112">唯一 id (不是团队的 appid) 。</span><span class="sxs-lookup"><span data-stu-id="1c5c4-112">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="1c5c4-113">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="1c5c4-113">teamsAppId</span></span>          | <span data-ttu-id="1c5c4-114">string</span><span class="sxs-lookup"><span data-stu-id="1c5c4-114">string</span></span>   | <span data-ttu-id="1c5c4-115">团队应用程序清单中的 id。</span><span class="sxs-lookup"><span data-stu-id="1c5c4-115">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="1c5c4-116">publishingState</span><span class="sxs-lookup"><span data-stu-id="1c5c4-116">publishingState</span></span>| <span data-ttu-id="1c5c4-117">string</span><span class="sxs-lookup"><span data-stu-id="1c5c4-117">string</span></span>|<span data-ttu-id="1c5c4-118">特定版本的团队应用程序的已发布状态。</span><span class="sxs-lookup"><span data-stu-id="1c5c4-118">The published status of a specific version of a Teams app.</span></span> <span data-ttu-id="1c5c4-119">可能的值是：</span><span class="sxs-lookup"><span data-stu-id="1c5c4-119">Possible values are:</span></span></br><span data-ttu-id="1c5c4-120">`submitted` —团队应用程序的特定版本已提交，正在进行审阅。</span><span class="sxs-lookup"><span data-stu-id="1c5c4-120">`submitted` — The specific version of the Teams app has been submitted and is under review.</span></span> </br><span data-ttu-id="1c5c4-121">`published`  —发布特定版本的团队应用程序的请求已由管理员批准，并且应用已发布。</span><span class="sxs-lookup"><span data-stu-id="1c5c4-121">`published`  — The request to publish the specific version of the Teams app has been approved by the admin and the app is published.</span></span> </br> <span data-ttu-id="1c5c4-122">`rejected` —管理员拒绝了发布特定版本的团队应用程序的请求。</span><span class="sxs-lookup"><span data-stu-id="1c5c4-122">`rejected` — The request to publish the specific version of the Teams app was rejected by the admin.</span></span> |
| <span data-ttu-id="1c5c4-123">azureADAppId</span><span class="sxs-lookup"><span data-stu-id="1c5c4-123">azureADAppId</span></span>        | <span data-ttu-id="1c5c4-124">string</span><span class="sxs-lookup"><span data-stu-id="1c5c4-124">string</span></span>   | <span data-ttu-id="1c5c4-125">来自团队应用程序清单的 WebApplicationInfo.id。</span><span class="sxs-lookup"><span data-stu-id="1c5c4-125">The WebApplicationInfo.id from the Teams App manifest.</span></span> |
| <span data-ttu-id="1c5c4-126">displayName</span><span class="sxs-lookup"><span data-stu-id="1c5c4-126">displayName</span></span>         | <span data-ttu-id="1c5c4-127">string</span><span class="sxs-lookup"><span data-stu-id="1c5c4-127">string</span></span>   | <span data-ttu-id="1c5c4-128">应用程序开发人员提供的应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="1c5c4-128">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="1c5c4-129">version</span><span class="sxs-lookup"><span data-stu-id="1c5c4-129">version</span></span>             | <span data-ttu-id="1c5c4-130">string</span><span class="sxs-lookup"><span data-stu-id="1c5c4-130">string</span></span>   | <span data-ttu-id="1c5c4-131">应用程序的版本号。</span><span class="sxs-lookup"><span data-stu-id="1c5c4-131">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1c5c4-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1c5c4-132">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="1c5c4-133">另请参阅</span><span class="sxs-lookup"><span data-stu-id="1c5c4-133">See also</span></span>

- [<span data-ttu-id="1c5c4-134">teamsApp</span><span class="sxs-lookup"><span data-stu-id="1c5c4-134">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="1c5c4-135">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="1c5c4-135">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="1c5c4-136">teamsTab</span><span class="sxs-lookup"><span data-stu-id="1c5c4-136">teamsTab</span></span>](../resources/teamstab.md)

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
