---
title: deviceManagementEnumConstraint 资源类型
description: 强制实施设置值的约束来自允许的一组字符串
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 202365368c17d22cf33ea78320ac2a2604a59194
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48061474"
---
# <a name="devicemanagementenumconstraint-resource-type"></a><span data-ttu-id="b9ff1-103">deviceManagementEnumConstraint 资源类型</span><span class="sxs-lookup"><span data-stu-id="b9ff1-103">deviceManagementEnumConstraint resource type</span></span>

<span data-ttu-id="b9ff1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9ff1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b9ff1-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b9ff1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9ff1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b9ff1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9ff1-107">强制实施设置值的约束来自允许的一组字符串</span><span class="sxs-lookup"><span data-stu-id="b9ff1-107">Constraint that enforces the setting value is from a permitted set of strings</span></span>


<span data-ttu-id="b9ff1-108">继承自 [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="b9ff1-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b9ff1-109">属性</span><span class="sxs-lookup"><span data-stu-id="b9ff1-109">Properties</span></span>
|<span data-ttu-id="b9ff1-110">属性</span><span class="sxs-lookup"><span data-stu-id="b9ff1-110">Property</span></span>|<span data-ttu-id="b9ff1-111">类型</span><span class="sxs-lookup"><span data-stu-id="b9ff1-111">Type</span></span>|<span data-ttu-id="b9ff1-112">说明</span><span class="sxs-lookup"><span data-stu-id="b9ff1-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9ff1-113">值</span><span class="sxs-lookup"><span data-stu-id="b9ff1-113">values</span></span>|<span data-ttu-id="b9ff1-114">[deviceManagementEnumValue](../resources/intune-deviceintent-devicemanagementenumvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b9ff1-114">[deviceManagementEnumValue](../resources/intune-deviceintent-devicemanagementenumvalue.md) collection</span></span>|<span data-ttu-id="b9ff1-115">此字符串的有效值列表</span><span class="sxs-lookup"><span data-stu-id="b9ff1-115">List of valid values for this string</span></span>|

## <a name="relationships"></a><span data-ttu-id="b9ff1-116">关系</span><span class="sxs-lookup"><span data-stu-id="b9ff1-116">Relationships</span></span>
<span data-ttu-id="b9ff1-117">无</span><span class="sxs-lookup"><span data-stu-id="b9ff1-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b9ff1-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b9ff1-118">JSON Representation</span></span>
<span data-ttu-id="b9ff1-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b9ff1-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementEnumConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementEnumConstraint",
  "values": [
    {
      "@odata.type": "microsoft.graph.deviceManagementEnumValue",
      "value": "String",
      "displayName": "String"
    }
  ]
}
```






