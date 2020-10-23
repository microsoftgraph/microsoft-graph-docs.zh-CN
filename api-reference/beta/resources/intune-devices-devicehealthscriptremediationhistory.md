---
title: deviceHealthScriptRemediationHistory 资源类型
description: 在给定日期之前通过设备运行状况脚本修正的设备数（上次修改时间）。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1ca94403decdc183748c8b147fae678e88aac264
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48697698"
---
# <a name="devicehealthscriptremediationhistory-resource-type"></a><span data-ttu-id="979a2-103">deviceHealthScriptRemediationHistory 资源类型</span><span class="sxs-lookup"><span data-stu-id="979a2-103">deviceHealthScriptRemediationHistory resource type</span></span>

<span data-ttu-id="979a2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="979a2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="979a2-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="979a2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="979a2-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="979a2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="979a2-107">在给定日期之前通过设备运行状况脚本修正的设备数（上次修改时间）。</span><span class="sxs-lookup"><span data-stu-id="979a2-107">The number of devices remediated by a device health script on a given date with the last modified time.</span></span>

## <a name="properties"></a><span data-ttu-id="979a2-108">属性</span><span class="sxs-lookup"><span data-stu-id="979a2-108">Properties</span></span>
|<span data-ttu-id="979a2-109">属性</span><span class="sxs-lookup"><span data-stu-id="979a2-109">Property</span></span>|<span data-ttu-id="979a2-110">类型</span><span class="sxs-lookup"><span data-stu-id="979a2-110">Type</span></span>|<span data-ttu-id="979a2-111">说明</span><span class="sxs-lookup"><span data-stu-id="979a2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="979a2-112">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="979a2-112">lastModifiedDateTime</span></span>|<span data-ttu-id="979a2-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="979a2-113">DateTimeOffset</span></span>|<span data-ttu-id="979a2-114">为 healthscript 计算结果历史记录的日期。</span><span class="sxs-lookup"><span data-stu-id="979a2-114">The date on which the results history is calculated for the healthscript.</span></span>|
|<span data-ttu-id="979a2-115">historyData</span><span class="sxs-lookup"><span data-stu-id="979a2-115">historyData</span></span>|<span data-ttu-id="979a2-116">[deviceHealthScriptRemediationHistoryData](../resources/intune-devices-devicehealthscriptremediationhistorydata.md) 集合</span><span class="sxs-lookup"><span data-stu-id="979a2-116">[deviceHealthScriptRemediationHistoryData](../resources/intune-devices-devicehealthscriptremediationhistorydata.md) collection</span></span>|<span data-ttu-id="979a2-117">在给定日期由设备运行状况脚本修正的设备的数量。</span><span class="sxs-lookup"><span data-stu-id="979a2-117">The number of devices remediated by the device health script on the given date.</span></span>|

## <a name="relationships"></a><span data-ttu-id="979a2-118">关系</span><span class="sxs-lookup"><span data-stu-id="979a2-118">Relationships</span></span>
<span data-ttu-id="979a2-119">无</span><span class="sxs-lookup"><span data-stu-id="979a2-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="979a2-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="979a2-120">JSON Representation</span></span>
<span data-ttu-id="979a2-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="979a2-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptRemediationHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRemediationHistory",
  "lastModifiedDateTime": "String (timestamp)",
  "historyData": [
    {
      "@odata.type": "microsoft.graph.deviceHealthScriptRemediationHistoryData",
      "date": "String (Date)",
      "remediatedDeviceCount": 1024,
      "noIssueDeviceCount": 1024
    }
  ]
}
```





