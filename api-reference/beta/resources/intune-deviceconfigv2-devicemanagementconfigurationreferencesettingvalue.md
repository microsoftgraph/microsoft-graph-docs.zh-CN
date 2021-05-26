---
title: deviceManagementConfigurationReferenceSettingValue 资源类型
description: ReferenceSettingValue 的模型
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1656b3e50094a55b4f2fe9ad422bbd54bd62bd6b
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666455"
---
# <a name="devicemanagementconfigurationreferencesettingvalue-resource-type"></a><span data-ttu-id="5514c-103">deviceManagementConfigurationReferenceSettingValue 资源类型</span><span class="sxs-lookup"><span data-stu-id="5514c-103">deviceManagementConfigurationReferenceSettingValue resource type</span></span>

<span data-ttu-id="5514c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5514c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5514c-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5514c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5514c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5514c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5514c-107">ReferenceSettingValue 的模型</span><span class="sxs-lookup"><span data-stu-id="5514c-107">Model for ReferenceSettingValue</span></span>


<span data-ttu-id="5514c-108">继承自 [deviceManagementConfigurationStringSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationstringsettingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="5514c-108">Inherits from [deviceManagementConfigurationStringSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationstringsettingvalue.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5514c-109">属性</span><span class="sxs-lookup"><span data-stu-id="5514c-109">Properties</span></span>
|<span data-ttu-id="5514c-110">属性</span><span class="sxs-lookup"><span data-stu-id="5514c-110">Property</span></span>|<span data-ttu-id="5514c-111">类型</span><span class="sxs-lookup"><span data-stu-id="5514c-111">Type</span></span>|<span data-ttu-id="5514c-112">说明</span><span class="sxs-lookup"><span data-stu-id="5514c-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5514c-113">settingValueTemplateReference</span><span class="sxs-lookup"><span data-stu-id="5514c-113">settingValueTemplateReference</span></span>|[<span data-ttu-id="5514c-114">deviceManagementConfigurationSettingValueTemplateReference</span><span class="sxs-lookup"><span data-stu-id="5514c-114">deviceManagementConfigurationSettingValueTemplateReference</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvaluetemplatereference.md)|<span data-ttu-id="5514c-115">设置值模板引用 继承自 [deviceManagementConfigurationSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="5514c-115">Setting value template reference Inherited from [deviceManagementConfigurationSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)</span></span>|
|<span data-ttu-id="5514c-116">value</span><span class="sxs-lookup"><span data-stu-id="5514c-116">value</span></span>|<span data-ttu-id="5514c-117">String</span><span class="sxs-lookup"><span data-stu-id="5514c-117">String</span></span>|<span data-ttu-id="5514c-118">字符串设置的值。</span><span class="sxs-lookup"><span data-stu-id="5514c-118">Value of the string setting.</span></span> <span data-ttu-id="5514c-119">继承自 [deviceManagementConfigurationStringSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationstringsettingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="5514c-119">Inherited from [deviceManagementConfigurationStringSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationstringsettingvalue.md)</span></span>|
|<span data-ttu-id="5514c-120">note</span><span class="sxs-lookup"><span data-stu-id="5514c-120">note</span></span>|<span data-ttu-id="5514c-121">String</span><span class="sxs-lookup"><span data-stu-id="5514c-121">String</span></span>|<span data-ttu-id="5514c-122">管理员可用于放入一些上下文信息的注释</span><span class="sxs-lookup"><span data-stu-id="5514c-122">A note that admin can use to put some contextual information</span></span>|

## <a name="relationships"></a><span data-ttu-id="5514c-123">关系</span><span class="sxs-lookup"><span data-stu-id="5514c-123">Relationships</span></span>
<span data-ttu-id="5514c-124">无</span><span class="sxs-lookup"><span data-stu-id="5514c-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5514c-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5514c-125">JSON Representation</span></span>
<span data-ttu-id="5514c-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5514c-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationReferenceSettingValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationReferenceSettingValue",
  "settingValueTemplateReference": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
    "settingValueTemplateId": "String",
    "useTemplateDefault": true
  },
  "value": "String",
  "note": "String"
}
```




