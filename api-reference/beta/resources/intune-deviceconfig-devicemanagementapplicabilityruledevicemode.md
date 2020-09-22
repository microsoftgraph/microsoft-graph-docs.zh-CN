---
title: deviceManagementApplicabilityRuleDeviceMode 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 660263e729c4de0603f7d683a585981e0a4fd98f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985949"
---
# <a name="devicemanagementapplicabilityruledevicemode-resource-type"></a><span data-ttu-id="5e933-103">deviceManagementApplicabilityRuleDeviceMode 资源类型</span><span class="sxs-lookup"><span data-stu-id="5e933-103">deviceManagementApplicabilityRuleDeviceMode resource type</span></span>

<span data-ttu-id="5e933-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e933-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5e933-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5e933-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5e933-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5e933-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e933-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5e933-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="5e933-108">属性</span><span class="sxs-lookup"><span data-stu-id="5e933-108">Properties</span></span>
|<span data-ttu-id="5e933-109">属性</span><span class="sxs-lookup"><span data-stu-id="5e933-109">Property</span></span>|<span data-ttu-id="5e933-110">类型</span><span class="sxs-lookup"><span data-stu-id="5e933-110">Type</span></span>|<span data-ttu-id="5e933-111">说明</span><span class="sxs-lookup"><span data-stu-id="5e933-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e933-112">deviceMode</span><span class="sxs-lookup"><span data-stu-id="5e933-112">deviceMode</span></span>|[<span data-ttu-id="5e933-113">windows10DeviceModeType</span><span class="sxs-lookup"><span data-stu-id="5e933-113">windows10DeviceModeType</span></span>](../resources/intune-deviceconfig-windows10devicemodetype.md)|<span data-ttu-id="5e933-114">设备模式的适用性规则。</span><span class="sxs-lookup"><span data-stu-id="5e933-114">Applicability rule for device mode.</span></span> <span data-ttu-id="5e933-115">可取值为：`standardConfiguration`、`sModeConfiguration`。</span><span class="sxs-lookup"><span data-stu-id="5e933-115">Possible values are: `standardConfiguration`, `sModeConfiguration`.</span></span>|
|<span data-ttu-id="5e933-116">name</span><span class="sxs-lookup"><span data-stu-id="5e933-116">name</span></span>|<span data-ttu-id="5e933-117">String</span><span class="sxs-lookup"><span data-stu-id="5e933-117">String</span></span>|<span data-ttu-id="5e933-118">对象的名称。</span><span class="sxs-lookup"><span data-stu-id="5e933-118">Name for object.</span></span>|
|<span data-ttu-id="5e933-119">ruleType</span><span class="sxs-lookup"><span data-stu-id="5e933-119">ruleType</span></span>|[<span data-ttu-id="5e933-120">deviceManagementApplicabilityRuleType</span><span class="sxs-lookup"><span data-stu-id="5e933-120">deviceManagementApplicabilityRuleType</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruletype.md)|<span data-ttu-id="5e933-121">适用性规则类型。</span><span class="sxs-lookup"><span data-stu-id="5e933-121">Applicability Rule type.</span></span> <span data-ttu-id="5e933-122">可取值为：`include`、`exclude`。</span><span class="sxs-lookup"><span data-stu-id="5e933-122">Possible values are: `include`, `exclude`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5e933-123">关系</span><span class="sxs-lookup"><span data-stu-id="5e933-123">Relationships</span></span>
<span data-ttu-id="5e933-124">无</span><span class="sxs-lookup"><span data-stu-id="5e933-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5e933-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5e933-125">JSON Representation</span></span>
<span data-ttu-id="5e933-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5e933-126">Here is a JSON representation of the resource.</span></span>
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






