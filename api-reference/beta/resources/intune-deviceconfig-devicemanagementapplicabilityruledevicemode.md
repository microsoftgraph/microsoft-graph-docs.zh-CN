---
title: deviceManagementApplicabilityRuleDeviceMode 资源类型
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f53d9f676dd50c49fc5222f50c24c2c9a6d08e22
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332860"
---
# <a name="devicemanagementapplicabilityruledevicemode-resource-type"></a><span data-ttu-id="fd9dc-103">deviceManagementApplicabilityRuleDeviceMode 资源类型</span><span class="sxs-lookup"><span data-stu-id="fd9dc-103">deviceManagementApplicabilityRuleDeviceMode resource type</span></span>

> <span data-ttu-id="fd9dc-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fd9dc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fd9dc-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fd9dc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd9dc-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="fd9dc-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="fd9dc-107">属性</span><span class="sxs-lookup"><span data-stu-id="fd9dc-107">Properties</span></span>
|<span data-ttu-id="fd9dc-108">属性</span><span class="sxs-lookup"><span data-stu-id="fd9dc-108">Property</span></span>|<span data-ttu-id="fd9dc-109">类型</span><span class="sxs-lookup"><span data-stu-id="fd9dc-109">Type</span></span>|<span data-ttu-id="fd9dc-110">说明</span><span class="sxs-lookup"><span data-stu-id="fd9dc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd9dc-111">deviceMode</span><span class="sxs-lookup"><span data-stu-id="fd9dc-111">deviceMode</span></span>|[<span data-ttu-id="fd9dc-112">windows10DeviceModeType</span><span class="sxs-lookup"><span data-stu-id="fd9dc-112">windows10DeviceModeType</span></span>](../resources/intune-deviceconfig-windows10devicemodetype.md)|<span data-ttu-id="fd9dc-113">设备模式的适用性规则。</span><span class="sxs-lookup"><span data-stu-id="fd9dc-113">Applicability rule for device mode.</span></span> <span data-ttu-id="fd9dc-114">可取值为：`standardConfiguration`、`sModeConfiguration`。</span><span class="sxs-lookup"><span data-stu-id="fd9dc-114">Possible values are: `standardConfiguration`, `sModeConfiguration`.</span></span>|
|<span data-ttu-id="fd9dc-115">name</span><span class="sxs-lookup"><span data-stu-id="fd9dc-115">name</span></span>|<span data-ttu-id="fd9dc-116">String</span><span class="sxs-lookup"><span data-stu-id="fd9dc-116">String</span></span>|<span data-ttu-id="fd9dc-117">对象的名称。</span><span class="sxs-lookup"><span data-stu-id="fd9dc-117">Name for object.</span></span>|
|<span data-ttu-id="fd9dc-118">ruleType</span><span class="sxs-lookup"><span data-stu-id="fd9dc-118">ruleType</span></span>|[<span data-ttu-id="fd9dc-119">deviceManagementApplicabilityRuleType</span><span class="sxs-lookup"><span data-stu-id="fd9dc-119">deviceManagementApplicabilityRuleType</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruletype.md)|<span data-ttu-id="fd9dc-120">适用性规则类型。</span><span class="sxs-lookup"><span data-stu-id="fd9dc-120">Applicability Rule type.</span></span> <span data-ttu-id="fd9dc-121">可取值为：`include`、`exclude`。</span><span class="sxs-lookup"><span data-stu-id="fd9dc-121">Possible values are: `include`, `exclude`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fd9dc-122">关系</span><span class="sxs-lookup"><span data-stu-id="fd9dc-122">Relationships</span></span>
<span data-ttu-id="fd9dc-123">无</span><span class="sxs-lookup"><span data-stu-id="fd9dc-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fd9dc-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fd9dc-124">JSON Representation</span></span>
<span data-ttu-id="fd9dc-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fd9dc-125">Here is a JSON representation of the resource.</span></span>
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



