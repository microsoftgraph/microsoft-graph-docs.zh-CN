---
title: deviceComplianceScriptError 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fd8a801d34bb5a7ad07c7e769d25fa0a05e31a53
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49260255"
---
# <a name="devicecompliancescripterror-resource-type"></a><span data-ttu-id="54309-103">deviceComplianceScriptError 资源类型</span><span class="sxs-lookup"><span data-stu-id="54309-103">deviceComplianceScriptError resource type</span></span>

<span data-ttu-id="54309-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54309-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="54309-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="54309-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="54309-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="54309-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54309-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="54309-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="54309-108">属性</span><span class="sxs-lookup"><span data-stu-id="54309-108">Properties</span></span>
|<span data-ttu-id="54309-109">属性</span><span class="sxs-lookup"><span data-stu-id="54309-109">Property</span></span>|<span data-ttu-id="54309-110">类型</span><span class="sxs-lookup"><span data-stu-id="54309-110">Type</span></span>|<span data-ttu-id="54309-111">说明</span><span class="sxs-lookup"><span data-stu-id="54309-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54309-112">code</span><span class="sxs-lookup"><span data-stu-id="54309-112">code</span></span>|[<span data-ttu-id="54309-113">code</span><span class="sxs-lookup"><span data-stu-id="54309-113">code</span></span>](../resources/intune-deviceconfig-code.md)|<span data-ttu-id="54309-114">错误代码。</span><span class="sxs-lookup"><span data-stu-id="54309-114">Error code.</span></span> <span data-ttu-id="54309-115">可以取值为：、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、 `none` `jsonFileInvalid` `jsonFileMissing` `jsonFileTooLarge` `rulesMissing` `duplicateRules` `tooManyRulesSpecified` `operatorMissing` `operatorNotSupported` `datatypeMissing` `datatypeNotSupported` `operatorDataTypeCombinationNotSupported` `moreInfoUriMissing` `moreInfoUriInvalid` `moreInfoUriTooLarge` `descriptionMissing` `descriptionInvalid` `descriptionTooLarge` `titleMissing` `titleInvalid` `titleTooLarge` `operandMissing` `operandInvalid` `operandTooLarge` `settingNameMissing` `settingNameInvalid` `settingNameTooLarge` `englishLocaleMissing` `duplicateLocales` `unrecognizedLocale` `unknown` `remediationStringsMissing` 。</span><span class="sxs-lookup"><span data-stu-id="54309-115">Possible values are: `none`, `jsonFileInvalid`, `jsonFileMissing`, `jsonFileTooLarge`, `rulesMissing`, `duplicateRules`, `tooManyRulesSpecified`, `operatorMissing`, `operatorNotSupported`, `datatypeMissing`, `datatypeNotSupported`, `operatorDataTypeCombinationNotSupported`, `moreInfoUriMissing`, `moreInfoUriInvalid`, `moreInfoUriTooLarge`, `descriptionMissing`, `descriptionInvalid`, `descriptionTooLarge`, `titleMissing`, `titleInvalid`, `titleTooLarge`, `operandMissing`, `operandInvalid`, `operandTooLarge`, `settingNameMissing`, `settingNameInvalid`, `settingNameTooLarge`, `englishLocaleMissing`, `duplicateLocales`, `unrecognizedLocale`, `unknown`, `remediationStringsMissing`.</span></span>|
|<span data-ttu-id="54309-116">message</span><span class="sxs-lookup"><span data-stu-id="54309-116">message</span></span>|<span data-ttu-id="54309-117">String</span><span class="sxs-lookup"><span data-stu-id="54309-117">String</span></span>|<span data-ttu-id="54309-118">错误消息：</span><span class="sxs-lookup"><span data-stu-id="54309-118">Error message.</span></span>|

## <a name="relationships"></a><span data-ttu-id="54309-119">关系</span><span class="sxs-lookup"><span data-stu-id="54309-119">Relationships</span></span>
<span data-ttu-id="54309-120">无</span><span class="sxs-lookup"><span data-stu-id="54309-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="54309-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="54309-121">JSON Representation</span></span>
<span data-ttu-id="54309-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="54309-122">Here is a JSON representation of the resource.</span></span>
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




