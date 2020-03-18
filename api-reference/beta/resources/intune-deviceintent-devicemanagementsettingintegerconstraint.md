---
title: deviceManagementSettingIntegerConstraint 资源类型
description: 强制整数设置允许的值范围的约束
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bc06c695ff9ad53a44a8218a64c3d6254db76203
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785307"
---
# <a name="devicemanagementsettingintegerconstraint-resource-type"></a><span data-ttu-id="92b65-103">deviceManagementSettingIntegerConstraint 资源类型</span><span class="sxs-lookup"><span data-stu-id="92b65-103">deviceManagementSettingIntegerConstraint resource type</span></span>

> <span data-ttu-id="92b65-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="92b65-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92b65-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="92b65-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92b65-106">强制整数设置允许的值范围的约束</span><span class="sxs-lookup"><span data-stu-id="92b65-106">Constraint enforcing the permitted value range for an integer setting</span></span>


<span data-ttu-id="92b65-107">继承自[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="92b65-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="92b65-108">属性</span><span class="sxs-lookup"><span data-stu-id="92b65-108">Properties</span></span>
|<span data-ttu-id="92b65-109">属性</span><span class="sxs-lookup"><span data-stu-id="92b65-109">Property</span></span>|<span data-ttu-id="92b65-110">类型</span><span class="sxs-lookup"><span data-stu-id="92b65-110">Type</span></span>|<span data-ttu-id="92b65-111">说明</span><span class="sxs-lookup"><span data-stu-id="92b65-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92b65-112">minimumValue</span><span class="sxs-lookup"><span data-stu-id="92b65-112">minimumValue</span></span>|<span data-ttu-id="92b65-113">Int32</span><span class="sxs-lookup"><span data-stu-id="92b65-113">Int32</span></span>|<span data-ttu-id="92b65-114">允许的最小值</span><span class="sxs-lookup"><span data-stu-id="92b65-114">The minimum permitted value</span></span>|
|<span data-ttu-id="92b65-115">maximumValue</span><span class="sxs-lookup"><span data-stu-id="92b65-115">maximumValue</span></span>|<span data-ttu-id="92b65-116">Int32</span><span class="sxs-lookup"><span data-stu-id="92b65-116">Int32</span></span>|<span data-ttu-id="92b65-117">允许的最大值</span><span class="sxs-lookup"><span data-stu-id="92b65-117">The maximum permitted value</span></span>|

## <a name="relationships"></a><span data-ttu-id="92b65-118">关系</span><span class="sxs-lookup"><span data-stu-id="92b65-118">Relationships</span></span>
<span data-ttu-id="92b65-119">无</span><span class="sxs-lookup"><span data-stu-id="92b65-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="92b65-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="92b65-120">JSON Representation</span></span>
<span data-ttu-id="92b65-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="92b65-121">Here is a JSON representation of the resource.</span></span>
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



