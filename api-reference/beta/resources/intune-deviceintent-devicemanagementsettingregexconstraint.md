---
title: deviceManagementSettingRegexConstraint 资源类型
description: 根据给定的 RegEx 模式强制设置匹配的约束
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 08734a71b179d55bc76e9cd82360773d7d17f3bb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48061131"
---
# <a name="devicemanagementsettingregexconstraint-resource-type"></a><span data-ttu-id="33869-103">deviceManagementSettingRegexConstraint 资源类型</span><span class="sxs-lookup"><span data-stu-id="33869-103">deviceManagementSettingRegexConstraint resource type</span></span>

<span data-ttu-id="33869-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33869-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="33869-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="33869-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="33869-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="33869-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33869-107">根据给定的 RegEx 模式强制设置匹配的约束</span><span class="sxs-lookup"><span data-stu-id="33869-107">Constraint enforcing the setting matches against a given RegEx pattern</span></span>


<span data-ttu-id="33869-108">继承自 [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="33869-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="33869-109">属性</span><span class="sxs-lookup"><span data-stu-id="33869-109">Properties</span></span>
|<span data-ttu-id="33869-110">属性</span><span class="sxs-lookup"><span data-stu-id="33869-110">Property</span></span>|<span data-ttu-id="33869-111">类型</span><span class="sxs-lookup"><span data-stu-id="33869-111">Type</span></span>|<span data-ttu-id="33869-112">说明</span><span class="sxs-lookup"><span data-stu-id="33869-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33869-113">正则表达式</span><span class="sxs-lookup"><span data-stu-id="33869-113">regex</span></span>|<span data-ttu-id="33869-114">String</span><span class="sxs-lookup"><span data-stu-id="33869-114">String</span></span>|<span data-ttu-id="33869-115">要匹配的正则表达式模式</span><span class="sxs-lookup"><span data-stu-id="33869-115">The RegEx pattern to match against</span></span>|

## <a name="relationships"></a><span data-ttu-id="33869-116">关系</span><span class="sxs-lookup"><span data-stu-id="33869-116">Relationships</span></span>
<span data-ttu-id="33869-117">无</span><span class="sxs-lookup"><span data-stu-id="33869-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="33869-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="33869-118">JSON Representation</span></span>
<span data-ttu-id="33869-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="33869-119">Here is a JSON representation of the resource.</span></span>
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






