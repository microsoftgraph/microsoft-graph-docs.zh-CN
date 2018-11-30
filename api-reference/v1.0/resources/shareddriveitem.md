---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharedDriveItem
ms.openlocfilehash: 3b4497c1a15704388dbb4bb4ba181d3985d65a69
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="shareddriveitem-resource-type"></a><span data-ttu-id="d3c36-102">SharedDriveItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="d3c36-102">SharedDriveItem resource type</span></span>

<span data-ttu-id="d3c36-103">使用 [Shares](../api/shares_get.md) API 访问共享的 [driveItem](driveitem.md) 时，返回 **sharedDriveItem** 资源。</span><span class="sxs-lookup"><span data-stu-id="d3c36-103">The **sharedDriveItem** resource is returned when using the [Shares](../api/shares_get.md) API to access a shared [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="d3c36-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d3c36-104">JSON representation</span></span>

<span data-ttu-id="d3c36-105">下面是 **sharedDriveItem** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d3c36-105">Here is a JSON representation of the **sharedDriveItem** resource.</span></span>

<span data-ttu-id="d3c36-106">**sharedDriveItem** 资源由 [**baseItem**](baseitem.md) 派生并继承该资源的属性。</span><span class="sxs-lookup"><span data-stu-id="d3c36-106">The **sharedDriveItem** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.sharedDriveItem"
}-->

```json
{
  "id": "string",
  "name": "string",
  "owner": { "@odata.type": "microsoft.graph.identitySet" },

  "driveItem": [ { "@odata.type": "microsoft.graph.driveItem" }],
  "items": [ { "@odata.type": "microsoft.graph.driveItem" }],
  "list": { "@odata.type": "microsoft.graph.list" },
  "listItem": { "@odata.type": "microsoft.graph.listItem" },
  "root": { "@odata.type": "microsoft.graph.driveItem" },
  "site": { "@odata.type": "microsoft.graph.site" }
}
```

## <a name="properties"></a><span data-ttu-id="d3c36-107">属性</span><span class="sxs-lookup"><span data-stu-id="d3c36-107">Properties</span></span>

