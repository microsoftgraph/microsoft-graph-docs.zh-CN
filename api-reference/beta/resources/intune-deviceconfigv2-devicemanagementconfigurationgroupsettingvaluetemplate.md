---
title: deviceManagementConfigurationGroupSettingValueTemplate 资源类型
description: 组设置值模板
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 510abd102fda4721a387359afbeaa870abac6be8
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868428"
---
# <a name="devicemanagementconfigurationgroupsettingvaluetemplate-resource-type"></a><span data-ttu-id="f1dc4-103">deviceManagementConfigurationGroupSettingValueTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="f1dc4-103">deviceManagementConfigurationGroupSettingValueTemplate resource type</span></span>

<span data-ttu-id="f1dc4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1dc4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f1dc4-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f1dc4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1dc4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f1dc4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1dc4-107">组设置值模板</span><span class="sxs-lookup"><span data-stu-id="f1dc4-107">Group Setting Value Template</span></span>

## <a name="properties"></a><span data-ttu-id="f1dc4-108">属性</span><span class="sxs-lookup"><span data-stu-id="f1dc4-108">Properties</span></span>
|<span data-ttu-id="f1dc4-109">属性</span><span class="sxs-lookup"><span data-stu-id="f1dc4-109">Property</span></span>|<span data-ttu-id="f1dc4-110">类型</span><span class="sxs-lookup"><span data-stu-id="f1dc4-110">Type</span></span>|<span data-ttu-id="f1dc4-111">说明</span><span class="sxs-lookup"><span data-stu-id="f1dc4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1dc4-112">children</span><span class="sxs-lookup"><span data-stu-id="f1dc4-112">children</span></span>|<span data-ttu-id="f1dc4-113">[deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f1dc4-113">[deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md) collection</span></span>|<span data-ttu-id="f1dc4-114">组设置值子值</span><span class="sxs-lookup"><span data-stu-id="f1dc4-114">Group setting value children</span></span>|
|<span data-ttu-id="f1dc4-115">settingValueTemplateId</span><span class="sxs-lookup"><span data-stu-id="f1dc4-115">settingValueTemplateId</span></span>|<span data-ttu-id="f1dc4-116">String</span><span class="sxs-lookup"><span data-stu-id="f1dc4-116">String</span></span>|<span data-ttu-id="f1dc4-117">设置值模板 ID</span><span class="sxs-lookup"><span data-stu-id="f1dc4-117">Setting Value Template Id</span></span>|

## <a name="relationships"></a><span data-ttu-id="f1dc4-118">关系</span><span class="sxs-lookup"><span data-stu-id="f1dc4-118">Relationships</span></span>
<span data-ttu-id="f1dc4-119">无</span><span class="sxs-lookup"><span data-stu-id="f1dc4-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f1dc4-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f1dc4-120">JSON Representation</span></span>
<span data-ttu-id="f1dc4-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f1dc4-121">Here is a JSON representation of the resource.</span></span>
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
        "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingValueTemplate",
        "settingValueTemplateId": "String"
      }
    }
  ],
  "settingValueTemplateId": "String"
}
```




