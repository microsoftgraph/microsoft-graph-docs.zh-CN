---
title: deviceManagementSettingIntegerConstraint 资源类型
description: 强制整数设置允许的值范围的约束
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e5cd1778ca89ad02fa564ed6e57c3e14744635f0
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43453363"
---
# <a name="devicemanagementsettingintegerconstraint-resource-type"></a><span data-ttu-id="bdd89-103">deviceManagementSettingIntegerConstraint 资源类型</span><span class="sxs-lookup"><span data-stu-id="bdd89-103">deviceManagementSettingIntegerConstraint resource type</span></span>

<span data-ttu-id="bdd89-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bdd89-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bdd89-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bdd89-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bdd89-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bdd89-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bdd89-107">强制整数设置允许的值范围的约束</span><span class="sxs-lookup"><span data-stu-id="bdd89-107">Constraint enforcing the permitted value range for an integer setting</span></span>


<span data-ttu-id="bdd89-108">继承自[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="bdd89-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bdd89-109">属性</span><span class="sxs-lookup"><span data-stu-id="bdd89-109">Properties</span></span>
|<span data-ttu-id="bdd89-110">属性</span><span class="sxs-lookup"><span data-stu-id="bdd89-110">Property</span></span>|<span data-ttu-id="bdd89-111">类型</span><span class="sxs-lookup"><span data-stu-id="bdd89-111">Type</span></span>|<span data-ttu-id="bdd89-112">说明</span><span class="sxs-lookup"><span data-stu-id="bdd89-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bdd89-113">minimumValue</span><span class="sxs-lookup"><span data-stu-id="bdd89-113">minimumValue</span></span>|<span data-ttu-id="bdd89-114">Int32</span><span class="sxs-lookup"><span data-stu-id="bdd89-114">Int32</span></span>|<span data-ttu-id="bdd89-115">允许的最小值</span><span class="sxs-lookup"><span data-stu-id="bdd89-115">The minimum permitted value</span></span>|
|<span data-ttu-id="bdd89-116">maximumValue</span><span class="sxs-lookup"><span data-stu-id="bdd89-116">maximumValue</span></span>|<span data-ttu-id="bdd89-117">Int32</span><span class="sxs-lookup"><span data-stu-id="bdd89-117">Int32</span></span>|<span data-ttu-id="bdd89-118">允许的最大值</span><span class="sxs-lookup"><span data-stu-id="bdd89-118">The maximum permitted value</span></span>|

## <a name="relationships"></a><span data-ttu-id="bdd89-119">关系</span><span class="sxs-lookup"><span data-stu-id="bdd89-119">Relationships</span></span>
<span data-ttu-id="bdd89-120">无</span><span class="sxs-lookup"><span data-stu-id="bdd89-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bdd89-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bdd89-121">JSON Representation</span></span>
<span data-ttu-id="bdd89-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bdd89-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingIntegerConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingIntegerConstraint",
  "minimumValue": 1024,
  "maximumValue": 1024
}
```



