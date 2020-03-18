---
title: deviceManagementApplicabilityRuleDeviceMode 资源类型
description: 尚未记录
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 099f6081366187e240bf8510fca30a548fea4fe3
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42792036"
---
# <a name="devicemanagementapplicabilityruledevicemode-resource-type"></a><span data-ttu-id="35d38-103">deviceManagementApplicabilityRuleDeviceMode 资源类型</span><span class="sxs-lookup"><span data-stu-id="35d38-103">deviceManagementApplicabilityRuleDeviceMode resource type</span></span>

> <span data-ttu-id="35d38-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="35d38-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="35d38-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="35d38-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35d38-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="35d38-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="35d38-107">属性</span><span class="sxs-lookup"><span data-stu-id="35d38-107">Properties</span></span>
|<span data-ttu-id="35d38-108">属性</span><span class="sxs-lookup"><span data-stu-id="35d38-108">Property</span></span>|<span data-ttu-id="35d38-109">类型</span><span class="sxs-lookup"><span data-stu-id="35d38-109">Type</span></span>|<span data-ttu-id="35d38-110">说明</span><span class="sxs-lookup"><span data-stu-id="35d38-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35d38-111">deviceMode</span><span class="sxs-lookup"><span data-stu-id="35d38-111">deviceMode</span></span>|[<span data-ttu-id="35d38-112">windows10DeviceModeType</span><span class="sxs-lookup"><span data-stu-id="35d38-112">windows10DeviceModeType</span></span>](../resources/intune-deviceconfig-windows10devicemodetype.md)|<span data-ttu-id="35d38-113">设备模式的适用性规则。</span><span class="sxs-lookup"><span data-stu-id="35d38-113">Applicability rule for device mode.</span></span> <span data-ttu-id="35d38-114">可取值为：`standardConfiguration`、`sModeConfiguration`。</span><span class="sxs-lookup"><span data-stu-id="35d38-114">Possible values are: `standardConfiguration`, `sModeConfiguration`.</span></span>|
|<span data-ttu-id="35d38-115">name</span><span class="sxs-lookup"><span data-stu-id="35d38-115">name</span></span>|<span data-ttu-id="35d38-116">String</span><span class="sxs-lookup"><span data-stu-id="35d38-116">String</span></span>|<span data-ttu-id="35d38-117">对象的名称。</span><span class="sxs-lookup"><span data-stu-id="35d38-117">Name for object.</span></span>|
|<span data-ttu-id="35d38-118">ruleType</span><span class="sxs-lookup"><span data-stu-id="35d38-118">ruleType</span></span>|[<span data-ttu-id="35d38-119">deviceManagementApplicabilityRuleType</span><span class="sxs-lookup"><span data-stu-id="35d38-119">deviceManagementApplicabilityRuleType</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruletype.md)|<span data-ttu-id="35d38-120">适用性规则类型。</span><span class="sxs-lookup"><span data-stu-id="35d38-120">Applicability Rule type.</span></span> <span data-ttu-id="35d38-121">可取值为：`include`、`exclude`。</span><span class="sxs-lookup"><span data-stu-id="35d38-121">Possible values are: `include`, `exclude`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="35d38-122">关系</span><span class="sxs-lookup"><span data-stu-id="35d38-122">Relationships</span></span>
<span data-ttu-id="35d38-123">无</span><span class="sxs-lookup"><span data-stu-id="35d38-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="35d38-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="35d38-124">JSON Representation</span></span>
<span data-ttu-id="35d38-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="35d38-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
  "deviceMode": "String",
  "name": "String",
  "ruleType": "String"
}
```



