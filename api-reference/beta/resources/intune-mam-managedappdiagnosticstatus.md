---
title: managedAppDiagnosticStatus 资源类型
description: 表示诊断状态。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4a896a17a2a79db6eea2ac2ece0973175506bac4
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940762"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="fc823-103">managedAppDiagnosticStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="fc823-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="fc823-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fc823-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc823-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fc823-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc823-106">表示诊断状态。</span><span class="sxs-lookup"><span data-stu-id="fc823-106">Represents diagnostics status.</span></span>

## <a name="properties"></a><span data-ttu-id="fc823-107">属性</span><span class="sxs-lookup"><span data-stu-id="fc823-107">Properties</span></span>
|<span data-ttu-id="fc823-108">属性</span><span class="sxs-lookup"><span data-stu-id="fc823-108">Property</span></span>|<span data-ttu-id="fc823-109">类型</span><span class="sxs-lookup"><span data-stu-id="fc823-109">Type</span></span>|<span data-ttu-id="fc823-110">说明</span><span class="sxs-lookup"><span data-stu-id="fc823-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc823-111">validationName</span><span class="sxs-lookup"><span data-stu-id="fc823-111">validationName</span></span>|<span data-ttu-id="fc823-112">String</span><span class="sxs-lookup"><span data-stu-id="fc823-112">String</span></span>|<span data-ttu-id="fc823-113">验证友好名称</span><span class="sxs-lookup"><span data-stu-id="fc823-113">The validation friendly name</span></span>|
|<span data-ttu-id="fc823-114">state</span><span class="sxs-lookup"><span data-stu-id="fc823-114">state</span></span>|<span data-ttu-id="fc823-115">String</span><span class="sxs-lookup"><span data-stu-id="fc823-115">String</span></span>|<span data-ttu-id="fc823-116">操作状态</span><span class="sxs-lookup"><span data-stu-id="fc823-116">The state of the operation</span></span>|
|<span data-ttu-id="fc823-117">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="fc823-117">mitigationInstruction</span></span>|<span data-ttu-id="fc823-118">String</span><span class="sxs-lookup"><span data-stu-id="fc823-118">String</span></span>|<span data-ttu-id="fc823-119">有关如何降低失败验证的说明</span><span class="sxs-lookup"><span data-stu-id="fc823-119">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="fc823-120">关系</span><span class="sxs-lookup"><span data-stu-id="fc823-120">Relationships</span></span>
<span data-ttu-id="fc823-121">无</span><span class="sxs-lookup"><span data-stu-id="fc823-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fc823-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fc823-122">JSON Representation</span></span>
<span data-ttu-id="fc823-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fc823-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedAppDiagnosticStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppDiagnosticStatus",
  "validationName": "String",
  "state": "String",
  "mitigationInstruction": "String"
}
```




