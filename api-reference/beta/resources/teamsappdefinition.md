---
title: teamsAppDefinition 资源类型
description: teamsApp 的一个版本的详细信息。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 4e8bfd4b7248d37ce8ec4d85e01a498a88fed1c3
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882318"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="e6fab-103">teamsAppDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="e6fab-103">teamsAppDefinition resource type</span></span>

<span data-ttu-id="e6fab-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6fab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6fab-105">teamsApp [版本的详细信息](teamsapp.md)。</span><span class="sxs-lookup"><span data-stu-id="e6fab-105">The details of a version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e6fab-106">属性</span><span class="sxs-lookup"><span data-stu-id="e6fab-106">Properties</span></span>

| <span data-ttu-id="e6fab-107">属性</span><span class="sxs-lookup"><span data-stu-id="e6fab-107">Property</span></span>            | <span data-ttu-id="e6fab-108">类型</span><span class="sxs-lookup"><span data-stu-id="e6fab-108">Type</span></span>     | <span data-ttu-id="e6fab-109">说明</span><span class="sxs-lookup"><span data-stu-id="e6fab-109">Description</span></span>                                            |
|:------------------- |:-------- |:------------------------------------------------------ |
| <span data-ttu-id="e6fab-110">id</span><span class="sxs-lookup"><span data-stu-id="e6fab-110">id</span></span>                  | <span data-ttu-id="e6fab-111">string</span><span class="sxs-lookup"><span data-stu-id="e6fab-111">string</span></span>   | <span data-ttu-id="e6fab-112">唯一 ID (Teams 应用 ID) 。</span><span class="sxs-lookup"><span data-stu-id="e6fab-112">A unique ID (not the Teams app ID).</span></span>                     |
| <span data-ttu-id="e6fab-113">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="e6fab-113">teamsAppId</span></span>          | <span data-ttu-id="e6fab-114">string</span><span class="sxs-lookup"><span data-stu-id="e6fab-114">string</span></span>   | <span data-ttu-id="e6fab-115">Teams 应用清单中的 ID。</span><span class="sxs-lookup"><span data-stu-id="e6fab-115">The ID from the Teams app manifest.</span></span>                    |
| <span data-ttu-id="e6fab-116">publishingState</span><span class="sxs-lookup"><span data-stu-id="e6fab-116">publishingState</span></span>     | <span data-ttu-id="e6fab-117">string</span><span class="sxs-lookup"><span data-stu-id="e6fab-117">string</span></span>   | <span data-ttu-id="e6fab-118">Teams 应用特定版本的已发布状态。</span><span class="sxs-lookup"><span data-stu-id="e6fab-118">The published status of a specific version of a Teams app.</span></span> <span data-ttu-id="e6fab-119">可能的值是：</span><span class="sxs-lookup"><span data-stu-id="e6fab-119">Possible values are:</span></span></br><span data-ttu-id="e6fab-120">`submitted` — Teams 应用的特定版本已提交，正在审查中。</span><span class="sxs-lookup"><span data-stu-id="e6fab-120">`submitted` — The specific version of the Teams app has been submitted and is under review.</span></span> </br><span data-ttu-id="e6fab-121">`published`  — 发布特定版本的 Teams 应用的请求已由管理员批准，并且该应用已发布。</span><span class="sxs-lookup"><span data-stu-id="e6fab-121">`published`  — The request to publish the specific version of the Teams app has been approved by the admin and the app is published.</span></span> </br> <span data-ttu-id="e6fab-122">`rejected` — 管理员拒绝了发布 Teams 应用的特定版本的请求。</span><span class="sxs-lookup"><span data-stu-id="e6fab-122">`rejected` — The request to publish the specific version of the Teams app was rejected by the admin.</span></span> |
| <span data-ttu-id="e6fab-123">azureADAppId</span><span class="sxs-lookup"><span data-stu-id="e6fab-123">azureADAppId</span></span>        | <span data-ttu-id="e6fab-124">string</span><span class="sxs-lookup"><span data-stu-id="e6fab-124">string</span></span>   | <span data-ttu-id="e6fab-125">Teams WebApplicationInfo.Id 清单中的设置。</span><span class="sxs-lookup"><span data-stu-id="e6fab-125">The WebApplicationInfo.Id from the Teams app manifest.</span></span> |
| <span data-ttu-id="e6fab-126">displayName</span><span class="sxs-lookup"><span data-stu-id="e6fab-126">displayName</span></span>         | <span data-ttu-id="e6fab-127">string</span><span class="sxs-lookup"><span data-stu-id="e6fab-127">string</span></span>   | <span data-ttu-id="e6fab-128">应用开发人员提供的应用的名称。</span><span class="sxs-lookup"><span data-stu-id="e6fab-128">The name of the app provided by the app developer.</span></span>     |
| <span data-ttu-id="e6fab-129">version</span><span class="sxs-lookup"><span data-stu-id="e6fab-129">version</span></span>             | <span data-ttu-id="e6fab-130">string</span><span class="sxs-lookup"><span data-stu-id="e6fab-130">string</span></span>   | <span data-ttu-id="e6fab-131">应用程序的版本号。</span><span class="sxs-lookup"><span data-stu-id="e6fab-131">The version number of the application.</span></span>                 |
| <span data-ttu-id="e6fab-132">allowedInstallationScopes</span><span class="sxs-lookup"><span data-stu-id="e6fab-132">allowedInstallationScopes</span></span> | <span data-ttu-id="e6fab-133">teamsAppInstallationScope 集合</span><span class="sxs-lookup"><span data-stu-id="e6fab-133">teamsAppInstallationScope collection</span></span> | <span data-ttu-id="e6fab-134">可在其中安装 Teams 应用的范围集合。</span><span class="sxs-lookup"><span data-stu-id="e6fab-134">A collection of scopes where the Teams app can be installed.</span></span> <span data-ttu-id="e6fab-135">可能的值是：</span><span class="sxs-lookup"><span data-stu-id="e6fab-135">Possible values are:</span></span></br><span data-ttu-id="e6fab-136">`team` — 指示 Teams 应用可以安装在团队中，并有权访问该团队的数据。</span><span class="sxs-lookup"><span data-stu-id="e6fab-136">`team` — Indicates that the Teams app can be installed within a team and is authorized to access that team's data.</span></span> </br><span data-ttu-id="e6fab-137">`groupChat`  — 指示 Teams 应用可以安装在群聊中，并有权访问该群聊的数据。</span><span class="sxs-lookup"><span data-stu-id="e6fab-137">`groupChat`  — Indicates that the Teams app can be installed within a group chat and is authorized to access that group chat's data.</span></span> </br> <span data-ttu-id="e6fab-138">`personal` — 指示 Teams 应用可以安装在用户的个人范围内，并有权访问该用户的数据。</span><span class="sxs-lookup"><span data-stu-id="e6fab-138">`personal` — Indicates that the Teams app can be installed in the personal scope of a user and is authorized to access that user's data.</span></span> | 

