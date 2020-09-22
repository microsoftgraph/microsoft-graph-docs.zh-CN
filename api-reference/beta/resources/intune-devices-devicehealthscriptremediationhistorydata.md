---
title: deviceHealthScriptRemediationHistoryData 资源类型
description: 给定日期设备运行状况脚本修正的设备数量。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7095dc821ccfaada8d1f83047895f54d823e1958
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060285"
---
# <a name="devicehealthscriptremediationhistorydata-resource-type"></a><span data-ttu-id="b5884-103">deviceHealthScriptRemediationHistoryData 资源类型</span><span class="sxs-lookup"><span data-stu-id="b5884-103">deviceHealthScriptRemediationHistoryData resource type</span></span>

<span data-ttu-id="b5884-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5884-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b5884-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b5884-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b5884-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b5884-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5884-107">给定日期设备运行状况脚本修正的设备数量。</span><span class="sxs-lookup"><span data-stu-id="b5884-107">The number of devices remediated by a device health script on a given date.</span></span>

## <a name="properties"></a><span data-ttu-id="b5884-108">属性</span><span class="sxs-lookup"><span data-stu-id="b5884-108">Properties</span></span>
|<span data-ttu-id="b5884-109">属性</span><span class="sxs-lookup"><span data-stu-id="b5884-109">Property</span></span>|<span data-ttu-id="b5884-110">类型</span><span class="sxs-lookup"><span data-stu-id="b5884-110">Type</span></span>|<span data-ttu-id="b5884-111">说明</span><span class="sxs-lookup"><span data-stu-id="b5884-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5884-112">date</span><span class="sxs-lookup"><span data-stu-id="b5884-112">date</span></span>|<span data-ttu-id="b5884-113">Date</span><span class="sxs-lookup"><span data-stu-id="b5884-113">Date</span></span>|<span data-ttu-id="b5884-114">设备运行状况脚本修正设备的日期。</span><span class="sxs-lookup"><span data-stu-id="b5884-114">The date on which devices were remediated by the device health script.</span></span>|
|<span data-ttu-id="b5884-115">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b5884-115">remediatedDeviceCount</span></span>|<span data-ttu-id="b5884-116">Int32</span><span class="sxs-lookup"><span data-stu-id="b5884-116">Int32</span></span>|<span data-ttu-id="b5884-117">设备运行状况脚本修正的设备数。</span><span class="sxs-lookup"><span data-stu-id="b5884-117">The number of devices remediated by the device health script.</span></span>|
|<span data-ttu-id="b5884-118">noIssueDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b5884-118">noIssueDeviceCount</span></span>|<span data-ttu-id="b5884-119">Int32</span><span class="sxs-lookup"><span data-stu-id="b5884-119">Int32</span></span>|<span data-ttu-id="b5884-120">设备运行状况脚本发现没有问题的设备数量。</span><span class="sxs-lookup"><span data-stu-id="b5884-120">The number of devices that were found to have no issue by the device health script.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b5884-121">关系</span><span class="sxs-lookup"><span data-stu-id="b5884-121">Relationships</span></span>
<span data-ttu-id="b5884-122">无</span><span class="sxs-lookup"><span data-stu-id="b5884-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b5884-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b5884-123">JSON Representation</span></span>
<span data-ttu-id="b5884-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b5884-124">Here is a JSON representation of the resource.</span></span>
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






