---
title: deviceHealthScriptRemediationSummary 资源类型
description: 已部署的设备运行状况脚本数以及脚本修正的设备数。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b59f2d057f258e60a8182194c1ac930e95012b93
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42784942"
---
# <a name="devicehealthscriptremediationsummary-resource-type"></a><span data-ttu-id="b02f3-103">deviceHealthScriptRemediationSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="b02f3-103">deviceHealthScriptRemediationSummary resource type</span></span>

> <span data-ttu-id="b02f3-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b02f3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b02f3-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b02f3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b02f3-106">已部署的设备运行状况脚本数以及脚本修正的设备数。</span><span class="sxs-lookup"><span data-stu-id="b02f3-106">The number of device health scripts deployed and the number of devices the scripts remediated.</span></span>

## <a name="properties"></a><span data-ttu-id="b02f3-107">属性</span><span class="sxs-lookup"><span data-stu-id="b02f3-107">Properties</span></span>
|<span data-ttu-id="b02f3-108">属性</span><span class="sxs-lookup"><span data-stu-id="b02f3-108">Property</span></span>|<span data-ttu-id="b02f3-109">类型</span><span class="sxs-lookup"><span data-stu-id="b02f3-109">Type</span></span>|<span data-ttu-id="b02f3-110">说明</span><span class="sxs-lookup"><span data-stu-id="b02f3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b02f3-111">scriptCount</span><span class="sxs-lookup"><span data-stu-id="b02f3-111">scriptCount</span></span>|<span data-ttu-id="b02f3-112">Int32</span><span class="sxs-lookup"><span data-stu-id="b02f3-112">Int32</span></span>|<span data-ttu-id="b02f3-113">已部署的设备运行状况脚本的数量。</span><span class="sxs-lookup"><span data-stu-id="b02f3-113">The number of device health scripts deployed.</span></span>|
|<span data-ttu-id="b02f3-114">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b02f3-114">remediatedDeviceCount</span></span>|<span data-ttu-id="b02f3-115">Int32</span><span class="sxs-lookup"><span data-stu-id="b02f3-115">Int32</span></span>|<span data-ttu-id="b02f3-116">设备运行状况脚本修正的设备数。</span><span class="sxs-lookup"><span data-stu-id="b02f3-116">The number of devices remediated by device health scripts.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b02f3-117">关系</span><span class="sxs-lookup"><span data-stu-id="b02f3-117">Relationships</span></span>
<span data-ttu-id="b02f3-118">无</span><span class="sxs-lookup"><span data-stu-id="b02f3-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b02f3-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b02f3-119">JSON Representation</span></span>
<span data-ttu-id="b02f3-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b02f3-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptRemediationSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRemediationSummary",
  "scriptCount": 1024,
  "remediatedDeviceCount": 1024
}
```



