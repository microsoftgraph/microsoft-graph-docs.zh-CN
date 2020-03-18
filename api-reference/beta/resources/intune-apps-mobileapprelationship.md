---
title: mobileAppRelationship 资源类型
description: 介绍了如何将子移动应用程序与其父移动应用程序之间的关系。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 98a758d6aee6e916430235d6ca39445292313a54
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797781"
---
# <a name="mobileapprelationship-resource-type"></a><span data-ttu-id="43725-103">mobileAppRelationship 资源类型</span><span class="sxs-lookup"><span data-stu-id="43725-103">mobileAppRelationship resource type</span></span>

> <span data-ttu-id="43725-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="43725-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="43725-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="43725-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43725-106">介绍了如何将子移动应用程序与其父移动应用程序之间的关系。</span><span class="sxs-lookup"><span data-stu-id="43725-106">Describes the relationship for a child mobile app to its parent mobile app.</span></span>

## <a name="methods"></a><span data-ttu-id="43725-107">方法</span><span class="sxs-lookup"><span data-stu-id="43725-107">Methods</span></span>
|<span data-ttu-id="43725-108">方法</span><span class="sxs-lookup"><span data-stu-id="43725-108">Method</span></span>|<span data-ttu-id="43725-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="43725-109">Return Type</span></span>|<span data-ttu-id="43725-110">说明</span><span class="sxs-lookup"><span data-stu-id="43725-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="43725-111">列出 mobileAppRelationships</span><span class="sxs-lookup"><span data-stu-id="43725-111">List mobileAppRelationships</span></span>](../api/intune-apps-mobileapprelationship-list.md)|<span data-ttu-id="43725-112">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)集合</span><span class="sxs-lookup"><span data-stu-id="43725-112">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) collection</span></span>|<span data-ttu-id="43725-113">列出[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="43725-113">List properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) objects.</span></span>|
|[<span data-ttu-id="43725-114">获取 mobileAppRelationship</span><span class="sxs-lookup"><span data-stu-id="43725-114">Get mobileAppRelationship</span></span>](../api/intune-apps-mobileapprelationship-get.md)|[<span data-ttu-id="43725-115">mobileAppRelationship</span><span class="sxs-lookup"><span data-stu-id="43725-115">mobileAppRelationship</span></span>](../resources/intune-apps-mobileapprelationship.md)|<span data-ttu-id="43725-116">读取[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="43725-116">Read properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="43725-117">属性</span><span class="sxs-lookup"><span data-stu-id="43725-117">Properties</span></span>
|<span data-ttu-id="43725-118">属性</span><span class="sxs-lookup"><span data-stu-id="43725-118">Property</span></span>|<span data-ttu-id="43725-119">类型</span><span class="sxs-lookup"><span data-stu-id="43725-119">Type</span></span>|<span data-ttu-id="43725-120">说明</span><span class="sxs-lookup"><span data-stu-id="43725-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43725-121">id</span><span class="sxs-lookup"><span data-stu-id="43725-121">id</span></span>|<span data-ttu-id="43725-122">String</span><span class="sxs-lookup"><span data-stu-id="43725-122">String</span></span>|<span data-ttu-id="43725-123">关系实体 id。</span><span class="sxs-lookup"><span data-stu-id="43725-123">The relationship entity id.</span></span>|
|<span data-ttu-id="43725-124">targetId</span><span class="sxs-lookup"><span data-stu-id="43725-124">targetId</span></span>|<span data-ttu-id="43725-125">String</span><span class="sxs-lookup"><span data-stu-id="43725-125">String</span></span>|<span data-ttu-id="43725-126">目标子移动应用程序的应用程序 id。</span><span class="sxs-lookup"><span data-stu-id="43725-126">The target child mobile app's app id.</span></span>|
|<span data-ttu-id="43725-127">targetDisplayName</span><span class="sxs-lookup"><span data-stu-id="43725-127">targetDisplayName</span></span>|<span data-ttu-id="43725-128">String</span><span class="sxs-lookup"><span data-stu-id="43725-128">String</span></span>|<span data-ttu-id="43725-129">目标子移动应用程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="43725-129">The target child mobile app's display name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="43725-130">关系</span><span class="sxs-lookup"><span data-stu-id="43725-130">Relationships</span></span>
<span data-ttu-id="43725-131">无</span><span class="sxs-lookup"><span data-stu-id="43725-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="43725-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="43725-132">JSON Representation</span></span>
<span data-ttu-id="43725-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="43725-133">Here is a JSON representation of the resource.</span></span>
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



