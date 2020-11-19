---
title: deviceManagementConfigurationIntegerSettingValueDefinition 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d4c2fdb6b26b67b6c61dcbba295933d0c3797500
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241421"
---
# <a name="devicemanagementconfigurationintegersettingvaluedefinition-resource-type"></a><span data-ttu-id="03735-103">deviceManagementConfigurationIntegerSettingValueDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="03735-103">deviceManagementConfigurationIntegerSettingValueDefinition resource type</span></span>

<span data-ttu-id="03735-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03735-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="03735-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="03735-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="03735-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="03735-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03735-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="03735-107">Not yet documented</span></span>


<span data-ttu-id="03735-108">继承自 [deviceManagementConfigurationSettingValueDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvaluedefinition.md)</span><span class="sxs-lookup"><span data-stu-id="03735-108">Inherits from [deviceManagementConfigurationSettingValueDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvaluedefinition.md)</span></span>

## <a name="properties"></a><span data-ttu-id="03735-109">属性</span><span class="sxs-lookup"><span data-stu-id="03735-109">Properties</span></span>
|<span data-ttu-id="03735-110">属性</span><span class="sxs-lookup"><span data-stu-id="03735-110">Property</span></span>|<span data-ttu-id="03735-111">类型</span><span class="sxs-lookup"><span data-stu-id="03735-111">Type</span></span>|<span data-ttu-id="03735-112">说明</span><span class="sxs-lookup"><span data-stu-id="03735-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03735-113">maximumValue</span><span class="sxs-lookup"><span data-stu-id="03735-113">maximumValue</span></span>|<span data-ttu-id="03735-114">Int64</span><span class="sxs-lookup"><span data-stu-id="03735-114">Int64</span></span>|<span data-ttu-id="03735-115">整数的最大允许值</span><span class="sxs-lookup"><span data-stu-id="03735-115">Maximum allowed value of the integer</span></span>|
|<span data-ttu-id="03735-116">minimumValue</span><span class="sxs-lookup"><span data-stu-id="03735-116">minimumValue</span></span>|<span data-ttu-id="03735-117">Int64</span><span class="sxs-lookup"><span data-stu-id="03735-117">Int64</span></span>|<span data-ttu-id="03735-118">整数允许的最小值</span><span class="sxs-lookup"><span data-stu-id="03735-118">Minimum allowed value of the integer</span></span>|

## <a name="relationships"></a><span data-ttu-id="03735-119">关系</span><span class="sxs-lookup"><span data-stu-id="03735-119">Relationships</span></span>
<span data-ttu-id="03735-120">无</span><span class="sxs-lookup"><span data-stu-id="03735-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="03735-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="03735-121">JSON Representation</span></span>
<span data-ttu-id="03735-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="03735-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationIntegerSettingValueDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationIntegerSettingValueDefinition",
  "maximumValue": 1024,
  "minimumValue": 1024
}
```




