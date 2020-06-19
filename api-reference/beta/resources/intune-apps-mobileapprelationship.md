---
title: mobileAppRelationship 资源类型
description: 描述两个移动应用程序之间的关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d09d9d7604699ee89b6dccc0f2f980cef26225e7
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44790864"
---
# <a name="mobileapprelationship-resource-type"></a><span data-ttu-id="a5d55-103">mobileAppRelationship 资源类型</span><span class="sxs-lookup"><span data-stu-id="a5d55-103">mobileAppRelationship resource type</span></span>

<span data-ttu-id="a5d55-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5d55-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a5d55-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a5d55-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a5d55-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a5d55-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5d55-107">描述两个移动应用程序之间的关系。</span><span class="sxs-lookup"><span data-stu-id="a5d55-107">Describes a relationship between two mobile apps.</span></span>

## <a name="methods"></a><span data-ttu-id="a5d55-108">Methods</span><span class="sxs-lookup"><span data-stu-id="a5d55-108">Methods</span></span>
|<span data-ttu-id="a5d55-109">方法</span><span class="sxs-lookup"><span data-stu-id="a5d55-109">Method</span></span>|<span data-ttu-id="a5d55-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="a5d55-110">Return Type</span></span>|<span data-ttu-id="a5d55-111">说明</span><span class="sxs-lookup"><span data-stu-id="a5d55-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a5d55-112">列出 mobileAppRelationships</span><span class="sxs-lookup"><span data-stu-id="a5d55-112">List mobileAppRelationships</span></span>](../api/intune-apps-mobileapprelationship-list.md)|<span data-ttu-id="a5d55-113">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)集合</span><span class="sxs-lookup"><span data-stu-id="a5d55-113">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) collection</span></span>|<span data-ttu-id="a5d55-114">列出[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a5d55-114">List properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) objects.</span></span>|
|[<span data-ttu-id="a5d55-115">获取 mobileAppRelationship</span><span class="sxs-lookup"><span data-stu-id="a5d55-115">Get mobileAppRelationship</span></span>](../api/intune-apps-mobileapprelationship-get.md)|[<span data-ttu-id="a5d55-116">mobileAppRelationship</span><span class="sxs-lookup"><span data-stu-id="a5d55-116">mobileAppRelationship</span></span>](../resources/intune-apps-mobileapprelationship.md)|<span data-ttu-id="a5d55-117">读取[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a5d55-117">Read properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a5d55-118">属性</span><span class="sxs-lookup"><span data-stu-id="a5d55-118">Properties</span></span>
|<span data-ttu-id="a5d55-119">属性</span><span class="sxs-lookup"><span data-stu-id="a5d55-119">Property</span></span>|<span data-ttu-id="a5d55-120">类型</span><span class="sxs-lookup"><span data-stu-id="a5d55-120">Type</span></span>|<span data-ttu-id="a5d55-121">说明</span><span class="sxs-lookup"><span data-stu-id="a5d55-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5d55-122">id</span><span class="sxs-lookup"><span data-stu-id="a5d55-122">id</span></span>|<span data-ttu-id="a5d55-123">String</span><span class="sxs-lookup"><span data-stu-id="a5d55-123">String</span></span>|<span data-ttu-id="a5d55-124">关系实体 id。</span><span class="sxs-lookup"><span data-stu-id="a5d55-124">The relationship entity id.</span></span>|
|<span data-ttu-id="a5d55-125">targetId</span><span class="sxs-lookup"><span data-stu-id="a5d55-125">targetId</span></span>|<span data-ttu-id="a5d55-126">String</span><span class="sxs-lookup"><span data-stu-id="a5d55-126">String</span></span>|<span data-ttu-id="a5d55-127">目标移动应用程序的应用程序 id。</span><span class="sxs-lookup"><span data-stu-id="a5d55-127">The target mobile app's app id.</span></span>|
|<span data-ttu-id="a5d55-128">targetDisplayName</span><span class="sxs-lookup"><span data-stu-id="a5d55-128">targetDisplayName</span></span>|<span data-ttu-id="a5d55-129">String</span><span class="sxs-lookup"><span data-stu-id="a5d55-129">String</span></span>|<span data-ttu-id="a5d55-130">目标移动应用程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="a5d55-130">The target mobile app's display name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a5d55-131">关系</span><span class="sxs-lookup"><span data-stu-id="a5d55-131">Relationships</span></span>
<span data-ttu-id="a5d55-132">无</span><span class="sxs-lookup"><span data-stu-id="a5d55-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a5d55-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a5d55-133">JSON Representation</span></span>
<span data-ttu-id="a5d55-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a5d55-134">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppRelationship"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppRelationship",
  "id": "String (identifier)",
  "targetId": "String",
  "targetDisplayName": "String"
}
```



