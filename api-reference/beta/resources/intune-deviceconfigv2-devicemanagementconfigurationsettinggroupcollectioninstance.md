---
title: deviceManagementConfigurationSettingGroupCollectionInstance 资源类型
description: 策略内的设置实例
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e639dca60ff57d577f44a1bab4bc0b4420e174b2
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241266"
---
# <a name="devicemanagementconfigurationsettinggroupcollectioninstance-resource-type"></a><span data-ttu-id="50715-103">deviceManagementConfigurationSettingGroupCollectionInstance 资源类型</span><span class="sxs-lookup"><span data-stu-id="50715-103">deviceManagementConfigurationSettingGroupCollectionInstance resource type</span></span>

<span data-ttu-id="50715-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50715-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="50715-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="50715-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50715-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="50715-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50715-107">策略内的设置实例</span><span class="sxs-lookup"><span data-stu-id="50715-107">Setting instance within policy</span></span>


<span data-ttu-id="50715-108">继承自 [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="50715-108">Inherits from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>

## <a name="properties"></a><span data-ttu-id="50715-109">属性</span><span class="sxs-lookup"><span data-stu-id="50715-109">Properties</span></span>
|<span data-ttu-id="50715-110">属性</span><span class="sxs-lookup"><span data-stu-id="50715-110">Property</span></span>|<span data-ttu-id="50715-111">类型</span><span class="sxs-lookup"><span data-stu-id="50715-111">Type</span></span>|<span data-ttu-id="50715-112">说明</span><span class="sxs-lookup"><span data-stu-id="50715-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50715-113">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="50715-113">settingDefinitionId</span></span>|<span data-ttu-id="50715-114">String</span><span class="sxs-lookup"><span data-stu-id="50715-114">String</span></span>|<span data-ttu-id="50715-115">从[DeviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)继承的设置定义 Id</span><span class="sxs-lookup"><span data-stu-id="50715-115">Setting Definition Id Inherited from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="50715-116">关系</span><span class="sxs-lookup"><span data-stu-id="50715-116">Relationships</span></span>
<span data-ttu-id="50715-117">无</span><span class="sxs-lookup"><span data-stu-id="50715-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="50715-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="50715-118">JSON Representation</span></span>
<span data-ttu-id="50715-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="50715-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingGroupCollectionInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingGroupCollectionInstance",
  "settingDefinitionId": "String"
}
```




