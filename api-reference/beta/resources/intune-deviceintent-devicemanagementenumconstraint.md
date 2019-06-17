---
title: deviceManagementEnumConstraint 资源类型
description: 强制实施设置值的约束来自允许的一组字符串
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 64c07f663d034cf6fa758155294730015ca6e3b4
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34964099"
---
# <a name="devicemanagementenumconstraint-resource-type"></a><span data-ttu-id="0f2ef-103">deviceManagementEnumConstraint 资源类型</span><span class="sxs-lookup"><span data-stu-id="0f2ef-103">deviceManagementEnumConstraint resource type</span></span>

> <span data-ttu-id="0f2ef-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0f2ef-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0f2ef-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0f2ef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f2ef-106">强制实施设置值的约束来自允许的一组字符串</span><span class="sxs-lookup"><span data-stu-id="0f2ef-106">Constraint that enforces the setting value is from a permitted set of strings</span></span>


<span data-ttu-id="0f2ef-107">继承自[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="0f2ef-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0f2ef-108">属性</span><span class="sxs-lookup"><span data-stu-id="0f2ef-108">Properties</span></span>
|<span data-ttu-id="0f2ef-109">属性</span><span class="sxs-lookup"><span data-stu-id="0f2ef-109">Property</span></span>|<span data-ttu-id="0f2ef-110">类型</span><span class="sxs-lookup"><span data-stu-id="0f2ef-110">Type</span></span>|<span data-ttu-id="0f2ef-111">说明</span><span class="sxs-lookup"><span data-stu-id="0f2ef-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f2ef-112">值</span><span class="sxs-lookup"><span data-stu-id="0f2ef-112">values</span></span>|<span data-ttu-id="0f2ef-113">[deviceManagementEnumValue](../resources/intune-deviceintent-devicemanagementenumvalue.md)集合</span><span class="sxs-lookup"><span data-stu-id="0f2ef-113">[deviceManagementEnumValue](../resources/intune-deviceintent-devicemanagementenumvalue.md) collection</span></span>|<span data-ttu-id="0f2ef-114">此字符串的有效值列表</span><span class="sxs-lookup"><span data-stu-id="0f2ef-114">List of valid values for this string</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f2ef-115">关系</span><span class="sxs-lookup"><span data-stu-id="0f2ef-115">Relationships</span></span>
<span data-ttu-id="0f2ef-116">无</span><span class="sxs-lookup"><span data-stu-id="0f2ef-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0f2ef-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0f2ef-117">JSON Representation</span></span>
<span data-ttu-id="0f2ef-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0f2ef-118">Here is a JSON representation of the resource.</span></span>
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





