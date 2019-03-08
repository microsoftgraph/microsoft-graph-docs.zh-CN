---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharedDriveItem
localization_priority: Normal
ms.openlocfilehash: b146fdf0f7ee2e2037fcb1d36511d0afa503005b
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480626"
---
# <a name="shareddriveitem-resource-type"></a><span data-ttu-id="7826b-102">SharedDriveItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="7826b-102">SharedDriveItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7826b-103">使用 [Shares](../api/shares-get.md) API 访问共享的 [driveItem](driveitem.md) 时，返回 **sharedDriveItem** 资源。</span><span class="sxs-lookup"><span data-stu-id="7826b-103">The **sharedDriveItem** resource is returned when using the [Shares](../api/shares-get.md) API to access a shared [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="7826b-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7826b-104">JSON representation</span></span>

<span data-ttu-id="7826b-105">下面是 **sharedDriveItem** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7826b-105">Here is a JSON representation of the **sharedDriveItem** resource.</span></span>

<span data-ttu-id="7826b-106">**sharedDriveItem** 资源由 [**baseItem**](baseitem.md) 派生并继承该资源的属性。</span><span class="sxs-lookup"><span data-stu-id="7826b-106">The **sharedDriveItem** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.baseItem",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.sharedDriveItem"
}-->

```json
{
  "id": "string",
  "name": "string",
  "owner": { "@odata.type": "microsoft.graph.identitySet" },

  "driveItem": { "@odata.type": "microsoft.graph.driveItem" },
  "items": [ { "@odata.type": "microsoft.graph.driveItem" }],
  "list": { "@odata.type": "microsoft.graph.list" },
  "listItem": { "@odata.type": "microsoft.graph.listItem" },
  "permission": { "@odata.type": "microsoft.graph.permission" },
  "root": { "@odata.type": "microsoft.graph.driveItem" },
  "site": { "@odata.type": "microsoft.graph.site" }
}
```

## <a name="properties"></a><span data-ttu-id="7826b-107">属性</span><span class="sxs-lookup"><span data-stu-id="7826b-107">Properties</span></span>

