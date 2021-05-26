---
title: deviceManagementConfigurationSimpleSettingCollectionInstanceTemplate 资源类型
description: 简单设置集合实例模板
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4270296c68bccf831fd7dd9e0475b7e16695fc19
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52664914"
---
# <a name="devicemanagementconfigurationsimplesettingcollectioninstancetemplate-resource-type"></a><span data-ttu-id="fa649-103">deviceManagementConfigurationSimpleSettingCollectionInstanceTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="fa649-103">deviceManagementConfigurationSimpleSettingCollectionInstanceTemplate resource type</span></span>

<span data-ttu-id="fa649-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa649-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fa649-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fa649-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fa649-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fa649-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa649-107">简单设置集合实例模板</span><span class="sxs-lookup"><span data-stu-id="fa649-107">Simple Setting Collection Instance Template</span></span>


<span data-ttu-id="fa649-108">继承自 [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="fa649-108">Inherits from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fa649-109">属性</span><span class="sxs-lookup"><span data-stu-id="fa649-109">Properties</span></span>
|<span data-ttu-id="fa649-110">属性</span><span class="sxs-lookup"><span data-stu-id="fa649-110">Property</span></span>|<span data-ttu-id="fa649-111">类型</span><span class="sxs-lookup"><span data-stu-id="fa649-111">Type</span></span>|<span data-ttu-id="fa649-112">说明</span><span class="sxs-lookup"><span data-stu-id="fa649-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa649-113">settingInstanceTemplateId</span><span class="sxs-lookup"><span data-stu-id="fa649-113">settingInstanceTemplateId</span></span>|<span data-ttu-id="fa649-114">String</span><span class="sxs-lookup"><span data-stu-id="fa649-114">String</span></span>|<span data-ttu-id="fa649-115">设置实例模板 ID 继承自 [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="fa649-115">Setting Instance Template Id Inherited from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>|
|<span data-ttu-id="fa649-116">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="fa649-116">settingDefinitionId</span></span>|<span data-ttu-id="fa649-117">String</span><span class="sxs-lookup"><span data-stu-id="fa649-117">String</span></span>|<span data-ttu-id="fa649-118">设置定义 ID 继承自 [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="fa649-118">Setting Definition Id Inherited from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>|
|<span data-ttu-id="fa649-119">isRequired</span><span class="sxs-lookup"><span data-stu-id="fa649-119">isRequired</span></span>|<span data-ttu-id="fa649-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="fa649-120">Boolean</span></span>|<span data-ttu-id="fa649-121">指示策略是否必须指定此设置。</span><span class="sxs-lookup"><span data-stu-id="fa649-121">Indicates if a policy must specify this setting.</span></span> <span data-ttu-id="fa649-122">继承自 [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="fa649-122">Inherited from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>|
|<span data-ttu-id="fa649-123">simpleSettingCollectionValueTemplate</span><span class="sxs-lookup"><span data-stu-id="fa649-123">simpleSettingCollectionValueTemplate</span></span>|<span data-ttu-id="fa649-124">[deviceManagementConfigurationSimpleSettingValueTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvaluetemplate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fa649-124">[deviceManagementConfigurationSimpleSettingValueTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvaluetemplate.md) collection</span></span>|<span data-ttu-id="fa649-125">简单设置集合值模板</span><span class="sxs-lookup"><span data-stu-id="fa649-125">Simple Setting Collection Value Template</span></span>|
|<span data-ttu-id="fa649-126">allowUnmanagedValues</span><span class="sxs-lookup"><span data-stu-id="fa649-126">allowUnmanagedValues</span></span>|<span data-ttu-id="fa649-127">布尔值</span><span class="sxs-lookup"><span data-stu-id="fa649-127">Boolean</span></span>|<span data-ttu-id="fa649-128">链接策略可能会追加模板中不存在的值。</span><span class="sxs-lookup"><span data-stu-id="fa649-128">Linked policy may append values which are not present in the template.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fa649-129">关系</span><span class="sxs-lookup"><span data-stu-id="fa649-129">Relationships</span></span>
<span data-ttu-id="fa649-130">无</span><span class="sxs-lookup"><span data-stu-id="fa649-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fa649-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fa649-131">JSON Representation</span></span>
<span data-ttu-id="fa649-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fa649-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingCollectionInstanceTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSimpleSettingCollectionInstanceTemplate",
  "settingInstanceTemplateId": "String",
  "settingDefinitionId": "String",
  "isRequired": true,
  "simpleSettingCollectionValueTemplate": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueTemplate",
      "settingValueTemplateId": "String",
      "defaultValue": {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueConstantDefaultTemplate",
        "constantValue": "String"
      }
    }
  ],
  "allowUnmanagedValues": true
}
```




