---
title: deviceComplianceScriptError 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c0ea8bf7c882d7a31c4f4477c7d7b74994676497
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026780"
---
# <a name="devicecompliancescripterror-resource-type"></a><span data-ttu-id="3120c-103">deviceComplianceScriptError 资源类型</span><span class="sxs-lookup"><span data-stu-id="3120c-103">deviceComplianceScriptError resource type</span></span>

<span data-ttu-id="3120c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3120c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3120c-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3120c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3120c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3120c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3120c-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3120c-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="3120c-108">属性</span><span class="sxs-lookup"><span data-stu-id="3120c-108">Properties</span></span>
|<span data-ttu-id="3120c-109">属性</span><span class="sxs-lookup"><span data-stu-id="3120c-109">Property</span></span>|<span data-ttu-id="3120c-110">类型</span><span class="sxs-lookup"><span data-stu-id="3120c-110">Type</span></span>|<span data-ttu-id="3120c-111">说明</span><span class="sxs-lookup"><span data-stu-id="3120c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3120c-112">code</span><span class="sxs-lookup"><span data-stu-id="3120c-112">code</span></span>|[<span data-ttu-id="3120c-113">code</span><span class="sxs-lookup"><span data-stu-id="3120c-113">code</span></span>](../resources/intune-deviceconfig-code.md)|<span data-ttu-id="3120c-114">错误代码。</span><span class="sxs-lookup"><span data-stu-id="3120c-114">Error code.</span></span> <span data-ttu-id="3120c-115">可以取值为：、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、 `none` `jsonFileInvalid` `jsonFileMissing` `jsonFileTooLarge` `rulesMissing` `duplicateRules` `tooManyRulesSpecified` `operatorMissing` `operatorNotSupported` `datatypeMissing` `datatypeNotSupported` `operatorDataTypeCombinationNotSupported` `moreInfoUriMissing` `moreInfoUriInvalid` `moreInfoUriTooLarge` `descriptionMissing` `descriptionInvalid` `descriptionTooLarge` `titleMissing` `titleInvalid` `titleTooLarge` `operandMissing` `operandInvalid` `operandTooLarge` `settingNameMissing` `settingNameInvalid` `settingNameTooLarge` `englishLocaleMissing` `duplicateLocales` `unrecognizedLocale` `unknown` `remediationStringsMissing` 。</span><span class="sxs-lookup"><span data-stu-id="3120c-115">Possible values are: `none`, `jsonFileInvalid`, `jsonFileMissing`, `jsonFileTooLarge`, `rulesMissing`, `duplicateRules`, `tooManyRulesSpecified`, `operatorMissing`, `operatorNotSupported`, `datatypeMissing`, `datatypeNotSupported`, `operatorDataTypeCombinationNotSupported`, `moreInfoUriMissing`, `moreInfoUriInvalid`, `moreInfoUriTooLarge`, `descriptionMissing`, `descriptionInvalid`, `descriptionTooLarge`, `titleMissing`, `titleInvalid`, `titleTooLarge`, `operandMissing`, `operandInvalid`, `operandTooLarge`, `settingNameMissing`, `settingNameInvalid`, `settingNameTooLarge`, `englishLocaleMissing`, `duplicateLocales`, `unrecognizedLocale`, `unknown`, `remediationStringsMissing`.</span></span>|
|<span data-ttu-id="3120c-116">message</span><span class="sxs-lookup"><span data-stu-id="3120c-116">message</span></span>|<span data-ttu-id="3120c-117">String</span><span class="sxs-lookup"><span data-stu-id="3120c-117">String</span></span>|<span data-ttu-id="3120c-118">错误消息。</span><span class="sxs-lookup"><span data-stu-id="3120c-118">Error message.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3120c-119">关系</span><span class="sxs-lookup"><span data-stu-id="3120c-119">Relationships</span></span>
<span data-ttu-id="3120c-120">无</span><span class="sxs-lookup"><span data-stu-id="3120c-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3120c-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3120c-121">JSON Representation</span></span>
<span data-ttu-id="3120c-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3120c-122">Here is a JSON representation of the resource.</span></span>
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






