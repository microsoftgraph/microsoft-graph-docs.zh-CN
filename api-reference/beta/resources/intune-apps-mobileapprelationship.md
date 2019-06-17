---
title: mobileAppRelationship 资源类型
description: 介绍了如何将子移动应用程序与其父移动应用程序之间的关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e193878122a3a43cd97d05ad1bdc5bea302fcc8a
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34991819"
---
# <a name="mobileapprelationship-resource-type"></a><span data-ttu-id="e4b48-103">mobileAppRelationship 资源类型</span><span class="sxs-lookup"><span data-stu-id="e4b48-103">mobileAppRelationship resource type</span></span>

> <span data-ttu-id="e4b48-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e4b48-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e4b48-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e4b48-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4b48-106">介绍了如何将子移动应用程序与其父移动应用程序之间的关系。</span><span class="sxs-lookup"><span data-stu-id="e4b48-106">Describes the relationship for a child mobile app to its parent mobile app.</span></span>

## <a name="methods"></a><span data-ttu-id="e4b48-107">方法</span><span class="sxs-lookup"><span data-stu-id="e4b48-107">Methods</span></span>
|<span data-ttu-id="e4b48-108">方法</span><span class="sxs-lookup"><span data-stu-id="e4b48-108">Method</span></span>|<span data-ttu-id="e4b48-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="e4b48-109">Return Type</span></span>|<span data-ttu-id="e4b48-110">说明</span><span class="sxs-lookup"><span data-stu-id="e4b48-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e4b48-111">列出 mobileAppRelationships</span><span class="sxs-lookup"><span data-stu-id="e4b48-111">List mobileAppRelationships</span></span>](../api/intune-apps-mobileapprelationship-list.md)|<span data-ttu-id="e4b48-112">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)集合</span><span class="sxs-lookup"><span data-stu-id="e4b48-112">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) collection</span></span>|<span data-ttu-id="e4b48-113">列出[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e4b48-113">List properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) objects.</span></span>|
|[<span data-ttu-id="e4b48-114">获取 mobileAppRelationship</span><span class="sxs-lookup"><span data-stu-id="e4b48-114">Get mobileAppRelationship</span></span>](../api/intune-apps-mobileapprelationship-get.md)|[<span data-ttu-id="e4b48-115">mobileAppRelationship</span><span class="sxs-lookup"><span data-stu-id="e4b48-115">mobileAppRelationship</span></span>](../resources/intune-apps-mobileapprelationship.md)|<span data-ttu-id="e4b48-116">读取[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e4b48-116">Read properties and relationships of the [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e4b48-117">属性</span><span class="sxs-lookup"><span data-stu-id="e4b48-117">Properties</span></span>
|<span data-ttu-id="e4b48-118">属性</span><span class="sxs-lookup"><span data-stu-id="e4b48-118">Property</span></span>|<span data-ttu-id="e4b48-119">类型</span><span class="sxs-lookup"><span data-stu-id="e4b48-119">Type</span></span>|<span data-ttu-id="e4b48-120">说明</span><span class="sxs-lookup"><span data-stu-id="e4b48-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4b48-121">id</span><span class="sxs-lookup"><span data-stu-id="e4b48-121">id</span></span>|<span data-ttu-id="e4b48-122">String</span><span class="sxs-lookup"><span data-stu-id="e4b48-122">String</span></span>|<span data-ttu-id="e4b48-123">关系实体 id。</span><span class="sxs-lookup"><span data-stu-id="e4b48-123">The relationship entity id.</span></span>|
|<span data-ttu-id="e4b48-124">targetId</span><span class="sxs-lookup"><span data-stu-id="e4b48-124">targetId</span></span>|<span data-ttu-id="e4b48-125">String</span><span class="sxs-lookup"><span data-stu-id="e4b48-125">String</span></span>|<span data-ttu-id="e4b48-126">目标子移动应用程序的应用程序 id。</span><span class="sxs-lookup"><span data-stu-id="e4b48-126">The target child mobile app's app id.</span></span>|
|<span data-ttu-id="e4b48-127">targetDisplayName</span><span class="sxs-lookup"><span data-stu-id="e4b48-127">targetDisplayName</span></span>|<span data-ttu-id="e4b48-128">String</span><span class="sxs-lookup"><span data-stu-id="e4b48-128">String</span></span>|<span data-ttu-id="e4b48-129">目标子移动应用程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="e4b48-129">The target child mobile app's display name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e4b48-130">关系</span><span class="sxs-lookup"><span data-stu-id="e4b48-130">Relationships</span></span>
<span data-ttu-id="e4b48-131">无</span><span class="sxs-lookup"><span data-stu-id="e4b48-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e4b48-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e4b48-132">JSON Representation</span></span>
<span data-ttu-id="e4b48-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e4b48-133">Here is a JSON representation of the resource.</span></span>
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





