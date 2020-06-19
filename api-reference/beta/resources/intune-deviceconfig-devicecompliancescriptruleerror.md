---
title: deviceComplianceScriptRuleError 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a842d33c52774d2f2d5e251d32980e7cd28d4ec5
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44789326"
---
# <a name="devicecompliancescriptruleerror-resource-type"></a><span data-ttu-id="079bf-103">deviceComplianceScriptRuleError 资源类型</span><span class="sxs-lookup"><span data-stu-id="079bf-103">deviceComplianceScriptRuleError resource type</span></span>

<span data-ttu-id="079bf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="079bf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="079bf-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="079bf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="079bf-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="079bf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="079bf-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="079bf-107">Not yet documented</span></span>


<span data-ttu-id="079bf-108">继承自[deviceComplianceScriptError](../resources/intune-deviceconfig-devicecompliancescripterror.md)</span><span class="sxs-lookup"><span data-stu-id="079bf-108">Inherits from [deviceComplianceScriptError](../resources/intune-deviceconfig-devicecompliancescripterror.md)</span></span>

## <a name="properties"></a><span data-ttu-id="079bf-109">属性</span><span class="sxs-lookup"><span data-stu-id="079bf-109">Properties</span></span>
|<span data-ttu-id="079bf-110">属性</span><span class="sxs-lookup"><span data-stu-id="079bf-110">Property</span></span>|<span data-ttu-id="079bf-111">类型</span><span class="sxs-lookup"><span data-stu-id="079bf-111">Type</span></span>|<span data-ttu-id="079bf-112">说明</span><span class="sxs-lookup"><span data-stu-id="079bf-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="079bf-113">code</span><span class="sxs-lookup"><span data-stu-id="079bf-113">code</span></span>|[<span data-ttu-id="079bf-114">code</span><span class="sxs-lookup"><span data-stu-id="079bf-114">code</span></span>](../resources/intune-deviceconfig-code.md)|<span data-ttu-id="079bf-115">错误代码。</span><span class="sxs-lookup"><span data-stu-id="079bf-115">Error code.</span></span> <span data-ttu-id="079bf-116">继承自[deviceComplianceScriptError](../resources/intune-deviceconfig-devicecompliancescripterror.md)。</span><span class="sxs-lookup"><span data-stu-id="079bf-116">Inherited from [deviceComplianceScriptError](../resources/intune-deviceconfig-devicecompliancescripterror.md).</span></span> <span data-ttu-id="079bf-117">可以取值为：、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、 `none` `jsonFileInvalid` `jsonFileMissing` `jsonFileTooLarge` `rulesMissing` `duplicateRules` `tooManyRulesSpecified` `operatorMissing` `operatorNotSupported` `datatypeMissing` `datatypeNotSupported` `operatorDataTypeCombinationNotSupported` `moreInfoUriMissing` `moreInfoUriInvalid` `moreInfoUriTooLarge` `descriptionMissing` `descriptionInvalid` `descriptionTooLarge` `titleMissing` `titleInvalid` `titleTooLarge` `operandMissing` `operandInvalid` `operandTooLarge` `settingNameMissing` `settingNameInvalid` `settingNameTooLarge` `englishLocaleMissing` `duplicateLocales` `unrecognizedLocale` `unknown` `remediationStringsMissing` 。</span><span class="sxs-lookup"><span data-stu-id="079bf-117">Possible values are: `none`, `jsonFileInvalid`, `jsonFileMissing`, `jsonFileTooLarge`, `rulesMissing`, `duplicateRules`, `tooManyRulesSpecified`, `operatorMissing`, `operatorNotSupported`, `datatypeMissing`, `datatypeNotSupported`, `operatorDataTypeCombinationNotSupported`, `moreInfoUriMissing`, `moreInfoUriInvalid`, `moreInfoUriTooLarge`, `descriptionMissing`, `descriptionInvalid`, `descriptionTooLarge`, `titleMissing`, `titleInvalid`, `titleTooLarge`, `operandMissing`, `operandInvalid`, `operandTooLarge`, `settingNameMissing`, `settingNameInvalid`, `settingNameTooLarge`, `englishLocaleMissing`, `duplicateLocales`, `unrecognizedLocale`, `unknown`, `remediationStringsMissing`.</span></span>|
|<span data-ttu-id="079bf-118">message</span><span class="sxs-lookup"><span data-stu-id="079bf-118">message</span></span>|<span data-ttu-id="079bf-119">String</span><span class="sxs-lookup"><span data-stu-id="079bf-119">String</span></span>|<span data-ttu-id="079bf-120">错误消息。</span><span class="sxs-lookup"><span data-stu-id="079bf-120">Error message.</span></span> <span data-ttu-id="079bf-121">继承自[deviceComplianceScriptError](../resources/intune-deviceconfig-devicecompliancescripterror.md)</span><span class="sxs-lookup"><span data-stu-id="079bf-121">Inherited from [deviceComplianceScriptError](../resources/intune-deviceconfig-devicecompliancescripterror.md)</span></span>|
|<span data-ttu-id="079bf-122">settingName</span><span class="sxs-lookup"><span data-stu-id="079bf-122">settingName</span></span>|<span data-ttu-id="079bf-123">String</span><span class="sxs-lookup"><span data-stu-id="079bf-123">String</span></span>|<span data-ttu-id="079bf-124">为包含错误的规则设置名称。</span><span class="sxs-lookup"><span data-stu-id="079bf-124">Setting name for the rule with error.</span></span>|

## <a name="relationships"></a><span data-ttu-id="079bf-125">关系</span><span class="sxs-lookup"><span data-stu-id="079bf-125">Relationships</span></span>
<span data-ttu-id="079bf-126">无</span><span class="sxs-lookup"><span data-stu-id="079bf-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="079bf-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="079bf-127">JSON Representation</span></span>
<span data-ttu-id="079bf-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="079bf-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceComplianceScriptRuleError"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceScriptRuleError",
  "code": "String",
  "message": "String",
  "settingName": "String"
}
```



