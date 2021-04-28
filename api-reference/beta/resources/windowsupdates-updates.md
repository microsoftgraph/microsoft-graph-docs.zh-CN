---
title: 更新资源类型
description: 充当所有 Windows Update for Business 部署服务功能的容器的实体。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 0306dbadd815bdd8ff0ffde5719a950bcdff4683
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067291"
---
# <a name="updates-resource-type"></a><span data-ttu-id="397a5-103">更新资源类型</span><span class="sxs-lookup"><span data-stu-id="397a5-103">updates resource type</span></span>

<span data-ttu-id="397a5-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="397a5-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="397a5-105">充当所有 Windows Update for Business 部署服务功能的容器的实体。</span><span class="sxs-lookup"><span data-stu-id="397a5-105">Entity that acts as a container for all Windows Update for Business deployment service functionality.</span></span>

## <a name="properties"></a><span data-ttu-id="397a5-106">属性</span><span class="sxs-lookup"><span data-stu-id="397a5-106">Properties</span></span>
|<span data-ttu-id="397a5-107">属性</span><span class="sxs-lookup"><span data-stu-id="397a5-107">Property</span></span>|<span data-ttu-id="397a5-108">类型</span><span class="sxs-lookup"><span data-stu-id="397a5-108">Type</span></span>|<span data-ttu-id="397a5-109">说明</span><span class="sxs-lookup"><span data-stu-id="397a5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="397a5-110">id</span><span class="sxs-lookup"><span data-stu-id="397a5-110">id</span></span>|<span data-ttu-id="397a5-111">String</span><span class="sxs-lookup"><span data-stu-id="397a5-111">String</span></span>|<span data-ttu-id="397a5-112">只读。</span><span class="sxs-lookup"><span data-stu-id="397a5-112">Read-only.</span></span> <span data-ttu-id="397a5-113">继承自 [实体](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="397a5-113">Inherited from [entity](../resources/entity.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="397a5-114">关系</span><span class="sxs-lookup"><span data-stu-id="397a5-114">Relationships</span></span>
|<span data-ttu-id="397a5-115">关系</span><span class="sxs-lookup"><span data-stu-id="397a5-115">Relationship</span></span>|<span data-ttu-id="397a5-116">类型</span><span class="sxs-lookup"><span data-stu-id="397a5-116">Type</span></span>|<span data-ttu-id="397a5-117">说明</span><span class="sxs-lookup"><span data-stu-id="397a5-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="397a5-118">catalog</span><span class="sxs-lookup"><span data-stu-id="397a5-118">catalog</span></span>|[<span data-ttu-id="397a5-119">microsoft.graph.windowsUpdates.catalog</span><span class="sxs-lookup"><span data-stu-id="397a5-119">microsoft.graph.windowsUpdates.catalog</span></span>](../resources/windowsupdates-catalog.md)|<span data-ttu-id="397a5-120">部署服务可以批准部署的内容目录。</span><span class="sxs-lookup"><span data-stu-id="397a5-120">Catalog of content that can be approved for deployment by the deployment service.</span></span> <span data-ttu-id="397a5-121">只读。</span><span class="sxs-lookup"><span data-stu-id="397a5-121">Read-only.</span></span>|
|<span data-ttu-id="397a5-122">部署</span><span class="sxs-lookup"><span data-stu-id="397a5-122">deployments</span></span>|<span data-ttu-id="397a5-123">[microsoft.graph.windowsUpdates.deployment](../resources/windowsupdates-deployment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="397a5-123">[microsoft.graph.windowsUpdates.deployment](../resources/windowsupdates-deployment.md) collection</span></span>|<span data-ttu-id="397a5-124">使用部署服务创建的部署。</span><span class="sxs-lookup"><span data-stu-id="397a5-124">Deployments created using the deployment service.</span></span> <span data-ttu-id="397a5-125">只读。</span><span class="sxs-lookup"><span data-stu-id="397a5-125">Read-only.</span></span>|
|<span data-ttu-id="397a5-126">updatableAssets</span><span class="sxs-lookup"><span data-stu-id="397a5-126">updatableAssets</span></span>|<span data-ttu-id="397a5-127">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) 集合</span><span class="sxs-lookup"><span data-stu-id="397a5-127">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="397a5-128">在部署服务中注册可接收更新的资产。</span><span class="sxs-lookup"><span data-stu-id="397a5-128">Assets registered with the deployment service that can receive updates.</span></span> <span data-ttu-id="397a5-129">只读。</span><span class="sxs-lookup"><span data-stu-id="397a5-129">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="397a5-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="397a5-130">JSON representation</span></span>
<span data-ttu-id="397a5-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="397a5-131">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.updates",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.updates",
  "id": "String (identifier)"
}
```

