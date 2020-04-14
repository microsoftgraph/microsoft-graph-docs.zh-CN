---
title: deviceManagementApplicabilityRuleDeviceMode 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 684dd5415d5ffa3c8884611efb1c9add8bdf0651
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43359659"
---
# <a name="devicemanagementapplicabilityruledevicemode-resource-type"></a><span data-ttu-id="1a9b8-103">deviceManagementApplicabilityRuleDeviceMode 资源类型</span><span class="sxs-lookup"><span data-stu-id="1a9b8-103">deviceManagementApplicabilityRuleDeviceMode resource type</span></span>

<span data-ttu-id="1a9b8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a9b8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1a9b8-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1a9b8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a9b8-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1a9b8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a9b8-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="1a9b8-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="1a9b8-108">属性</span><span class="sxs-lookup"><span data-stu-id="1a9b8-108">Properties</span></span>
|<span data-ttu-id="1a9b8-109">属性</span><span class="sxs-lookup"><span data-stu-id="1a9b8-109">Property</span></span>|<span data-ttu-id="1a9b8-110">类型</span><span class="sxs-lookup"><span data-stu-id="1a9b8-110">Type</span></span>|<span data-ttu-id="1a9b8-111">说明</span><span class="sxs-lookup"><span data-stu-id="1a9b8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a9b8-112">deviceMode</span><span class="sxs-lookup"><span data-stu-id="1a9b8-112">deviceMode</span></span>|[<span data-ttu-id="1a9b8-113">windows10DeviceModeType</span><span class="sxs-lookup"><span data-stu-id="1a9b8-113">windows10DeviceModeType</span></span>](../resources/intune-deviceconfig-windows10devicemodetype.md)|<span data-ttu-id="1a9b8-114">设备模式的适用性规则。</span><span class="sxs-lookup"><span data-stu-id="1a9b8-114">Applicability rule for device mode.</span></span> <span data-ttu-id="1a9b8-115">可取值为：`standardConfiguration`、`sModeConfiguration`。</span><span class="sxs-lookup"><span data-stu-id="1a9b8-115">Possible values are: `standardConfiguration`, `sModeConfiguration`.</span></span>|
|<span data-ttu-id="1a9b8-116">name</span><span class="sxs-lookup"><span data-stu-id="1a9b8-116">name</span></span>|<span data-ttu-id="1a9b8-117">字符串</span><span class="sxs-lookup"><span data-stu-id="1a9b8-117">String</span></span>|<span data-ttu-id="1a9b8-118">对象的名称。</span><span class="sxs-lookup"><span data-stu-id="1a9b8-118">Name for object.</span></span>|
|<span data-ttu-id="1a9b8-119">ruleType</span><span class="sxs-lookup"><span data-stu-id="1a9b8-119">ruleType</span></span>|[<span data-ttu-id="1a9b8-120">deviceManagementApplicabilityRuleType</span><span class="sxs-lookup"><span data-stu-id="1a9b8-120">deviceManagementApplicabilityRuleType</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruletype.md)|<span data-ttu-id="1a9b8-121">适用性规则类型。</span><span class="sxs-lookup"><span data-stu-id="1a9b8-121">Applicability Rule type.</span></span> <span data-ttu-id="1a9b8-122">可取值为：`include`、`exclude`。</span><span class="sxs-lookup"><span data-stu-id="1a9b8-122">Possible values are: `include`, `exclude`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a9b8-123">关系</span><span class="sxs-lookup"><span data-stu-id="1a9b8-123">Relationships</span></span>
<span data-ttu-id="1a9b8-124">无</span><span class="sxs-lookup"><span data-stu-id="1a9b8-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1a9b8-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1a9b8-125">JSON Representation</span></span>
<span data-ttu-id="1a9b8-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1a9b8-126">Here is a JSON representation of the resource.</span></span>
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