## <a name="relationships"></a><span data-ttu-id="e6fab-139">关系</span><span class="sxs-lookup"><span data-stu-id="e6fab-139">Relationships</span></span>

| <span data-ttu-id="e6fab-140">关系</span><span class="sxs-lookup"><span data-stu-id="e6fab-140">Relationship</span></span>   | <span data-ttu-id="e6fab-141">类型</span><span class="sxs-lookup"><span data-stu-id="e6fab-141">Type</span></span>                           | <span data-ttu-id="e6fab-142">说明</span><span class="sxs-lookup"><span data-stu-id="e6fab-142">Description</span></span>                                                 |
|:-------------- |:------------------------------ |:----------------------------------------------------------- |
| <span data-ttu-id="e6fab-143">bot</span><span class="sxs-lookup"><span data-stu-id="e6fab-143">bot</span></span>            |[<span data-ttu-id="e6fab-144">teamworkBot</span><span class="sxs-lookup"><span data-stu-id="e6fab-144">teamworkBot</span></span>](teamworkbot.md)   | <span data-ttu-id="e6fab-145">Teams 应用清单中指定的自动程序的详细信息。</span><span class="sxs-lookup"><span data-stu-id="e6fab-145">The details of the bot specified in the Teams app manifest.</span></span> |
| <span data-ttu-id="e6fab-146">colorIcon</span><span class="sxs-lookup"><span data-stu-id="e6fab-146">colorIcon</span></span>      |[<span data-ttu-id="e6fab-147">teamsAppIcon</span><span class="sxs-lookup"><span data-stu-id="e6fab-147">teamsAppIcon</span></span>](teamsappicon.md) | <span data-ttu-id="e6fab-148">Teams 应用图标的颜色版本。</span><span class="sxs-lookup"><span data-stu-id="e6fab-148">The color version of the Teams app's icon.</span></span>                   |
| <span data-ttu-id="e6fab-149">outlineIcon</span><span class="sxs-lookup"><span data-stu-id="e6fab-149">outlineIcon</span></span>    |[<span data-ttu-id="e6fab-150">teamsAppIcon</span><span class="sxs-lookup"><span data-stu-id="e6fab-150">teamsAppIcon</span></span>](teamsappicon.md) | <span data-ttu-id="e6fab-151">Teams 应用图标的大纲版本。</span><span class="sxs-lookup"><span data-stu-id="e6fab-151">The outline version of the Teams app's icon.</span></span>                 |

## <a name="json-representation"></a><span data-ttu-id="e6fab-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e6fab-152">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppDefinition",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
  "teamsAppId": "string",
  "publishingState": "#microsoft.graph.teamsAppPublishingState",
  "azureADAppId": "string",
  "displayName": "string",
  "version": "string"
}
```

## <a name="see-also"></a><span data-ttu-id="e6fab-153">另请参阅</span><span class="sxs-lookup"><span data-stu-id="e6fab-153">See also</span></span>

- [<span data-ttu-id="e6fab-154">teamsApp</span><span class="sxs-lookup"><span data-stu-id="e6fab-154">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="e6fab-155">teamsAppIcon</span><span class="sxs-lookup"><span data-stu-id="e6fab-155">teamsAppIcon</span></span>](teamsappicon.md)
- [<span data-ttu-id="e6fab-156">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="e6fab-156">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="e6fab-157">teamsTab</span><span class="sxs-lookup"><span data-stu-id="e6fab-157">teamsTab</span></span>](../resources/teamstab.md)

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


