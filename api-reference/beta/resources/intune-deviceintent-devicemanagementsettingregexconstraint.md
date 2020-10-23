---
title: deviceManagementSettingRegexConstraint 资源类型
description: 根据给定的 RegEx 模式强制设置匹配的约束
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3d6f811330ceaa282a547de0f51d075598bd16fc
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48730440"
---
# <a name="devicemanagementsettingregexconstraint-resource-type"></a><span data-ttu-id="5339a-103">deviceManagementSettingRegexConstraint 资源类型</span><span class="sxs-lookup"><span data-stu-id="5339a-103">deviceManagementSettingRegexConstraint resource type</span></span>

<span data-ttu-id="5339a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5339a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5339a-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5339a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5339a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5339a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5339a-107">根据给定的 RegEx 模式强制设置匹配的约束</span><span class="sxs-lookup"><span data-stu-id="5339a-107">Constraint enforcing the setting matches against a given RegEx pattern</span></span>


<span data-ttu-id="5339a-108">继承自 [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="5339a-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5339a-109">属性</span><span class="sxs-lookup"><span data-stu-id="5339a-109">Properties</span></span>
|<span data-ttu-id="5339a-110">属性</span><span class="sxs-lookup"><span data-stu-id="5339a-110">Property</span></span>|<span data-ttu-id="5339a-111">类型</span><span class="sxs-lookup"><span data-stu-id="5339a-111">Type</span></span>|<span data-ttu-id="5339a-112">说明</span><span class="sxs-lookup"><span data-stu-id="5339a-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5339a-113">正则表达式</span><span class="sxs-lookup"><span data-stu-id="5339a-113">regex</span></span>|<span data-ttu-id="5339a-114">String</span><span class="sxs-lookup"><span data-stu-id="5339a-114">String</span></span>|<span data-ttu-id="5339a-115">要匹配的正则表达式模式</span><span class="sxs-lookup"><span data-stu-id="5339a-115">The RegEx pattern to match against</span></span>|

## <a name="relationships"></a><span data-ttu-id="5339a-116">关系</span><span class="sxs-lookup"><span data-stu-id="5339a-116">Relationships</span></span>
<span data-ttu-id="5339a-117">无</span><span class="sxs-lookup"><span data-stu-id="5339a-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5339a-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5339a-118">JSON Representation</span></span>
<span data-ttu-id="5339a-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5339a-119">Here is a JSON representation of the resource.</span></span>
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





