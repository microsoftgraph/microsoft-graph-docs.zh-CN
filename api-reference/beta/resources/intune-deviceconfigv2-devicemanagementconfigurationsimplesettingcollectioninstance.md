---
title: deviceManagementConfigurationSimpleSettingCollectionInstance 资源类型
description: 简单设置集合实例
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b0886b7665f1f3ce16780f2ecccc77635fd70cf3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241526"
---
# <a name="devicemanagementconfigurationsimplesettingcollectioninstance-resource-type"></a><span data-ttu-id="5968a-103">deviceManagementConfigurationSimpleSettingCollectionInstance 资源类型</span><span class="sxs-lookup"><span data-stu-id="5968a-103">deviceManagementConfigurationSimpleSettingCollectionInstance resource type</span></span>

<span data-ttu-id="5968a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5968a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5968a-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5968a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5968a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5968a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5968a-107">简单设置集合实例</span><span class="sxs-lookup"><span data-stu-id="5968a-107">Simple setting collection instance</span></span>


<span data-ttu-id="5968a-108">继承自 [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="5968a-108">Inherits from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5968a-109">属性</span><span class="sxs-lookup"><span data-stu-id="5968a-109">Properties</span></span>
|<span data-ttu-id="5968a-110">属性</span><span class="sxs-lookup"><span data-stu-id="5968a-110">Property</span></span>|<span data-ttu-id="5968a-111">类型</span><span class="sxs-lookup"><span data-stu-id="5968a-111">Type</span></span>|<span data-ttu-id="5968a-112">说明</span><span class="sxs-lookup"><span data-stu-id="5968a-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5968a-113">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="5968a-113">settingDefinitionId</span></span>|<span data-ttu-id="5968a-114">String</span><span class="sxs-lookup"><span data-stu-id="5968a-114">String</span></span>|<span data-ttu-id="5968a-115">从[DeviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)继承的设置定义 Id</span><span class="sxs-lookup"><span data-stu-id="5968a-115">Setting Definition Id Inherited from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>|
|<span data-ttu-id="5968a-116">simpleSettingCollectionValue</span><span class="sxs-lookup"><span data-stu-id="5968a-116">simpleSettingCollectionValue</span></span>|<span data-ttu-id="5968a-117">[deviceManagementConfigurationSimpleSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5968a-117">[deviceManagementConfigurationSimpleSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvalue.md) collection</span></span>|<span data-ttu-id="5968a-118">简单设置集合实例值</span><span class="sxs-lookup"><span data-stu-id="5968a-118">Simple setting collection instance value</span></span>|

## <a name="relationships"></a><span data-ttu-id="5968a-119">关系</span><span class="sxs-lookup"><span data-stu-id="5968a-119">Relationships</span></span>
<span data-ttu-id="5968a-120">无</span><span class="sxs-lookup"><span data-stu-id="5968a-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5968a-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5968a-121">JSON Representation</span></span>
<span data-ttu-id="5968a-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5968a-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingCollectionInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSimpleSettingCollectionInstance",
  "settingDefinitionId": "String",
  "simpleSettingCollectionValue": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValue",
      "value": "String"
    }
  ]
}
```




