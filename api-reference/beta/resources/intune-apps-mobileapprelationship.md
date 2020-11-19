---
title: mobileAppRelationship 资源类型
description: 描述两个移动应用程序之间的关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 22af70876075aa12b5493cfa413c79bd2c71c7cf
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49217191"
---
# <a name="mobileapprelationship-resource-type"></a><span data-ttu-id="ba5b9-103">mobileAppRelationship 资源类型</span><span class="sxs-lookup"><span data-stu-id="ba5b9-103">mobileAppRelationship resource type</span></span>

<span data-ttu-id="ba5b9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba5b9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ba5b9-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ba5b9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba5b9-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ba5b9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba5b9-107">描述两个移动应用程序之间的关系。</span><span class="sxs-lookup"><span data-stu-id="ba5b9-107">Describes a relationship between two mobile apps.</span></span>

## <a name="methods"></a><span data-ttu-id="ba5b9-108">方法</span><span class="sxs-lookup"><span data-stu-id="ba5b9-108">Methods</span></span>
|<span data-ttu-id="ba5b9-109">方法</span><span class="sxs-lookup"><span data-stu-id="ba5b9-109">Method</span></span>|<span data-ttu-id="ba5b9-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="ba5b9-110">Return Type</span></span>|<span data-ttu-id="ba5b9-111">说明</span><span class="sxs-lookup"><span data-stu-id="ba5b9-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ba5b9-112">列出 mobileAppRelationships</span><span class="sxs-lookup"><span data-stu-id="ba5b9-112">List mobileAppRelationships</span></span>](../api/intune-apps-mobileapprelationship-list.md)|<span data-ttu-id="ba5b9-113">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ba5b9-113">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) collection</span></span>|<span data-ttu-id="ba5b9-114">列出 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ba5b9-114">List properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) objects.</span></span>|
|[<span data-ttu-id="ba5b9-115">获取 mobileAppRelationship</span><span class="sxs-lookup"><span data-stu-id="ba5b9-115">Get mobileAppRelationship</span></span>](../api/intune-apps-mobileapprelationship-get.md)|[<span data-ttu-id="ba5b9-116">mobileAppRelationship</span><span class="sxs-lookup"><span data-stu-id="ba5b9-116">mobileAppRelationship</span></span>](../resources/intune-apps-mobileapprelationship.md)|<span data-ttu-id="ba5b9-117">读取 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ba5b9-117">Read properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ba5b9-118">属性</span><span class="sxs-lookup"><span data-stu-id="ba5b9-118">Properties</span></span>
|<span data-ttu-id="ba5b9-119">属性</span><span class="sxs-lookup"><span data-stu-id="ba5b9-119">Property</span></span>|<span data-ttu-id="ba5b9-120">类型</span><span class="sxs-lookup"><span data-stu-id="ba5b9-120">Type</span></span>|<span data-ttu-id="ba5b9-121">说明</span><span class="sxs-lookup"><span data-stu-id="ba5b9-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba5b9-122">id</span><span class="sxs-lookup"><span data-stu-id="ba5b9-122">id</span></span>|<span data-ttu-id="ba5b9-123">String</span><span class="sxs-lookup"><span data-stu-id="ba5b9-123">String</span></span>|<span data-ttu-id="ba5b9-124">关系实体 id。</span><span class="sxs-lookup"><span data-stu-id="ba5b9-124">The relationship entity id.</span></span>|
|<span data-ttu-id="ba5b9-125">targetId</span><span class="sxs-lookup"><span data-stu-id="ba5b9-125">targetId</span></span>|<span data-ttu-id="ba5b9-126">String</span><span class="sxs-lookup"><span data-stu-id="ba5b9-126">String</span></span>|<span data-ttu-id="ba5b9-127">目标移动应用程序的应用程序 id。</span><span class="sxs-lookup"><span data-stu-id="ba5b9-127">The target mobile app's app id.</span></span>|
|<span data-ttu-id="ba5b9-128">targetDisplayName</span><span class="sxs-lookup"><span data-stu-id="ba5b9-128">targetDisplayName</span></span>|<span data-ttu-id="ba5b9-129">String</span><span class="sxs-lookup"><span data-stu-id="ba5b9-129">String</span></span>|<span data-ttu-id="ba5b9-130">目标移动应用程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="ba5b9-130">The target mobile app's display name.</span></span>|
|<span data-ttu-id="ba5b9-131">targetDisplayVersion</span><span class="sxs-lookup"><span data-stu-id="ba5b9-131">targetDisplayVersion</span></span>|<span data-ttu-id="ba5b9-132">String</span><span class="sxs-lookup"><span data-stu-id="ba5b9-132">String</span></span>|<span data-ttu-id="ba5b9-133">目标移动应用程序的显示版本。</span><span class="sxs-lookup"><span data-stu-id="ba5b9-133">The target mobile app's display version.</span></span>|
|<span data-ttu-id="ba5b9-134">targetPublisher</span><span class="sxs-lookup"><span data-stu-id="ba5b9-134">targetPublisher</span></span>|<span data-ttu-id="ba5b9-135">String</span><span class="sxs-lookup"><span data-stu-id="ba5b9-135">String</span></span>|<span data-ttu-id="ba5b9-136">目标移动应用程序的发布者。</span><span class="sxs-lookup"><span data-stu-id="ba5b9-136">The target mobile app's publisher.</span></span>|
|<span data-ttu-id="ba5b9-137">targetType</span><span class="sxs-lookup"><span data-stu-id="ba5b9-137">targetType</span></span>|[<span data-ttu-id="ba5b9-138">mobileAppRelationshipType</span><span class="sxs-lookup"><span data-stu-id="ba5b9-138">mobileAppRelationshipType</span></span>](../resources/intune-apps-mobileapprelationshiptype.md)|<span data-ttu-id="ba5b9-139">表示目标是父项还是子项的关系的类型。</span><span class="sxs-lookup"><span data-stu-id="ba5b9-139">The type of relationship indicating whether the target is a parent or child.</span></span> <span data-ttu-id="ba5b9-140">可取值为：`child`、`parent`。</span><span class="sxs-lookup"><span data-stu-id="ba5b9-140">Possible values are: `child`, `parent`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ba5b9-141">关系</span><span class="sxs-lookup"><span data-stu-id="ba5b9-141">Relationships</span></span>
<span data-ttu-id="ba5b9-142">无</span><span class="sxs-lookup"><span data-stu-id="ba5b9-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ba5b9-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ba5b9-143">JSON Representation</span></span>
<span data-ttu-id="ba5b9-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ba5b9-144">Here is a JSON representation of the resource.</span></span>
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
  "targetDisplayName": "String",
  "targetDisplayVersion": "String",
  "targetPublisher": "String",
  "targetType": "String"
}
```




