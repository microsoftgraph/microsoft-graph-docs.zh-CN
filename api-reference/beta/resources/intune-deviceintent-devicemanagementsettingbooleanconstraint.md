---
title: deviceManagementSettingBooleanConstraint 资源类型
description: 约束强制实施特定的布尔值
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ee2689bfbc6b407a688c0422c568d4b311694c06
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562284"
---
# <a name="devicemanagementsettingbooleanconstraint-resource-type"></a><span data-ttu-id="542ce-103">deviceManagementSettingBooleanConstraint 资源类型</span><span class="sxs-lookup"><span data-stu-id="542ce-103">deviceManagementSettingBooleanConstraint resource type</span></span>

> <span data-ttu-id="542ce-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="542ce-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="542ce-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="542ce-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="542ce-106">约束强制实施特定的布尔值</span><span class="sxs-lookup"><span data-stu-id="542ce-106">Constraint the enforces a particular boolean value</span></span>


<span data-ttu-id="542ce-107">继承自[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="542ce-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="542ce-108">属性</span><span class="sxs-lookup"><span data-stu-id="542ce-108">Properties</span></span>
|<span data-ttu-id="542ce-109">属性</span><span class="sxs-lookup"><span data-stu-id="542ce-109">Property</span></span>|<span data-ttu-id="542ce-110">类型</span><span class="sxs-lookup"><span data-stu-id="542ce-110">Type</span></span>|<span data-ttu-id="542ce-111">说明</span><span class="sxs-lookup"><span data-stu-id="542ce-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="542ce-112">值</span><span class="sxs-lookup"><span data-stu-id="542ce-112">value</span></span>|<span data-ttu-id="542ce-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="542ce-113">Boolean</span></span>|<span data-ttu-id="542ce-114">要与之比较的布尔值</span><span class="sxs-lookup"><span data-stu-id="542ce-114">The boolean value to compare against</span></span>|

## <a name="relationships"></a><span data-ttu-id="542ce-115">关系</span><span class="sxs-lookup"><span data-stu-id="542ce-115">Relationships</span></span>
<span data-ttu-id="542ce-116">无</span><span class="sxs-lookup"><span data-stu-id="542ce-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="542ce-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="542ce-117">JSON Representation</span></span>
<span data-ttu-id="542ce-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="542ce-118">Here is a JSON representation of the resource.</span></span>
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





