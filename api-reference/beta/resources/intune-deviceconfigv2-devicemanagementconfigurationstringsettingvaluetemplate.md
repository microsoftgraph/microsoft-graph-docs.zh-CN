---
title: deviceManagementConfigurationStringSettingValueTemplate 资源类型
description: 字符串设置值模板
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: db9e15e7aae70b4023aaf9305ef533ea37597e3b
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666852"
---
# <a name="devicemanagementconfigurationstringsettingvaluetemplate-resource-type"></a><span data-ttu-id="6e6f3-103">deviceManagementConfigurationStringSettingValueTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="6e6f3-103">deviceManagementConfigurationStringSettingValueTemplate resource type</span></span>

<span data-ttu-id="6e6f3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e6f3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6e6f3-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6e6f3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6e6f3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6e6f3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e6f3-107">字符串设置值模板</span><span class="sxs-lookup"><span data-stu-id="6e6f3-107">String Setting Value Template</span></span>


<span data-ttu-id="6e6f3-108">继承自 [deviceManagementConfigurationSimpleSettingValueTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvaluetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="6e6f3-108">Inherits from [deviceManagementConfigurationSimpleSettingValueTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvaluetemplate.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6e6f3-109">属性</span><span class="sxs-lookup"><span data-stu-id="6e6f3-109">Properties</span></span>
|<span data-ttu-id="6e6f3-110">属性</span><span class="sxs-lookup"><span data-stu-id="6e6f3-110">Property</span></span>|<span data-ttu-id="6e6f3-111">类型</span><span class="sxs-lookup"><span data-stu-id="6e6f3-111">Type</span></span>|<span data-ttu-id="6e6f3-112">说明</span><span class="sxs-lookup"><span data-stu-id="6e6f3-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e6f3-113">settingValueTemplateId</span><span class="sxs-lookup"><span data-stu-id="6e6f3-113">settingValueTemplateId</span></span>|<span data-ttu-id="6e6f3-114">String</span><span class="sxs-lookup"><span data-stu-id="6e6f3-114">String</span></span>|<span data-ttu-id="6e6f3-115">设置值模板 ID 继承自 [deviceManagementConfigurationSimpleSettingValueTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvaluetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="6e6f3-115">Setting Value Template Id Inherited from [deviceManagementConfigurationSimpleSettingValueTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvaluetemplate.md)</span></span>|
|<span data-ttu-id="6e6f3-116">defaultValue</span><span class="sxs-lookup"><span data-stu-id="6e6f3-116">defaultValue</span></span>|[<span data-ttu-id="6e6f3-117">deviceManagementConfigurationStringSettingValueDefaultTemplate</span><span class="sxs-lookup"><span data-stu-id="6e6f3-117">deviceManagementConfigurationStringSettingValueDefaultTemplate</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationstringsettingvaluedefaulttemplate.md)|<span data-ttu-id="6e6f3-118">字符串设置值默认模板。</span><span class="sxs-lookup"><span data-stu-id="6e6f3-118">String Setting Value Default Template.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6e6f3-119">关系</span><span class="sxs-lookup"><span data-stu-id="6e6f3-119">Relationships</span></span>
<span data-ttu-id="6e6f3-120">无</span><span class="sxs-lookup"><span data-stu-id="6e6f3-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6e6f3-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6e6f3-121">JSON Representation</span></span>
<span data-ttu-id="6e6f3-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6e6f3-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationStringSettingValueTemplate",
  "settingValueTemplateId": "String",
  "defaultValue": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueConstantDefaultTemplate",
    "constantValue": "String"
  }
}
```




