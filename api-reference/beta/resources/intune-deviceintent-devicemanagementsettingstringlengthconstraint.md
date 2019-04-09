---
title: deviceManagementSettingStringLengthConstraint 资源类型
description: 强制实施给定字符串长度范围的约束
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 49d009571cdccf60dc8adcc2f1a703d39d0674c7
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522333"
---
# <a name="devicemanagementsettingstringlengthconstraint-resource-type"></a><span data-ttu-id="6ff9b-103">deviceManagementSettingStringLengthConstraint 资源类型</span><span class="sxs-lookup"><span data-stu-id="6ff9b-103">deviceManagementSettingStringLengthConstraint resource type</span></span>

> <span data-ttu-id="6ff9b-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6ff9b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ff9b-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6ff9b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ff9b-106">强制实施给定字符串长度范围的约束</span><span class="sxs-lookup"><span data-stu-id="6ff9b-106">Constraint enforcing a given string length range</span></span>


<span data-ttu-id="6ff9b-107">继承自[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="6ff9b-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6ff9b-108">属性</span><span class="sxs-lookup"><span data-stu-id="6ff9b-108">Properties</span></span>
|<span data-ttu-id="6ff9b-109">属性</span><span class="sxs-lookup"><span data-stu-id="6ff9b-109">Property</span></span>|<span data-ttu-id="6ff9b-110">类型</span><span class="sxs-lookup"><span data-stu-id="6ff9b-110">Type</span></span>|<span data-ttu-id="6ff9b-111">说明</span><span class="sxs-lookup"><span data-stu-id="6ff9b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ff9b-112">minimumheight</span><span class="sxs-lookup"><span data-stu-id="6ff9b-112">minimumLength</span></span>|<span data-ttu-id="6ff9b-113">Int32</span><span class="sxs-lookup"><span data-stu-id="6ff9b-113">Int32</span></span>|<span data-ttu-id="6ff9b-114">允许的最小字符串长度</span><span class="sxs-lookup"><span data-stu-id="6ff9b-114">The minimum permitted string length</span></span>|
|<span data-ttu-id="6ff9b-115">maximumLength</span><span class="sxs-lookup"><span data-stu-id="6ff9b-115">maximumLength</span></span>|<span data-ttu-id="6ff9b-116">Int32</span><span class="sxs-lookup"><span data-stu-id="6ff9b-116">Int32</span></span>|<span data-ttu-id="6ff9b-117">允许的最大字符串长度</span><span class="sxs-lookup"><span data-stu-id="6ff9b-117">The maximum permitted string length</span></span>|

## <a name="relationships"></a><span data-ttu-id="6ff9b-118">关系</span><span class="sxs-lookup"><span data-stu-id="6ff9b-118">Relationships</span></span>
<span data-ttu-id="6ff9b-119">无</span><span class="sxs-lookup"><span data-stu-id="6ff9b-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6ff9b-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6ff9b-120">JSON Representation</span></span>
<span data-ttu-id="6ff9b-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6ff9b-121">Here is a JSON representation of the resource.</span></span>
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







