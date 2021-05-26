---
title: deviceManagementConfigurationOptionDefinitionTemplate 资源类型
description: 选项定义模板
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b95ea51cab8bc3f56d7b5679743a4019e54eba54
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666511"
---
# <a name="devicemanagementconfigurationoptiondefinitiontemplate-resource-type"></a><span data-ttu-id="a2e64-103">deviceManagementConfigurationOptionDefinitionTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="a2e64-103">deviceManagementConfigurationOptionDefinitionTemplate resource type</span></span>

<span data-ttu-id="a2e64-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2e64-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a2e64-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a2e64-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a2e64-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a2e64-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2e64-107">选项定义模板</span><span class="sxs-lookup"><span data-stu-id="a2e64-107">Option Definition Template</span></span>

## <a name="properties"></a><span data-ttu-id="a2e64-108">属性</span><span class="sxs-lookup"><span data-stu-id="a2e64-108">Properties</span></span>
|<span data-ttu-id="a2e64-109">属性</span><span class="sxs-lookup"><span data-stu-id="a2e64-109">Property</span></span>|<span data-ttu-id="a2e64-110">类型</span><span class="sxs-lookup"><span data-stu-id="a2e64-110">Type</span></span>|<span data-ttu-id="a2e64-111">说明</span><span class="sxs-lookup"><span data-stu-id="a2e64-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2e64-112">itemId</span><span class="sxs-lookup"><span data-stu-id="a2e64-112">itemId</span></span>|<span data-ttu-id="a2e64-113">String</span><span class="sxs-lookup"><span data-stu-id="a2e64-113">String</span></span>|<span data-ttu-id="a2e64-114">Option ItemId</span><span class="sxs-lookup"><span data-stu-id="a2e64-114">Option ItemId</span></span>|
|<span data-ttu-id="a2e64-115">children</span><span class="sxs-lookup"><span data-stu-id="a2e64-115">children</span></span>|<span data-ttu-id="a2e64-116">[deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a2e64-116">[deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md) collection</span></span>|<span data-ttu-id="a2e64-117">选项子项</span><span class="sxs-lookup"><span data-stu-id="a2e64-117">Option Children</span></span>|

## <a name="relationships"></a><span data-ttu-id="a2e64-118">关系</span><span class="sxs-lookup"><span data-stu-id="a2e64-118">Relationships</span></span>
<span data-ttu-id="a2e64-119">无</span><span class="sxs-lookup"><span data-stu-id="a2e64-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a2e64-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a2e64-120">JSON Representation</span></span>
<span data-ttu-id="a2e64-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a2e64-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationOptionDefinitionTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationOptionDefinitionTemplate",
  "itemId": "String",
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
  ]
}
```




