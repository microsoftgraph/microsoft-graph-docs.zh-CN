---
title: deviceManagementApplicabilityRuleDeviceMode 资源类型
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8465f9276e573a44c2b7d80663d1de66bed83bef
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "35002523"
---
# <a name="devicemanagementapplicabilityruledevicemode-resource-type"></a><span data-ttu-id="49853-103">deviceManagementApplicabilityRuleDeviceMode 资源类型</span><span class="sxs-lookup"><span data-stu-id="49853-103">deviceManagementApplicabilityRuleDeviceMode resource type</span></span>

> <span data-ttu-id="49853-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="49853-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49853-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="49853-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49853-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="49853-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="49853-107">属性</span><span class="sxs-lookup"><span data-stu-id="49853-107">Properties</span></span>
|<span data-ttu-id="49853-108">属性</span><span class="sxs-lookup"><span data-stu-id="49853-108">Property</span></span>|<span data-ttu-id="49853-109">类型</span><span class="sxs-lookup"><span data-stu-id="49853-109">Type</span></span>|<span data-ttu-id="49853-110">说明</span><span class="sxs-lookup"><span data-stu-id="49853-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49853-111">deviceMode</span><span class="sxs-lookup"><span data-stu-id="49853-111">deviceMode</span></span>|[<span data-ttu-id="49853-112">windows10DeviceModeType</span><span class="sxs-lookup"><span data-stu-id="49853-112">windows10DeviceModeType</span></span>](../resources/intune-deviceconfig-windows10devicemodetype.md)|<span data-ttu-id="49853-113">设备模式的适用性规则。</span><span class="sxs-lookup"><span data-stu-id="49853-113">Applicability rule for device mode.</span></span> <span data-ttu-id="49853-114">可取值为：`standardConfiguration`、`sModeConfiguration`。</span><span class="sxs-lookup"><span data-stu-id="49853-114">Possible values are: `standardConfiguration`, `sModeConfiguration`.</span></span>|
|<span data-ttu-id="49853-115">name</span><span class="sxs-lookup"><span data-stu-id="49853-115">name</span></span>|<span data-ttu-id="49853-116">String</span><span class="sxs-lookup"><span data-stu-id="49853-116">String</span></span>|<span data-ttu-id="49853-117">对象的名称。</span><span class="sxs-lookup"><span data-stu-id="49853-117">Name for object.</span></span>|
|<span data-ttu-id="49853-118">ruleType</span><span class="sxs-lookup"><span data-stu-id="49853-118">ruleType</span></span>|[<span data-ttu-id="49853-119">deviceManagementApplicabilityRuleType</span><span class="sxs-lookup"><span data-stu-id="49853-119">deviceManagementApplicabilityRuleType</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruletype.md)|<span data-ttu-id="49853-120">适用性规则类型。</span><span class="sxs-lookup"><span data-stu-id="49853-120">Applicability Rule type.</span></span> <span data-ttu-id="49853-121">可取值为：`include`、`exclude`。</span><span class="sxs-lookup"><span data-stu-id="49853-121">Possible values are: `include`, `exclude`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="49853-122">关系</span><span class="sxs-lookup"><span data-stu-id="49853-122">Relationships</span></span>
<span data-ttu-id="49853-123">无</span><span class="sxs-lookup"><span data-stu-id="49853-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="49853-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="49853-124">JSON Representation</span></span>
<span data-ttu-id="49853-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="49853-125">Here is a JSON representation of the resource.</span></span>
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





