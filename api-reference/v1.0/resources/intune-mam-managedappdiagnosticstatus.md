---
title: managedAppDiagnosticStatus 资源类型
description: 表示诊断状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c2477039c3a0ebca3de09a4042691045782848b3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32465303"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="6e06b-103">managedAppDiagnosticStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="6e06b-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="6e06b-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6e06b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e06b-105">表示诊断状态。</span><span class="sxs-lookup"><span data-stu-id="6e06b-105">Represents diagnostics status.</span></span>

## <a name="properties"></a><span data-ttu-id="6e06b-106">属性</span><span class="sxs-lookup"><span data-stu-id="6e06b-106">Properties</span></span>
|<span data-ttu-id="6e06b-107">属性</span><span class="sxs-lookup"><span data-stu-id="6e06b-107">Property</span></span>|<span data-ttu-id="6e06b-108">类型</span><span class="sxs-lookup"><span data-stu-id="6e06b-108">Type</span></span>|<span data-ttu-id="6e06b-109">说明</span><span class="sxs-lookup"><span data-stu-id="6e06b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e06b-110">validationName</span><span class="sxs-lookup"><span data-stu-id="6e06b-110">validationName</span></span>|<span data-ttu-id="6e06b-111">字符串</span><span class="sxs-lookup"><span data-stu-id="6e06b-111">String</span></span>|<span data-ttu-id="6e06b-112">验证友好名称</span><span class="sxs-lookup"><span data-stu-id="6e06b-112">The validation friendly name</span></span>|
|<span data-ttu-id="6e06b-113">state</span><span class="sxs-lookup"><span data-stu-id="6e06b-113">state</span></span>|<span data-ttu-id="6e06b-114">String</span><span class="sxs-lookup"><span data-stu-id="6e06b-114">String</span></span>|<span data-ttu-id="6e06b-115">操作状态</span><span class="sxs-lookup"><span data-stu-id="6e06b-115">The state of the operation</span></span>|
|<span data-ttu-id="6e06b-116">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="6e06b-116">mitigationInstruction</span></span>|<span data-ttu-id="6e06b-117">String</span><span class="sxs-lookup"><span data-stu-id="6e06b-117">String</span></span>|<span data-ttu-id="6e06b-118">有关如何降低失败验证的说明</span><span class="sxs-lookup"><span data-stu-id="6e06b-118">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="6e06b-119">关系</span><span class="sxs-lookup"><span data-stu-id="6e06b-119">Relationships</span></span>
<span data-ttu-id="6e06b-120">无</span><span class="sxs-lookup"><span data-stu-id="6e06b-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6e06b-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6e06b-121">JSON Representation</span></span>
<span data-ttu-id="6e06b-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6e06b-122">Here is a JSON representation of the resource.</span></span>
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



