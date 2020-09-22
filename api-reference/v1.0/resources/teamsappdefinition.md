---
title: teamsAppDefinition 资源类型
description: 表示一个版本的 teamsApp 的详细信息。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 08a652c5b4ad4b9555eb7c09e33398f140ed97b0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48036931"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="91728-103">teamsAppDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="91728-103">teamsAppDefinition resource type</span></span>

<span data-ttu-id="91728-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91728-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="91728-105">表示一个版本的 [teamsApp](teamsapp.md)的详细信息。</span><span class="sxs-lookup"><span data-stu-id="91728-105">Represents the details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="91728-106">属性</span><span class="sxs-lookup"><span data-stu-id="91728-106">Properties</span></span>

| <span data-ttu-id="91728-107">属性</span><span class="sxs-lookup"><span data-stu-id="91728-107">Property</span></span>            | <span data-ttu-id="91728-108">类型</span><span class="sxs-lookup"><span data-stu-id="91728-108">Type</span></span>     | <span data-ttu-id="91728-109">说明</span><span class="sxs-lookup"><span data-stu-id="91728-109">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="91728-110">id</span><span class="sxs-lookup"><span data-stu-id="91728-110">id</span></span>                  | <span data-ttu-id="91728-111">string</span><span class="sxs-lookup"><span data-stu-id="91728-111">string</span></span>   | <span data-ttu-id="91728-112">唯一 ID (团队应用程序 ID) 。</span><span class="sxs-lookup"><span data-stu-id="91728-112">A unique ID (not the Teams app ID).</span></span> |
| <span data-ttu-id="91728-113">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="91728-113">teamsAppId</span></span>          | <span data-ttu-id="91728-114">字符串</span><span class="sxs-lookup"><span data-stu-id="91728-114">string</span></span>   | <span data-ttu-id="91728-115">团队应用程序清单中的 ID。</span><span class="sxs-lookup"><span data-stu-id="91728-115">The ID from the Teams app manifest.</span></span> |
| <span data-ttu-id="91728-116">publishingState</span><span class="sxs-lookup"><span data-stu-id="91728-116">publishingState</span></span>| <span data-ttu-id="91728-117">字符串</span><span class="sxs-lookup"><span data-stu-id="91728-117">string</span></span>|<span data-ttu-id="91728-118">特定版本的团队应用程序的已发布状态。</span><span class="sxs-lookup"><span data-stu-id="91728-118">The published status of a specific version of a Teams app.</span></span> <span data-ttu-id="91728-119">可能的值是：</span><span class="sxs-lookup"><span data-stu-id="91728-119">Possible values are:</span></span></br><span data-ttu-id="91728-120">`submitted` —团队应用程序的特定版本已提交，正在进行审阅。</span><span class="sxs-lookup"><span data-stu-id="91728-120">`submitted` — The specific version of the Teams app has been submitted and is under review.</span></span> </br><span data-ttu-id="91728-121">`published`  —发布特定版本的团队应用程序的请求已由管理员批准，并且应用已发布。</span><span class="sxs-lookup"><span data-stu-id="91728-121">`published`  — The request to publish the specific version of the Teams app has been approved by the admin and the app is published.</span></span> </br> <span data-ttu-id="91728-122">`rejected` —管理员拒绝了发布特定版本的团队应用程序的请求。</span><span class="sxs-lookup"><span data-stu-id="91728-122">`rejected` — The request to publish the specific version of the Teams app was rejected by the admin.</span></span> |
| <span data-ttu-id="91728-123">displayName</span><span class="sxs-lookup"><span data-stu-id="91728-123">displayName</span></span>         | <span data-ttu-id="91728-124">string</span><span class="sxs-lookup"><span data-stu-id="91728-124">string</span></span>   | <span data-ttu-id="91728-125">应用程序开发人员提供的应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="91728-125">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="91728-126">version</span><span class="sxs-lookup"><span data-stu-id="91728-126">version</span></span>             | <span data-ttu-id="91728-127">字符串</span><span class="sxs-lookup"><span data-stu-id="91728-127">string</span></span>   | <span data-ttu-id="91728-128">应用程序的版本号。</span><span class="sxs-lookup"><span data-stu-id="91728-128">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="91728-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="91728-129">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="91728-130">另请参阅</span><span class="sxs-lookup"><span data-stu-id="91728-130">See also</span></span>

- [<span data-ttu-id="91728-131">teamsApp</span><span class="sxs-lookup"><span data-stu-id="91728-131">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="91728-132">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="91728-132">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="91728-133">teamsTab</span><span class="sxs-lookup"><span data-stu-id="91728-133">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

