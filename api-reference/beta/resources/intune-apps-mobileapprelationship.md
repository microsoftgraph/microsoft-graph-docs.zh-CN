---
title: mobileAppRelationship 资源类型
description: 介绍了如何将子移动应用程序与其父移动应用程序之间的关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 80cf0fd5897d0ff3d1b3b3adc5343ad4c059442e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43462580"
---
# <a name="mobileapprelationship-resource-type"></a><span data-ttu-id="c9322-103">mobileAppRelationship 资源类型</span><span class="sxs-lookup"><span data-stu-id="c9322-103">mobileAppRelationship resource type</span></span>

<span data-ttu-id="c9322-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9322-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c9322-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c9322-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c9322-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c9322-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9322-107">介绍了如何将子移动应用程序与其父移动应用程序之间的关系。</span><span class="sxs-lookup"><span data-stu-id="c9322-107">Describes the relationship for a child mobile app to its parent mobile app.</span></span>

## <a name="methods"></a><span data-ttu-id="c9322-108">方法</span><span class="sxs-lookup"><span data-stu-id="c9322-108">Methods</span></span>
|<span data-ttu-id="c9322-109">方法</span><span class="sxs-lookup"><span data-stu-id="c9322-109">Method</span></span>|<span data-ttu-id="c9322-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="c9322-110">Return Type</span></span>|<span data-ttu-id="c9322-111">说明</span><span class="sxs-lookup"><span data-stu-id="c9322-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c9322-112">列出 mobileAppRelationships</span><span class="sxs-lookup"><span data-stu-id="c9322-112">List mobileAppRelationships</span></span>](../api/intune-apps-mobileapprelationship-list.md)|<span data-ttu-id="c9322-113">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)集合</span><span class="sxs-lookup"><span data-stu-id="c9322-113">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) collection</span></span>|<span data-ttu-id="c9322-114">列出[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c9322-114">List properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) objects.</span></span>|
|[<span data-ttu-id="c9322-115">获取 mobileAppRelationship</span><span class="sxs-lookup"><span data-stu-id="c9322-115">Get mobileAppRelationship</span></span>](../api/intune-apps-mobileapprelationship-get.md)|[<span data-ttu-id="c9322-116">mobileAppRelationship</span><span class="sxs-lookup"><span data-stu-id="c9322-116">mobileAppRelationship</span></span>](../resources/intune-apps-mobileapprelationship.md)|<span data-ttu-id="c9322-117">读取[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c9322-117">Read properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c9322-118">属性</span><span class="sxs-lookup"><span data-stu-id="c9322-118">Properties</span></span>
|<span data-ttu-id="c9322-119">属性</span><span class="sxs-lookup"><span data-stu-id="c9322-119">Property</span></span>|<span data-ttu-id="c9322-120">类型</span><span class="sxs-lookup"><span data-stu-id="c9322-120">Type</span></span>|<span data-ttu-id="c9322-121">说明</span><span class="sxs-lookup"><span data-stu-id="c9322-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9322-122">id</span><span class="sxs-lookup"><span data-stu-id="c9322-122">id</span></span>|<span data-ttu-id="c9322-123">String</span><span class="sxs-lookup"><span data-stu-id="c9322-123">String</span></span>|<span data-ttu-id="c9322-124">关系实体 id。</span><span class="sxs-lookup"><span data-stu-id="c9322-124">The relationship entity id.</span></span>|
|<span data-ttu-id="c9322-125">targetId</span><span class="sxs-lookup"><span data-stu-id="c9322-125">targetId</span></span>|<span data-ttu-id="c9322-126">String</span><span class="sxs-lookup"><span data-stu-id="c9322-126">String</span></span>|<span data-ttu-id="c9322-127">目标子移动应用程序的应用程序 id。</span><span class="sxs-lookup"><span data-stu-id="c9322-127">The target child mobile app's app id.</span></span>|
|<span data-ttu-id="c9322-128">targetDisplayName</span><span class="sxs-lookup"><span data-stu-id="c9322-128">targetDisplayName</span></span>|<span data-ttu-id="c9322-129">String</span><span class="sxs-lookup"><span data-stu-id="c9322-129">String</span></span>|<span data-ttu-id="c9322-130">目标子移动应用程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="c9322-130">The target child mobile app's display name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c9322-131">关系</span><span class="sxs-lookup"><span data-stu-id="c9322-131">Relationships</span></span>
<span data-ttu-id="c9322-132">无</span><span class="sxs-lookup"><span data-stu-id="c9322-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c9322-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c9322-133">JSON Representation</span></span>
<span data-ttu-id="c9322-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c9322-134">Here is a JSON representation of the resource.</span></span>
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



