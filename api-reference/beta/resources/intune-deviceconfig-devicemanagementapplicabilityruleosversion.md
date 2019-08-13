---
title: deviceManagementApplicabilityRuleOsVersion 资源类型
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7a81e8d096e8c11d6e1b3dd5117af1b384268095
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332846"
---
# <a name="devicemanagementapplicabilityruleosversion-resource-type"></a><span data-ttu-id="40b61-103">deviceManagementApplicabilityRuleOsVersion 资源类型</span><span class="sxs-lookup"><span data-stu-id="40b61-103">deviceManagementApplicabilityRuleOsVersion resource type</span></span>

> <span data-ttu-id="40b61-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="40b61-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="40b61-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="40b61-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40b61-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="40b61-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="40b61-107">属性</span><span class="sxs-lookup"><span data-stu-id="40b61-107">Properties</span></span>
|<span data-ttu-id="40b61-108">属性</span><span class="sxs-lookup"><span data-stu-id="40b61-108">Property</span></span>|<span data-ttu-id="40b61-109">类型</span><span class="sxs-lookup"><span data-stu-id="40b61-109">Type</span></span>|<span data-ttu-id="40b61-110">说明</span><span class="sxs-lookup"><span data-stu-id="40b61-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40b61-111">minOSVersion</span><span class="sxs-lookup"><span data-stu-id="40b61-111">minOSVersion</span></span>|<span data-ttu-id="40b61-112">String</span><span class="sxs-lookup"><span data-stu-id="40b61-112">String</span></span>|<span data-ttu-id="40b61-113">适用性规则的最小 OS 版本。</span><span class="sxs-lookup"><span data-stu-id="40b61-113">Min OS version for Applicability Rule.</span></span>|
|<span data-ttu-id="40b61-114">maxOSVersion</span><span class="sxs-lookup"><span data-stu-id="40b61-114">maxOSVersion</span></span>|<span data-ttu-id="40b61-115">String</span><span class="sxs-lookup"><span data-stu-id="40b61-115">String</span></span>|<span data-ttu-id="40b61-116">适用性规则的最大 OS 版本。</span><span class="sxs-lookup"><span data-stu-id="40b61-116">Max OS version for Applicability Rule.</span></span>|
|<span data-ttu-id="40b61-117">name</span><span class="sxs-lookup"><span data-stu-id="40b61-117">name</span></span>|<span data-ttu-id="40b61-118">String</span><span class="sxs-lookup"><span data-stu-id="40b61-118">String</span></span>|<span data-ttu-id="40b61-119">对象的名称。</span><span class="sxs-lookup"><span data-stu-id="40b61-119">Name for object.</span></span>|
|<span data-ttu-id="40b61-120">ruleType</span><span class="sxs-lookup"><span data-stu-id="40b61-120">ruleType</span></span>|[<span data-ttu-id="40b61-121">deviceManagementApplicabilityRuleType</span><span class="sxs-lookup"><span data-stu-id="40b61-121">deviceManagementApplicabilityRuleType</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruletype.md)|<span data-ttu-id="40b61-122">适用性规则类型。</span><span class="sxs-lookup"><span data-stu-id="40b61-122">Applicability Rule type.</span></span> <span data-ttu-id="40b61-123">可取值为：`include`、`exclude`。</span><span class="sxs-lookup"><span data-stu-id="40b61-123">Possible values are: `include`, `exclude`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="40b61-124">关系</span><span class="sxs-lookup"><span data-stu-id="40b61-124">Relationships</span></span>
<span data-ttu-id="40b61-125">无</span><span class="sxs-lookup"><span data-stu-id="40b61-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="40b61-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="40b61-126">JSON Representation</span></span>
<span data-ttu-id="40b61-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="40b61-127">Here is a JSON representation of the resource.</span></span>
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



