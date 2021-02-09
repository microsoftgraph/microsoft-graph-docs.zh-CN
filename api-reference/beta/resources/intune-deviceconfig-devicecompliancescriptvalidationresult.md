---
title: deviceComplianceScriptValidationResult 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d76d96acf8dc96275902d1fba30f8ba6f49cc088
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154276"
---
# <a name="devicecompliancescriptvalidationresult-resource-type"></a><span data-ttu-id="03008-103">deviceComplianceScriptValidationResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="03008-103">deviceComplianceScriptValidationResult resource type</span></span>

<span data-ttu-id="03008-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03008-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="03008-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="03008-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="03008-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="03008-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03008-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="03008-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="03008-108">属性</span><span class="sxs-lookup"><span data-stu-id="03008-108">Properties</span></span>
|<span data-ttu-id="03008-109">属性</span><span class="sxs-lookup"><span data-stu-id="03008-109">Property</span></span>|<span data-ttu-id="03008-110">类型</span><span class="sxs-lookup"><span data-stu-id="03008-110">Type</span></span>|<span data-ttu-id="03008-111">说明</span><span class="sxs-lookup"><span data-stu-id="03008-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03008-112">规则</span><span class="sxs-lookup"><span data-stu-id="03008-112">rules</span></span>|<span data-ttu-id="03008-113">[deviceComplianceScriptRule](../resources/intune-deviceconfig-devicecompliancescriptrule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="03008-113">[deviceComplianceScriptRule](../resources/intune-deviceconfig-devicecompliancescriptrule.md) collection</span></span>|<span data-ttu-id="03008-114">从 json 分析规则。</span><span class="sxs-lookup"><span data-stu-id="03008-114">Parsed rules from json.</span></span>|
|<span data-ttu-id="03008-115">scriptErrors</span><span class="sxs-lookup"><span data-stu-id="03008-115">scriptErrors</span></span>|<span data-ttu-id="03008-116">[deviceComplianceScriptError](../resources/intune-deviceconfig-devicecompliancescripterror.md) 集合</span><span class="sxs-lookup"><span data-stu-id="03008-116">[deviceComplianceScriptError](../resources/intune-deviceconfig-devicecompliancescripterror.md) collection</span></span>|<span data-ttu-id="03008-117">脚本的 json 错误。</span><span class="sxs-lookup"><span data-stu-id="03008-117">Errors in json for the script.</span></span>|
|<span data-ttu-id="03008-118">ruleErrors</span><span class="sxs-lookup"><span data-stu-id="03008-118">ruleErrors</span></span>|<span data-ttu-id="03008-119">[deviceComplianceScriptRuleError](../resources/intune-deviceconfig-devicecompliancescriptruleerror.md) 集合</span><span class="sxs-lookup"><span data-stu-id="03008-119">[deviceComplianceScriptRuleError](../resources/intune-deviceconfig-devicecompliancescriptruleerror.md) collection</span></span>|<span data-ttu-id="03008-120">规则脚本的 json 错误。</span><span class="sxs-lookup"><span data-stu-id="03008-120">Errors in json for the script for rules.</span></span>|

## <a name="relationships"></a><span data-ttu-id="03008-121">关系</span><span class="sxs-lookup"><span data-stu-id="03008-121">Relationships</span></span>
<span data-ttu-id="03008-122">无</span><span class="sxs-lookup"><span data-stu-id="03008-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="03008-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="03008-123">JSON Representation</span></span>
<span data-ttu-id="03008-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="03008-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceComplianceScriptValidationResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceScriptValidationResult",
  "rules": [
    {
      "@odata.type": "microsoft.graph.deviceComplianceScriptRule",
      "settingName": "String",
      "operator": "String",
      "deviceComplianceScriptRulOperator": "String",
      "dataType": "String",
      "deviceComplianceScriptRuleDataType": "String",
      "operand": "String"
    }
  ],
  "scriptErrors": [
    {
      "@odata.type": "microsoft.graph.deviceComplianceScriptError",
      "code": "String",
      "deviceComplianceScriptRulesValidationError": "String",
      "message": "String"
    }
  ],
  "ruleErrors": [
    {
      "@odata.type": "microsoft.graph.deviceComplianceScriptRuleError",
      "code": "String",
      "deviceComplianceScriptRulesValidationError": "String",
      "message": "String",
      "settingName": "String"
    }
  ]
}
```




