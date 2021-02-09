---
title: dataSource 资源类型
description: Datasource 实体 - 抽象基类
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: c019a6b8338180584a31382c0741018791973184
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161920"
---
# <a name="datasource-resource-type"></a><span data-ttu-id="2f1c6-103">dataSource 资源类型</span><span class="sxs-lookup"><span data-stu-id="2f1c6-103">dataSource resource type</span></span>

<span data-ttu-id="2f1c6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f1c6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2f1c6-105">DataSource 实体是一个抽象基类，用于标识电子数据展示的内容源。</span><span class="sxs-lookup"><span data-stu-id="2f1c6-105">The dataSource entity is an abstract baseclass used to identify sources of content for eDiscovery.</span></span>

## <a name="methods"></a><span data-ttu-id="2f1c6-106">方法</span><span class="sxs-lookup"><span data-stu-id="2f1c6-106">Methods</span></span>

<span data-ttu-id="2f1c6-107">无</span><span class="sxs-lookup"><span data-stu-id="2f1c6-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="2f1c6-108">属性</span><span class="sxs-lookup"><span data-stu-id="2f1c6-108">Properties</span></span>

|<span data-ttu-id="2f1c6-109">属性</span><span class="sxs-lookup"><span data-stu-id="2f1c6-109">Property</span></span>|<span data-ttu-id="2f1c6-110">类型</span><span class="sxs-lookup"><span data-stu-id="2f1c6-110">Type</span></span>|<span data-ttu-id="2f1c6-111">说明</span><span class="sxs-lookup"><span data-stu-id="2f1c6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f1c6-112">createdBy</span><span class="sxs-lookup"><span data-stu-id="2f1c6-112">createdBy</span></span>|[<span data-ttu-id="2f1c6-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="2f1c6-113">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="2f1c6-114">创建 **DataSource 的用户**。</span><span class="sxs-lookup"><span data-stu-id="2f1c6-114">The user who created the **dataSource**.</span></span>|
|<span data-ttu-id="2f1c6-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2f1c6-115">createdDateTime</span></span>|<span data-ttu-id="2f1c6-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f1c6-116">DateTimeOffset</span></span>|<span data-ttu-id="2f1c6-117">DataSource **的** 创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2f1c6-117">The date and time the **dataSource** was created.</span></span>|
|<span data-ttu-id="2f1c6-118">displayName</span><span class="sxs-lookup"><span data-stu-id="2f1c6-118">displayName</span></span>|<span data-ttu-id="2f1c6-119">String</span><span class="sxs-lookup"><span data-stu-id="2f1c6-119">String</span></span>|<span data-ttu-id="2f1c6-120">dataSource 的 显示名称。</span><span class="sxs-lookup"><span data-stu-id="2f1c6-120">The display name of the **dataSource**.</span></span> <span data-ttu-id="2f1c6-121">这将是 SharePoint 网站的名称。</span><span class="sxs-lookup"><span data-stu-id="2f1c6-121">This will be the name of the SharePoint site.</span></span>|
|<span data-ttu-id="2f1c6-122">id</span><span class="sxs-lookup"><span data-stu-id="2f1c6-122">id</span></span>|<span data-ttu-id="2f1c6-123">String</span><span class="sxs-lookup"><span data-stu-id="2f1c6-123">String</span></span>| <span data-ttu-id="2f1c6-124">DataSource 的ID。</span><span class="sxs-lookup"><span data-stu-id="2f1c6-124">The ID of the **dataSource**.</span></span> <span data-ttu-id="2f1c6-125">这不是实际网站的 ID。</span><span class="sxs-lookup"><span data-stu-id="2f1c6-125">This is not the ID of the actual site.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2f1c6-126">关系</span><span class="sxs-lookup"><span data-stu-id="2f1c6-126">Relationships</span></span>

<span data-ttu-id="2f1c6-127">无。</span><span class="sxs-lookup"><span data-stu-id="2f1c6-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2f1c6-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2f1c6-128">JSON representation</span></span>

<span data-ttu-id="2f1c6-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2f1c6-129">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.dataSource",
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
