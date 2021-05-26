---
title: deviceManagementConfigurationSimpleSettingValue 资源类型
description: 简单设置值
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1f56883a53cab24f9859e968c11827a7a104a776
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666707"
---
# <a name="devicemanagementconfigurationsimplesettingvalue-resource-type"></a><span data-ttu-id="b07bc-103">deviceManagementConfigurationSimpleSettingValue 资源类型</span><span class="sxs-lookup"><span data-stu-id="b07bc-103">deviceManagementConfigurationSimpleSettingValue resource type</span></span>

<span data-ttu-id="b07bc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b07bc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b07bc-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b07bc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b07bc-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b07bc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b07bc-107">简单设置值</span><span class="sxs-lookup"><span data-stu-id="b07bc-107">Simple setting value</span></span>


<span data-ttu-id="b07bc-108">继承自 [deviceManagementConfigurationSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="b07bc-108">Inherits from [deviceManagementConfigurationSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b07bc-109">属性</span><span class="sxs-lookup"><span data-stu-id="b07bc-109">Properties</span></span>
|<span data-ttu-id="b07bc-110">属性</span><span class="sxs-lookup"><span data-stu-id="b07bc-110">Property</span></span>|<span data-ttu-id="b07bc-111">类型</span><span class="sxs-lookup"><span data-stu-id="b07bc-111">Type</span></span>|<span data-ttu-id="b07bc-112">说明</span><span class="sxs-lookup"><span data-stu-id="b07bc-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b07bc-113">settingValueTemplateReference</span><span class="sxs-lookup"><span data-stu-id="b07bc-113">settingValueTemplateReference</span></span>|[<span data-ttu-id="b07bc-114">deviceManagementConfigurationSettingValueTemplateReference</span><span class="sxs-lookup"><span data-stu-id="b07bc-114">deviceManagementConfigurationSettingValueTemplateReference</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvaluetemplatereference.md)|<span data-ttu-id="b07bc-115">设置值模板引用 继承自 [deviceManagementConfigurationSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="b07bc-115">Setting value template reference Inherited from [deviceManagementConfigurationSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="b07bc-116">关系</span><span class="sxs-lookup"><span data-stu-id="b07bc-116">Relationships</span></span>
<span data-ttu-id="b07bc-117">无</span><span class="sxs-lookup"><span data-stu-id="b07bc-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b07bc-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b07bc-118">JSON Representation</span></span>
<span data-ttu-id="b07bc-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b07bc-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSimpleSettingValue",
  "settingValueTemplateReference": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
    "settingValueTemplateId": "String",
    "useTemplateDefault": true
  }
}
```




