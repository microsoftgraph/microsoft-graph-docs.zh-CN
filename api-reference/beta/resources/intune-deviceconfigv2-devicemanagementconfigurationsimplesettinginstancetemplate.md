---
title: deviceManagementConfigurationSimpleSettingInstanceTemplate 资源类型
description: 简单设置实例模板
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 74c1e599aecadcb8c6181c39cc0691f8b2e5aec5
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666714"
---
# <a name="devicemanagementconfigurationsimplesettinginstancetemplate-resource-type"></a><span data-ttu-id="0ee2f-103">deviceManagementConfigurationSimpleSettingInstanceTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="0ee2f-103">deviceManagementConfigurationSimpleSettingInstanceTemplate resource type</span></span>

<span data-ttu-id="0ee2f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ee2f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0ee2f-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0ee2f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0ee2f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0ee2f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ee2f-107">简单设置实例模板</span><span class="sxs-lookup"><span data-stu-id="0ee2f-107">Simple Setting Instance Template</span></span>


<span data-ttu-id="0ee2f-108">继承自 [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="0ee2f-108">Inherits from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0ee2f-109">属性</span><span class="sxs-lookup"><span data-stu-id="0ee2f-109">Properties</span></span>
|<span data-ttu-id="0ee2f-110">属性</span><span class="sxs-lookup"><span data-stu-id="0ee2f-110">Property</span></span>|<span data-ttu-id="0ee2f-111">类型</span><span class="sxs-lookup"><span data-stu-id="0ee2f-111">Type</span></span>|<span data-ttu-id="0ee2f-112">说明</span><span class="sxs-lookup"><span data-stu-id="0ee2f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ee2f-113">settingInstanceTemplateId</span><span class="sxs-lookup"><span data-stu-id="0ee2f-113">settingInstanceTemplateId</span></span>|<span data-ttu-id="0ee2f-114">String</span><span class="sxs-lookup"><span data-stu-id="0ee2f-114">String</span></span>|<span data-ttu-id="0ee2f-115">设置实例模板 ID 继承自 [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="0ee2f-115">Setting Instance Template Id Inherited from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>|
|<span data-ttu-id="0ee2f-116">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="0ee2f-116">settingDefinitionId</span></span>|<span data-ttu-id="0ee2f-117">String</span><span class="sxs-lookup"><span data-stu-id="0ee2f-117">String</span></span>|<span data-ttu-id="0ee2f-118">设置定义 ID 继承自 [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="0ee2f-118">Setting Definition Id Inherited from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>|
|<span data-ttu-id="0ee2f-119">isRequired</span><span class="sxs-lookup"><span data-stu-id="0ee2f-119">isRequired</span></span>|<span data-ttu-id="0ee2f-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ee2f-120">Boolean</span></span>|<span data-ttu-id="0ee2f-121">指示策略是否必须指定此设置。</span><span class="sxs-lookup"><span data-stu-id="0ee2f-121">Indicates if a policy must specify this setting.</span></span> <span data-ttu-id="0ee2f-122">继承自 [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="0ee2f-122">Inherited from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>|
|<span data-ttu-id="0ee2f-123">simpleSettingValueTemplate</span><span class="sxs-lookup"><span data-stu-id="0ee2f-123">simpleSettingValueTemplate</span></span>|[<span data-ttu-id="0ee2f-124">deviceManagementConfigurationSimpleSettingValueTemplate</span><span class="sxs-lookup"><span data-stu-id="0ee2f-124">deviceManagementConfigurationSimpleSettingValueTemplate</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvaluetemplate.md)|<span data-ttu-id="0ee2f-125">简单设置值模板</span><span class="sxs-lookup"><span data-stu-id="0ee2f-125">Simple Setting Value Template</span></span>|

## <a name="relationships"></a><span data-ttu-id="0ee2f-126">关系</span><span class="sxs-lookup"><span data-stu-id="0ee2f-126">Relationships</span></span>
<span data-ttu-id="0ee2f-127">无</span><span class="sxs-lookup"><span data-stu-id="0ee2f-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0ee2f-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0ee2f-128">JSON Representation</span></span>
<span data-ttu-id="0ee2f-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0ee2f-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingInstanceTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSimpleSettingInstanceTemplate",
  "settingInstanceTemplateId": "String",
  "settingDefinitionId": "String",
  "isRequired": true,
  "simpleSettingValueTemplate": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueTemplate",
    "settingValueTemplateId": "String",
    "defaultValue": {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueConstantDefaultTemplate",
      "constantValue": "String"
    }
  }
}
```




