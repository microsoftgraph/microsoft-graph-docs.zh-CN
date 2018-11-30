---
title: teamsAppInstallation 资源类型
description: '团队中安装 teamsApp。 '
ms.openlocfilehash: 194a0525f46f57b9caca13f6308a31d56a84a299
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008843"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="92355-103">teamsAppInstallation 资源类型</span><span class="sxs-lookup"><span data-stu-id="92355-103">teamsAppInstallation resource type</span></span>



<span data-ttu-id="92355-104">安装在[工作组](team.md) [teamsApp](teamsapp.md) 。</span><span class="sxs-lookup"><span data-stu-id="92355-104">A [teamsApp](teamsapp.md) installed in a [team](team.md).</span></span> <span data-ttu-id="92355-105">应用程序一部分的任何 bot 将成为应用程序添加到任何工作组的一部分。</span><span class="sxs-lookup"><span data-stu-id="92355-105">Any bots that are part of the app will become part of any team the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="92355-106">方法</span><span class="sxs-lookup"><span data-stu-id="92355-106">Methods</span></span>

| <span data-ttu-id="92355-107">方法</span><span class="sxs-lookup"><span data-stu-id="92355-107">Method</span></span>       | <span data-ttu-id="92355-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="92355-108">Return Type</span></span>  |<span data-ttu-id="92355-109">说明</span><span class="sxs-lookup"><span data-stu-id="92355-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="92355-110">列表应用程序</span><span class="sxs-lookup"><span data-stu-id="92355-110">List apps</span></span>](../api/teamsappinstallation-list.md) | [<span data-ttu-id="92355-111">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="92355-111">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="92355-112">列出了安装团队中的应用程序。</span><span class="sxs-lookup"><span data-stu-id="92355-112">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="92355-113">添加应用程序</span><span class="sxs-lookup"><span data-stu-id="92355-113">Add app</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="92355-114">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="92355-114">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="92355-115">将 （安装） 添加到团队应用程序。</span><span class="sxs-lookup"><span data-stu-id="92355-115">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="92355-116">删除应用程序</span><span class="sxs-lookup"><span data-stu-id="92355-116">Remove app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="92355-117">无</span><span class="sxs-lookup"><span data-stu-id="92355-117">None</span></span> | <span data-ttu-id="92355-118">删除 （卸载） 从团队应用程序。</span><span class="sxs-lookup"><span data-stu-id="92355-118">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="92355-119">升级的应用程序</span><span class="sxs-lookup"><span data-stu-id="92355-119">Upgrade app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="92355-120">无</span><span class="sxs-lookup"><span data-stu-id="92355-120">None</span></span> | <span data-ttu-id="92355-121">升级到最新版本的应用程序。</span><span class="sxs-lookup"><span data-stu-id="92355-121">Upgrades to the latest version of the app.</span></span>|

## <a name="properties"></a><span data-ttu-id="92355-122">属性</span><span class="sxs-lookup"><span data-stu-id="92355-122">Properties</span></span>

| <span data-ttu-id="92355-123">属性</span><span class="sxs-lookup"><span data-stu-id="92355-123">Property</span></span>            | <span data-ttu-id="92355-124">类型</span><span class="sxs-lookup"><span data-stu-id="92355-124">Type</span></span>     | <span data-ttu-id="92355-125">说明</span><span class="sxs-lookup"><span data-stu-id="92355-125">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="92355-126">ID</span><span class="sxs-lookup"><span data-stu-id="92355-126">id</span></span>                  | <span data-ttu-id="92355-127">string</span><span class="sxs-lookup"><span data-stu-id="92355-127">string</span></span>   | <span data-ttu-id="92355-128">唯一的 id (不团队 appid)。</span><span class="sxs-lookup"><span data-stu-id="92355-128">A unique id (not the teams appid).</span></span> |

## <a name="relationships"></a><span data-ttu-id="92355-129">Relationships</span><span class="sxs-lookup"><span data-stu-id="92355-129">Relationships</span></span>

| <span data-ttu-id="92355-130">关系</span><span class="sxs-lookup"><span data-stu-id="92355-130">Relationship</span></span>   | <span data-ttu-id="92355-131">类型</span><span class="sxs-lookup"><span data-stu-id="92355-131">Type</span></span>    | <span data-ttu-id="92355-132">说明</span><span class="sxs-lookup"><span data-stu-id="92355-132">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="92355-133">teamsApp</span><span class="sxs-lookup"><span data-stu-id="92355-133">teamsApp</span></span>|[<span data-ttu-id="92355-134">teamsApp</span><span class="sxs-lookup"><span data-stu-id="92355-134">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="92355-135">安装应用程序。</span><span class="sxs-lookup"><span data-stu-id="92355-135">The app that is installed.</span></span> |
|<span data-ttu-id="92355-136">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="92355-136">teamsAppDefinition</span></span>|[<span data-ttu-id="92355-137">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="92355-137">teamsAppDefinition</span></span>](teamsapp.md)| <span data-ttu-id="92355-138">此版本的应用程序的详细信息。</span><span class="sxs-lookup"><span data-stu-id="92355-138">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="92355-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="92355-139">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="92355-140">另请参阅</span><span class="sxs-lookup"><span data-stu-id="92355-140">See also</span></span>

- [<span data-ttu-id="92355-141">teamsApp</span><span class="sxs-lookup"><span data-stu-id="92355-141">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="92355-142">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="92355-142">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="92355-143">teamsTab</span><span class="sxs-lookup"><span data-stu-id="92355-143">teamsTab</span></span>](../resources/teamstab.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

