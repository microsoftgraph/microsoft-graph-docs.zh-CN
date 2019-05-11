---
title: mobileAppRelationship 资源类型
description: 介绍了如何将子移动应用程序与其父移动应用程序之间的关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c871ba51733195947243fa9b22824156108f5eb7
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949883"
---
# <a name="mobileapprelationship-resource-type"></a><span data-ttu-id="87c50-103">mobileAppRelationship 资源类型</span><span class="sxs-lookup"><span data-stu-id="87c50-103">mobileAppRelationship resource type</span></span>

> <span data-ttu-id="87c50-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="87c50-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="87c50-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="87c50-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87c50-106">介绍了如何将子移动应用程序与其父移动应用程序之间的关系。</span><span class="sxs-lookup"><span data-stu-id="87c50-106">Describes the relationship for a child mobile app to its parent mobile app.</span></span>

## <a name="methods"></a><span data-ttu-id="87c50-107">方法</span><span class="sxs-lookup"><span data-stu-id="87c50-107">Methods</span></span>
|<span data-ttu-id="87c50-108">方法</span><span class="sxs-lookup"><span data-stu-id="87c50-108">Method</span></span>|<span data-ttu-id="87c50-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="87c50-109">Return Type</span></span>|<span data-ttu-id="87c50-110">说明</span><span class="sxs-lookup"><span data-stu-id="87c50-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="87c50-111">列出 mobileAppRelationships</span><span class="sxs-lookup"><span data-stu-id="87c50-111">List mobileAppRelationships</span></span>](../api/intune-apps-mobileapprelationship-list.md)|<span data-ttu-id="87c50-112">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)集合</span><span class="sxs-lookup"><span data-stu-id="87c50-112">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) collection</span></span>|<span data-ttu-id="87c50-113">列出[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="87c50-113">List properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) objects.</span></span>|
|[<span data-ttu-id="87c50-114">获取 mobileAppRelationship</span><span class="sxs-lookup"><span data-stu-id="87c50-114">Get mobileAppRelationship</span></span>](../api/intune-apps-mobileapprelationship-get.md)|[<span data-ttu-id="87c50-115">mobileAppRelationship</span><span class="sxs-lookup"><span data-stu-id="87c50-115">mobileAppRelationship</span></span>](../resources/intune-apps-mobileapprelationship.md)|<span data-ttu-id="87c50-116">读取[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="87c50-116">Read properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="87c50-117">属性</span><span class="sxs-lookup"><span data-stu-id="87c50-117">Properties</span></span>
|<span data-ttu-id="87c50-118">属性</span><span class="sxs-lookup"><span data-stu-id="87c50-118">Property</span></span>|<span data-ttu-id="87c50-119">类型</span><span class="sxs-lookup"><span data-stu-id="87c50-119">Type</span></span>|<span data-ttu-id="87c50-120">说明</span><span class="sxs-lookup"><span data-stu-id="87c50-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87c50-121">id</span><span class="sxs-lookup"><span data-stu-id="87c50-121">id</span></span>|<span data-ttu-id="87c50-122">String</span><span class="sxs-lookup"><span data-stu-id="87c50-122">String</span></span>|<span data-ttu-id="87c50-123">关系实体 id。</span><span class="sxs-lookup"><span data-stu-id="87c50-123">The relationship entity id.</span></span>|
|<span data-ttu-id="87c50-124">targetId</span><span class="sxs-lookup"><span data-stu-id="87c50-124">targetId</span></span>|<span data-ttu-id="87c50-125">String</span><span class="sxs-lookup"><span data-stu-id="87c50-125">String</span></span>|<span data-ttu-id="87c50-126">目标子移动应用程序的应用程序 id。</span><span class="sxs-lookup"><span data-stu-id="87c50-126">The target child mobile app's app id.</span></span>|
|<span data-ttu-id="87c50-127">targetDisplayName</span><span class="sxs-lookup"><span data-stu-id="87c50-127">targetDisplayName</span></span>|<span data-ttu-id="87c50-128">String</span><span class="sxs-lookup"><span data-stu-id="87c50-128">String</span></span>|<span data-ttu-id="87c50-129">目标子移动应用程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="87c50-129">The target child mobile app's display name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="87c50-130">关系</span><span class="sxs-lookup"><span data-stu-id="87c50-130">Relationships</span></span>
<span data-ttu-id="87c50-131">无</span><span class="sxs-lookup"><span data-stu-id="87c50-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="87c50-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="87c50-132">JSON Representation</span></span>
<span data-ttu-id="87c50-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="87c50-133">Here is a JSON representation of the resource.</span></span>
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




