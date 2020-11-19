---
title: deviceManagementConfigurationIntegerSettingValue 资源类型
description: 简单设置值
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 23765f3dbfab6eb449d3f666e28fdfe11d470ef8
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241426"
---
# <a name="devicemanagementconfigurationintegersettingvalue-resource-type"></a><span data-ttu-id="b2b54-103">deviceManagementConfigurationIntegerSettingValue 资源类型</span><span class="sxs-lookup"><span data-stu-id="b2b54-103">deviceManagementConfigurationIntegerSettingValue resource type</span></span>

<span data-ttu-id="b2b54-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2b54-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b2b54-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b2b54-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2b54-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b2b54-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2b54-107">简单设置值</span><span class="sxs-lookup"><span data-stu-id="b2b54-107">Simple setting value</span></span>


<span data-ttu-id="b2b54-108">继承自 [deviceManagementConfigurationSimpleSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="b2b54-108">Inherits from [deviceManagementConfigurationSimpleSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvalue.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b2b54-109">属性</span><span class="sxs-lookup"><span data-stu-id="b2b54-109">Properties</span></span>
|<span data-ttu-id="b2b54-110">属性</span><span class="sxs-lookup"><span data-stu-id="b2b54-110">Property</span></span>|<span data-ttu-id="b2b54-111">类型</span><span class="sxs-lookup"><span data-stu-id="b2b54-111">Type</span></span>|<span data-ttu-id="b2b54-112">说明</span><span class="sxs-lookup"><span data-stu-id="b2b54-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2b54-113">值</span><span class="sxs-lookup"><span data-stu-id="b2b54-113">value</span></span>|<span data-ttu-id="b2b54-114">Int32</span><span class="sxs-lookup"><span data-stu-id="b2b54-114">Int32</span></span>|<span data-ttu-id="b2b54-115">整数设置的值。</span><span class="sxs-lookup"><span data-stu-id="b2b54-115">Value of the integer setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b2b54-116">关系</span><span class="sxs-lookup"><span data-stu-id="b2b54-116">Relationships</span></span>
<span data-ttu-id="b2b54-117">无</span><span class="sxs-lookup"><span data-stu-id="b2b54-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b2b54-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b2b54-118">JSON Representation</span></span>
<span data-ttu-id="b2b54-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b2b54-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationIntegerSettingValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationIntegerSettingValue",
  "value": 1024
}
```




