---
title: deviceManagementSettingIntegerConstraint 资源类型
description: 强制整数设置允许的值范围的约束
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7f67e3507d58e2208c7f0022724516f1646ad0fd
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2019
ms.locfileid: "31523635"
---
# <a name="devicemanagementsettingintegerconstraint-resource-type"></a><span data-ttu-id="9ef1a-103">deviceManagementSettingIntegerConstraint 资源类型</span><span class="sxs-lookup"><span data-stu-id="9ef1a-103">deviceManagementSettingIntegerConstraint resource type</span></span>

> <span data-ttu-id="9ef1a-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9ef1a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9ef1a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9ef1a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ef1a-106">强制整数设置允许的值范围的约束</span><span class="sxs-lookup"><span data-stu-id="9ef1a-106">Constraint enforcing the permitted value range for an integer setting</span></span>


<span data-ttu-id="9ef1a-107">继承自[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="9ef1a-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9ef1a-108">属性</span><span class="sxs-lookup"><span data-stu-id="9ef1a-108">Properties</span></span>
|<span data-ttu-id="9ef1a-109">属性</span><span class="sxs-lookup"><span data-stu-id="9ef1a-109">Property</span></span>|<span data-ttu-id="9ef1a-110">类型</span><span class="sxs-lookup"><span data-stu-id="9ef1a-110">Type</span></span>|<span data-ttu-id="9ef1a-111">说明</span><span class="sxs-lookup"><span data-stu-id="9ef1a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ef1a-112">minimumValue</span><span class="sxs-lookup"><span data-stu-id="9ef1a-112">minimumValue</span></span>|<span data-ttu-id="9ef1a-113">Int32</span><span class="sxs-lookup"><span data-stu-id="9ef1a-113">Int32</span></span>|<span data-ttu-id="9ef1a-114">允许的最小值</span><span class="sxs-lookup"><span data-stu-id="9ef1a-114">The minimum permitted value</span></span>|
|<span data-ttu-id="9ef1a-115">maximumValue</span><span class="sxs-lookup"><span data-stu-id="9ef1a-115">maximumValue</span></span>|<span data-ttu-id="9ef1a-116">Int32</span><span class="sxs-lookup"><span data-stu-id="9ef1a-116">Int32</span></span>|<span data-ttu-id="9ef1a-117">允许的最大值</span><span class="sxs-lookup"><span data-stu-id="9ef1a-117">The maximum permitted value</span></span>|

## <a name="relationships"></a><span data-ttu-id="9ef1a-118">关系</span><span class="sxs-lookup"><span data-stu-id="9ef1a-118">Relationships</span></span>
<span data-ttu-id="9ef1a-119">无</span><span class="sxs-lookup"><span data-stu-id="9ef1a-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9ef1a-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9ef1a-120">JSON Representation</span></span>
<span data-ttu-id="9ef1a-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9ef1a-121">Here is a JSON representation of the resource.</span></span>
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







