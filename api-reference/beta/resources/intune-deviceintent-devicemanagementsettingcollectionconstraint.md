---
title: deviceManagementSettingCollectionConstraint 资源类型
description: 强制实施集合中最大元素数的约束
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a6bd64e29e01858ce6f1b09ef822e2a3621d5720
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48061264"
---
# <a name="devicemanagementsettingcollectionconstraint-resource-type"></a><span data-ttu-id="5a8d7-103">deviceManagementSettingCollectionConstraint 资源类型</span><span class="sxs-lookup"><span data-stu-id="5a8d7-103">deviceManagementSettingCollectionConstraint resource type</span></span>

<span data-ttu-id="5a8d7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a8d7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5a8d7-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5a8d7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5a8d7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5a8d7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a8d7-107">强制实施集合中最大元素数的约束</span><span class="sxs-lookup"><span data-stu-id="5a8d7-107">Constraint that enforces the maximum number of elements a collection</span></span>


<span data-ttu-id="5a8d7-108">继承自 [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="5a8d7-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5a8d7-109">属性</span><span class="sxs-lookup"><span data-stu-id="5a8d7-109">Properties</span></span>
|<span data-ttu-id="5a8d7-110">属性</span><span class="sxs-lookup"><span data-stu-id="5a8d7-110">Property</span></span>|<span data-ttu-id="5a8d7-111">类型</span><span class="sxs-lookup"><span data-stu-id="5a8d7-111">Type</span></span>|<span data-ttu-id="5a8d7-112">说明</span><span class="sxs-lookup"><span data-stu-id="5a8d7-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a8d7-113">Minimumheight</span><span class="sxs-lookup"><span data-stu-id="5a8d7-113">minimumLength</span></span>|<span data-ttu-id="5a8d7-114">Int32</span><span class="sxs-lookup"><span data-stu-id="5a8d7-114">Int32</span></span>|<span data-ttu-id="5a8d7-115">集合中元素的最小数目</span><span class="sxs-lookup"><span data-stu-id="5a8d7-115">The minimum number of elements in the collection</span></span>|
|<span data-ttu-id="5a8d7-116">maximumLength</span><span class="sxs-lookup"><span data-stu-id="5a8d7-116">maximumLength</span></span>|<span data-ttu-id="5a8d7-117">Int32</span><span class="sxs-lookup"><span data-stu-id="5a8d7-117">Int32</span></span>|<span data-ttu-id="5a8d7-118">集合中元素的最大数目</span><span class="sxs-lookup"><span data-stu-id="5a8d7-118">The maximum number of elements in the collection</span></span>|

## <a name="relationships"></a><span data-ttu-id="5a8d7-119">关系</span><span class="sxs-lookup"><span data-stu-id="5a8d7-119">Relationships</span></span>
<span data-ttu-id="5a8d7-120">无</span><span class="sxs-lookup"><span data-stu-id="5a8d7-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5a8d7-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5a8d7-121">JSON Representation</span></span>
<span data-ttu-id="5a8d7-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5a8d7-122">Here is a JSON representation of the resource.</span></span>
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






