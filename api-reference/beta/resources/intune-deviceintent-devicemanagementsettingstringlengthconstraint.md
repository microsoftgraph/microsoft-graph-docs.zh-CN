---
title: deviceManagementSettingStringLengthConstraint 资源类型
description: 强制实施给定字符串长度范围的约束
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 308bb7b723e9d8ac47bca72f342adb3f2a987ea5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48061124"
---
# <a name="devicemanagementsettingstringlengthconstraint-resource-type"></a><span data-ttu-id="5294f-103">deviceManagementSettingStringLengthConstraint 资源类型</span><span class="sxs-lookup"><span data-stu-id="5294f-103">deviceManagementSettingStringLengthConstraint resource type</span></span>

<span data-ttu-id="5294f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5294f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5294f-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5294f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5294f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5294f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5294f-107">强制实施给定字符串长度范围的约束</span><span class="sxs-lookup"><span data-stu-id="5294f-107">Constraint enforcing a given string length range</span></span>


<span data-ttu-id="5294f-108">继承自 [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="5294f-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5294f-109">属性</span><span class="sxs-lookup"><span data-stu-id="5294f-109">Properties</span></span>
|<span data-ttu-id="5294f-110">属性</span><span class="sxs-lookup"><span data-stu-id="5294f-110">Property</span></span>|<span data-ttu-id="5294f-111">类型</span><span class="sxs-lookup"><span data-stu-id="5294f-111">Type</span></span>|<span data-ttu-id="5294f-112">说明</span><span class="sxs-lookup"><span data-stu-id="5294f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5294f-113">Minimumheight</span><span class="sxs-lookup"><span data-stu-id="5294f-113">minimumLength</span></span>|<span data-ttu-id="5294f-114">Int32</span><span class="sxs-lookup"><span data-stu-id="5294f-114">Int32</span></span>|<span data-ttu-id="5294f-115">允许的最小字符串长度</span><span class="sxs-lookup"><span data-stu-id="5294f-115">The minimum permitted string length</span></span>|
|<span data-ttu-id="5294f-116">maximumLength</span><span class="sxs-lookup"><span data-stu-id="5294f-116">maximumLength</span></span>|<span data-ttu-id="5294f-117">Int32</span><span class="sxs-lookup"><span data-stu-id="5294f-117">Int32</span></span>|<span data-ttu-id="5294f-118">允许的最大字符串长度</span><span class="sxs-lookup"><span data-stu-id="5294f-118">The maximum permitted string length</span></span>|

## <a name="relationships"></a><span data-ttu-id="5294f-119">关系</span><span class="sxs-lookup"><span data-stu-id="5294f-119">Relationships</span></span>
<span data-ttu-id="5294f-120">无</span><span class="sxs-lookup"><span data-stu-id="5294f-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5294f-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5294f-121">JSON Representation</span></span>
<span data-ttu-id="5294f-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5294f-122">Here is a JSON representation of the resource.</span></span>
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






