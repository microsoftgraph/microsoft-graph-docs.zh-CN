---
title: deviceManagementSettingBooleanConstraint 资源类型
description: 约束强制实施特定的布尔值
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8c39fbb19439572b1e698b3c5db3bcf0bf6c8ea5
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2019
ms.locfileid: "31523691"
---
# <a name="devicemanagementsettingbooleanconstraint-resource-type"></a><span data-ttu-id="3c23a-103">deviceManagementSettingBooleanConstraint 资源类型</span><span class="sxs-lookup"><span data-stu-id="3c23a-103">deviceManagementSettingBooleanConstraint resource type</span></span>

> <span data-ttu-id="3c23a-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3c23a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c23a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3c23a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c23a-106">约束强制实施特定的布尔值</span><span class="sxs-lookup"><span data-stu-id="3c23a-106">Constraint the enforces a particular boolean value</span></span>


<span data-ttu-id="3c23a-107">继承自[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="3c23a-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3c23a-108">属性</span><span class="sxs-lookup"><span data-stu-id="3c23a-108">Properties</span></span>
|<span data-ttu-id="3c23a-109">属性</span><span class="sxs-lookup"><span data-stu-id="3c23a-109">Property</span></span>|<span data-ttu-id="3c23a-110">类型</span><span class="sxs-lookup"><span data-stu-id="3c23a-110">Type</span></span>|<span data-ttu-id="3c23a-111">说明</span><span class="sxs-lookup"><span data-stu-id="3c23a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c23a-112">value</span><span class="sxs-lookup"><span data-stu-id="3c23a-112">value</span></span>|<span data-ttu-id="3c23a-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="3c23a-113">Boolean</span></span>|<span data-ttu-id="3c23a-114">要与之比较的布尔值</span><span class="sxs-lookup"><span data-stu-id="3c23a-114">The boolean value to compare against</span></span>|

## <a name="relationships"></a><span data-ttu-id="3c23a-115">关系</span><span class="sxs-lookup"><span data-stu-id="3c23a-115">Relationships</span></span>
<span data-ttu-id="3c23a-116">无</span><span class="sxs-lookup"><span data-stu-id="3c23a-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3c23a-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3c23a-117">JSON Representation</span></span>
<span data-ttu-id="3c23a-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3c23a-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingBooleanConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingBooleanConstraint",
  "value": true
}
```







