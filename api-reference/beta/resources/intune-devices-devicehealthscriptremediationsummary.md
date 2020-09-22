---
title: deviceHealthScriptRemediationSummary 资源类型
description: 已部署的设备运行状况脚本数以及脚本修正的设备数。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 06e48973305dbbdf7ae276e4d14d3307da74c36e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060286"
---
# <a name="devicehealthscriptremediationsummary-resource-type"></a><span data-ttu-id="4e65b-103">deviceHealthScriptRemediationSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="4e65b-103">deviceHealthScriptRemediationSummary resource type</span></span>

<span data-ttu-id="4e65b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e65b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4e65b-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4e65b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e65b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4e65b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e65b-107">已部署的设备运行状况脚本数以及脚本修正的设备数。</span><span class="sxs-lookup"><span data-stu-id="4e65b-107">The number of device health scripts deployed and the number of devices the scripts remediated.</span></span>

## <a name="properties"></a><span data-ttu-id="4e65b-108">属性</span><span class="sxs-lookup"><span data-stu-id="4e65b-108">Properties</span></span>
|<span data-ttu-id="4e65b-109">属性</span><span class="sxs-lookup"><span data-stu-id="4e65b-109">Property</span></span>|<span data-ttu-id="4e65b-110">类型</span><span class="sxs-lookup"><span data-stu-id="4e65b-110">Type</span></span>|<span data-ttu-id="4e65b-111">说明</span><span class="sxs-lookup"><span data-stu-id="4e65b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e65b-112">scriptCount</span><span class="sxs-lookup"><span data-stu-id="4e65b-112">scriptCount</span></span>|<span data-ttu-id="4e65b-113">Int32</span><span class="sxs-lookup"><span data-stu-id="4e65b-113">Int32</span></span>|<span data-ttu-id="4e65b-114">已部署的设备运行状况脚本的数量。</span><span class="sxs-lookup"><span data-stu-id="4e65b-114">The number of device health scripts deployed.</span></span>|
|<span data-ttu-id="4e65b-115">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4e65b-115">remediatedDeviceCount</span></span>|<span data-ttu-id="4e65b-116">Int32</span><span class="sxs-lookup"><span data-stu-id="4e65b-116">Int32</span></span>|<span data-ttu-id="4e65b-117">设备运行状况脚本修正的设备数。</span><span class="sxs-lookup"><span data-stu-id="4e65b-117">The number of devices remediated by device health scripts.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4e65b-118">关系</span><span class="sxs-lookup"><span data-stu-id="4e65b-118">Relationships</span></span>
<span data-ttu-id="4e65b-119">无</span><span class="sxs-lookup"><span data-stu-id="4e65b-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4e65b-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4e65b-120">JSON Representation</span></span>
<span data-ttu-id="4e65b-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4e65b-121">Here is a JSON representation of the resource.</span></span>
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






