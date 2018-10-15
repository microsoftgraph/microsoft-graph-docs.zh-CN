---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharedDriveItem
ms.openlocfilehash: abcf686be46e15a523a1a88170981cb318e71b00
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2018
ms.locfileid: "23268198"
---
# <a name="shareddriveitem-resource-type"></a><span data-ttu-id="def41-102">SharedDriveItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="def41-102">SharedDriveItem resource type</span></span>

<span data-ttu-id="def41-103">使用 [Shares](../api/shares_get.md) API 访问共享的 [driveItem](driveitem.md) 时，返回 **sharedDriveItem** 资源。</span><span class="sxs-lookup"><span data-stu-id="def41-103">The **sharedDriveItem** resource is returned when using the [Shares](../api/shares_get.md) API to access a shared [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="def41-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="def41-104">JSON representation</span></span>

<span data-ttu-id="def41-105">下面是 **sharedDriveItem** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="def41-105">Here is a JSON representation of the **sharedDriveItem** resource.</span></span>

<span data-ttu-id="def41-106">**sharedDriveItem** 资源由 [**baseItem**](baseitem.md) 派生并继承该资源的属性。</span><span class="sxs-lookup"><span data-stu-id="def41-106">The **sharedDriveItem** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="def41-107">属性</span><span class="sxs-lookup"><span data-stu-id="def41-107">Properties</span></span>

| <span data-ttu-id="def41-108">属性</span><span class="sxs-lookup"><span data-stu-id="def41-108">Property</span></span> | <span data-ttu-id="def41-109">类型</span><span class="sxs-lookup"><span data-stu-id="def41-109">Type</span></span>                          | <span data-ttu-id="def41-110">说明</span><span class="sxs-lookup"><span data-stu-id="def41-110">Description</span></span>                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="def41-111">id</span><span class="sxs-lookup"><span data-stu-id="def41-111">id</span></span>       | <span data-ttu-id="def41-112">字符串</span><span class="sxs-lookup"><span data-stu-id="def41-112">String</span></span>                        | <span data-ttu-id="def41-113">要访问的内容的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="def41-113">The unique identifier for the share being accessed.</span></span>              |
| <span data-ttu-id="def41-114">name</span><span class="sxs-lookup"><span data-stu-id="def41-114">name</span></span>     | <span data-ttu-id="def41-115">字符串</span><span class="sxs-lookup"><span data-stu-id="def41-115">String</span></span>                        | <span data-ttu-id="def41-116">共享项的显示名称。</span><span class="sxs-lookup"><span data-stu-id="def41-116">The display name of the shared item.</span></span>                             |
| <span data-ttu-id="def41-117">所有者</span><span class="sxs-lookup"><span data-stu-id="def41-117">owner</span></span>    | [<span data-ttu-id="def41-118">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="def41-118">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="def41-119">正在引用的共享项的所有者信息。</span><span class="sxs-lookup"><span data-stu-id="def41-119">Information about the owner of the shared item being referenced.</span></span> |

## <a name="relationships"></a><span data-ttu-id="def41-120">关系</span><span class="sxs-lookup"><span data-stu-id="def41-120">Relationships</span></span>

| <span data-ttu-id="def41-121">关系名称</span><span class="sxs-lookup"><span data-stu-id="def41-121">Relationship name</span></span> | <span data-ttu-id="def41-122">类型</span><span class="sxs-lookup"><span data-stu-id="def41-122">Type</span></span>                | <span data-ttu-id="def41-123">说明</span><span class="sxs-lookup"><span data-stu-id="def41-123">Description</span></span>
| ------------------|:--------------------|:-----------------------------------
| <span data-ttu-id="def41-124">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="def41-124">**driveItem**</span></span>     | <span data-ttu-id="def41-125">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="def41-125">[**driveItem**][driveItem]</span></span>   | <span data-ttu-id="def41-126">用于访问基础 **driveItem**</span><span class="sxs-lookup"><span data-stu-id="def41-126">Used to access the underlying **driveItem**</span></span>
| <span data-ttu-id="def41-127">**list**</span><span class="sxs-lookup"><span data-stu-id="def41-127">**list**</span></span>          | <span data-ttu-id="def41-128">[**list**][list]</span><span class="sxs-lookup"><span data-stu-id="def41-128">[**list**][list]</span></span>        | <span data-ttu-id="def41-129">用于访问基础 **list**</span><span class="sxs-lookup"><span data-stu-id="def41-129">Used to access the underlying **list**</span></span>
| <span data-ttu-id="def41-130">**listItem**</span><span class="sxs-lookup"><span data-stu-id="def41-130">**listItem**</span></span>      | <span data-ttu-id="def41-131">[**listItem**][listItem]</span><span class="sxs-lookup"><span data-stu-id="def41-131">[**listItem**][listItem]</span></span>    | <span data-ttu-id="def41-132">用于访问基础 **listItem**</span><span class="sxs-lookup"><span data-stu-id="def41-132">Used to access the underlying **listItem**</span></span>
| <span data-ttu-id="def41-133">**site**</span><span class="sxs-lookup"><span data-stu-id="def41-133">**site**</span></span>          | <span data-ttu-id="def41-134">[**site**][site]</span><span class="sxs-lookup"><span data-stu-id="def41-134">[**site**][site]</span></span>        | <span data-ttu-id="def41-135">用于访问基础 **site**</span><span class="sxs-lookup"><span data-stu-id="def41-135">Used to access the underlying **site**</span></span>

<span data-ttu-id="def41-136">另外，对于从个人 OneDrive 帐户共享的 **driveItems**，也可使用以下关系。</span><span class="sxs-lookup"><span data-stu-id="def41-136">Alternatively, for **driveItems** shared from personal OneDrive accounts, the following relationships may also be used.</span></span>

| <span data-ttu-id="def41-137">关系名称</span><span class="sxs-lookup"><span data-stu-id="def41-137">Relationship name</span></span> | <span data-ttu-id="def41-138">类型</span><span class="sxs-lookup"><span data-stu-id="def41-138">Type</span></span>                         | <span data-ttu-id="def41-139">说明</span><span class="sxs-lookup"><span data-stu-id="def41-139">Description</span></span>
| ------------------|:-----------------------------|:-----------------------------------
| <span data-ttu-id="def41-140">**items**</span><span class="sxs-lookup"><span data-stu-id="def41-140">**items**</span></span>         | <span data-ttu-id="def41-141">[**driveItem**][driveItem] 集合</span><span class="sxs-lookup"><span data-stu-id="def41-141">[**driveItem**][driveItem] collection</span></span> | <span data-ttu-id="def41-142">共享根中包含的所有 driveItem。</span><span class="sxs-lookup"><span data-stu-id="def41-142">All driveItems contained in the sharing root.</span></span> <span data-ttu-id="def41-143">不能枚举此集合。</span><span class="sxs-lookup"><span data-stu-id="def41-143">This collection cannot be enumerated.</span></span>
| <span data-ttu-id="def41-144">**root**</span><span class="sxs-lookup"><span data-stu-id="def41-144">**root**</span></span>          | <span data-ttu-id="def41-145">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="def41-145">[**driveItem**][driveItem]</span></span>   | <span data-ttu-id="def41-146">用于访问基础 **driveItem**。</span><span class="sxs-lookup"><span data-stu-id="def41-146">Used to access the underlying **driveItem**</span></span> <span data-ttu-id="def41-147">弃用——以 `driveItem` 取代。</span><span class="sxs-lookup"><span data-stu-id="def41-147">Deprecated -- use `driveItem` instead.</span></span>

[driveItem]: driveItem.md
[list]: list.md
[listItem]: listItem.md
[site]: site.md

## <a name="methods"></a><span data-ttu-id="def41-148">方法</span><span class="sxs-lookup"><span data-stu-id="def41-148">Methods</span></span>

| <span data-ttu-id="def41-149">方法</span><span class="sxs-lookup"><span data-stu-id="def41-149">Method</span></span>                                  | <span data-ttu-id="def41-150">REST 路径</span><span class="sxs-lookup"><span data-stu-id="def41-150">REST Path</span></span>                |
| :-------------------------------------- | :----------------------- |
| [<span data-ttu-id="def41-151">获取共享项目</span><span class="sxs-lookup"><span data-stu-id="def41-151">Get shared item</span></span>](../api/shares_get.md) | `GET /shares/{share-id}` |

## <a name="remarks"></a><span data-ttu-id="def41-152">注解</span><span class="sxs-lookup"><span data-stu-id="def41-152">Remarks</span></span>

<span data-ttu-id="def41-153">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="def41-153">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Share resource returns information about a shared item or collection of items.",
  "keywords": "share,shared,sharing root,shared files, shared items",
  "section": "documentation",
  "tocPath": "Resources/Share"
} -->
