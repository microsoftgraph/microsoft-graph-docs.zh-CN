---
title: deviceManagementSettingBooleanConstraint 资源类型
description: 约束强制实施特定的布尔值
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9a83a0747e0960aeebaa0de472fae4d587111946
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36364724"
---
# <a name="devicemanagementsettingbooleanconstraint-resource-type"></a><span data-ttu-id="64f7a-103">deviceManagementSettingBooleanConstraint 资源类型</span><span class="sxs-lookup"><span data-stu-id="64f7a-103">deviceManagementSettingBooleanConstraint resource type</span></span>

> <span data-ttu-id="64f7a-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="64f7a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64f7a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="64f7a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64f7a-106">约束强制实施特定的布尔值</span><span class="sxs-lookup"><span data-stu-id="64f7a-106">Constraint the enforces a particular boolean value</span></span>


<span data-ttu-id="64f7a-107">继承自[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="64f7a-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="64f7a-108">属性</span><span class="sxs-lookup"><span data-stu-id="64f7a-108">Properties</span></span>
|<span data-ttu-id="64f7a-109">属性</span><span class="sxs-lookup"><span data-stu-id="64f7a-109">Property</span></span>|<span data-ttu-id="64f7a-110">类型</span><span class="sxs-lookup"><span data-stu-id="64f7a-110">Type</span></span>|<span data-ttu-id="64f7a-111">说明</span><span class="sxs-lookup"><span data-stu-id="64f7a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64f7a-112">值</span><span class="sxs-lookup"><span data-stu-id="64f7a-112">value</span></span>|<span data-ttu-id="64f7a-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="64f7a-113">Boolean</span></span>|<span data-ttu-id="64f7a-114">要与之比较的布尔值</span><span class="sxs-lookup"><span data-stu-id="64f7a-114">The boolean value to compare against</span></span>|

## <a name="relationships"></a><span data-ttu-id="64f7a-115">关系</span><span class="sxs-lookup"><span data-stu-id="64f7a-115">Relationships</span></span>
<span data-ttu-id="64f7a-116">无</span><span class="sxs-lookup"><span data-stu-id="64f7a-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="64f7a-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="64f7a-117">JSON Representation</span></span>
<span data-ttu-id="64f7a-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="64f7a-118">Here is a JSON representation of the resource.</span></span>
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



