---
title: managedAppDiagnosticStatus 资源类型
description: 表示诊断状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 588338589d90ad54db43810d5fd45541cea483eb
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31800649"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="704f3-103">managedAppDiagnosticStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="704f3-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="704f3-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="704f3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="704f3-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="704f3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="704f3-106">表示诊断状态。</span><span class="sxs-lookup"><span data-stu-id="704f3-106">Represents diagnostics status.</span></span>

## <a name="properties"></a><span data-ttu-id="704f3-107">属性</span><span class="sxs-lookup"><span data-stu-id="704f3-107">Properties</span></span>
|<span data-ttu-id="704f3-108">属性</span><span class="sxs-lookup"><span data-stu-id="704f3-108">Property</span></span>|<span data-ttu-id="704f3-109">类型</span><span class="sxs-lookup"><span data-stu-id="704f3-109">Type</span></span>|<span data-ttu-id="704f3-110">说明</span><span class="sxs-lookup"><span data-stu-id="704f3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="704f3-111">validationName</span><span class="sxs-lookup"><span data-stu-id="704f3-111">validationName</span></span>|<span data-ttu-id="704f3-112">String</span><span class="sxs-lookup"><span data-stu-id="704f3-112">String</span></span>|<span data-ttu-id="704f3-113">验证友好名称</span><span class="sxs-lookup"><span data-stu-id="704f3-113">The validation friendly name</span></span>|
|<span data-ttu-id="704f3-114">state</span><span class="sxs-lookup"><span data-stu-id="704f3-114">state</span></span>|<span data-ttu-id="704f3-115">String</span><span class="sxs-lookup"><span data-stu-id="704f3-115">String</span></span>|<span data-ttu-id="704f3-116">操作状态</span><span class="sxs-lookup"><span data-stu-id="704f3-116">The state of the operation</span></span>|
|<span data-ttu-id="704f3-117">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="704f3-117">mitigationInstruction</span></span>|<span data-ttu-id="704f3-118">String</span><span class="sxs-lookup"><span data-stu-id="704f3-118">String</span></span>|<span data-ttu-id="704f3-119">有关如何降低失败验证的说明</span><span class="sxs-lookup"><span data-stu-id="704f3-119">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="704f3-120">关系</span><span class="sxs-lookup"><span data-stu-id="704f3-120">Relationships</span></span>
<span data-ttu-id="704f3-121">无</span><span class="sxs-lookup"><span data-stu-id="704f3-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="704f3-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="704f3-122">JSON Representation</span></span>
<span data-ttu-id="704f3-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="704f3-123">Here is a JSON representation of the resource.</span></span>
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





