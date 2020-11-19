---
title: deviceManagementSettingBooleanConstraint 资源类型
description: 约束强制实施特定的布尔值
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2a50b5a4c8f51b7b9a4bc548245f9bd24d36f383
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49275564"
---
# <a name="devicemanagementsettingbooleanconstraint-resource-type"></a><span data-ttu-id="42d2d-103">deviceManagementSettingBooleanConstraint 资源类型</span><span class="sxs-lookup"><span data-stu-id="42d2d-103">deviceManagementSettingBooleanConstraint resource type</span></span>

<span data-ttu-id="42d2d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42d2d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="42d2d-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="42d2d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42d2d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="42d2d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42d2d-107">约束强制实施特定的布尔值</span><span class="sxs-lookup"><span data-stu-id="42d2d-107">Constraint the enforces a particular boolean value</span></span>


<span data-ttu-id="42d2d-108">继承自 [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="42d2d-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="42d2d-109">属性</span><span class="sxs-lookup"><span data-stu-id="42d2d-109">Properties</span></span>
|<span data-ttu-id="42d2d-110">属性</span><span class="sxs-lookup"><span data-stu-id="42d2d-110">Property</span></span>|<span data-ttu-id="42d2d-111">类型</span><span class="sxs-lookup"><span data-stu-id="42d2d-111">Type</span></span>|<span data-ttu-id="42d2d-112">说明</span><span class="sxs-lookup"><span data-stu-id="42d2d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42d2d-113">值</span><span class="sxs-lookup"><span data-stu-id="42d2d-113">value</span></span>|<span data-ttu-id="42d2d-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="42d2d-114">Boolean</span></span>|<span data-ttu-id="42d2d-115">要与之比较的布尔值</span><span class="sxs-lookup"><span data-stu-id="42d2d-115">The boolean value to compare against</span></span>|

## <a name="relationships"></a><span data-ttu-id="42d2d-116">关系</span><span class="sxs-lookup"><span data-stu-id="42d2d-116">Relationships</span></span>
<span data-ttu-id="42d2d-117">无</span><span class="sxs-lookup"><span data-stu-id="42d2d-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="42d2d-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="42d2d-118">JSON Representation</span></span>
<span data-ttu-id="42d2d-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="42d2d-119">Here is a JSON representation of the resource.</span></span>
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




