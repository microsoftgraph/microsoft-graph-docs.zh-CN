---
title: teamsAppInstallation 资源类型
description: '团队中安装 teamsApp。 '
author: nkramer
ms.openlocfilehash: cab42c3bc2bde2e20dff3478d432d70e1563d248
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27341795"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="672bc-103">teamsAppInstallation 资源类型</span><span class="sxs-lookup"><span data-stu-id="672bc-103">teamsAppInstallation resource type</span></span>

> <span data-ttu-id="672bc-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="672bc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="672bc-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="672bc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="672bc-106">安装在[工作组](team.md) [teamsApp](teamsapp.md) 。</span><span class="sxs-lookup"><span data-stu-id="672bc-106">A [teamsApp](teamsapp.md) installed in a [team](team.md).</span></span> <span data-ttu-id="672bc-107">应用程序一部分的任何 bot 将成为应用程序添加到任何工作组的一部分。</span><span class="sxs-lookup"><span data-stu-id="672bc-107">Any bots that are part of the app will become part of any team the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="672bc-108">方法</span><span class="sxs-lookup"><span data-stu-id="672bc-108">Methods</span></span>

| <span data-ttu-id="672bc-109">方法</span><span class="sxs-lookup"><span data-stu-id="672bc-109">Method</span></span>       | <span data-ttu-id="672bc-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="672bc-110">Return Type</span></span>  |<span data-ttu-id="672bc-111">说明</span><span class="sxs-lookup"><span data-stu-id="672bc-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="672bc-112">列表应用程序</span><span class="sxs-lookup"><span data-stu-id="672bc-112">List apps</span></span>](../api/teamsappinstallation-list.md) | [<span data-ttu-id="672bc-113">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="672bc-113">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="672bc-114">列出了安装团队中的应用程序。</span><span class="sxs-lookup"><span data-stu-id="672bc-114">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="672bc-115">添加应用程序</span><span class="sxs-lookup"><span data-stu-id="672bc-115">Add app</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="672bc-116">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="672bc-116">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="672bc-117">将 （安装） 添加到团队应用程序。</span><span class="sxs-lookup"><span data-stu-id="672bc-117">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="672bc-118">删除应用程序</span><span class="sxs-lookup"><span data-stu-id="672bc-118">Remove app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="672bc-119">无</span><span class="sxs-lookup"><span data-stu-id="672bc-119">None</span></span> | <span data-ttu-id="672bc-120">删除 （卸载） 从团队应用程序。</span><span class="sxs-lookup"><span data-stu-id="672bc-120">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="672bc-121">升级的应用程序</span><span class="sxs-lookup"><span data-stu-id="672bc-121">Upgrade app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="672bc-122">无</span><span class="sxs-lookup"><span data-stu-id="672bc-122">None</span></span> | <span data-ttu-id="672bc-123">升级到最新版本的应用程序。</span><span class="sxs-lookup"><span data-stu-id="672bc-123">Upgrades to the latest version of the app.</span></span>|

## <a name="properties"></a><span data-ttu-id="672bc-124">属性</span><span class="sxs-lookup"><span data-stu-id="672bc-124">Properties</span></span>

| <span data-ttu-id="672bc-125">属性</span><span class="sxs-lookup"><span data-stu-id="672bc-125">Property</span></span>            | <span data-ttu-id="672bc-126">类型</span><span class="sxs-lookup"><span data-stu-id="672bc-126">Type</span></span>     | <span data-ttu-id="672bc-127">说明</span><span class="sxs-lookup"><span data-stu-id="672bc-127">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="672bc-128">ID</span><span class="sxs-lookup"><span data-stu-id="672bc-128">id</span></span>                  | <span data-ttu-id="672bc-129">string</span><span class="sxs-lookup"><span data-stu-id="672bc-129">string</span></span>   | <span data-ttu-id="672bc-130">唯一的 id (不团队 appid)。</span><span class="sxs-lookup"><span data-stu-id="672bc-130">A unique id (not the teams appid).</span></span> |

## <a name="relationships"></a><span data-ttu-id="672bc-131">Relationships</span><span class="sxs-lookup"><span data-stu-id="672bc-131">Relationships</span></span>

| <span data-ttu-id="672bc-132">关系</span><span class="sxs-lookup"><span data-stu-id="672bc-132">Relationship</span></span>   | <span data-ttu-id="672bc-133">类型</span><span class="sxs-lookup"><span data-stu-id="672bc-133">Type</span></span>    | <span data-ttu-id="672bc-134">说明</span><span class="sxs-lookup"><span data-stu-id="672bc-134">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="672bc-135">teamsApp</span><span class="sxs-lookup"><span data-stu-id="672bc-135">teamsApp</span></span>|[<span data-ttu-id="672bc-136">teamsApp</span><span class="sxs-lookup"><span data-stu-id="672bc-136">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="672bc-137">安装应用程序。</span><span class="sxs-lookup"><span data-stu-id="672bc-137">The app that is installed.</span></span> |
|<span data-ttu-id="672bc-138">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="672bc-138">teamsAppDefinition</span></span>|[<span data-ttu-id="672bc-139">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="672bc-139">teamsAppDefinition</span></span>](teamsapp.md)| <span data-ttu-id="672bc-140">此版本的应用程序的详细信息。</span><span class="sxs-lookup"><span data-stu-id="672bc-140">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="672bc-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="672bc-141">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
}
```

# <a name="see-also"></a><span data-ttu-id="672bc-142">另请参阅</span><span class="sxs-lookup"><span data-stu-id="672bc-142">See also</span></span>

- [<span data-ttu-id="672bc-143">teamsApp</span><span class="sxs-lookup"><span data-stu-id="672bc-143">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="672bc-144">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="672bc-144">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="672bc-145">teamsTab</span><span class="sxs-lookup"><span data-stu-id="672bc-145">teamsTab</span></span>](../resources/teamstab.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

