---
title: deviceManagementSettingStringLengthConstraint 资源类型
description: 强制实施给定字符串长度范围的约束
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d7cdcdeb138dce2c5b201527a079e3ee2de03737
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34984462"
---
# <a name="devicemanagementsettingstringlengthconstraint-resource-type"></a><span data-ttu-id="b0fdf-103">deviceManagementSettingStringLengthConstraint 资源类型</span><span class="sxs-lookup"><span data-stu-id="b0fdf-103">deviceManagementSettingStringLengthConstraint resource type</span></span>

> <span data-ttu-id="b0fdf-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b0fdf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0fdf-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b0fdf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0fdf-106">强制实施给定字符串长度范围的约束</span><span class="sxs-lookup"><span data-stu-id="b0fdf-106">Constraint enforcing a given string length range</span></span>


<span data-ttu-id="b0fdf-107">继承自[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="b0fdf-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b0fdf-108">属性</span><span class="sxs-lookup"><span data-stu-id="b0fdf-108">Properties</span></span>
|<span data-ttu-id="b0fdf-109">属性</span><span class="sxs-lookup"><span data-stu-id="b0fdf-109">Property</span></span>|<span data-ttu-id="b0fdf-110">类型</span><span class="sxs-lookup"><span data-stu-id="b0fdf-110">Type</span></span>|<span data-ttu-id="b0fdf-111">说明</span><span class="sxs-lookup"><span data-stu-id="b0fdf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0fdf-112">Minimumheight</span><span class="sxs-lookup"><span data-stu-id="b0fdf-112">minimumLength</span></span>|<span data-ttu-id="b0fdf-113">Int32</span><span class="sxs-lookup"><span data-stu-id="b0fdf-113">Int32</span></span>|<span data-ttu-id="b0fdf-114">允许的最小字符串长度</span><span class="sxs-lookup"><span data-stu-id="b0fdf-114">The minimum permitted string length</span></span>|
|<span data-ttu-id="b0fdf-115">maximumLength</span><span class="sxs-lookup"><span data-stu-id="b0fdf-115">maximumLength</span></span>|<span data-ttu-id="b0fdf-116">Int32</span><span class="sxs-lookup"><span data-stu-id="b0fdf-116">Int32</span></span>|<span data-ttu-id="b0fdf-117">允许的最大字符串长度</span><span class="sxs-lookup"><span data-stu-id="b0fdf-117">The maximum permitted string length</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0fdf-118">关系</span><span class="sxs-lookup"><span data-stu-id="b0fdf-118">Relationships</span></span>
<span data-ttu-id="b0fdf-119">无</span><span class="sxs-lookup"><span data-stu-id="b0fdf-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b0fdf-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b0fdf-120">JSON Representation</span></span>
<span data-ttu-id="b0fdf-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b0fdf-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingStringLengthConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingStringLengthConstraint",
  "minimumLength": 1024,
  "maximumLength": 1024
}
```





