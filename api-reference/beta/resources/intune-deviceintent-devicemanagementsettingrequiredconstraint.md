---
title: deviceManagementSettingRequiredConstraint 资源类型
description: 强制实施特定的必需设置（非 null/未定义/空字符串/未配置）的约束
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5b2df645780cdd7d06847d3acb18766027bf4ad8
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636600"
---
# <a name="devicemanagementsettingrequiredconstraint-resource-type"></a><span data-ttu-id="e583d-103">deviceManagementSettingRequiredConstraint 资源类型</span><span class="sxs-lookup"><span data-stu-id="e583d-103">deviceManagementSettingRequiredConstraint resource type</span></span>

> <span data-ttu-id="e583d-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e583d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e583d-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e583d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e583d-106">强制实施特定的必需设置（非 null/未定义/空字符串/未配置）的约束</span><span class="sxs-lookup"><span data-stu-id="e583d-106">Constraint that enforces a particular required setting that is not null/undefined/empty string/not configured</span></span>


<span data-ttu-id="e583d-107">继承自[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="e583d-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e583d-108">属性</span><span class="sxs-lookup"><span data-stu-id="e583d-108">Properties</span></span>
|<span data-ttu-id="e583d-109">属性</span><span class="sxs-lookup"><span data-stu-id="e583d-109">Property</span></span>|<span data-ttu-id="e583d-110">类型</span><span class="sxs-lookup"><span data-stu-id="e583d-110">Type</span></span>|<span data-ttu-id="e583d-111">Description</span><span class="sxs-lookup"><span data-stu-id="e583d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e583d-112">notConfiguredValue</span><span class="sxs-lookup"><span data-stu-id="e583d-112">notConfiguredValue</span></span>|<span data-ttu-id="e583d-113">字符串</span><span class="sxs-lookup"><span data-stu-id="e583d-113">String</span></span>|<span data-ttu-id="e583d-114">值的列表，表示未配置设置</span><span class="sxs-lookup"><span data-stu-id="e583d-114">List of value which means not configured for the setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="e583d-115">关系</span><span class="sxs-lookup"><span data-stu-id="e583d-115">Relationships</span></span>
<span data-ttu-id="e583d-116">无</span><span class="sxs-lookup"><span data-stu-id="e583d-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e583d-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e583d-117">JSON Representation</span></span>
<span data-ttu-id="e583d-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e583d-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingRequiredConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingRequiredConstraint",
  "notConfiguredValue": "String"
}
```



