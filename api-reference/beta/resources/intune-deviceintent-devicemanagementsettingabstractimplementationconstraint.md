---
title: deviceManagementSettingAbstractImplementationConstraint 资源类型
description: 强制实施 AbstractComplex 类型的约束已将或设置为特定值
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e8fd314d2e71b95e446009e70a35166a9aa2e0ff
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43443325"
---
# <a name="devicemanagementsettingabstractimplementationconstraint-resource-type"></a><span data-ttu-id="ee2f3-103">deviceManagementSettingAbstractImplementationConstraint 资源类型</span><span class="sxs-lookup"><span data-stu-id="ee2f3-103">deviceManagementSettingAbstractImplementationConstraint resource type</span></span>

<span data-ttu-id="ee2f3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee2f3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ee2f3-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ee2f3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ee2f3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ee2f3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee2f3-107">强制实施 AbstractComplex 类型的约束已将或设置为特定值</span><span class="sxs-lookup"><span data-stu-id="ee2f3-107">Constraint that enforces an AbstractComplex type has or is set to a particular value</span></span>


<span data-ttu-id="ee2f3-108">继承自[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="ee2f3-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ee2f3-109">属性</span><span class="sxs-lookup"><span data-stu-id="ee2f3-109">Properties</span></span>
|<span data-ttu-id="ee2f3-110">属性</span><span class="sxs-lookup"><span data-stu-id="ee2f3-110">Property</span></span>|<span data-ttu-id="ee2f3-111">类型</span><span class="sxs-lookup"><span data-stu-id="ee2f3-111">Type</span></span>|<span data-ttu-id="ee2f3-112">说明</span><span class="sxs-lookup"><span data-stu-id="ee2f3-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee2f3-113">allowedAbstractImplementationDefinitionIds</span><span class="sxs-lookup"><span data-stu-id="ee2f3-113">allowedAbstractImplementationDefinitionIds</span></span>|<span data-ttu-id="ee2f3-114">String 集合</span><span class="sxs-lookup"><span data-stu-id="ee2f3-114">String collection</span></span>|<span data-ttu-id="ee2f3-115">值的列表，表示未配置设置</span><span class="sxs-lookup"><span data-stu-id="ee2f3-115">List of value which means not configured for the setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="ee2f3-116">关系</span><span class="sxs-lookup"><span data-stu-id="ee2f3-116">Relationships</span></span>
<span data-ttu-id="ee2f3-117">无</span><span class="sxs-lookup"><span data-stu-id="ee2f3-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ee2f3-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ee2f3-118">JSON Representation</span></span>
<span data-ttu-id="ee2f3-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ee2f3-119">Here is a JSON representation of the resource.</span></span>
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



