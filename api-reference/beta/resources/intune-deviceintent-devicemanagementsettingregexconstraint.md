---
title: deviceManagementSettingRegexConstraint 资源类型
description: 根据给定的 RegEx 模式强制设置匹配的约束
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 76bb80edaec0ccd53cc9f0923a7df7b1c595dc60
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31792284"
---
# <a name="devicemanagementsettingregexconstraint-resource-type"></a><span data-ttu-id="263b5-103">deviceManagementSettingRegexConstraint 资源类型</span><span class="sxs-lookup"><span data-stu-id="263b5-103">deviceManagementSettingRegexConstraint resource type</span></span>

> <span data-ttu-id="263b5-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="263b5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="263b5-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="263b5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="263b5-106">根据给定的 RegEx 模式强制设置匹配的约束</span><span class="sxs-lookup"><span data-stu-id="263b5-106">Constraint enforcing the setting matches against a given RegEx pattern</span></span>


<span data-ttu-id="263b5-107">继承自[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="263b5-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="263b5-108">属性</span><span class="sxs-lookup"><span data-stu-id="263b5-108">Properties</span></span>
|<span data-ttu-id="263b5-109">属性</span><span class="sxs-lookup"><span data-stu-id="263b5-109">Property</span></span>|<span data-ttu-id="263b5-110">类型</span><span class="sxs-lookup"><span data-stu-id="263b5-110">Type</span></span>|<span data-ttu-id="263b5-111">说明</span><span class="sxs-lookup"><span data-stu-id="263b5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="263b5-112">正则表达式</span><span class="sxs-lookup"><span data-stu-id="263b5-112">regex</span></span>|<span data-ttu-id="263b5-113">String</span><span class="sxs-lookup"><span data-stu-id="263b5-113">String</span></span>|<span data-ttu-id="263b5-114">要匹配的正则表达式模式</span><span class="sxs-lookup"><span data-stu-id="263b5-114">The RegEx pattern to match against</span></span>|

## <a name="relationships"></a><span data-ttu-id="263b5-115">关系</span><span class="sxs-lookup"><span data-stu-id="263b5-115">Relationships</span></span>
<span data-ttu-id="263b5-116">无</span><span class="sxs-lookup"><span data-stu-id="263b5-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="263b5-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="263b5-117">JSON Representation</span></span>
<span data-ttu-id="263b5-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="263b5-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingRegexConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingRegexConstraint",
  "regex": "String"
}
```





