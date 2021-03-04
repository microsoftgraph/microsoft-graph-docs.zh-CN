---
title: dataSource 资源类型
description: DataSource 实体是一个抽象基类，用于标识电子数据展示的内容源。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 2f945ba74a5576a35146ee1832f3740b537ed23b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446156"
---
# <a name="datasource-resource-type"></a><span data-ttu-id="3d11b-103">dataSource 资源类型</span><span class="sxs-lookup"><span data-stu-id="3d11b-103">dataSource resource type</span></span>

<span data-ttu-id="3d11b-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="3d11b-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d11b-105">DataSource 实体是一个抽象基类，用于标识电子数据展示的内容源。</span><span class="sxs-lookup"><span data-stu-id="3d11b-105">The dataSource entity is an abstract base class used to identify sources of content for eDiscovery.</span></span>

## <a name="methods"></a><span data-ttu-id="3d11b-106">Methods</span><span class="sxs-lookup"><span data-stu-id="3d11b-106">Methods</span></span>

<span data-ttu-id="3d11b-107">无</span><span class="sxs-lookup"><span data-stu-id="3d11b-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="3d11b-108">属性</span><span class="sxs-lookup"><span data-stu-id="3d11b-108">Properties</span></span>

|<span data-ttu-id="3d11b-109">属性</span><span class="sxs-lookup"><span data-stu-id="3d11b-109">Property</span></span>|<span data-ttu-id="3d11b-110">类型</span><span class="sxs-lookup"><span data-stu-id="3d11b-110">Type</span></span>|<span data-ttu-id="3d11b-111">说明</span><span class="sxs-lookup"><span data-stu-id="3d11b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d11b-112">createdBy</span><span class="sxs-lookup"><span data-stu-id="3d11b-112">createdBy</span></span>|[<span data-ttu-id="3d11b-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="3d11b-113">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="3d11b-114">创建 **DataSource 的用户**。</span><span class="sxs-lookup"><span data-stu-id="3d11b-114">The user who created the **dataSource**.</span></span>|
|<span data-ttu-id="3d11b-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3d11b-115">createdDateTime</span></span>|<span data-ttu-id="3d11b-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d11b-116">DateTimeOffset</span></span>|<span data-ttu-id="3d11b-117">创建 **dataSource 的** 日期和时间。</span><span class="sxs-lookup"><span data-stu-id="3d11b-117">The date and time the **dataSource** was created.</span></span>|
|<span data-ttu-id="3d11b-118">displayName</span><span class="sxs-lookup"><span data-stu-id="3d11b-118">displayName</span></span>|<span data-ttu-id="3d11b-119">String</span><span class="sxs-lookup"><span data-stu-id="3d11b-119">String</span></span>|<span data-ttu-id="3d11b-120">dataSource 显示名称 **。**</span><span class="sxs-lookup"><span data-stu-id="3d11b-120">The display name of the **dataSource**.</span></span> <span data-ttu-id="3d11b-121">这将是 SharePoint 网站的名称。</span><span class="sxs-lookup"><span data-stu-id="3d11b-121">This will be the name of the SharePoint site.</span></span>|
|<span data-ttu-id="3d11b-122">id</span><span class="sxs-lookup"><span data-stu-id="3d11b-122">id</span></span>|<span data-ttu-id="3d11b-123">String</span><span class="sxs-lookup"><span data-stu-id="3d11b-123">String</span></span>| <span data-ttu-id="3d11b-124">DataSource 的ID。</span><span class="sxs-lookup"><span data-stu-id="3d11b-124">The ID of the **dataSource**.</span></span> <span data-ttu-id="3d11b-125">这不是实际网站的 ID。</span><span class="sxs-lookup"><span data-stu-id="3d11b-125">This is not the ID of the actual site.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3d11b-126">关系</span><span class="sxs-lookup"><span data-stu-id="3d11b-126">Relationships</span></span>

<span data-ttu-id="3d11b-127">无。</span><span class="sxs-lookup"><span data-stu-id="3d11b-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3d11b-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3d11b-128">JSON representation</span></span>

<span data-ttu-id="3d11b-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3d11b-129">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.dataSource",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.dataSource",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "id": "String (identifier)"
}
```
