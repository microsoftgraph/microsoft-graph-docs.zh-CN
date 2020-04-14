---
title: deviceManagementSettingCollectionConstraint 资源类型
description: 强制实施集合中最大元素数的约束
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: dc3b3d9a8c03c323f142186baab01e34a71ce4aa
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43443273"
---
# <a name="devicemanagementsettingcollectionconstraint-resource-type"></a><span data-ttu-id="f8994-103">deviceManagementSettingCollectionConstraint 资源类型</span><span class="sxs-lookup"><span data-stu-id="f8994-103">deviceManagementSettingCollectionConstraint resource type</span></span>

<span data-ttu-id="f8994-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8994-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f8994-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f8994-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f8994-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f8994-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8994-107">强制实施集合中最大元素数的约束</span><span class="sxs-lookup"><span data-stu-id="f8994-107">Constraint that enforces the maximum number of elements a collection</span></span>


<span data-ttu-id="f8994-108">继承自[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="f8994-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f8994-109">属性</span><span class="sxs-lookup"><span data-stu-id="f8994-109">Properties</span></span>
|<span data-ttu-id="f8994-110">属性</span><span class="sxs-lookup"><span data-stu-id="f8994-110">Property</span></span>|<span data-ttu-id="f8994-111">类型</span><span class="sxs-lookup"><span data-stu-id="f8994-111">Type</span></span>|<span data-ttu-id="f8994-112">说明</span><span class="sxs-lookup"><span data-stu-id="f8994-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8994-113">Minimumheight</span><span class="sxs-lookup"><span data-stu-id="f8994-113">minimumLength</span></span>|<span data-ttu-id="f8994-114">Int32</span><span class="sxs-lookup"><span data-stu-id="f8994-114">Int32</span></span>|<span data-ttu-id="f8994-115">集合中元素的最小数目</span><span class="sxs-lookup"><span data-stu-id="f8994-115">The minimum number of elements in the collection</span></span>|
|<span data-ttu-id="f8994-116">maximumLength</span><span class="sxs-lookup"><span data-stu-id="f8994-116">maximumLength</span></span>|<span data-ttu-id="f8994-117">Int32</span><span class="sxs-lookup"><span data-stu-id="f8994-117">Int32</span></span>|<span data-ttu-id="f8994-118">集合中元素的最大数目</span><span class="sxs-lookup"><span data-stu-id="f8994-118">The maximum number of elements in the collection</span></span>|

## <a name="relationships"></a><span data-ttu-id="f8994-119">关系</span><span class="sxs-lookup"><span data-stu-id="f8994-119">Relationships</span></span>
<span data-ttu-id="f8994-120">无</span><span class="sxs-lookup"><span data-stu-id="f8994-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f8994-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f8994-121">JSON Representation</span></span>
<span data-ttu-id="f8994-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f8994-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingCollectionConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingCollectionConstraint",
  "minimumLength": 1024,
  "maximumLength": 1024
}
```



