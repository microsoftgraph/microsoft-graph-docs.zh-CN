---
title: deviceHealthScriptRemediationHistoryData 资源类型
description: 给定日期设备运行状况脚本修正的设备数量。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b9c04485659482d3f3ad28e3242bfb90b069a1d7
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48693736"
---
# <a name="devicehealthscriptremediationhistorydata-resource-type"></a><span data-ttu-id="cddd8-103">deviceHealthScriptRemediationHistoryData 资源类型</span><span class="sxs-lookup"><span data-stu-id="cddd8-103">deviceHealthScriptRemediationHistoryData resource type</span></span>

<span data-ttu-id="cddd8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cddd8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cddd8-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cddd8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cddd8-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cddd8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cddd8-107">给定日期设备运行状况脚本修正的设备数量。</span><span class="sxs-lookup"><span data-stu-id="cddd8-107">The number of devices remediated by a device health script on a given date.</span></span>

## <a name="properties"></a><span data-ttu-id="cddd8-108">属性</span><span class="sxs-lookup"><span data-stu-id="cddd8-108">Properties</span></span>
|<span data-ttu-id="cddd8-109">属性</span><span class="sxs-lookup"><span data-stu-id="cddd8-109">Property</span></span>|<span data-ttu-id="cddd8-110">类型</span><span class="sxs-lookup"><span data-stu-id="cddd8-110">Type</span></span>|<span data-ttu-id="cddd8-111">说明</span><span class="sxs-lookup"><span data-stu-id="cddd8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cddd8-112">date</span><span class="sxs-lookup"><span data-stu-id="cddd8-112">date</span></span>|<span data-ttu-id="cddd8-113">Date</span><span class="sxs-lookup"><span data-stu-id="cddd8-113">Date</span></span>|<span data-ttu-id="cddd8-114">设备运行状况脚本修正设备的日期。</span><span class="sxs-lookup"><span data-stu-id="cddd8-114">The date on which devices were remediated by the device health script.</span></span>|
|<span data-ttu-id="cddd8-115">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cddd8-115">remediatedDeviceCount</span></span>|<span data-ttu-id="cddd8-116">Int32</span><span class="sxs-lookup"><span data-stu-id="cddd8-116">Int32</span></span>|<span data-ttu-id="cddd8-117">设备运行状况脚本修正的设备数。</span><span class="sxs-lookup"><span data-stu-id="cddd8-117">The number of devices remediated by the device health script.</span></span>|
|<span data-ttu-id="cddd8-118">noIssueDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cddd8-118">noIssueDeviceCount</span></span>|<span data-ttu-id="cddd8-119">Int32</span><span class="sxs-lookup"><span data-stu-id="cddd8-119">Int32</span></span>|<span data-ttu-id="cddd8-120">设备运行状况脚本发现没有问题的设备数量。</span><span class="sxs-lookup"><span data-stu-id="cddd8-120">The number of devices that were found to have no issue by the device health script.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cddd8-121">关系</span><span class="sxs-lookup"><span data-stu-id="cddd8-121">Relationships</span></span>
<span data-ttu-id="cddd8-122">无</span><span class="sxs-lookup"><span data-stu-id="cddd8-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cddd8-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cddd8-123">JSON Representation</span></span>
<span data-ttu-id="cddd8-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cddd8-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptRemediationHistoryData"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRemediationHistoryData",
  "date": "String (Date)",
  "remediatedDeviceCount": 1024,
  "noIssueDeviceCount": 1024
}
```





