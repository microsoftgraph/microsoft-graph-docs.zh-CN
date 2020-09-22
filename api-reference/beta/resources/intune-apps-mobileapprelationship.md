---
title: mobileAppRelationship 资源类型
description: 描述两个移动应用程序之间的关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a2c7af932983b9b3657a94a7448149b75b3c8eea
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48076343"
---
# <a name="mobileapprelationship-resource-type"></a><span data-ttu-id="b57a5-103">mobileAppRelationship 资源类型</span><span class="sxs-lookup"><span data-stu-id="b57a5-103">mobileAppRelationship resource type</span></span>

<span data-ttu-id="b57a5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b57a5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b57a5-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b57a5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b57a5-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b57a5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b57a5-107">描述两个移动应用程序之间的关系。</span><span class="sxs-lookup"><span data-stu-id="b57a5-107">Describes a relationship between two mobile apps.</span></span>

## <a name="methods"></a><span data-ttu-id="b57a5-108">方法</span><span class="sxs-lookup"><span data-stu-id="b57a5-108">Methods</span></span>
|<span data-ttu-id="b57a5-109">方法</span><span class="sxs-lookup"><span data-stu-id="b57a5-109">Method</span></span>|<span data-ttu-id="b57a5-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="b57a5-110">Return Type</span></span>|<span data-ttu-id="b57a5-111">说明</span><span class="sxs-lookup"><span data-stu-id="b57a5-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b57a5-112">列出 mobileAppRelationships</span><span class="sxs-lookup"><span data-stu-id="b57a5-112">List mobileAppRelationships</span></span>](../api/intune-apps-mobileapprelationship-list.md)|<span data-ttu-id="b57a5-113">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b57a5-113">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) collection</span></span>|<span data-ttu-id="b57a5-114">列出 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b57a5-114">List properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) objects.</span></span>|
|[<span data-ttu-id="b57a5-115">获取 mobileAppRelationship</span><span class="sxs-lookup"><span data-stu-id="b57a5-115">Get mobileAppRelationship</span></span>](../api/intune-apps-mobileapprelationship-get.md)|[<span data-ttu-id="b57a5-116">mobileAppRelationship</span><span class="sxs-lookup"><span data-stu-id="b57a5-116">mobileAppRelationship</span></span>](../resources/intune-apps-mobileapprelationship.md)|<span data-ttu-id="b57a5-117">读取 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b57a5-117">Read properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b57a5-118">属性</span><span class="sxs-lookup"><span data-stu-id="b57a5-118">Properties</span></span>
|<span data-ttu-id="b57a5-119">属性</span><span class="sxs-lookup"><span data-stu-id="b57a5-119">Property</span></span>|<span data-ttu-id="b57a5-120">类型</span><span class="sxs-lookup"><span data-stu-id="b57a5-120">Type</span></span>|<span data-ttu-id="b57a5-121">说明</span><span class="sxs-lookup"><span data-stu-id="b57a5-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b57a5-122">id</span><span class="sxs-lookup"><span data-stu-id="b57a5-122">id</span></span>|<span data-ttu-id="b57a5-123">String</span><span class="sxs-lookup"><span data-stu-id="b57a5-123">String</span></span>|<span data-ttu-id="b57a5-124">关系实体 id。</span><span class="sxs-lookup"><span data-stu-id="b57a5-124">The relationship entity id.</span></span>|
|<span data-ttu-id="b57a5-125">targetId</span><span class="sxs-lookup"><span data-stu-id="b57a5-125">targetId</span></span>|<span data-ttu-id="b57a5-126">String</span><span class="sxs-lookup"><span data-stu-id="b57a5-126">String</span></span>|<span data-ttu-id="b57a5-127">目标移动应用程序的应用程序 id。</span><span class="sxs-lookup"><span data-stu-id="b57a5-127">The target mobile app's app id.</span></span>|
|<span data-ttu-id="b57a5-128">targetDisplayName</span><span class="sxs-lookup"><span data-stu-id="b57a5-128">targetDisplayName</span></span>|<span data-ttu-id="b57a5-129">String</span><span class="sxs-lookup"><span data-stu-id="b57a5-129">String</span></span>|<span data-ttu-id="b57a5-130">目标移动应用程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="b57a5-130">The target mobile app's display name.</span></span>|
|<span data-ttu-id="b57a5-131">targetType</span><span class="sxs-lookup"><span data-stu-id="b57a5-131">targetType</span></span>|[<span data-ttu-id="b57a5-132">mobileAppRelationshipType</span><span class="sxs-lookup"><span data-stu-id="b57a5-132">mobileAppRelationshipType</span></span>](../resources/intune-apps-mobileapprelationshiptype.md)|<span data-ttu-id="b57a5-133">表示目标是父项还是子项的关系的类型。</span><span class="sxs-lookup"><span data-stu-id="b57a5-133">The type of relationship indicating whether the target is a parent or child.</span></span> <span data-ttu-id="b57a5-134">可取值为：`child`、`parent`。</span><span class="sxs-lookup"><span data-stu-id="b57a5-134">Possible values are: `child`, `parent`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b57a5-135">关系</span><span class="sxs-lookup"><span data-stu-id="b57a5-135">Relationships</span></span>
<span data-ttu-id="b57a5-136">无</span><span class="sxs-lookup"><span data-stu-id="b57a5-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b57a5-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b57a5-137">JSON Representation</span></span>
<span data-ttu-id="b57a5-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b57a5-138">Here is a JSON representation of the resource.</span></span>
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
  "targetType": "String"
}
```






