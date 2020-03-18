---
title: deviceManagementSettingCollectionConstraint 资源类型
description: 强制实施集合中最大元素数的约束
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 180d199997f288945ba9be282ebd7c2bdbee31ec
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785356"
---
# <a name="devicemanagementsettingcollectionconstraint-resource-type"></a><span data-ttu-id="53e30-103">deviceManagementSettingCollectionConstraint 资源类型</span><span class="sxs-lookup"><span data-stu-id="53e30-103">deviceManagementSettingCollectionConstraint resource type</span></span>

> <span data-ttu-id="53e30-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="53e30-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="53e30-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="53e30-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53e30-106">强制实施集合中最大元素数的约束</span><span class="sxs-lookup"><span data-stu-id="53e30-106">Constraint that enforces the maximum number of elements a collection</span></span>


<span data-ttu-id="53e30-107">继承自[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="53e30-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="53e30-108">属性</span><span class="sxs-lookup"><span data-stu-id="53e30-108">Properties</span></span>
|<span data-ttu-id="53e30-109">属性</span><span class="sxs-lookup"><span data-stu-id="53e30-109">Property</span></span>|<span data-ttu-id="53e30-110">类型</span><span class="sxs-lookup"><span data-stu-id="53e30-110">Type</span></span>|<span data-ttu-id="53e30-111">说明</span><span class="sxs-lookup"><span data-stu-id="53e30-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53e30-112">Minimumheight</span><span class="sxs-lookup"><span data-stu-id="53e30-112">minimumLength</span></span>|<span data-ttu-id="53e30-113">Int32</span><span class="sxs-lookup"><span data-stu-id="53e30-113">Int32</span></span>|<span data-ttu-id="53e30-114">集合中元素的最小数目</span><span class="sxs-lookup"><span data-stu-id="53e30-114">The minimum number of elements in the collection</span></span>|
|<span data-ttu-id="53e30-115">maximumLength</span><span class="sxs-lookup"><span data-stu-id="53e30-115">maximumLength</span></span>|<span data-ttu-id="53e30-116">Int32</span><span class="sxs-lookup"><span data-stu-id="53e30-116">Int32</span></span>|<span data-ttu-id="53e30-117">集合中元素的最大数目</span><span class="sxs-lookup"><span data-stu-id="53e30-117">The maximum number of elements in the collection</span></span>|

## <a name="relationships"></a><span data-ttu-id="53e30-118">关系</span><span class="sxs-lookup"><span data-stu-id="53e30-118">Relationships</span></span>
<span data-ttu-id="53e30-119">无</span><span class="sxs-lookup"><span data-stu-id="53e30-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="53e30-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="53e30-120">JSON Representation</span></span>
<span data-ttu-id="53e30-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="53e30-121">Here is a JSON representation of the resource.</span></span>
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



