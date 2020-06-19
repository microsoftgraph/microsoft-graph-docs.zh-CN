---
title: deviceComplianceScriptError 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7d37e750d60d50a166d7c9d89f3049959f33e5da
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44789330"
---
# <a name="devicecompliancescripterror-resource-type"></a><span data-ttu-id="64cfb-103">deviceComplianceScriptError 资源类型</span><span class="sxs-lookup"><span data-stu-id="64cfb-103">deviceComplianceScriptError resource type</span></span>

<span data-ttu-id="64cfb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64cfb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="64cfb-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="64cfb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64cfb-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="64cfb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64cfb-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="64cfb-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="64cfb-108">属性</span><span class="sxs-lookup"><span data-stu-id="64cfb-108">Properties</span></span>
|<span data-ttu-id="64cfb-109">属性</span><span class="sxs-lookup"><span data-stu-id="64cfb-109">Property</span></span>|<span data-ttu-id="64cfb-110">类型</span><span class="sxs-lookup"><span data-stu-id="64cfb-110">Type</span></span>|<span data-ttu-id="64cfb-111">说明</span><span class="sxs-lookup"><span data-stu-id="64cfb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64cfb-112">code</span><span class="sxs-lookup"><span data-stu-id="64cfb-112">code</span></span>|[<span data-ttu-id="64cfb-113">code</span><span class="sxs-lookup"><span data-stu-id="64cfb-113">code</span></span>](../resources/intune-deviceconfig-code.md)|<span data-ttu-id="64cfb-114">错误代码。</span><span class="sxs-lookup"><span data-stu-id="64cfb-114">Error code.</span></span> <span data-ttu-id="64cfb-115">可以取值为：、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、 `none` `jsonFileInvalid` `jsonFileMissing` `jsonFileTooLarge` `rulesMissing` `duplicateRules` `tooManyRulesSpecified` `operatorMissing` `operatorNotSupported` `datatypeMissing` `datatypeNotSupported` `operatorDataTypeCombinationNotSupported` `moreInfoUriMissing` `moreInfoUriInvalid` `moreInfoUriTooLarge` `descriptionMissing` `descriptionInvalid` `descriptionTooLarge` `titleMissing` `titleInvalid` `titleTooLarge` `operandMissing` `operandInvalid` `operandTooLarge` `settingNameMissing` `settingNameInvalid` `settingNameTooLarge` `englishLocaleMissing` `duplicateLocales` `unrecognizedLocale` `unknown` `remediationStringsMissing` 。</span><span class="sxs-lookup"><span data-stu-id="64cfb-115">Possible values are: `none`, `jsonFileInvalid`, `jsonFileMissing`, `jsonFileTooLarge`, `rulesMissing`, `duplicateRules`, `tooManyRulesSpecified`, `operatorMissing`, `operatorNotSupported`, `datatypeMissing`, `datatypeNotSupported`, `operatorDataTypeCombinationNotSupported`, `moreInfoUriMissing`, `moreInfoUriInvalid`, `moreInfoUriTooLarge`, `descriptionMissing`, `descriptionInvalid`, `descriptionTooLarge`, `titleMissing`, `titleInvalid`, `titleTooLarge`, `operandMissing`, `operandInvalid`, `operandTooLarge`, `settingNameMissing`, `settingNameInvalid`, `settingNameTooLarge`, `englishLocaleMissing`, `duplicateLocales`, `unrecognizedLocale`, `unknown`, `remediationStringsMissing`.</span></span>|
|<span data-ttu-id="64cfb-116">message</span><span class="sxs-lookup"><span data-stu-id="64cfb-116">message</span></span>|<span data-ttu-id="64cfb-117">String</span><span class="sxs-lookup"><span data-stu-id="64cfb-117">String</span></span>|<span data-ttu-id="64cfb-118">错误消息。</span><span class="sxs-lookup"><span data-stu-id="64cfb-118">Error message.</span></span>|

## <a name="relationships"></a><span data-ttu-id="64cfb-119">关系</span><span class="sxs-lookup"><span data-stu-id="64cfb-119">Relationships</span></span>
<span data-ttu-id="64cfb-120">无</span><span class="sxs-lookup"><span data-stu-id="64cfb-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="64cfb-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="64cfb-121">JSON Representation</span></span>
<span data-ttu-id="64cfb-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="64cfb-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceComplianceScriptError"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceScriptError",
  "code": "String",
  "message": "String"
}
```



