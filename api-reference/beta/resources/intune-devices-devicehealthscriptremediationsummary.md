---
title: deviceHealthScriptRemediationSummary 资源类型
description: 已部署的设备运行状况脚本数以及脚本修正的设备数。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5ca477131c3051161b17ed3f3e90aaf172662dfc
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43388445"
---
# <a name="devicehealthscriptremediationsummary-resource-type"></a><span data-ttu-id="3aee6-103">deviceHealthScriptRemediationSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="3aee6-103">deviceHealthScriptRemediationSummary resource type</span></span>

<span data-ttu-id="3aee6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3aee6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3aee6-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3aee6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3aee6-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3aee6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3aee6-107">已部署的设备运行状况脚本数以及脚本修正的设备数。</span><span class="sxs-lookup"><span data-stu-id="3aee6-107">The number of device health scripts deployed and the number of devices the scripts remediated.</span></span>

## <a name="properties"></a><span data-ttu-id="3aee6-108">属性</span><span class="sxs-lookup"><span data-stu-id="3aee6-108">Properties</span></span>
|<span data-ttu-id="3aee6-109">属性</span><span class="sxs-lookup"><span data-stu-id="3aee6-109">Property</span></span>|<span data-ttu-id="3aee6-110">类型</span><span class="sxs-lookup"><span data-stu-id="3aee6-110">Type</span></span>|<span data-ttu-id="3aee6-111">说明</span><span class="sxs-lookup"><span data-stu-id="3aee6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3aee6-112">scriptCount</span><span class="sxs-lookup"><span data-stu-id="3aee6-112">scriptCount</span></span>|<span data-ttu-id="3aee6-113">Int32</span><span class="sxs-lookup"><span data-stu-id="3aee6-113">Int32</span></span>|<span data-ttu-id="3aee6-114">已部署的设备运行状况脚本的数量。</span><span class="sxs-lookup"><span data-stu-id="3aee6-114">The number of device health scripts deployed.</span></span>|
|<span data-ttu-id="3aee6-115">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3aee6-115">remediatedDeviceCount</span></span>|<span data-ttu-id="3aee6-116">Int32</span><span class="sxs-lookup"><span data-stu-id="3aee6-116">Int32</span></span>|<span data-ttu-id="3aee6-117">设备运行状况脚本修正的设备数。</span><span class="sxs-lookup"><span data-stu-id="3aee6-117">The number of devices remediated by device health scripts.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3aee6-118">关系</span><span class="sxs-lookup"><span data-stu-id="3aee6-118">Relationships</span></span>
<span data-ttu-id="3aee6-119">无</span><span class="sxs-lookup"><span data-stu-id="3aee6-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3aee6-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3aee6-120">JSON Representation</span></span>
<span data-ttu-id="3aee6-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3aee6-121">Here is a JSON representation of the resource.</span></span>
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



