---
title: deviceManagementConfigurationSettingGroupInstance 资源类型
description: 策略内的设置实例
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1ab5093675e8d1bc9b0796a5a937b9bed894ca24
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241264"
---
# <a name="devicemanagementconfigurationsettinggroupinstance-resource-type"></a><span data-ttu-id="c6c94-103">deviceManagementConfigurationSettingGroupInstance 资源类型</span><span class="sxs-lookup"><span data-stu-id="c6c94-103">deviceManagementConfigurationSettingGroupInstance resource type</span></span>

<span data-ttu-id="c6c94-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6c94-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c6c94-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c6c94-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c6c94-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c6c94-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6c94-107">策略内的设置实例</span><span class="sxs-lookup"><span data-stu-id="c6c94-107">Setting instance within policy</span></span>


<span data-ttu-id="c6c94-108">继承自 [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="c6c94-108">Inherits from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c6c94-109">属性</span><span class="sxs-lookup"><span data-stu-id="c6c94-109">Properties</span></span>
|<span data-ttu-id="c6c94-110">属性</span><span class="sxs-lookup"><span data-stu-id="c6c94-110">Property</span></span>|<span data-ttu-id="c6c94-111">类型</span><span class="sxs-lookup"><span data-stu-id="c6c94-111">Type</span></span>|<span data-ttu-id="c6c94-112">说明</span><span class="sxs-lookup"><span data-stu-id="c6c94-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6c94-113">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="c6c94-113">settingDefinitionId</span></span>|<span data-ttu-id="c6c94-114">String</span><span class="sxs-lookup"><span data-stu-id="c6c94-114">String</span></span>|<span data-ttu-id="c6c94-115">从[DeviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)继承的设置定义 Id</span><span class="sxs-lookup"><span data-stu-id="c6c94-115">Setting Definition Id Inherited from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="c6c94-116">关系</span><span class="sxs-lookup"><span data-stu-id="c6c94-116">Relationships</span></span>
<span data-ttu-id="c6c94-117">无</span><span class="sxs-lookup"><span data-stu-id="c6c94-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c6c94-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c6c94-118">JSON Representation</span></span>
<span data-ttu-id="c6c94-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c6c94-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingGroupInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingGroupInstance",
  "settingDefinitionId": "String"
}
```