| <span data-ttu-id="7826b-108">属性</span><span class="sxs-lookup"><span data-stu-id="7826b-108">Property</span></span> | <span data-ttu-id="7826b-109">类型</span><span class="sxs-lookup"><span data-stu-id="7826b-109">Type</span></span>                          | <span data-ttu-id="7826b-110">说明</span><span class="sxs-lookup"><span data-stu-id="7826b-110">Description</span></span>                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="7826b-111">id</span><span class="sxs-lookup"><span data-stu-id="7826b-111">id</span></span>       | <span data-ttu-id="7826b-112">String</span><span class="sxs-lookup"><span data-stu-id="7826b-112">String</span></span>                        | <span data-ttu-id="7826b-113">要访问的内容的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="7826b-113">The unique identifier for the share being accessed.</span></span>              |
| <span data-ttu-id="7826b-114">名称</span><span class="sxs-lookup"><span data-stu-id="7826b-114">name</span></span>     | <span data-ttu-id="7826b-115">String</span><span class="sxs-lookup"><span data-stu-id="7826b-115">String</span></span>                        | <span data-ttu-id="7826b-116">共享项的显示名称。</span><span class="sxs-lookup"><span data-stu-id="7826b-116">The display name of the shared item.</span></span>                             |
| <span data-ttu-id="7826b-117">所有者</span><span class="sxs-lookup"><span data-stu-id="7826b-117">owner</span></span>    | [<span data-ttu-id="7826b-118">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="7826b-118">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="7826b-119">正在引用的共享项的所有者信息。</span><span class="sxs-lookup"><span data-stu-id="7826b-119">Information about the owner of the shared item being referenced.</span></span> |

## <a name="relationships"></a><span data-ttu-id="7826b-120">关系</span><span class="sxs-lookup"><span data-stu-id="7826b-120">Relationships</span></span>

| <span data-ttu-id="7826b-121">关系名称</span><span class="sxs-lookup"><span data-stu-id="7826b-121">Relationship name</span></span> | <span data-ttu-id="7826b-122">类型</span><span class="sxs-lookup"><span data-stu-id="7826b-122">Type</span></span>                | <span data-ttu-id="7826b-123">说明</span><span class="sxs-lookup"><span data-stu-id="7826b-123">Description</span></span>
| ------------------|:--------------------|:-----------------------------------
| <span data-ttu-id="7826b-124">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="7826b-124">**driveItem**</span></span>     | <span data-ttu-id="7826b-125">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="7826b-125">[**driveItem**][driveItem]</span></span> | <span data-ttu-id="7826b-126">用于访问基础 **driveItem**</span><span class="sxs-lookup"><span data-stu-id="7826b-126">Used to access the underlying **driveItem**</span></span>
| <span data-ttu-id="7826b-127">**list**</span><span class="sxs-lookup"><span data-stu-id="7826b-127">**list**</span></span>          | <span data-ttu-id="7826b-128">[**list**][list]</span><span class="sxs-lookup"><span data-stu-id="7826b-128">[**list**][list]</span></span>           | <span data-ttu-id="7826b-129">用于访问基础 **list**</span><span class="sxs-lookup"><span data-stu-id="7826b-129">Used to access the underlying **list**</span></span>
| <span data-ttu-id="7826b-130">**listItem**</span><span class="sxs-lookup"><span data-stu-id="7826b-130">**listItem**</span></span>      | <span data-ttu-id="7826b-131">[**listItem**][listItem]</span><span class="sxs-lookup"><span data-stu-id="7826b-131">[**listItem**][listItem]</span></span>   | <span data-ttu-id="7826b-132">用于访问基础 **listItem**</span><span class="sxs-lookup"><span data-stu-id="7826b-132">Used to access the underlying **listItem**</span></span>
| <span data-ttu-id="7826b-133">**permission**</span><span class="sxs-lookup"><span data-stu-id="7826b-133">**permission**</span></span>    | <span data-ttu-id="7826b-134">[**拒绝**][permission]</span><span class="sxs-lookup"><span data-stu-id="7826b-134">[**permission**][permission]</span></span> | <span data-ttu-id="7826b-135">用于访问代表基础共享链接的**权限**</span><span class="sxs-lookup"><span data-stu-id="7826b-135">Used to access the **permission** representing the underlying sharing link</span></span>
| <span data-ttu-id="7826b-136">**site**</span><span class="sxs-lookup"><span data-stu-id="7826b-136">**site**</span></span>          | <span data-ttu-id="7826b-137">[**site**][site]</span><span class="sxs-lookup"><span data-stu-id="7826b-137">[**site**][site]</span></span>           | <span data-ttu-id="7826b-138">用于访问基础 **site**</span><span class="sxs-lookup"><span data-stu-id="7826b-138">Used to access the underlying **site**</span></span>

<span data-ttu-id="7826b-139">另外，对于从个人 OneDrive 帐户共享的 **driveItems**，也可使用以下关系。</span><span class="sxs-lookup"><span data-stu-id="7826b-139">Alternatively, for **driveItems** shared from personal OneDrive accounts, the following relationships may also be used.</span></span>

| <span data-ttu-id="7826b-140">关系名称</span><span class="sxs-lookup"><span data-stu-id="7826b-140">Relationship name</span></span> | <span data-ttu-id="7826b-141">类型</span><span class="sxs-lookup"><span data-stu-id="7826b-141">Type</span></span>                         | <span data-ttu-id="7826b-142">说明</span><span class="sxs-lookup"><span data-stu-id="7826b-142">Description</span></span>
| ------------------|:-----------------------------|:-----------------------------------
| <span data-ttu-id="7826b-143">**项目**</span><span class="sxs-lookup"><span data-stu-id="7826b-143">**items**</span></span>         | <span data-ttu-id="7826b-144">[**driveItem**][driveItem] 集合</span><span class="sxs-lookup"><span data-stu-id="7826b-144">[**driveItem**][driveItem] collection</span></span> | <span data-ttu-id="7826b-145">共享根中包含的所有 driveItem。</span><span class="sxs-lookup"><span data-stu-id="7826b-145">All driveItems contained in the sharing root.</span></span> <span data-ttu-id="7826b-146">不能枚举该集合。</span><span class="sxs-lookup"><span data-stu-id="7826b-146">This collection cannot be enumerated.</span></span>
| <span data-ttu-id="7826b-147">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="7826b-147">**driveItem**</span></span>     | <span data-ttu-id="7826b-148">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="7826b-148">[**driveItem**][driveItem]</span></span>            | <span data-ttu-id="7826b-149">用于访问基础 **driveItem**</span><span class="sxs-lookup"><span data-stu-id="7826b-149">Used to access the underlying **driveItem**</span></span>

[driveItem]: driveitem.md
[list]: list.md
[listItem]: listitem.md
[permission]: permission.md
[site]: site.md

## <a name="methods"></a><span data-ttu-id="7826b-150">方法</span><span class="sxs-lookup"><span data-stu-id="7826b-150">Methods</span></span>

| <span data-ttu-id="7826b-151">方法</span><span class="sxs-lookup"><span data-stu-id="7826b-151">Method</span></span>                                  | <span data-ttu-id="7826b-152">REST 路径</span><span class="sxs-lookup"><span data-stu-id="7826b-152">REST Path</span></span>                |
| :-------------------------------------- | :----------------------- |
| [<span data-ttu-id="7826b-153">获取共享项目</span><span class="sxs-lookup"><span data-stu-id="7826b-153">Get shared item</span></span>](../api/shares-get.md) | `GET /shares/{share-id}` |

## <a name="remarks"></a><span data-ttu-id="7826b-154">注解</span><span class="sxs-lookup"><span data-stu-id="7826b-154">Remarks</span></span>

<span data-ttu-id="7826b-155">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="7826b-155">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "Share resource returns information about a shared item or collection of items.",
  "keywords": "share,shared,sharing root,shared files, shared items",
  "section": "documentation",
  "tocPath": "Resources/Share",
  "suppressions": [
    "Error: /api-reference/beta/resources/shareddriveitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
