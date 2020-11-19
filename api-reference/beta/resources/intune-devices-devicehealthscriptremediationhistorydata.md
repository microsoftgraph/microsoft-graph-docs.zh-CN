---
title: deviceHealthScriptRemediationHistoryData 资源类型
description: 给定日期设备运行状况脚本修正的设备数量。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d1940328e9690414dc9ce4b4958f6f5e34751b1b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49259989"
---
# <a name="devicehealthscriptremediationhistorydata-resource-type"></a><span data-ttu-id="23004-103">deviceHealthScriptRemediationHistoryData 资源类型</span><span class="sxs-lookup"><span data-stu-id="23004-103">deviceHealthScriptRemediationHistoryData resource type</span></span>

<span data-ttu-id="23004-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23004-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="23004-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="23004-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="23004-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="23004-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23004-107">给定日期设备运行状况脚本修正的设备数量。</span><span class="sxs-lookup"><span data-stu-id="23004-107">The number of devices remediated by a device health script on a given date.</span></span>

## <a name="properties"></a><span data-ttu-id="23004-108">属性</span><span class="sxs-lookup"><span data-stu-id="23004-108">Properties</span></span>
|<span data-ttu-id="23004-109">属性</span><span class="sxs-lookup"><span data-stu-id="23004-109">Property</span></span>|<span data-ttu-id="23004-110">类型</span><span class="sxs-lookup"><span data-stu-id="23004-110">Type</span></span>|<span data-ttu-id="23004-111">描述</span><span class="sxs-lookup"><span data-stu-id="23004-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23004-112">date</span><span class="sxs-lookup"><span data-stu-id="23004-112">date</span></span>|<span data-ttu-id="23004-113">Date</span><span class="sxs-lookup"><span data-stu-id="23004-113">Date</span></span>|<span data-ttu-id="23004-114">设备运行状况脚本修正设备的日期。</span><span class="sxs-lookup"><span data-stu-id="23004-114">The date on which devices were remediated by the device health script.</span></span>|
|<span data-ttu-id="23004-115">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="23004-115">remediatedDeviceCount</span></span>|<span data-ttu-id="23004-116">Int32</span><span class="sxs-lookup"><span data-stu-id="23004-116">Int32</span></span>|<span data-ttu-id="23004-117">设备运行状况脚本修正的设备数。</span><span class="sxs-lookup"><span data-stu-id="23004-117">The number of devices remediated by the device health script.</span></span>|
|<span data-ttu-id="23004-118">noIssueDeviceCount</span><span class="sxs-lookup"><span data-stu-id="23004-118">noIssueDeviceCount</span></span>|<span data-ttu-id="23004-119">Int32</span><span class="sxs-lookup"><span data-stu-id="23004-119">Int32</span></span>|<span data-ttu-id="23004-120">设备运行状况脚本发现没有问题的设备数量。</span><span class="sxs-lookup"><span data-stu-id="23004-120">The number of devices that were found to have no issue by the device health script.</span></span>|

## <a name="relationships"></a><span data-ttu-id="23004-121">关系</span><span class="sxs-lookup"><span data-stu-id="23004-121">Relationships</span></span>
<span data-ttu-id="23004-122">无</span><span class="sxs-lookup"><span data-stu-id="23004-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="23004-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="23004-123">JSON Representation</span></span>
<span data-ttu-id="23004-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="23004-124">Here is a JSON representation of the resource.</span></span>
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




