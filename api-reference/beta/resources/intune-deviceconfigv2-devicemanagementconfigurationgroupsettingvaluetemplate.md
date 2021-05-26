---
title: deviceManagementConfigurationGroupSettingValueTemplate 资源类型
description: 组设置值模板
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: aa840fe5755955d8d1649f64f4b0ea610bd53cd0
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666532"
---
# <a name="devicemanagementconfigurationgroupsettingvaluetemplate-resource-type"></a><span data-ttu-id="fb688-103">deviceManagementConfigurationGroupSettingValueTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="fb688-103">deviceManagementConfigurationGroupSettingValueTemplate resource type</span></span>

<span data-ttu-id="fb688-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb688-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fb688-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fb688-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fb688-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fb688-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb688-107">组设置值模板</span><span class="sxs-lookup"><span data-stu-id="fb688-107">Group Setting Value Template</span></span>

## <a name="properties"></a><span data-ttu-id="fb688-108">属性</span><span class="sxs-lookup"><span data-stu-id="fb688-108">Properties</span></span>
|<span data-ttu-id="fb688-109">属性</span><span class="sxs-lookup"><span data-stu-id="fb688-109">Property</span></span>|<span data-ttu-id="fb688-110">类型</span><span class="sxs-lookup"><span data-stu-id="fb688-110">Type</span></span>|<span data-ttu-id="fb688-111">说明</span><span class="sxs-lookup"><span data-stu-id="fb688-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb688-112">children</span><span class="sxs-lookup"><span data-stu-id="fb688-112">children</span></span>|<span data-ttu-id="fb688-113">[deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fb688-113">[deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md) collection</span></span>|<span data-ttu-id="fb688-114">组设置值子值</span><span class="sxs-lookup"><span data-stu-id="fb688-114">Group setting value children</span></span>|
|<span data-ttu-id="fb688-115">settingValueTemplateId</span><span class="sxs-lookup"><span data-stu-id="fb688-115">settingValueTemplateId</span></span>|<span data-ttu-id="fb688-116">String</span><span class="sxs-lookup"><span data-stu-id="fb688-116">String</span></span>|<span data-ttu-id="fb688-117">设置值模板 ID</span><span class="sxs-lookup"><span data-stu-id="fb688-117">Setting Value Template Id</span></span>|

## <a name="relationships"></a><span data-ttu-id="fb688-118">关系</span><span class="sxs-lookup"><span data-stu-id="fb688-118">Relationships</span></span>
<span data-ttu-id="fb688-119">无</span><span class="sxs-lookup"><span data-stu-id="fb688-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fb688-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fb688-120">JSON Representation</span></span>
<span data-ttu-id="fb688-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fb688-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationGroupSettingValueTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationGroupSettingValueTemplate",
  "children": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingInstanceTemplate",
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
  ],
  "settingValueTemplateId": "String"
}
```




