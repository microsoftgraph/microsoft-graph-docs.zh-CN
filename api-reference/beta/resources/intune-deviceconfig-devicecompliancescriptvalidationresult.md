---
title: deviceComplianceScriptValidationResult 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2d91c9ca3b234971a6acc58b7dee8cc736745d85
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44789327"
---
# <a name="devicecompliancescriptvalidationresult-resource-type"></a><span data-ttu-id="fc34c-103">deviceComplianceScriptValidationResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="fc34c-103">deviceComplianceScriptValidationResult resource type</span></span>

<span data-ttu-id="fc34c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc34c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fc34c-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fc34c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc34c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fc34c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc34c-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="fc34c-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="fc34c-108">属性</span><span class="sxs-lookup"><span data-stu-id="fc34c-108">Properties</span></span>
|<span data-ttu-id="fc34c-109">属性</span><span class="sxs-lookup"><span data-stu-id="fc34c-109">Property</span></span>|<span data-ttu-id="fc34c-110">类型</span><span class="sxs-lookup"><span data-stu-id="fc34c-110">Type</span></span>|<span data-ttu-id="fc34c-111">说明</span><span class="sxs-lookup"><span data-stu-id="fc34c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc34c-112">规则</span><span class="sxs-lookup"><span data-stu-id="fc34c-112">rules</span></span>|<span data-ttu-id="fc34c-113">[deviceComplianceScriptRule](../resources/intune-deviceconfig-devicecompliancescriptrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="fc34c-113">[deviceComplianceScriptRule](../resources/intune-deviceconfig-devicecompliancescriptrule.md) collection</span></span>|<span data-ttu-id="fc34c-114">解析了 json 的规则。</span><span class="sxs-lookup"><span data-stu-id="fc34c-114">Parsed rules from json.</span></span>|
|<span data-ttu-id="fc34c-115">scriptErrors</span><span class="sxs-lookup"><span data-stu-id="fc34c-115">scriptErrors</span></span>|<span data-ttu-id="fc34c-116">[deviceComplianceScriptError](../resources/intune-deviceconfig-devicecompliancescripterror.md)集合</span><span class="sxs-lookup"><span data-stu-id="fc34c-116">[deviceComplianceScriptError](../resources/intune-deviceconfig-devicecompliancescripterror.md) collection</span></span>|<span data-ttu-id="fc34c-117">Json 中的脚本错误。</span><span class="sxs-lookup"><span data-stu-id="fc34c-117">Errors in json for the script.</span></span>|
|<span data-ttu-id="fc34c-118">ruleErrors</span><span class="sxs-lookup"><span data-stu-id="fc34c-118">ruleErrors</span></span>|<span data-ttu-id="fc34c-119">[deviceComplianceScriptRuleError](../resources/intune-deviceconfig-devicecompliancescriptruleerror.md)集合</span><span class="sxs-lookup"><span data-stu-id="fc34c-119">[deviceComplianceScriptRuleError](../resources/intune-deviceconfig-devicecompliancescriptruleerror.md) collection</span></span>|<span data-ttu-id="fc34c-120">Json 中适用于规则的脚本的错误。</span><span class="sxs-lookup"><span data-stu-id="fc34c-120">Errors in json for the script for rules.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fc34c-121">关系</span><span class="sxs-lookup"><span data-stu-id="fc34c-121">Relationships</span></span>
<span data-ttu-id="fc34c-122">无</span><span class="sxs-lookup"><span data-stu-id="fc34c-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fc34c-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fc34c-123">JSON Representation</span></span>
<span data-ttu-id="fc34c-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fc34c-124">Here is a JSON representation of the resource.</span></span>
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
      "dataType": "String",
      "operand": "String"
    }
  ],
  "scriptErrors": [
    {
      "@odata.type": "microsoft.graph.deviceComplianceScriptError",
      "code": "String",
      "message": "String"
    }
  ],
  "ruleErrors": [
    {
      "@odata.type": "microsoft.graph.deviceComplianceScriptRuleError",
      "code": "String",
      "message": "String",
      "settingName": "String"
    }
  ]
}
```



