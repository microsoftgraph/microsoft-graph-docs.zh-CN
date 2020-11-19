---
title: deviceManagementSettingIntegerConstraint 资源类型
description: 强制整数设置允许的值范围的约束
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f04745c70a61f71a6d0ba90dc680adaaba35fee4
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49268051"
---
# <a name="devicemanagementsettingintegerconstraint-resource-type"></a><span data-ttu-id="99012-103">deviceManagementSettingIntegerConstraint 资源类型</span><span class="sxs-lookup"><span data-stu-id="99012-103">deviceManagementSettingIntegerConstraint resource type</span></span>

<span data-ttu-id="99012-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99012-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="99012-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="99012-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="99012-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="99012-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99012-107">强制整数设置允许的值范围的约束</span><span class="sxs-lookup"><span data-stu-id="99012-107">Constraint enforcing the permitted value range for an integer setting</span></span>


<span data-ttu-id="99012-108">继承自 [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="99012-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="99012-109">属性</span><span class="sxs-lookup"><span data-stu-id="99012-109">Properties</span></span>
|<span data-ttu-id="99012-110">属性</span><span class="sxs-lookup"><span data-stu-id="99012-110">Property</span></span>|<span data-ttu-id="99012-111">类型</span><span class="sxs-lookup"><span data-stu-id="99012-111">Type</span></span>|<span data-ttu-id="99012-112">说明</span><span class="sxs-lookup"><span data-stu-id="99012-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99012-113">minimumValue</span><span class="sxs-lookup"><span data-stu-id="99012-113">minimumValue</span></span>|<span data-ttu-id="99012-114">Int32</span><span class="sxs-lookup"><span data-stu-id="99012-114">Int32</span></span>|<span data-ttu-id="99012-115">允许的最小值</span><span class="sxs-lookup"><span data-stu-id="99012-115">The minimum permitted value</span></span>|
|<span data-ttu-id="99012-116">maximumValue</span><span class="sxs-lookup"><span data-stu-id="99012-116">maximumValue</span></span>|<span data-ttu-id="99012-117">Int32</span><span class="sxs-lookup"><span data-stu-id="99012-117">Int32</span></span>|<span data-ttu-id="99012-118">允许的最大值</span><span class="sxs-lookup"><span data-stu-id="99012-118">The maximum permitted value</span></span>|

## <a name="relationships"></a><span data-ttu-id="99012-119">关系</span><span class="sxs-lookup"><span data-stu-id="99012-119">Relationships</span></span>
<span data-ttu-id="99012-120">无</span><span class="sxs-lookup"><span data-stu-id="99012-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="99012-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="99012-121">JSON Representation</span></span>
<span data-ttu-id="99012-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="99012-122">Here is a JSON representation of the resource.</span></span>
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




