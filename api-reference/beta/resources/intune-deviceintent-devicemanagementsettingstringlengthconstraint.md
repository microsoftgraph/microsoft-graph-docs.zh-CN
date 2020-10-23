---
title: deviceManagementSettingStringLengthConstraint 资源类型
description: 强制实施给定字符串长度范围的约束
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0ce9e4657d51c42861e34a8eb5548846af91432a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48730425"
---
# <a name="devicemanagementsettingstringlengthconstraint-resource-type"></a><span data-ttu-id="0f9c8-103">deviceManagementSettingStringLengthConstraint 资源类型</span><span class="sxs-lookup"><span data-stu-id="0f9c8-103">deviceManagementSettingStringLengthConstraint resource type</span></span>

<span data-ttu-id="0f9c8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f9c8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0f9c8-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0f9c8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0f9c8-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0f9c8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f9c8-107">强制实施给定字符串长度范围的约束</span><span class="sxs-lookup"><span data-stu-id="0f9c8-107">Constraint enforcing a given string length range</span></span>


<span data-ttu-id="0f9c8-108">继承自 [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="0f9c8-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0f9c8-109">属性</span><span class="sxs-lookup"><span data-stu-id="0f9c8-109">Properties</span></span>
|<span data-ttu-id="0f9c8-110">属性</span><span class="sxs-lookup"><span data-stu-id="0f9c8-110">Property</span></span>|<span data-ttu-id="0f9c8-111">类型</span><span class="sxs-lookup"><span data-stu-id="0f9c8-111">Type</span></span>|<span data-ttu-id="0f9c8-112">说明</span><span class="sxs-lookup"><span data-stu-id="0f9c8-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f9c8-113">Minimumheight</span><span class="sxs-lookup"><span data-stu-id="0f9c8-113">minimumLength</span></span>|<span data-ttu-id="0f9c8-114">Int32</span><span class="sxs-lookup"><span data-stu-id="0f9c8-114">Int32</span></span>|<span data-ttu-id="0f9c8-115">允许的最小字符串长度</span><span class="sxs-lookup"><span data-stu-id="0f9c8-115">The minimum permitted string length</span></span>|
|<span data-ttu-id="0f9c8-116">maximumLength</span><span class="sxs-lookup"><span data-stu-id="0f9c8-116">maximumLength</span></span>|<span data-ttu-id="0f9c8-117">Int32</span><span class="sxs-lookup"><span data-stu-id="0f9c8-117">Int32</span></span>|<span data-ttu-id="0f9c8-118">允许的最大字符串长度</span><span class="sxs-lookup"><span data-stu-id="0f9c8-118">The maximum permitted string length</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f9c8-119">关系</span><span class="sxs-lookup"><span data-stu-id="0f9c8-119">Relationships</span></span>
<span data-ttu-id="0f9c8-120">无</span><span class="sxs-lookup"><span data-stu-id="0f9c8-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0f9c8-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0f9c8-121">JSON Representation</span></span>
<span data-ttu-id="0f9c8-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0f9c8-122">Here is a JSON representation of the resource.</span></span>
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





