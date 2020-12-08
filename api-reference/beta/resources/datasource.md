---
title: dataSource 资源类型
description: 数据源实体-摘要基类
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 645ae33eb6c43972122623e52bfecf17f39491e4
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597594"
---
# <a name="datasource-resource-type"></a><span data-ttu-id="f7398-103">dataSource 资源类型</span><span class="sxs-lookup"><span data-stu-id="f7398-103">dataSource resource type</span></span>

<span data-ttu-id="f7398-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7398-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f7398-105">DataSource 实体是一个抽象 baseclass，用于标识电子数据展示的内容源。</span><span class="sxs-lookup"><span data-stu-id="f7398-105">The dataSource entity is an abstract baseclass used to identify sources of content for eDiscovery.</span></span>

## <a name="methods"></a><span data-ttu-id="f7398-106">方法</span><span class="sxs-lookup"><span data-stu-id="f7398-106">Methods</span></span>

<span data-ttu-id="f7398-107">无</span><span class="sxs-lookup"><span data-stu-id="f7398-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="f7398-108">属性</span><span class="sxs-lookup"><span data-stu-id="f7398-108">Properties</span></span>

|<span data-ttu-id="f7398-109">属性</span><span class="sxs-lookup"><span data-stu-id="f7398-109">Property</span></span>|<span data-ttu-id="f7398-110">类型</span><span class="sxs-lookup"><span data-stu-id="f7398-110">Type</span></span>|<span data-ttu-id="f7398-111">说明</span><span class="sxs-lookup"><span data-stu-id="f7398-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7398-112">createdBy</span><span class="sxs-lookup"><span data-stu-id="f7398-112">createdBy</span></span>|[<span data-ttu-id="f7398-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="f7398-113">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="f7398-114">创建 **数据源** 的用户。</span><span class="sxs-lookup"><span data-stu-id="f7398-114">The user who created the **dataSource**.</span></span>|
|<span data-ttu-id="f7398-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f7398-115">createdDateTime</span></span>|<span data-ttu-id="f7398-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7398-116">DateTimeOffset</span></span>|<span data-ttu-id="f7398-117">**数据源** 的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f7398-117">The date and time the **dataSource** was created.</span></span>|
|<span data-ttu-id="f7398-118">displayName</span><span class="sxs-lookup"><span data-stu-id="f7398-118">displayName</span></span>|<span data-ttu-id="f7398-119">String</span><span class="sxs-lookup"><span data-stu-id="f7398-119">String</span></span>|<span data-ttu-id="f7398-120">**数据源** 的显示名称。</span><span class="sxs-lookup"><span data-stu-id="f7398-120">The display name of the **dataSource**.</span></span> <span data-ttu-id="f7398-121">这将是 SharePoint 网站的名称。</span><span class="sxs-lookup"><span data-stu-id="f7398-121">This will be the name of the SharePoint site.</span></span>|
|<span data-ttu-id="f7398-122">id</span><span class="sxs-lookup"><span data-stu-id="f7398-122">id</span></span>|<span data-ttu-id="f7398-123">String</span><span class="sxs-lookup"><span data-stu-id="f7398-123">String</span></span>| <span data-ttu-id="f7398-124">**数据源** 的 ID。</span><span class="sxs-lookup"><span data-stu-id="f7398-124">The ID of the **dataSource**.</span></span> <span data-ttu-id="f7398-125">这不是实际网站的 ID。</span><span class="sxs-lookup"><span data-stu-id="f7398-125">This is not the ID of the actual site.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f7398-126">关系</span><span class="sxs-lookup"><span data-stu-id="f7398-126">Relationships</span></span>

<span data-ttu-id="f7398-127">无。</span><span class="sxs-lookup"><span data-stu-id="f7398-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f7398-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f7398-128">JSON representation</span></span>

<span data-ttu-id="f7398-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f7398-129">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.dataSource",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.dataSource",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "id": "String (identifier)"
}
```
