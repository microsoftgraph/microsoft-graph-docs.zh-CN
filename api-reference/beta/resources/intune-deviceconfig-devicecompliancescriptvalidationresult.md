---
title: deviceComplianceScriptValidationResult 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 08b79c44d65c896f0b7a4190678f3569189cd075
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729719"
---
# <a name="devicecompliancescriptvalidationresult-resource-type"></a><span data-ttu-id="3c3eb-103">deviceComplianceScriptValidationResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="3c3eb-103">deviceComplianceScriptValidationResult resource type</span></span>

<span data-ttu-id="3c3eb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c3eb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3c3eb-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3c3eb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c3eb-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3c3eb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c3eb-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3c3eb-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="3c3eb-108">属性</span><span class="sxs-lookup"><span data-stu-id="3c3eb-108">Properties</span></span>
|<span data-ttu-id="3c3eb-109">属性</span><span class="sxs-lookup"><span data-stu-id="3c3eb-109">Property</span></span>|<span data-ttu-id="3c3eb-110">类型</span><span class="sxs-lookup"><span data-stu-id="3c3eb-110">Type</span></span>|<span data-ttu-id="3c3eb-111">说明</span><span class="sxs-lookup"><span data-stu-id="3c3eb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c3eb-112">规则</span><span class="sxs-lookup"><span data-stu-id="3c3eb-112">rules</span></span>|<span data-ttu-id="3c3eb-113">[deviceComplianceScriptRule](../resources/intune-deviceconfig-devicecompliancescriptrule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3c3eb-113">[deviceComplianceScriptRule](../resources/intune-deviceconfig-devicecompliancescriptrule.md) collection</span></span>|<span data-ttu-id="3c3eb-114">解析了 json 的规则。</span><span class="sxs-lookup"><span data-stu-id="3c3eb-114">Parsed rules from json.</span></span>|
|<span data-ttu-id="3c3eb-115">scriptErrors</span><span class="sxs-lookup"><span data-stu-id="3c3eb-115">scriptErrors</span></span>|<span data-ttu-id="3c3eb-116">[deviceComplianceScriptError](../resources/intune-deviceconfig-devicecompliancescripterror.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3c3eb-116">[deviceComplianceScriptError](../resources/intune-deviceconfig-devicecompliancescripterror.md) collection</span></span>|<span data-ttu-id="3c3eb-117">Json 中的脚本错误。</span><span class="sxs-lookup"><span data-stu-id="3c3eb-117">Errors in json for the script.</span></span>|
|<span data-ttu-id="3c3eb-118">ruleErrors</span><span class="sxs-lookup"><span data-stu-id="3c3eb-118">ruleErrors</span></span>|<span data-ttu-id="3c3eb-119">[deviceComplianceScriptRuleError](../resources/intune-deviceconfig-devicecompliancescriptruleerror.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3c3eb-119">[deviceComplianceScriptRuleError](../resources/intune-deviceconfig-devicecompliancescriptruleerror.md) collection</span></span>|<span data-ttu-id="3c3eb-120">Json 中适用于规则的脚本的错误。</span><span class="sxs-lookup"><span data-stu-id="3c3eb-120">Errors in json for the script for rules.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3c3eb-121">关系</span><span class="sxs-lookup"><span data-stu-id="3c3eb-121">Relationships</span></span>
<span data-ttu-id="3c3eb-122">无</span><span class="sxs-lookup"><span data-stu-id="3c3eb-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3c3eb-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3c3eb-123">JSON Representation</span></span>
<span data-ttu-id="3c3eb-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3c3eb-124">Here is a JSON representation of the resource.</span></span>
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





