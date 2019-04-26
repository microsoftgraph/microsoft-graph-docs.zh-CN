---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharedDriveItem
localization_priority: Normal
ms.openlocfilehash: 0d0c5a34d12fe467196c0616befc7376835b632c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549634"
---
# <a name="shareddriveitem-resource-type"></a><span data-ttu-id="4105f-102">SharedDriveItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="4105f-102">SharedDriveItem resource type</span></span>

<span data-ttu-id="4105f-103">使用 [Shares](../api/shares-get.md) API 访问共享的 [driveItem](driveitem.md) 时，返回 **sharedDriveItem** 资源。</span><span class="sxs-lookup"><span data-stu-id="4105f-103">The **sharedDriveItem** resource is returned when using the [Shares](../api/shares-get.md) API to access a shared [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="4105f-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4105f-104">JSON representation</span></span>

<span data-ttu-id="4105f-105">下面是 **sharedDriveItem** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4105f-105">Here is a JSON representation of the **sharedDriveItem** resource.</span></span>

<span data-ttu-id="4105f-106">**sharedDriveItem** 资源由 [**baseItem**](baseitem.md) 派生并继承该资源的属性。</span><span class="sxs-lookup"><span data-stu-id="4105f-106">The **sharedDriveItem** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="4105f-107">属性</span><span class="sxs-lookup"><span data-stu-id="4105f-107">Properties</span></span>

| <span data-ttu-id="4105f-108">属性</span><span class="sxs-lookup"><span data-stu-id="4105f-108">Property</span></span> | <span data-ttu-id="4105f-109">类型</span><span class="sxs-lookup"><span data-stu-id="4105f-109">Type</span></span>                          | <span data-ttu-id="4105f-110">说明</span><span class="sxs-lookup"><span data-stu-id="4105f-110">Description</span></span>                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="4105f-111">id</span><span class="sxs-lookup"><span data-stu-id="4105f-111">id</span></span>       | <span data-ttu-id="4105f-112">字符串</span><span class="sxs-lookup"><span data-stu-id="4105f-112">String</span></span>                        | <span data-ttu-id="4105f-113">要访问的内容的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="4105f-113">The unique identifier for the share being accessed.</span></span>              |
| <span data-ttu-id="4105f-114">name</span><span class="sxs-lookup"><span data-stu-id="4105f-114">name</span></span>     | <span data-ttu-id="4105f-115">String</span><span class="sxs-lookup"><span data-stu-id="4105f-115">String</span></span>                        | <span data-ttu-id="4105f-116">共享项的显示名称。</span><span class="sxs-lookup"><span data-stu-id="4105f-116">The display name of the shared item.</span></span>                             |
| <span data-ttu-id="4105f-117">所有者</span><span class="sxs-lookup"><span data-stu-id="4105f-117">owner</span></span>    | [<span data-ttu-id="4105f-118">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="4105f-118">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="4105f-119">正在引用的共享项的所有者信息。</span><span class="sxs-lookup"><span data-stu-id="4105f-119">Information about the owner of the shared item being referenced.</span></span> |

## <a name="relationships"></a><span data-ttu-id="4105f-120">关系</span><span class="sxs-lookup"><span data-stu-id="4105f-120">Relationships</span></span>

| <span data-ttu-id="4105f-121">关系名称</span><span class="sxs-lookup"><span data-stu-id="4105f-121">Relationship name</span></span> | <span data-ttu-id="4105f-122">类型</span><span class="sxs-lookup"><span data-stu-id="4105f-122">Type</span></span>                | <span data-ttu-id="4105f-123">说明</span><span class="sxs-lookup"><span data-stu-id="4105f-123">Description</span></span>
| ------------------|:--------------------|:-----------------------------------
| <span data-ttu-id="4105f-124">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="4105f-124">**driveItem**</span></span>     | <span data-ttu-id="4105f-125">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="4105f-125">[**driveItem**][driveItem]</span></span>   | <span data-ttu-id="4105f-126">用于访问基础 **driveItem**</span><span class="sxs-lookup"><span data-stu-id="4105f-126">Used to access the underlying **driveItem**</span></span>
| <span data-ttu-id="4105f-127">**list**</span><span class="sxs-lookup"><span data-stu-id="4105f-127">**list**</span></span>          | <span data-ttu-id="4105f-128">[**list**][list]</span><span class="sxs-lookup"><span data-stu-id="4105f-128">[**list**][list]</span></span>        | <span data-ttu-id="4105f-129">用于访问基础 **list**</span><span class="sxs-lookup"><span data-stu-id="4105f-129">Used to access the underlying **list**</span></span>
| <span data-ttu-id="4105f-130">**listItem**</span><span class="sxs-lookup"><span data-stu-id="4105f-130">**listItem**</span></span>      | <span data-ttu-id="4105f-131">[**listItem**][listItem]</span><span class="sxs-lookup"><span data-stu-id="4105f-131">[**listItem**][listItem]</span></span>    | <span data-ttu-id="4105f-132">用于访问基础 **listItem**</span><span class="sxs-lookup"><span data-stu-id="4105f-132">Used to access the underlying **listItem**</span></span>
| <span data-ttu-id="4105f-133">**site**</span><span class="sxs-lookup"><span data-stu-id="4105f-133">**site**</span></span>          | <span data-ttu-id="4105f-134">[**site**][site]</span><span class="sxs-lookup"><span data-stu-id="4105f-134">[**site**][site]</span></span>        | <span data-ttu-id="4105f-135">用于访问基础 **site**</span><span class="sxs-lookup"><span data-stu-id="4105f-135">Used to access the underlying **site**</span></span>

<span data-ttu-id="4105f-136">另外，对于从个人 OneDrive 帐户共享的 **driveItems**，也可使用以下关系。</span><span class="sxs-lookup"><span data-stu-id="4105f-136">Alternatively, for **driveItems** shared from personal OneDrive accounts, the following relationships may also be used.</span></span>

| <span data-ttu-id="4105f-137">关系名称</span><span class="sxs-lookup"><span data-stu-id="4105f-137">Relationship name</span></span> | <span data-ttu-id="4105f-138">类型</span><span class="sxs-lookup"><span data-stu-id="4105f-138">Type</span></span>                         | <span data-ttu-id="4105f-139">说明</span><span class="sxs-lookup"><span data-stu-id="4105f-139">Description</span></span>
| ------------------|:-----------------------------|:-----------------------------------
| <span data-ttu-id="4105f-140">**项目**</span><span class="sxs-lookup"><span data-stu-id="4105f-140">**items**</span></span>         | <span data-ttu-id="4105f-141">[**driveItem**][driveItem] 集合</span><span class="sxs-lookup"><span data-stu-id="4105f-141">[**driveItem**][driveItem] collection</span></span> | <span data-ttu-id="4105f-142">共享根中包含的所有 driveItem。</span><span class="sxs-lookup"><span data-stu-id="4105f-142">All driveItems contained in the sharing root.</span></span> <span data-ttu-id="4105f-143">不能枚举此集合。</span><span class="sxs-lookup"><span data-stu-id="4105f-143">This collection cannot be enumerated.</span></span>
| <span data-ttu-id="4105f-144">**root**</span><span class="sxs-lookup"><span data-stu-id="4105f-144">**root**</span></span>          | <span data-ttu-id="4105f-145">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="4105f-145">[**driveItem**][driveItem]</span></span>   | <span data-ttu-id="4105f-146">用于访问基础**driveItem**。</span><span class="sxs-lookup"><span data-stu-id="4105f-146">Used to access the underlying **driveItem**.</span></span> <span data-ttu-id="4105f-147">已弃用-- `driveItem`改用。</span><span class="sxs-lookup"><span data-stu-id="4105f-147">Deprecated -- use `driveItem` instead.</span></span>

[driveItem]: driveitem.md
[list]: list.md
[listItem]: listitem.md
[site]: site.md

## <a name="methods"></a><span data-ttu-id="4105f-148">方法</span><span class="sxs-lookup"><span data-stu-id="4105f-148">Methods</span></span>

| <span data-ttu-id="4105f-149">方法</span><span class="sxs-lookup"><span data-stu-id="4105f-149">Method</span></span>                                  | <span data-ttu-id="4105f-150">REST 路径</span><span class="sxs-lookup"><span data-stu-id="4105f-150">REST Path</span></span>                |
| :-------------------------------------- | :----------------------- |
| [<span data-ttu-id="4105f-151">获取共享项目</span><span class="sxs-lookup"><span data-stu-id="4105f-151">Get shared item</span></span>](../api/shares-get.md) | `GET /shares/{share-id}` |

## <a name="remarks"></a><span data-ttu-id="4105f-152">注解</span><span class="sxs-lookup"><span data-stu-id="4105f-152">Remarks</span></span>

<span data-ttu-id="4105f-153">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="4105f-153">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Share resource returns information about a shared item or collection of items.",
  "keywords": "share,shared,sharing root,shared files, shared items",
  "section": "documentation",
  "tocPath": "Resources/Share"
} -->
