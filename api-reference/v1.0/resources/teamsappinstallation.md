---
title: teamsAppInstallation 资源类型
description: '在团队中安装的 teamsApp。 '
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 70dfe86840bd908a2e626b7f965d89251b9221aa
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533499"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="0910a-103">teamsAppInstallation 资源类型</span><span class="sxs-lookup"><span data-stu-id="0910a-103">teamsAppInstallation resource type</span></span>

<span data-ttu-id="0910a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0910a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0910a-105">在[团队](team.md)中安装的[teamsApp](teamsapp.md) 。</span><span class="sxs-lookup"><span data-stu-id="0910a-105">A [teamsApp](teamsapp.md) installed in a [team](team.md).</span></span> <span data-ttu-id="0910a-106">作为应用程序的一部分的任何 bot 都将成为向其添加应用程序的任何团队的一部分。</span><span class="sxs-lookup"><span data-stu-id="0910a-106">Any bots that are part of the app will become part of any team the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="0910a-107">Methods</span><span class="sxs-lookup"><span data-stu-id="0910a-107">Methods</span></span>

| <span data-ttu-id="0910a-108">方法</span><span class="sxs-lookup"><span data-stu-id="0910a-108">Method</span></span>       | <span data-ttu-id="0910a-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="0910a-109">Return Type</span></span>  |<span data-ttu-id="0910a-110">说明</span><span class="sxs-lookup"><span data-stu-id="0910a-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0910a-111">列出应用程序</span><span class="sxs-lookup"><span data-stu-id="0910a-111">List apps</span></span>](../api/teamsappinstallation-list.md) | [<span data-ttu-id="0910a-112">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="0910a-112">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="0910a-113">列出在团队中安装的应用程序。</span><span class="sxs-lookup"><span data-stu-id="0910a-113">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="0910a-114">添加应用程序</span><span class="sxs-lookup"><span data-stu-id="0910a-114">Add app</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="0910a-115">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="0910a-115">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="0910a-116">将应用添加（安装）到团队。</span><span class="sxs-lookup"><span data-stu-id="0910a-116">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="0910a-117">删除应用程序</span><span class="sxs-lookup"><span data-stu-id="0910a-117">Remove app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="0910a-118">无</span><span class="sxs-lookup"><span data-stu-id="0910a-118">None</span></span> | <span data-ttu-id="0910a-119">从团队中删除（卸载）应用程序。</span><span class="sxs-lookup"><span data-stu-id="0910a-119">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="0910a-120">升级应用</span><span class="sxs-lookup"><span data-stu-id="0910a-120">Upgrade app</span></span>](../api/teamsappinstallation-upgrade.md) | <span data-ttu-id="0910a-121">无</span><span class="sxs-lookup"><span data-stu-id="0910a-121">None</span></span> | <span data-ttu-id="0910a-122">升级到最新版本的应用程序。</span><span class="sxs-lookup"><span data-stu-id="0910a-122">Upgrades to the latest version of the app.</span></span>|

## <a name="properties"></a><span data-ttu-id="0910a-123">属性</span><span class="sxs-lookup"><span data-stu-id="0910a-123">Properties</span></span>

| <span data-ttu-id="0910a-124">属性</span><span class="sxs-lookup"><span data-stu-id="0910a-124">Property</span></span>            | <span data-ttu-id="0910a-125">类型</span><span class="sxs-lookup"><span data-stu-id="0910a-125">Type</span></span>     | <span data-ttu-id="0910a-126">说明</span><span class="sxs-lookup"><span data-stu-id="0910a-126">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="0910a-127">id</span><span class="sxs-lookup"><span data-stu-id="0910a-127">id</span></span>                  | <span data-ttu-id="0910a-128">string</span><span class="sxs-lookup"><span data-stu-id="0910a-128">string</span></span>   | <span data-ttu-id="0910a-129">唯一 id （而不是团队 appid）。</span><span class="sxs-lookup"><span data-stu-id="0910a-129">A unique id (not the teams appid).</span></span> |

## <a name="relationships"></a><span data-ttu-id="0910a-130">关系</span><span class="sxs-lookup"><span data-stu-id="0910a-130">Relationships</span></span>

| <span data-ttu-id="0910a-131">关系</span><span class="sxs-lookup"><span data-stu-id="0910a-131">Relationship</span></span>   | <span data-ttu-id="0910a-132">类型</span><span class="sxs-lookup"><span data-stu-id="0910a-132">Type</span></span>    | <span data-ttu-id="0910a-133">说明</span><span class="sxs-lookup"><span data-stu-id="0910a-133">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="0910a-134">teamsApp</span><span class="sxs-lookup"><span data-stu-id="0910a-134">teamsApp</span></span>|[<span data-ttu-id="0910a-135">teamsApp</span><span class="sxs-lookup"><span data-stu-id="0910a-135">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="0910a-136">已安装的应用程序。</span><span class="sxs-lookup"><span data-stu-id="0910a-136">The app that is installed.</span></span> |
|<span data-ttu-id="0910a-137">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="0910a-137">teamsAppDefinition</span></span>|[<span data-ttu-id="0910a-138">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="0910a-138">teamsAppDefinition</span></span>](teamsappdefinition.md)| <span data-ttu-id="0910a-139">此版本的应用程序的详细信息。</span><span class="sxs-lookup"><span data-stu-id="0910a-139">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0910a-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0910a-140">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string"
}
```

# <a name="see-also"></a><span data-ttu-id="0910a-141">另请参阅</span><span class="sxs-lookup"><span data-stu-id="0910a-141">See also</span></span>

- [<span data-ttu-id="0910a-142">teamsApp</span><span class="sxs-lookup"><span data-stu-id="0910a-142">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="0910a-143">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="0910a-143">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="0910a-144">teamsTab</span><span class="sxs-lookup"><span data-stu-id="0910a-144">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
