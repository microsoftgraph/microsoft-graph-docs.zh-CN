---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharedDriveItem
localization_priority: Normal
description: 使用 Shares API 访问共享的 driveItem 时，返回 sharedDriveItem 资源。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 1f6684e9c266a800f5a76a7085a8af22ea9518e8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034333"
---
# <a name="shareddriveitem-resource-type"></a><span data-ttu-id="1b3ff-103">SharedDriveItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="1b3ff-103">SharedDriveItem resource type</span></span>

<span data-ttu-id="1b3ff-104">使用 [Shares](../api/shares-get.md) API 访问共享的 [driveItem](driveitem.md) 时，返回 **sharedDriveItem** 资源。</span><span class="sxs-lookup"><span data-stu-id="1b3ff-104">The **sharedDriveItem** resource is returned when using the [Shares](../api/shares-get.md) API to access a shared [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="1b3ff-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1b3ff-105">JSON representation</span></span>

<span data-ttu-id="1b3ff-106">下面是 **sharedDriveItem** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1b3ff-106">Here is a JSON representation of the **sharedDriveItem** resource.</span></span>

<span data-ttu-id="1b3ff-107">**sharedDriveItem** 资源由 [**baseItem**](baseitem.md) 派生并继承该资源的属性。</span><span class="sxs-lookup"><span data-stu-id="1b3ff-107">The **sharedDriveItem** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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
  "root": { "@odata.type": "microsoft.graph.driveItem" },
  "site": { "@odata.type": "microsoft.graph.site" }
}
```

## <a name="properties"></a><span data-ttu-id="1b3ff-108">属性</span><span class="sxs-lookup"><span data-stu-id="1b3ff-108">Properties</span></span>

| <span data-ttu-id="1b3ff-109">属性</span><span class="sxs-lookup"><span data-stu-id="1b3ff-109">Property</span></span> | <span data-ttu-id="1b3ff-110">类型</span><span class="sxs-lookup"><span data-stu-id="1b3ff-110">Type</span></span>                          | <span data-ttu-id="1b3ff-111">说明</span><span class="sxs-lookup"><span data-stu-id="1b3ff-111">Description</span></span>                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="1b3ff-112">id</span><span class="sxs-lookup"><span data-stu-id="1b3ff-112">id</span></span>       | <span data-ttu-id="1b3ff-113">String</span><span class="sxs-lookup"><span data-stu-id="1b3ff-113">String</span></span>                        | <span data-ttu-id="1b3ff-114">要访问的内容的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="1b3ff-114">The unique identifier for the share being accessed.</span></span>              |
| <span data-ttu-id="1b3ff-115">name</span><span class="sxs-lookup"><span data-stu-id="1b3ff-115">name</span></span>     | <span data-ttu-id="1b3ff-116">String</span><span class="sxs-lookup"><span data-stu-id="1b3ff-116">String</span></span>                        | <span data-ttu-id="1b3ff-117">共享项的显示名称。</span><span class="sxs-lookup"><span data-stu-id="1b3ff-117">The display name of the shared item.</span></span>                             |
| <span data-ttu-id="1b3ff-118">所有者</span><span class="sxs-lookup"><span data-stu-id="1b3ff-118">owner</span></span>    | [<span data-ttu-id="1b3ff-119">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="1b3ff-119">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="1b3ff-120">正在引用的共享项的所有者信息。</span><span class="sxs-lookup"><span data-stu-id="1b3ff-120">Information about the owner of the shared item being referenced.</span></span> |

## <a name="relationships"></a><span data-ttu-id="1b3ff-121">关系</span><span class="sxs-lookup"><span data-stu-id="1b3ff-121">Relationships</span></span>

| <span data-ttu-id="1b3ff-122">关系名称</span><span class="sxs-lookup"><span data-stu-id="1b3ff-122">Relationship name</span></span> | <span data-ttu-id="1b3ff-123">类型</span><span class="sxs-lookup"><span data-stu-id="1b3ff-123">Type</span></span>                | <span data-ttu-id="1b3ff-124">说明</span><span class="sxs-lookup"><span data-stu-id="1b3ff-124">Description</span></span>
| ------------------|:--------------------|:-----------------------------------
| <span data-ttu-id="1b3ff-125">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="1b3ff-125">**driveItem**</span></span>     | <span data-ttu-id="1b3ff-126">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="1b3ff-126">[**driveItem**][driveItem]</span></span>   | <span data-ttu-id="1b3ff-127">用于访问基础 **driveItem**</span><span class="sxs-lookup"><span data-stu-id="1b3ff-127">Used to access the underlying **driveItem**</span></span>
| <span data-ttu-id="1b3ff-128">**list**</span><span class="sxs-lookup"><span data-stu-id="1b3ff-128">**list**</span></span>          | <span data-ttu-id="1b3ff-129">[**簿**][list]</span><span class="sxs-lookup"><span data-stu-id="1b3ff-129">[**list**][list]</span></span>        | <span data-ttu-id="1b3ff-130">用于访问基础 **list**</span><span class="sxs-lookup"><span data-stu-id="1b3ff-130">Used to access the underlying **list**</span></span>
| <span data-ttu-id="1b3ff-131">**listItem**</span><span class="sxs-lookup"><span data-stu-id="1b3ff-131">**listItem**</span></span>      | <span data-ttu-id="1b3ff-132">[**listItem**][listItem]</span><span class="sxs-lookup"><span data-stu-id="1b3ff-132">[**listItem**][listItem]</span></span>    | <span data-ttu-id="1b3ff-133">用于访问基础 **listItem**</span><span class="sxs-lookup"><span data-stu-id="1b3ff-133">Used to access the underlying **listItem**</span></span>
| <span data-ttu-id="1b3ff-134">**site**</span><span class="sxs-lookup"><span data-stu-id="1b3ff-134">**site**</span></span>          | <span data-ttu-id="1b3ff-135">[**网站**][site]</span><span class="sxs-lookup"><span data-stu-id="1b3ff-135">[**site**][site]</span></span>        | <span data-ttu-id="1b3ff-136">用于访问基础 **site**</span><span class="sxs-lookup"><span data-stu-id="1b3ff-136">Used to access the underlying **site**</span></span>

<span data-ttu-id="1b3ff-137">另外，对于从个人 OneDrive 帐户共享的 **driveItems**，也可使用以下关系。</span><span class="sxs-lookup"><span data-stu-id="1b3ff-137">Alternatively, for **driveItems** shared from personal OneDrive accounts, the following relationships may also be used.</span></span>

| <span data-ttu-id="1b3ff-138">关系名称</span><span class="sxs-lookup"><span data-stu-id="1b3ff-138">Relationship name</span></span> | <span data-ttu-id="1b3ff-139">类型</span><span class="sxs-lookup"><span data-stu-id="1b3ff-139">Type</span></span>                         | <span data-ttu-id="1b3ff-140">说明</span><span class="sxs-lookup"><span data-stu-id="1b3ff-140">Description</span></span>
| ------------------|:-----------------------------|:-----------------------------------
| <span data-ttu-id="1b3ff-141">**items**</span><span class="sxs-lookup"><span data-stu-id="1b3ff-141">**items**</span></span>         | <span data-ttu-id="1b3ff-142">[**driveItem**][driveItem]集合</span><span class="sxs-lookup"><span data-stu-id="1b3ff-142">[**driveItem**][driveItem] collection</span></span> | <span data-ttu-id="1b3ff-143">共享根中包含的所有 driveItem。</span><span class="sxs-lookup"><span data-stu-id="1b3ff-143">All driveItems contained in the sharing root.</span></span> <span data-ttu-id="1b3ff-144">不能枚举此集合。</span><span class="sxs-lookup"><span data-stu-id="1b3ff-144">This collection cannot be enumerated.</span></span>
| <span data-ttu-id="1b3ff-145">**root**</span><span class="sxs-lookup"><span data-stu-id="1b3ff-145">**root**</span></span>          | <span data-ttu-id="1b3ff-146">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="1b3ff-146">[**driveItem**][driveItem]</span></span>   | <span data-ttu-id="1b3ff-147">用于访问基础**driveItem**。</span><span class="sxs-lookup"><span data-stu-id="1b3ff-147">Used to access the underlying **driveItem**.</span></span> <span data-ttu-id="1b3ff-148">已弃用-- `driveItem`改用。</span><span class="sxs-lookup"><span data-stu-id="1b3ff-148">Deprecated -- use `driveItem` instead.</span></span>

[driveItem]: driveitem.md
[list]: list.md
[listItem]: listitem.md
[site]: site.md

## <a name="methods"></a><span data-ttu-id="1b3ff-149">方法</span><span class="sxs-lookup"><span data-stu-id="1b3ff-149">Methods</span></span>

| <span data-ttu-id="1b3ff-150">方法</span><span class="sxs-lookup"><span data-stu-id="1b3ff-150">Method</span></span>                                  | <span data-ttu-id="1b3ff-151">REST 路径</span><span class="sxs-lookup"><span data-stu-id="1b3ff-151">REST Path</span></span>                |
| :-------------------------------------- | :----------------------- |
| [<span data-ttu-id="1b3ff-152">获取共享项目</span><span class="sxs-lookup"><span data-stu-id="1b3ff-152">Get shared item</span></span>](../api/shares-get.md) | `GET /shares/{share-id}` |

## <a name="remarks"></a><span data-ttu-id="1b3ff-153">注解</span><span class="sxs-lookup"><span data-stu-id="1b3ff-153">Remarks</span></span>

<span data-ttu-id="1b3ff-154">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="1b3ff-154">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Share resource returns information about a shared item or collection of items.",
  "keywords": "share,shared,sharing root,shared files, shared items",
  "section": "documentation",
  "tocPath": "Resources/Share"
} -->
