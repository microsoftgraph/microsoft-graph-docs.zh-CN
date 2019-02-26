---
title: managedAppDiagnosticStatus 资源类型
description: 表示诊断状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c2477039c3a0ebca3de09a4042691045782848b3
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261549"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="ea7a8-103">managedAppDiagnosticStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="ea7a8-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="ea7a8-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ea7a8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea7a8-105">表示诊断状态。</span><span class="sxs-lookup"><span data-stu-id="ea7a8-105">Represents diagnostics status.</span></span>

## <a name="properties"></a><span data-ttu-id="ea7a8-106">属性</span><span class="sxs-lookup"><span data-stu-id="ea7a8-106">Properties</span></span>
|<span data-ttu-id="ea7a8-107">属性</span><span class="sxs-lookup"><span data-stu-id="ea7a8-107">Property</span></span>|<span data-ttu-id="ea7a8-108">类型</span><span class="sxs-lookup"><span data-stu-id="ea7a8-108">Type</span></span>|<span data-ttu-id="ea7a8-109">说明</span><span class="sxs-lookup"><span data-stu-id="ea7a8-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea7a8-110">validationName</span><span class="sxs-lookup"><span data-stu-id="ea7a8-110">validationName</span></span>|<span data-ttu-id="ea7a8-111">String</span><span class="sxs-lookup"><span data-stu-id="ea7a8-111">String</span></span>|<span data-ttu-id="ea7a8-112">验证友好名称</span><span class="sxs-lookup"><span data-stu-id="ea7a8-112">The validation friendly name</span></span>|
|<span data-ttu-id="ea7a8-113">状态</span><span class="sxs-lookup"><span data-stu-id="ea7a8-113">state</span></span>|<span data-ttu-id="ea7a8-114">String</span><span class="sxs-lookup"><span data-stu-id="ea7a8-114">String</span></span>|<span data-ttu-id="ea7a8-115">操作状态</span><span class="sxs-lookup"><span data-stu-id="ea7a8-115">The state of the operation</span></span>|
|<span data-ttu-id="ea7a8-116">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="ea7a8-116">mitigationInstruction</span></span>|<span data-ttu-id="ea7a8-117">String</span><span class="sxs-lookup"><span data-stu-id="ea7a8-117">String</span></span>|<span data-ttu-id="ea7a8-118">有关如何降低失败验证的说明</span><span class="sxs-lookup"><span data-stu-id="ea7a8-118">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="ea7a8-119">关系</span><span class="sxs-lookup"><span data-stu-id="ea7a8-119">Relationships</span></span>
<span data-ttu-id="ea7a8-120">无</span><span class="sxs-lookup"><span data-stu-id="ea7a8-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ea7a8-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ea7a8-121">JSON Representation</span></span>
<span data-ttu-id="ea7a8-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ea7a8-122">Here is a JSON representation of the resource.</span></span>
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



