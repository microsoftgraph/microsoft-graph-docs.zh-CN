---
author: JeremyKelley
description: 使用 Shares API 访问共享的 driveItem 时，返回 sharedDriveItem 资源。
ms.date: 09/10/2017
title: SharedDriveItem
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: f310d35c6126573f022a13934faf911de1122606
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520729"
---
# <a name="shareddriveitem-resource-type"></a><span data-ttu-id="34cd3-103">SharedDriveItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="34cd3-103">SharedDriveItem resource type</span></span>

<span data-ttu-id="34cd3-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="34cd3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="34cd3-105">使用 [Shares](../api/shares-get.md) API 访问共享的 [driveItem](driveitem.md) 时，返回 **sharedDriveItem** 资源。</span><span class="sxs-lookup"><span data-stu-id="34cd3-105">The **sharedDriveItem** resource is returned when using the [Shares](../api/shares-get.md) API to access a shared [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="34cd3-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="34cd3-106">JSON representation</span></span>

<span data-ttu-id="34cd3-107">下面是 **sharedDriveItem** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="34cd3-107">Here is a JSON representation of the **sharedDriveItem** resource.</span></span>

<span data-ttu-id="34cd3-108">**sharedDriveItem** 资源由 [**baseItem**](baseitem.md) 派生并继承该资源的属性。</span><span class="sxs-lookup"><span data-stu-id="34cd3-108">The **sharedDriveItem** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="34cd3-109">属性</span><span class="sxs-lookup"><span data-stu-id="34cd3-109">Properties</span></span>

| <span data-ttu-id="34cd3-110">属性</span><span class="sxs-lookup"><span data-stu-id="34cd3-110">Property</span></span> | <span data-ttu-id="34cd3-111">类型</span><span class="sxs-lookup"><span data-stu-id="34cd3-111">Type</span></span>                          | <span data-ttu-id="34cd3-112">说明</span><span class="sxs-lookup"><span data-stu-id="34cd3-112">Description</span></span>                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="34cd3-113">id</span><span class="sxs-lookup"><span data-stu-id="34cd3-113">id</span></span>       | <span data-ttu-id="34cd3-114">String</span><span class="sxs-lookup"><span data-stu-id="34cd3-114">String</span></span>                        | <span data-ttu-id="34cd3-115">要访问的内容的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="34cd3-115">The unique identifier for the share being accessed.</span></span>              |
| <span data-ttu-id="34cd3-116">name</span><span class="sxs-lookup"><span data-stu-id="34cd3-116">name</span></span>     | <span data-ttu-id="34cd3-117">String</span><span class="sxs-lookup"><span data-stu-id="34cd3-117">String</span></span>                        | <span data-ttu-id="34cd3-118">共享项的显示名称。</span><span class="sxs-lookup"><span data-stu-id="34cd3-118">The display name of the shared item.</span></span>                             |
| <span data-ttu-id="34cd3-119">所有者</span><span class="sxs-lookup"><span data-stu-id="34cd3-119">owner</span></span>    | [<span data-ttu-id="34cd3-120">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="34cd3-120">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="34cd3-121">正在引用的共享项的所有者信息。</span><span class="sxs-lookup"><span data-stu-id="34cd3-121">Information about the owner of the shared item being referenced.</span></span> |

## <a name="relationships"></a><span data-ttu-id="34cd3-122">关系</span><span class="sxs-lookup"><span data-stu-id="34cd3-122">Relationships</span></span>

| <span data-ttu-id="34cd3-123">关系名称</span><span class="sxs-lookup"><span data-stu-id="34cd3-123">Relationship name</span></span> | <span data-ttu-id="34cd3-124">类型</span><span class="sxs-lookup"><span data-stu-id="34cd3-124">Type</span></span>                | <span data-ttu-id="34cd3-125">说明</span><span class="sxs-lookup"><span data-stu-id="34cd3-125">Description</span></span>
| ------------------|:--------------------|:-----------------------------------
| <span data-ttu-id="34cd3-126">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="34cd3-126">**driveItem**</span></span>     | <span data-ttu-id="34cd3-127">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="34cd3-127">[**driveItem**][driveItem]</span></span> | <span data-ttu-id="34cd3-128">用于访问基础 **driveItem**</span><span class="sxs-lookup"><span data-stu-id="34cd3-128">Used to access the underlying **driveItem**</span></span>
| <span data-ttu-id="34cd3-129">**list**</span><span class="sxs-lookup"><span data-stu-id="34cd3-129">**list**</span></span>          | <span data-ttu-id="34cd3-130">[**簿**][list]</span><span class="sxs-lookup"><span data-stu-id="34cd3-130">[**list**][list]</span></span>           | <span data-ttu-id="34cd3-131">用于访问基础 **list**</span><span class="sxs-lookup"><span data-stu-id="34cd3-131">Used to access the underlying **list**</span></span>
| <span data-ttu-id="34cd3-132">**listItem**</span><span class="sxs-lookup"><span data-stu-id="34cd3-132">**listItem**</span></span>      | <span data-ttu-id="34cd3-133">[**listItem**][listItem]</span><span class="sxs-lookup"><span data-stu-id="34cd3-133">[**listItem**][listItem]</span></span>   | <span data-ttu-id="34cd3-134">用于访问基础 **listItem**</span><span class="sxs-lookup"><span data-stu-id="34cd3-134">Used to access the underlying **listItem**</span></span>
| <span data-ttu-id="34cd3-135">**权限**</span><span class="sxs-lookup"><span data-stu-id="34cd3-135">**permission**</span></span>    | <span data-ttu-id="34cd3-136">[**拒绝**][permission]</span><span class="sxs-lookup"><span data-stu-id="34cd3-136">[**permission**][permission]</span></span> | <span data-ttu-id="34cd3-137">用于访问代表基础共享链接的**权限**</span><span class="sxs-lookup"><span data-stu-id="34cd3-137">Used to access the **permission** representing the underlying sharing link</span></span>
| <span data-ttu-id="34cd3-138">**site**</span><span class="sxs-lookup"><span data-stu-id="34cd3-138">**site**</span></span>          | <span data-ttu-id="34cd3-139">[**网站**][site]</span><span class="sxs-lookup"><span data-stu-id="34cd3-139">[**site**][site]</span></span>           | <span data-ttu-id="34cd3-140">用于访问基础 **site**</span><span class="sxs-lookup"><span data-stu-id="34cd3-140">Used to access the underlying **site**</span></span>

<span data-ttu-id="34cd3-141">另外，对于从个人 OneDrive 帐户共享的 **driveItems**，也可使用以下关系。</span><span class="sxs-lookup"><span data-stu-id="34cd3-141">Alternatively, for **driveItems** shared from personal OneDrive accounts, the following relationships may also be used.</span></span>

| <span data-ttu-id="34cd3-142">关系名称</span><span class="sxs-lookup"><span data-stu-id="34cd3-142">Relationship name</span></span> | <span data-ttu-id="34cd3-143">类型</span><span class="sxs-lookup"><span data-stu-id="34cd3-143">Type</span></span>                         | <span data-ttu-id="34cd3-144">说明</span><span class="sxs-lookup"><span data-stu-id="34cd3-144">Description</span></span>
| ------------------|:-----------------------------|:-----------------------------------
| <span data-ttu-id="34cd3-145">**items**</span><span class="sxs-lookup"><span data-stu-id="34cd3-145">**items**</span></span>         | <span data-ttu-id="34cd3-146">[**driveItem**][driveItem]集合</span><span class="sxs-lookup"><span data-stu-id="34cd3-146">[**driveItem**][driveItem] collection</span></span> | <span data-ttu-id="34cd3-147">共享根中包含的所有 driveItem。</span><span class="sxs-lookup"><span data-stu-id="34cd3-147">All driveItems contained in the sharing root.</span></span> <span data-ttu-id="34cd3-148">不能枚举该集合。</span><span class="sxs-lookup"><span data-stu-id="34cd3-148">This collection cannot be enumerated.</span></span>
| <span data-ttu-id="34cd3-149">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="34cd3-149">**driveItem**</span></span>     | <span data-ttu-id="34cd3-150">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="34cd3-150">[**driveItem**][driveItem]</span></span>            | <span data-ttu-id="34cd3-151">用于访问基础 **driveItem**</span><span class="sxs-lookup"><span data-stu-id="34cd3-151">Used to access the underlying **driveItem**</span></span>

[driveItem]: driveitem.md
[list]: list.md
[listItem]: listitem.md
[permission]: permission.md
[site]: site.md

## <a name="methods"></a><span data-ttu-id="34cd3-152">方法</span><span class="sxs-lookup"><span data-stu-id="34cd3-152">Methods</span></span>

| <span data-ttu-id="34cd3-153">方法</span><span class="sxs-lookup"><span data-stu-id="34cd3-153">Method</span></span>                                  | <span data-ttu-id="34cd3-154">REST 路径</span><span class="sxs-lookup"><span data-stu-id="34cd3-154">REST Path</span></span>                |
| :-------------------------------------- | :----------------------- |
| [<span data-ttu-id="34cd3-155">获取共享项目</span><span class="sxs-lookup"><span data-stu-id="34cd3-155">Get shared item</span></span>](../api/shares-get.md) | `GET /shares/{share-id}` |

## <a name="remarks"></a><span data-ttu-id="34cd3-156">注解</span><span class="sxs-lookup"><span data-stu-id="34cd3-156">Remarks</span></span>

<span data-ttu-id="34cd3-157">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="34cd3-157">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "Share resource returns information about a shared item or collection of items.",
  "keywords": "share,shared,sharing root,shared files, shared items",
  "section": "documentation",
  "tocPath": "Resources/Share",
  "suppressions": []
}
-->
