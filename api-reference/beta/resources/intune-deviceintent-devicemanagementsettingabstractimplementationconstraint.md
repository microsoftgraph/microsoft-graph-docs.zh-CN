---
title: deviceManagementSettingAbstractImplementationConstraint 资源类型
description: 强制实施 AbstractComplex 类型的约束已将或设置为特定值
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 62b257e7d6199798d2a4f13a3210e98d53b82de6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48061313"
---
# <a name="devicemanagementsettingabstractimplementationconstraint-resource-type"></a><span data-ttu-id="1a61d-103">deviceManagementSettingAbstractImplementationConstraint 资源类型</span><span class="sxs-lookup"><span data-stu-id="1a61d-103">deviceManagementSettingAbstractImplementationConstraint resource type</span></span>

<span data-ttu-id="1a61d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a61d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1a61d-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1a61d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a61d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1a61d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a61d-107">强制实施 AbstractComplex 类型的约束已将或设置为特定值</span><span class="sxs-lookup"><span data-stu-id="1a61d-107">Constraint that enforces an AbstractComplex type has or is set to a particular value</span></span>


<span data-ttu-id="1a61d-108">继承自 [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="1a61d-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1a61d-109">属性</span><span class="sxs-lookup"><span data-stu-id="1a61d-109">Properties</span></span>
|<span data-ttu-id="1a61d-110">属性</span><span class="sxs-lookup"><span data-stu-id="1a61d-110">Property</span></span>|<span data-ttu-id="1a61d-111">类型</span><span class="sxs-lookup"><span data-stu-id="1a61d-111">Type</span></span>|<span data-ttu-id="1a61d-112">说明</span><span class="sxs-lookup"><span data-stu-id="1a61d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a61d-113">allowedAbstractImplementationDefinitionIds</span><span class="sxs-lookup"><span data-stu-id="1a61d-113">allowedAbstractImplementationDefinitionIds</span></span>|<span data-ttu-id="1a61d-114">String 集合</span><span class="sxs-lookup"><span data-stu-id="1a61d-114">String collection</span></span>|<span data-ttu-id="1a61d-115">值的列表，表示未配置设置</span><span class="sxs-lookup"><span data-stu-id="1a61d-115">List of value which means not configured for the setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a61d-116">关系</span><span class="sxs-lookup"><span data-stu-id="1a61d-116">Relationships</span></span>
<span data-ttu-id="1a61d-117">无</span><span class="sxs-lookup"><span data-stu-id="1a61d-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1a61d-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1a61d-118">JSON Representation</span></span>
<span data-ttu-id="1a61d-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1a61d-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingAbstractImplementationConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingAbstractImplementationConstraint",
  "allowedAbstractImplementationDefinitionIds": [
    "String"
  ]
}
```






