---
author: JeremyKelley
ms.date: 09/10/2017
title: SharedDriveItem
localization_priority: Normal
description: 使用 Shares API 访问共享的 driveItem 时，返回 sharedDriveItem 资源。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 9b00703b1fea7689eae942ffb790e8d65672b89b
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238874"
---
# <a name="shareddriveitem-resource-type"></a><span data-ttu-id="50d12-103">SharedDriveItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="50d12-103">SharedDriveItem resource type</span></span>

<span data-ttu-id="50d12-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50d12-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="50d12-105">使用 [Shares](../api/shares-get.md) API 访问共享的 [driveItem](driveitem.md) 时，返回 **sharedDriveItem** 资源。</span><span class="sxs-lookup"><span data-stu-id="50d12-105">The **sharedDriveItem** resource is returned when using the [Shares](../api/shares-get.md) API to access a shared [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="50d12-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="50d12-106">JSON representation</span></span>

<span data-ttu-id="50d12-107">下面是 **sharedDriveItem** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="50d12-107">Here is a JSON representation of the **sharedDriveItem** resource.</span></span>

<span data-ttu-id="50d12-108">**sharedDriveItem** 资源由 [**baseItem**](baseitem.md) 派生并继承该资源的属性。</span><span class="sxs-lookup"><span data-stu-id="50d12-108">The **sharedDriveItem** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="50d12-109">属性</span><span class="sxs-lookup"><span data-stu-id="50d12-109">Properties</span></span>

