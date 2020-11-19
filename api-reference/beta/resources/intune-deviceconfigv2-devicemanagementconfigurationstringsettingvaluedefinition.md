---
title: deviceManagementConfigurationStringSettingValueDefinition 资源类型
description: 字符串约束
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 03a96252cffabddd2acb613ff365fd16951fd55c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241538"
---
# <a name="devicemanagementconfigurationstringsettingvaluedefinition-resource-type"></a><span data-ttu-id="14068-103">deviceManagementConfigurationStringSettingValueDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="14068-103">deviceManagementConfigurationStringSettingValueDefinition resource type</span></span>

<span data-ttu-id="14068-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14068-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="14068-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="14068-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="14068-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="14068-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14068-107">字符串约束</span><span class="sxs-lookup"><span data-stu-id="14068-107">String constraints</span></span>


<span data-ttu-id="14068-108">继承自 [deviceManagementConfigurationSettingValueDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvaluedefinition.md)</span><span class="sxs-lookup"><span data-stu-id="14068-108">Inherits from [deviceManagementConfigurationSettingValueDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvaluedefinition.md)</span></span>

## <a name="properties"></a><span data-ttu-id="14068-109">属性</span><span class="sxs-lookup"><span data-stu-id="14068-109">Properties</span></span>
|<span data-ttu-id="14068-110">属性</span><span class="sxs-lookup"><span data-stu-id="14068-110">Property</span></span>|<span data-ttu-id="14068-111">类型</span><span class="sxs-lookup"><span data-stu-id="14068-111">Type</span></span>|<span data-ttu-id="14068-112">说明</span><span class="sxs-lookup"><span data-stu-id="14068-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14068-113">format</span><span class="sxs-lookup"><span data-stu-id="14068-113">format</span></span>|[<span data-ttu-id="14068-114">deviceManagementConfigurationStringFormat</span><span class="sxs-lookup"><span data-stu-id="14068-114">deviceManagementConfigurationStringFormat</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationstringformat.md)|<span data-ttu-id="14068-115">预定义的字符串格式。</span><span class="sxs-lookup"><span data-stu-id="14068-115">Pre-defined format of the string.</span></span> <span data-ttu-id="14068-116">可能的值为：、、、、、、、、、、、、、、 `none` `email` `guid` `ip` `base64` `url` `version` `xml` `date` `time` `binary` `regEx` `json` `dateTime` `surfaceHub` 。</span><span class="sxs-lookup"><span data-stu-id="14068-116">Possible values are: `none`, `email`, `guid`, `ip`, `base64`, `url`, `version`, `xml`, `date`, `time`, `binary`, `regEx`, `json`, `dateTime`, `surfaceHub`.</span></span>|
|<span data-ttu-id="14068-117">inputValidationSchema</span><span class="sxs-lookup"><span data-stu-id="14068-117">inputValidationSchema</span></span>|<span data-ttu-id="14068-118">String</span><span class="sxs-lookup"><span data-stu-id="14068-118">String</span></span>|<span data-ttu-id="14068-119">输入字符串应匹配的正则表达式或任何 xml 或 json 架构</span><span class="sxs-lookup"><span data-stu-id="14068-119">Regular expression or any xml or json schema that the input string should match</span></span>|
|<span data-ttu-id="14068-120">maximumLength</span><span class="sxs-lookup"><span data-stu-id="14068-120">maximumLength</span></span>|<span data-ttu-id="14068-121">Int64</span><span class="sxs-lookup"><span data-stu-id="14068-121">Int64</span></span>|<span data-ttu-id="14068-122">字符串的最大长度。</span><span class="sxs-lookup"><span data-stu-id="14068-122">Maximum length of string.</span></span> <span data-ttu-id="14068-123">有效值为0至87516</span><span class="sxs-lookup"><span data-stu-id="14068-123">Valid values 0 to 87516</span></span>|
|<span data-ttu-id="14068-124">Minimumheight</span><span class="sxs-lookup"><span data-stu-id="14068-124">minimumLength</span></span>|<span data-ttu-id="14068-125">Int64</span><span class="sxs-lookup"><span data-stu-id="14068-125">Int64</span></span>|<span data-ttu-id="14068-126">字符串的最小长度。</span><span class="sxs-lookup"><span data-stu-id="14068-126">Minimum length of string.</span></span> <span data-ttu-id="14068-127">有效值为0至87516</span><span class="sxs-lookup"><span data-stu-id="14068-127">Valid values 0 to 87516</span></span>|
|<span data-ttu-id="14068-128">isSecret</span><span class="sxs-lookup"><span data-stu-id="14068-128">isSecret</span></span>|<span data-ttu-id="14068-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="14068-129">Boolean</span></span>|<span data-ttu-id="14068-130">指定是否需要将设置视为机密。</span><span class="sxs-lookup"><span data-stu-id="14068-130">Specifies whether the setting needs to be treated as a secret.</span></span> <span data-ttu-id="14068-131">标记为 "是" 的设置将在传输过程中和 rest 中进行加密，并在 UX 中表示为星号时将显示为星号。</span><span class="sxs-lookup"><span data-stu-id="14068-131">Settings marked as yes will be encrypted in transit and at rest and will be displayed as asterisks when represented in the UX.</span></span>|

## <a name="relationships"></a><span data-ttu-id="14068-132">关系</span><span class="sxs-lookup"><span data-stu-id="14068-132">Relationships</span></span>
<span data-ttu-id="14068-133">无</span><span class="sxs-lookup"><span data-stu-id="14068-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="14068-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="14068-134">JSON Representation</span></span>
<span data-ttu-id="14068-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="14068-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationStringSettingValueDefinition",
  "format": "String",
  "inputValidationSchema": "String",
  "maximumLength": 1024,
  "minimumLength": 1024,
  "isSecret": true
}
```




