---
author: JeremyKelley
description: 使用 Shares API 访问共享的 driveItem 时，返回 sharedDriveItem 资源。
ms.date: 09/10/2017
title: SharedDriveItem
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: a2e1252437608d474e92346ed0aaba4a3a50053d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060027"
---
# <a name="shareddriveitem-resource-type"></a><span data-ttu-id="0e4bd-103">SharedDriveItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="0e4bd-103">SharedDriveItem resource type</span></span>

<span data-ttu-id="0e4bd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e4bd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e4bd-105">使用 [Shares](../api/shares-get.md) API 访问共享的 [driveItem](driveitem.md) 时，返回 **sharedDriveItem** 资源。</span><span class="sxs-lookup"><span data-stu-id="0e4bd-105">The **sharedDriveItem** resource is returned when using the [Shares](../api/shares-get.md) API to access a shared [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="0e4bd-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0e4bd-106">JSON representation</span></span>

<span data-ttu-id="0e4bd-107">下面是 **sharedDriveItem** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0e4bd-107">Here is a JSON representation of the **sharedDriveItem** resource.</span></span>

<span data-ttu-id="0e4bd-108">**sharedDriveItem** 资源由 [**baseItem**](baseitem.md) 派生并继承该资源的属性。</span><span class="sxs-lookup"><span data-stu-id="0e4bd-108">The **sharedDriveItem** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="0e4bd-109">属性</span><span class="sxs-lookup"><span data-stu-id="0e4bd-109">Properties</span></span>

| <span data-ttu-id="0e4bd-110">属性</span><span class="sxs-lookup"><span data-stu-id="0e4bd-110">Property</span></span> | <span data-ttu-id="0e4bd-111">类型</span><span class="sxs-lookup"><span data-stu-id="0e4bd-111">Type</span></span>                          | <span data-ttu-id="0e4bd-112">说明</span><span class="sxs-lookup"><span data-stu-id="0e4bd-112">Description</span></span>                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="0e4bd-113">id</span><span class="sxs-lookup"><span data-stu-id="0e4bd-113">id</span></span>       | <span data-ttu-id="0e4bd-114">String</span><span class="sxs-lookup"><span data-stu-id="0e4bd-114">String</span></span>                        | <span data-ttu-id="0e4bd-115">要访问的内容的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="0e4bd-115">The unique identifier for the share being accessed.</span></span>              |
| <span data-ttu-id="0e4bd-116">名称</span><span class="sxs-lookup"><span data-stu-id="0e4bd-116">name</span></span>     | <span data-ttu-id="0e4bd-117">String</span><span class="sxs-lookup"><span data-stu-id="0e4bd-117">String</span></span>                        | <span data-ttu-id="0e4bd-118">共享项的显示名称。</span><span class="sxs-lookup"><span data-stu-id="0e4bd-118">The display name of the shared item.</span></span>                             |
| <span data-ttu-id="0e4bd-119">所有者</span><span class="sxs-lookup"><span data-stu-id="0e4bd-119">owner</span></span>    | [<span data-ttu-id="0e4bd-120">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="0e4bd-120">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="0e4bd-121">正在引用的共享项的所有者信息。</span><span class="sxs-lookup"><span data-stu-id="0e4bd-121">Information about the owner of the shared item being referenced.</span></span> |

## <a name="relationships"></a><span data-ttu-id="0e4bd-122">关系</span><span class="sxs-lookup"><span data-stu-id="0e4bd-122">Relationships</span></span>

| <span data-ttu-id="0e4bd-123">关系名称</span><span class="sxs-lookup"><span data-stu-id="0e4bd-123">Relationship name</span></span> | <span data-ttu-id="0e4bd-124">类型</span><span class="sxs-lookup"><span data-stu-id="0e4bd-124">Type</span></span>                | <span data-ttu-id="0e4bd-125">说明</span><span class="sxs-lookup"><span data-stu-id="0e4bd-125">Description</span></span>
| ------------------|:--------------------|:-----------------------------------
| <span data-ttu-id="0e4bd-126">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="0e4bd-126">**driveItem**</span></span>     | <span data-ttu-id="0e4bd-127">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="0e4bd-127">[**driveItem**][driveItem]</span></span> | <span data-ttu-id="0e4bd-128">用于访问基础 **driveItem**</span><span class="sxs-lookup"><span data-stu-id="0e4bd-128">Used to access the underlying **driveItem**</span></span>
| <span data-ttu-id="0e4bd-129">**list**</span><span class="sxs-lookup"><span data-stu-id="0e4bd-129">**list**</span></span>          | <span data-ttu-id="0e4bd-130">[**list**][list]</span><span class="sxs-lookup"><span data-stu-id="0e4bd-130">[**list**][list]</span></span>           | <span data-ttu-id="0e4bd-131">用于访问基础 **list**</span><span class="sxs-lookup"><span data-stu-id="0e4bd-131">Used to access the underlying **list**</span></span>
| <span data-ttu-id="0e4bd-132">**listItem**</span><span class="sxs-lookup"><span data-stu-id="0e4bd-132">**listItem**</span></span>      | <span data-ttu-id="0e4bd-133">[**listItem**][listItem]</span><span class="sxs-lookup"><span data-stu-id="0e4bd-133">[**listItem**][listItem]</span></span>   | <span data-ttu-id="0e4bd-134">用于访问基础 **listItem**</span><span class="sxs-lookup"><span data-stu-id="0e4bd-134">Used to access the underlying **listItem**</span></span>
| <span data-ttu-id="0e4bd-135">**权限**</span><span class="sxs-lookup"><span data-stu-id="0e4bd-135">**permission**</span></span>    | <span data-ttu-id="0e4bd-136">[**拒绝**][permission]</span><span class="sxs-lookup"><span data-stu-id="0e4bd-136">[**permission**][permission]</span></span> | <span data-ttu-id="0e4bd-137">用于访问代表基础共享链接的**权限**</span><span class="sxs-lookup"><span data-stu-id="0e4bd-137">Used to access the **permission** representing the underlying sharing link</span></span>
| <span data-ttu-id="0e4bd-138">**site**</span><span class="sxs-lookup"><span data-stu-id="0e4bd-138">**site**</span></span>          | <span data-ttu-id="0e4bd-139">[**site**][site]</span><span class="sxs-lookup"><span data-stu-id="0e4bd-139">[**site**][site]</span></span>           | <span data-ttu-id="0e4bd-140">用于访问基础 **site**</span><span class="sxs-lookup"><span data-stu-id="0e4bd-140">Used to access the underlying **site**</span></span>

<span data-ttu-id="0e4bd-141">另外，对于从个人 OneDrive 帐户共享的 **driveItems**，也可使用以下关系。</span><span class="sxs-lookup"><span data-stu-id="0e4bd-141">Alternatively, for **driveItems** shared from personal OneDrive accounts, the following relationships may also be used.</span></span>

| <span data-ttu-id="0e4bd-142">关系名称</span><span class="sxs-lookup"><span data-stu-id="0e4bd-142">Relationship name</span></span> | <span data-ttu-id="0e4bd-143">类型</span><span class="sxs-lookup"><span data-stu-id="0e4bd-143">Type</span></span>                         | <span data-ttu-id="0e4bd-144">说明</span><span class="sxs-lookup"><span data-stu-id="0e4bd-144">Description</span></span>
| ------------------|:-----------------------------|:-----------------------------------
| <span data-ttu-id="0e4bd-145">**items**</span><span class="sxs-lookup"><span data-stu-id="0e4bd-145">**items**</span></span>         | <span data-ttu-id="0e4bd-146">[**driveItem**][driveItem] 集合</span><span class="sxs-lookup"><span data-stu-id="0e4bd-146">[**driveItem**][driveItem] collection</span></span> | <span data-ttu-id="0e4bd-147">共享根中包含的所有 driveItem。</span><span class="sxs-lookup"><span data-stu-id="0e4bd-147">All driveItems contained in the sharing root.</span></span> <span data-ttu-id="0e4bd-148">不能枚举该集合。</span><span class="sxs-lookup"><span data-stu-id="0e4bd-148">This collection cannot be enumerated.</span></span>
| <span data-ttu-id="0e4bd-149">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="0e4bd-149">**driveItem**</span></span>     | <span data-ttu-id="0e4bd-150">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="0e4bd-150">[**driveItem**][driveItem]</span></span>            | <span data-ttu-id="0e4bd-151">用于访问基础 **driveItem**</span><span class="sxs-lookup"><span data-stu-id="0e4bd-151">Used to access the underlying **driveItem**</span></span>

[driveItem]: driveitem.md
[list]: list.md
[listItem]: listitem.md
[permission]: permission.md
[site]: site.md

## <a name="methods"></a><span data-ttu-id="0e4bd-152">方法</span><span class="sxs-lookup"><span data-stu-id="0e4bd-152">Methods</span></span>

| <span data-ttu-id="0e4bd-153">方法</span><span class="sxs-lookup"><span data-stu-id="0e4bd-153">Method</span></span>                                  | <span data-ttu-id="0e4bd-154">REST 路径</span><span class="sxs-lookup"><span data-stu-id="0e4bd-154">REST Path</span></span>                |
| :-------------------------------------- | :----------------------- |
| [<span data-ttu-id="0e4bd-155">获取共享项目</span><span class="sxs-lookup"><span data-stu-id="0e4bd-155">Get shared item</span></span>](../api/shares-get.md) | `GET /shares/{share-id}` |

## <a name="remarks"></a><span data-ttu-id="0e4bd-156">注解</span><span class="sxs-lookup"><span data-stu-id="0e4bd-156">Remarks</span></span>

<span data-ttu-id="0e4bd-157">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="0e4bd-157">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

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


