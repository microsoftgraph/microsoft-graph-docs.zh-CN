---
title: managedAppDiagnosticStatus 资源类型
description: 表示诊断状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 74743a345688699ac25399e92af53f17afe86626
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48030337"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="5c3cf-103">managedAppDiagnosticStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="5c3cf-103">managedAppDiagnosticStatus resource type</span></span>

<span data-ttu-id="5c3cf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c3cf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5c3cf-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5c3cf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5c3cf-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5c3cf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c3cf-107">表示诊断状态。</span><span class="sxs-lookup"><span data-stu-id="5c3cf-107">Represents diagnostics status.</span></span>

## <a name="properties"></a><span data-ttu-id="5c3cf-108">属性</span><span class="sxs-lookup"><span data-stu-id="5c3cf-108">Properties</span></span>
|<span data-ttu-id="5c3cf-109">属性</span><span class="sxs-lookup"><span data-stu-id="5c3cf-109">Property</span></span>|<span data-ttu-id="5c3cf-110">类型</span><span class="sxs-lookup"><span data-stu-id="5c3cf-110">Type</span></span>|<span data-ttu-id="5c3cf-111">说明</span><span class="sxs-lookup"><span data-stu-id="5c3cf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c3cf-112">validationName</span><span class="sxs-lookup"><span data-stu-id="5c3cf-112">validationName</span></span>|<span data-ttu-id="5c3cf-113">String</span><span class="sxs-lookup"><span data-stu-id="5c3cf-113">String</span></span>|<span data-ttu-id="5c3cf-114">验证友好名称</span><span class="sxs-lookup"><span data-stu-id="5c3cf-114">The validation friendly name</span></span>|
|<span data-ttu-id="5c3cf-115">state</span><span class="sxs-lookup"><span data-stu-id="5c3cf-115">state</span></span>|<span data-ttu-id="5c3cf-116">String</span><span class="sxs-lookup"><span data-stu-id="5c3cf-116">String</span></span>|<span data-ttu-id="5c3cf-117">操作状态</span><span class="sxs-lookup"><span data-stu-id="5c3cf-117">The state of the operation</span></span>|
|<span data-ttu-id="5c3cf-118">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="5c3cf-118">mitigationInstruction</span></span>|<span data-ttu-id="5c3cf-119">String</span><span class="sxs-lookup"><span data-stu-id="5c3cf-119">String</span></span>|<span data-ttu-id="5c3cf-120">有关如何降低失败验证的说明</span><span class="sxs-lookup"><span data-stu-id="5c3cf-120">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="5c3cf-121">关系</span><span class="sxs-lookup"><span data-stu-id="5c3cf-121">Relationships</span></span>
<span data-ttu-id="5c3cf-122">无</span><span class="sxs-lookup"><span data-stu-id="5c3cf-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5c3cf-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5c3cf-123">JSON Representation</span></span>
<span data-ttu-id="5c3cf-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5c3cf-124">Here is a JSON representation of the resource.</span></span>
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