| <span data-ttu-id="d3c36-108">属性</span><span class="sxs-lookup"><span data-stu-id="d3c36-108">Property</span></span> | <span data-ttu-id="d3c36-109">类型</span><span class="sxs-lookup"><span data-stu-id="d3c36-109">Type</span></span>                          | <span data-ttu-id="d3c36-110">说明</span><span class="sxs-lookup"><span data-stu-id="d3c36-110">Description</span></span>                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="d3c36-111">id</span><span class="sxs-lookup"><span data-stu-id="d3c36-111">id</span></span>       | <span data-ttu-id="d3c36-112">String</span><span class="sxs-lookup"><span data-stu-id="d3c36-112">String</span></span>                        | <span data-ttu-id="d3c36-113">要访问的内容的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d3c36-113">The unique identifier for the share being accessed.</span></span>              |
| <span data-ttu-id="d3c36-114">名称</span><span class="sxs-lookup"><span data-stu-id="d3c36-114">name</span></span>     | <span data-ttu-id="d3c36-115">String</span><span class="sxs-lookup"><span data-stu-id="d3c36-115">String</span></span>                        | <span data-ttu-id="d3c36-116">共享项的显示名称。</span><span class="sxs-lookup"><span data-stu-id="d3c36-116">The display name of the shared item.</span></span>                             |
| <span data-ttu-id="d3c36-117">所有者</span><span class="sxs-lookup"><span data-stu-id="d3c36-117">owner</span></span>    | [<span data-ttu-id="d3c36-118">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="d3c36-118">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="d3c36-119">正在引用的共享项的所有者信息。</span><span class="sxs-lookup"><span data-stu-id="d3c36-119">Information about the owner of the shared item being referenced.</span></span> |

## <a name="relationships"></a><span data-ttu-id="d3c36-120">关系</span><span class="sxs-lookup"><span data-stu-id="d3c36-120">Relationships</span></span>

| <span data-ttu-id="d3c36-121">关系名称</span><span class="sxs-lookup"><span data-stu-id="d3c36-121">Relationship name</span></span> | <span data-ttu-id="d3c36-122">类型</span><span class="sxs-lookup"><span data-stu-id="d3c36-122">Type</span></span>                | <span data-ttu-id="d3c36-123">说明</span><span class="sxs-lookup"><span data-stu-id="d3c36-123">Description</span></span>
| ------------------|:--------------------|:-----------------------------------
| <span data-ttu-id="d3c36-124">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="d3c36-124">**DriveItem**</span></span>     | <span data-ttu-id="d3c36-125">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="d3c36-125">DriveItem</span></span>   | <span data-ttu-id="d3c36-126">用于访问基础 **driveItem**</span><span class="sxs-lookup"><span data-stu-id="d3c36-126">Used to access the underlying **driveItem**</span></span>
| <span data-ttu-id="d3c36-127">**list**</span><span class="sxs-lookup"><span data-stu-id="d3c36-127">**list**</span></span>          | <span data-ttu-id="d3c36-128">[**list**][list]</span><span class="sxs-lookup"><span data-stu-id="d3c36-128">List</span></span>        | <span data-ttu-id="d3c36-129">用于访问基础 **list**</span><span class="sxs-lookup"><span data-stu-id="d3c36-129">Used to access the underlying **list**</span></span>
| <span data-ttu-id="d3c36-130">**listItem**</span><span class="sxs-lookup"><span data-stu-id="d3c36-130">**listItem**</span></span>      | <span data-ttu-id="d3c36-131">[**listItem**][listItem]</span><span class="sxs-lookup"><span data-stu-id="d3c36-131">**ListItem**</span></span>    | <span data-ttu-id="d3c36-132">用于访问基础 **listItem**</span><span class="sxs-lookup"><span data-stu-id="d3c36-132">Used to access the underlying **listItem**</span></span>
| <span data-ttu-id="d3c36-133">**site**</span><span class="sxs-lookup"><span data-stu-id="d3c36-133">**site**</span></span>          | <span data-ttu-id="d3c36-134">[**site**][site]</span><span class="sxs-lookup"><span data-stu-id="d3c36-134">**site**</span></span>        | <span data-ttu-id="d3c36-135">用于访问基础 **site**</span><span class="sxs-lookup"><span data-stu-id="d3c36-135">Used to access the underlying **site**</span></span>


<span data-ttu-id="d3c36-136">另外，对于从个人 OneDrive 帐户共享的 **driveItems**，也可使用以下关系。</span><span class="sxs-lookup"><span data-stu-id="d3c36-136">Alternatively, for **driveItems** shared from personal OneDrive accounts, the following relationships may also be used.</span></span>

| <span data-ttu-id="d3c36-137">关系名称</span><span class="sxs-lookup"><span data-stu-id="d3c36-137">Relationship name</span></span> | <span data-ttu-id="d3c36-138">类型</span><span class="sxs-lookup"><span data-stu-id="d3c36-138">Type</span></span>                         | <span data-ttu-id="d3c36-139">说明</span><span class="sxs-lookup"><span data-stu-id="d3c36-139">Description</span></span>
| ------------------|:-----------------------------|:-----------------------------------
| <span data-ttu-id="d3c36-140">**items**</span><span class="sxs-lookup"><span data-stu-id="d3c36-140">**items**</span></span>         | <span data-ttu-id="d3c36-141">[**driveItem**][driveItem] 集合</span><span class="sxs-lookup"><span data-stu-id="d3c36-141">**driveItem** collection</span></span> | <span data-ttu-id="d3c36-142">共享根中包含的所有 driveItem。</span><span class="sxs-lookup"><span data-stu-id="d3c36-142">All items contained in the sharing root.</span></span> <span data-ttu-id="d3c36-143">不能枚举该集合。</span><span class="sxs-lookup"><span data-stu-id="d3c36-143">This collection cannot be enumerated.</span></span>
| <span data-ttu-id="d3c36-144">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="d3c36-144">**DriveItem**</span></span>     | <span data-ttu-id="d3c36-145">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="d3c36-145">DriveItem</span></span>            | <span data-ttu-id="d3c36-146">用于访问基础 **driveItem**</span><span class="sxs-lookup"><span data-stu-id="d3c36-146">Used to access the underlying **driveItem**</span></span>

[driveItem]: driveItem.md
[list]: list.md
[listItem]: listItem.md
[site]: site.md

## <a name="methods"></a><span data-ttu-id="d3c36-147">方法</span><span class="sxs-lookup"><span data-stu-id="d3c36-147">Methods</span></span>

| <span data-ttu-id="d3c36-148">方法</span><span class="sxs-lookup"><span data-stu-id="d3c36-148">Method</span></span>                                  | <span data-ttu-id="d3c36-149">REST 路径</span><span class="sxs-lookup"><span data-stu-id="d3c36-149">REST Path</span></span>                |
| :-------------------------------------- | :----------------------- |
| [<span data-ttu-id="d3c36-150">获取共享项目</span><span class="sxs-lookup"><span data-stu-id="d3c36-150">Get shared item</span></span>](../api/shares_get.md) | `GET /shares/{share-id}` |

## <a name="remarks"></a><span data-ttu-id="d3c36-151">注解</span><span class="sxs-lookup"><span data-stu-id="d3c36-151">Remarks</span></span>

<span data-ttu-id="d3c36-152">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="d3c36-152">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Share resource returns information about a shared item or collection of items.",
  "keywords": "share,shared,sharing root,shared files, shared items",
  "section": "documentation",
  "tocPath": "Resources/Share"
} -->
