---
title: deviceManagementSettingRequiredConstraint 资源类型
description: 强制实施特定的必需设置（非 null/未定义/空字符串/未配置）的约束
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a077be2aac78b468ba7b265f8154ceee29803eef
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785286"
---
# <a name="devicemanagementsettingrequiredconstraint-resource-type"></a><span data-ttu-id="416b1-103">deviceManagementSettingRequiredConstraint 资源类型</span><span class="sxs-lookup"><span data-stu-id="416b1-103">deviceManagementSettingRequiredConstraint resource type</span></span>

> <span data-ttu-id="416b1-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="416b1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="416b1-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="416b1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="416b1-106">强制实施特定的必需设置（非 null/未定义/空字符串/未配置）的约束</span><span class="sxs-lookup"><span data-stu-id="416b1-106">Constraint that enforces a particular required setting that is not null/undefined/empty string/not configured</span></span>


<span data-ttu-id="416b1-107">继承自[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="416b1-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="416b1-108">属性</span><span class="sxs-lookup"><span data-stu-id="416b1-108">Properties</span></span>
|<span data-ttu-id="416b1-109">属性</span><span class="sxs-lookup"><span data-stu-id="416b1-109">Property</span></span>|<span data-ttu-id="416b1-110">类型</span><span class="sxs-lookup"><span data-stu-id="416b1-110">Type</span></span>|<span data-ttu-id="416b1-111">说明</span><span class="sxs-lookup"><span data-stu-id="416b1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="416b1-112">notConfiguredValue</span><span class="sxs-lookup"><span data-stu-id="416b1-112">notConfiguredValue</span></span>|<span data-ttu-id="416b1-113">String</span><span class="sxs-lookup"><span data-stu-id="416b1-113">String</span></span>|<span data-ttu-id="416b1-114">值的列表，表示未配置设置</span><span class="sxs-lookup"><span data-stu-id="416b1-114">List of value which means not configured for the setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="416b1-115">关系</span><span class="sxs-lookup"><span data-stu-id="416b1-115">Relationships</span></span>
<span data-ttu-id="416b1-116">无</span><span class="sxs-lookup"><span data-stu-id="416b1-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="416b1-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="416b1-117">JSON Representation</span></span>
<span data-ttu-id="416b1-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="416b1-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingRequiredConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingRequiredConstraint",
  "notConfiguredValue": "String"
}
```