| <span data-ttu-id="50d12-110">属性</span><span class="sxs-lookup"><span data-stu-id="50d12-110">Property</span></span> | <span data-ttu-id="50d12-111">类型</span><span class="sxs-lookup"><span data-stu-id="50d12-111">Type</span></span>                          | <span data-ttu-id="50d12-112">说明</span><span class="sxs-lookup"><span data-stu-id="50d12-112">Description</span></span>                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="50d12-113">id</span><span class="sxs-lookup"><span data-stu-id="50d12-113">id</span></span>       | <span data-ttu-id="50d12-114">String</span><span class="sxs-lookup"><span data-stu-id="50d12-114">String</span></span>                        | <span data-ttu-id="50d12-115">要访问的内容的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="50d12-115">The unique identifier for the share being accessed.</span></span>              |
| <span data-ttu-id="50d12-116">名称</span><span class="sxs-lookup"><span data-stu-id="50d12-116">name</span></span>     | <span data-ttu-id="50d12-117">String</span><span class="sxs-lookup"><span data-stu-id="50d12-117">String</span></span>                        | <span data-ttu-id="50d12-118">共享项的显示名称。</span><span class="sxs-lookup"><span data-stu-id="50d12-118">The display name of the shared item.</span></span>                             |
| <span data-ttu-id="50d12-119">所有者</span><span class="sxs-lookup"><span data-stu-id="50d12-119">owner</span></span>    | [<span data-ttu-id="50d12-120">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="50d12-120">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="50d12-121">正在引用的共享项的所有者信息。</span><span class="sxs-lookup"><span data-stu-id="50d12-121">Information about the owner of the shared item being referenced.</span></span> |

## <a name="relationships"></a><span data-ttu-id="50d12-122">关系</span><span class="sxs-lookup"><span data-stu-id="50d12-122">Relationships</span></span>

| <span data-ttu-id="50d12-123">关系名称</span><span class="sxs-lookup"><span data-stu-id="50d12-123">Relationship name</span></span> | <span data-ttu-id="50d12-124">类型</span><span class="sxs-lookup"><span data-stu-id="50d12-124">Type</span></span>                | <span data-ttu-id="50d12-125">说明</span><span class="sxs-lookup"><span data-stu-id="50d12-125">Description</span></span>
| ------------------|:--------------------|:-----------------------------------
| <span data-ttu-id="50d12-126">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="50d12-126">**driveItem**</span></span>     | <span data-ttu-id="50d12-127">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="50d12-127">[**driveItem**][driveItem]</span></span>   | <span data-ttu-id="50d12-128">用于访问基础 **driveItem**</span><span class="sxs-lookup"><span data-stu-id="50d12-128">Used to access the underlying **driveItem**</span></span>
| <span data-ttu-id="50d12-129">**list**</span><span class="sxs-lookup"><span data-stu-id="50d12-129">**list**</span></span>          | <span data-ttu-id="50d12-130">[**list**][list]</span><span class="sxs-lookup"><span data-stu-id="50d12-130">[**list**][list]</span></span>        | <span data-ttu-id="50d12-131">用于访问基础 **list**</span><span class="sxs-lookup"><span data-stu-id="50d12-131">Used to access the underlying **list**</span></span>
| <span data-ttu-id="50d12-132">**listItem**</span><span class="sxs-lookup"><span data-stu-id="50d12-132">**listItem**</span></span>      | <span data-ttu-id="50d12-133">[**listItem**][listItem]</span><span class="sxs-lookup"><span data-stu-id="50d12-133">[**listItem**][listItem]</span></span>    | <span data-ttu-id="50d12-134">用于访问基础 **listItem**</span><span class="sxs-lookup"><span data-stu-id="50d12-134">Used to access the underlying **listItem**</span></span>
| <span data-ttu-id="50d12-135">**权限**</span><span class="sxs-lookup"><span data-stu-id="50d12-135">**permission**</span></span>    | <span data-ttu-id="50d12-136">[**权限**][permission]</span><span class="sxs-lookup"><span data-stu-id="50d12-136">[**permission**][permission]</span></span> | <span data-ttu-id="50d12-137">用于访问 **表示** 基础共享链接的权限</span><span class="sxs-lookup"><span data-stu-id="50d12-137">Used to access the **permission** representing the underlying sharing link</span></span>
| <span data-ttu-id="50d12-138">**网站**</span><span class="sxs-lookup"><span data-stu-id="50d12-138">**site**</span></span>          | <span data-ttu-id="50d12-139">[**网站**][site]</span><span class="sxs-lookup"><span data-stu-id="50d12-139">[**site**][site]</span></span>        | <span data-ttu-id="50d12-140">用于访问基础 **site**</span><span class="sxs-lookup"><span data-stu-id="50d12-140">Used to access the underlying **site**</span></span>

<span data-ttu-id="50d12-141">另外，对于从个人 OneDrive 帐户共享的 **driveItems**，也可使用以下关系。</span><span class="sxs-lookup"><span data-stu-id="50d12-141">Alternatively, for **driveItems** shared from personal OneDrive accounts, the following relationships may also be used.</span></span>

| <span data-ttu-id="50d12-142">关系名称</span><span class="sxs-lookup"><span data-stu-id="50d12-142">Relationship name</span></span> | <span data-ttu-id="50d12-143">类型</span><span class="sxs-lookup"><span data-stu-id="50d12-143">Type</span></span>                         | <span data-ttu-id="50d12-144">说明</span><span class="sxs-lookup"><span data-stu-id="50d12-144">Description</span></span>
| ------------------|:-----------------------------|:-----------------------------------
| <span data-ttu-id="50d12-145">**items**</span><span class="sxs-lookup"><span data-stu-id="50d12-145">**items**</span></span>         | <span data-ttu-id="50d12-146">[**driveItem**][driveItem] 集合</span><span class="sxs-lookup"><span data-stu-id="50d12-146">[**driveItem**][driveItem] collection</span></span> | <span data-ttu-id="50d12-147">共享根中包含的所有 driveItem。</span><span class="sxs-lookup"><span data-stu-id="50d12-147">All driveItems contained in the sharing root.</span></span> <span data-ttu-id="50d12-148">不能枚举此集合。</span><span class="sxs-lookup"><span data-stu-id="50d12-148">This collection cannot be enumerated.</span></span>
| <span data-ttu-id="50d12-149">**root**</span><span class="sxs-lookup"><span data-stu-id="50d12-149">**root**</span></span>          | <span data-ttu-id="50d12-150">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="50d12-150">[**driveItem**][driveItem]</span></span>   | <span data-ttu-id="50d12-151">用于访问基础 **driveItem**。</span><span class="sxs-lookup"><span data-stu-id="50d12-151">Used to access the underlying **driveItem**.</span></span> <span data-ttu-id="50d12-152">已弃用 -- 请 `driveItem` 改为使用。</span><span class="sxs-lookup"><span data-stu-id="50d12-152">Deprecated -- use `driveItem` instead.</span></span>

[driveItem]: driveitem.md
[list]: list.md
[listItem]: listitem.md
[permission]: permission.md
[site]: site.md

## <a name="methods"></a><span data-ttu-id="50d12-153">方法</span><span class="sxs-lookup"><span data-stu-id="50d12-153">Methods</span></span>

| <span data-ttu-id="50d12-154">方法</span><span class="sxs-lookup"><span data-stu-id="50d12-154">Method</span></span>                                  | <span data-ttu-id="50d12-155">REST 路径</span><span class="sxs-lookup"><span data-stu-id="50d12-155">REST Path</span></span>                |
| :-------------------------------------- | :----------------------- |
| [<span data-ttu-id="50d12-156">获取共享项目</span><span class="sxs-lookup"><span data-stu-id="50d12-156">Get shared item</span></span>](../api/shares-get.md) | `GET /shares/{share-id}` |

## <a name="remarks"></a><span data-ttu-id="50d12-157">注解</span><span class="sxs-lookup"><span data-stu-id="50d12-157">Remarks</span></span>

<span data-ttu-id="50d12-158">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="50d12-158">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Share resource returns information about a shared item or collection of items.",
  "keywords": "share,shared,sharing root,shared files, shared items",
  "section": "documentation",
  "tocPath": "Resources/Share"
} -->

