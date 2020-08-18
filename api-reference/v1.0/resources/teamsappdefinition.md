---
title: teamsAppDefinition 资源类型
description: 表示一个版本的 teamsApp 的详细信息。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 322b7f50ccb51702ae05ca55f8e73396321a0283
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/18/2020
ms.locfileid: "46791678"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="681a6-103">teamsAppDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="681a6-103">teamsAppDefinition resource type</span></span>

<span data-ttu-id="681a6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="681a6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="681a6-105">表示一个版本的 [teamsApp](teamsapp.md)的详细信息。</span><span class="sxs-lookup"><span data-stu-id="681a6-105">Represents the details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="681a6-106">属性</span><span class="sxs-lookup"><span data-stu-id="681a6-106">Properties</span></span>

| <span data-ttu-id="681a6-107">属性</span><span class="sxs-lookup"><span data-stu-id="681a6-107">Property</span></span>            | <span data-ttu-id="681a6-108">类型</span><span class="sxs-lookup"><span data-stu-id="681a6-108">Type</span></span>     | <span data-ttu-id="681a6-109">说明</span><span class="sxs-lookup"><span data-stu-id="681a6-109">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="681a6-110">id</span><span class="sxs-lookup"><span data-stu-id="681a6-110">id</span></span>                  | <span data-ttu-id="681a6-111">string</span><span class="sxs-lookup"><span data-stu-id="681a6-111">string</span></span>   | <span data-ttu-id="681a6-112">唯一 ID (团队应用程序 ID) 。</span><span class="sxs-lookup"><span data-stu-id="681a6-112">A unique ID (not the Teams app ID).</span></span> |
| <span data-ttu-id="681a6-113">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="681a6-113">teamsAppId</span></span>          | <span data-ttu-id="681a6-114">字符串</span><span class="sxs-lookup"><span data-stu-id="681a6-114">string</span></span>   | <span data-ttu-id="681a6-115">团队应用程序清单中的 ID。</span><span class="sxs-lookup"><span data-stu-id="681a6-115">The ID from the Teams app manifest.</span></span> |
| <span data-ttu-id="681a6-116">publishingState</span><span class="sxs-lookup"><span data-stu-id="681a6-116">publishingState</span></span>| <span data-ttu-id="681a6-117">字符串</span><span class="sxs-lookup"><span data-stu-id="681a6-117">string</span></span>|<span data-ttu-id="681a6-118">特定版本的团队应用程序的已发布状态。</span><span class="sxs-lookup"><span data-stu-id="681a6-118">The published status of a specific version of a Teams app.</span></span> <span data-ttu-id="681a6-119">可能的值是：</span><span class="sxs-lookup"><span data-stu-id="681a6-119">Possible values are:</span></span></br><span data-ttu-id="681a6-120">`submitted` —团队应用程序的特定版本已提交，正在进行审阅。</span><span class="sxs-lookup"><span data-stu-id="681a6-120">`submitted` — The specific version of the Teams app has been submitted and is under review.</span></span> </br><span data-ttu-id="681a6-121">`published`  —发布特定版本的团队应用程序的请求已由管理员批准，并且应用已发布。</span><span class="sxs-lookup"><span data-stu-id="681a6-121">`published`  — The request to publish the specific version of the Teams app has been approved by the admin and the app is published.</span></span> </br> <span data-ttu-id="681a6-122">`rejected` —管理员拒绝了发布特定版本的团队应用程序的请求。</span><span class="sxs-lookup"><span data-stu-id="681a6-122">`rejected` — The request to publish the specific version of the Teams app was rejected by the admin.</span></span> |
| <span data-ttu-id="681a6-123">displayName</span><span class="sxs-lookup"><span data-stu-id="681a6-123">displayName</span></span>         | <span data-ttu-id="681a6-124">string</span><span class="sxs-lookup"><span data-stu-id="681a6-124">string</span></span>   | <span data-ttu-id="681a6-125">应用程序开发人员提供的应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="681a6-125">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="681a6-126">version</span><span class="sxs-lookup"><span data-stu-id="681a6-126">version</span></span>             | <span data-ttu-id="681a6-127">字符串</span><span class="sxs-lookup"><span data-stu-id="681a6-127">string</span></span>   | <span data-ttu-id="681a6-128">应用程序的版本号。</span><span class="sxs-lookup"><span data-stu-id="681a6-128">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="681a6-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="681a6-129">JSON representation</span></span>

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
  "version": "string",
}
```

## <a name="see-also"></a><span data-ttu-id="681a6-130">另请参阅</span><span class="sxs-lookup"><span data-stu-id="681a6-130">See also</span></span>

- [<span data-ttu-id="681a6-131">teamsApp</span><span class="sxs-lookup"><span data-stu-id="681a6-131">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="681a6-132">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="681a6-132">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="681a6-133">teamsTab</span><span class="sxs-lookup"><span data-stu-id="681a6-133">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
