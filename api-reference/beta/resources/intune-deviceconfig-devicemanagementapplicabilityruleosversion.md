---
title: deviceManagementApplicabilityRuleOsVersion 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5a8195bd67cf64d1875b795c3609cf04f9c13b31
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48031695"
---
# <a name="devicemanagementapplicabilityruleosversion-resource-type"></a><span data-ttu-id="50fdf-103">deviceManagementApplicabilityRuleOsVersion 资源类型</span><span class="sxs-lookup"><span data-stu-id="50fdf-103">deviceManagementApplicabilityRuleOsVersion resource type</span></span>

<span data-ttu-id="50fdf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50fdf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="50fdf-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="50fdf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50fdf-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="50fdf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50fdf-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="50fdf-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="50fdf-108">属性</span><span class="sxs-lookup"><span data-stu-id="50fdf-108">Properties</span></span>
|<span data-ttu-id="50fdf-109">属性</span><span class="sxs-lookup"><span data-stu-id="50fdf-109">Property</span></span>|<span data-ttu-id="50fdf-110">类型</span><span class="sxs-lookup"><span data-stu-id="50fdf-110">Type</span></span>|<span data-ttu-id="50fdf-111">说明</span><span class="sxs-lookup"><span data-stu-id="50fdf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50fdf-112">minOSVersion</span><span class="sxs-lookup"><span data-stu-id="50fdf-112">minOSVersion</span></span>|<span data-ttu-id="50fdf-113">String</span><span class="sxs-lookup"><span data-stu-id="50fdf-113">String</span></span>|<span data-ttu-id="50fdf-114">适用性规则的最小 OS 版本。</span><span class="sxs-lookup"><span data-stu-id="50fdf-114">Min OS version for Applicability Rule.</span></span>|
|<span data-ttu-id="50fdf-115">maxOSVersion</span><span class="sxs-lookup"><span data-stu-id="50fdf-115">maxOSVersion</span></span>|<span data-ttu-id="50fdf-116">String</span><span class="sxs-lookup"><span data-stu-id="50fdf-116">String</span></span>|<span data-ttu-id="50fdf-117">适用性规则的最大 OS 版本。</span><span class="sxs-lookup"><span data-stu-id="50fdf-117">Max OS version for Applicability Rule.</span></span>|
|<span data-ttu-id="50fdf-118">name</span><span class="sxs-lookup"><span data-stu-id="50fdf-118">name</span></span>|<span data-ttu-id="50fdf-119">String</span><span class="sxs-lookup"><span data-stu-id="50fdf-119">String</span></span>|<span data-ttu-id="50fdf-120">对象的名称。</span><span class="sxs-lookup"><span data-stu-id="50fdf-120">Name for object.</span></span>|
|<span data-ttu-id="50fdf-121">ruleType</span><span class="sxs-lookup"><span data-stu-id="50fdf-121">ruleType</span></span>|[<span data-ttu-id="50fdf-122">deviceManagementApplicabilityRuleType</span><span class="sxs-lookup"><span data-stu-id="50fdf-122">deviceManagementApplicabilityRuleType</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruletype.md)|<span data-ttu-id="50fdf-123">适用性规则类型。</span><span class="sxs-lookup"><span data-stu-id="50fdf-123">Applicability Rule type.</span></span> <span data-ttu-id="50fdf-124">可取值为：`include`、`exclude`。</span><span class="sxs-lookup"><span data-stu-id="50fdf-124">Possible values are: `include`, `exclude`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="50fdf-125">关系</span><span class="sxs-lookup"><span data-stu-id="50fdf-125">Relationships</span></span>
<span data-ttu-id="50fdf-126">无</span><span class="sxs-lookup"><span data-stu-id="50fdf-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="50fdf-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="50fdf-127">JSON Representation</span></span>
<span data-ttu-id="50fdf-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="50fdf-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
  "minOSVersion": "String",
  "maxOSVersion": "String",
  "name": "String",
  "ruleType": "String"
}
```






