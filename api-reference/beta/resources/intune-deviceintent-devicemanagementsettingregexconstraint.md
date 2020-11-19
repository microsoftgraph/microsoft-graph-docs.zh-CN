---
title: deviceManagementSettingRegexConstraint 资源类型
description: 根据给定的 RegEx 模式强制设置匹配的约束
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 11d06b2af4273166b3d6cf93a36a76fecc7ec548
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49267927"
---
# <a name="devicemanagementsettingregexconstraint-resource-type"></a><span data-ttu-id="5e42b-103">deviceManagementSettingRegexConstraint 资源类型</span><span class="sxs-lookup"><span data-stu-id="5e42b-103">deviceManagementSettingRegexConstraint resource type</span></span>

<span data-ttu-id="5e42b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e42b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5e42b-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5e42b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5e42b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5e42b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e42b-107">根据给定的 RegEx 模式强制设置匹配的约束</span><span class="sxs-lookup"><span data-stu-id="5e42b-107">Constraint enforcing the setting matches against a given RegEx pattern</span></span>


<span data-ttu-id="5e42b-108">继承自 [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="5e42b-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5e42b-109">属性</span><span class="sxs-lookup"><span data-stu-id="5e42b-109">Properties</span></span>
|<span data-ttu-id="5e42b-110">属性</span><span class="sxs-lookup"><span data-stu-id="5e42b-110">Property</span></span>|<span data-ttu-id="5e42b-111">类型</span><span class="sxs-lookup"><span data-stu-id="5e42b-111">Type</span></span>|<span data-ttu-id="5e42b-112">说明</span><span class="sxs-lookup"><span data-stu-id="5e42b-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e42b-113">正则表达式</span><span class="sxs-lookup"><span data-stu-id="5e42b-113">regex</span></span>|<span data-ttu-id="5e42b-114">字符串</span><span class="sxs-lookup"><span data-stu-id="5e42b-114">String</span></span>|<span data-ttu-id="5e42b-115">要匹配的正则表达式模式</span><span class="sxs-lookup"><span data-stu-id="5e42b-115">The RegEx pattern to match against</span></span>|

## <a name="relationships"></a><span data-ttu-id="5e42b-116">关系</span><span class="sxs-lookup"><span data-stu-id="5e42b-116">Relationships</span></span>
<span data-ttu-id="5e42b-117">无</span><span class="sxs-lookup"><span data-stu-id="5e42b-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5e42b-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5e42b-118">JSON Representation</span></span>
<span data-ttu-id="5e42b-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5e42b-119">Here is a JSON representation of the resource.</span></span>
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




