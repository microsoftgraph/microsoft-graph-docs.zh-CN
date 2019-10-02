---
title: managedAppDiagnosticStatus 资源类型
description: 表示诊断状态。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 33a975318854ab8bfec35ca257ee0c59fc29c188
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356364"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="a6ec8-103">managedAppDiagnosticStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="a6ec8-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="a6ec8-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a6ec8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6ec8-105">表示诊断状态。</span><span class="sxs-lookup"><span data-stu-id="a6ec8-105">Represents diagnostics status.</span></span>

## <a name="properties"></a><span data-ttu-id="a6ec8-106">属性</span><span class="sxs-lookup"><span data-stu-id="a6ec8-106">Properties</span></span>
|<span data-ttu-id="a6ec8-107">属性</span><span class="sxs-lookup"><span data-stu-id="a6ec8-107">Property</span></span>|<span data-ttu-id="a6ec8-108">类型</span><span class="sxs-lookup"><span data-stu-id="a6ec8-108">Type</span></span>|<span data-ttu-id="a6ec8-109">说明</span><span class="sxs-lookup"><span data-stu-id="a6ec8-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6ec8-110">validationName</span><span class="sxs-lookup"><span data-stu-id="a6ec8-110">validationName</span></span>|<span data-ttu-id="a6ec8-111">String</span><span class="sxs-lookup"><span data-stu-id="a6ec8-111">String</span></span>|<span data-ttu-id="a6ec8-112">验证友好名称</span><span class="sxs-lookup"><span data-stu-id="a6ec8-112">The validation friendly name</span></span>|
|<span data-ttu-id="a6ec8-113">state</span><span class="sxs-lookup"><span data-stu-id="a6ec8-113">state</span></span>|<span data-ttu-id="a6ec8-114">String</span><span class="sxs-lookup"><span data-stu-id="a6ec8-114">String</span></span>|<span data-ttu-id="a6ec8-115">操作状态</span><span class="sxs-lookup"><span data-stu-id="a6ec8-115">The state of the operation</span></span>|
|<span data-ttu-id="a6ec8-116">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="a6ec8-116">mitigationInstruction</span></span>|<span data-ttu-id="a6ec8-117">String</span><span class="sxs-lookup"><span data-stu-id="a6ec8-117">String</span></span>|<span data-ttu-id="a6ec8-118">有关如何降低失败验证的说明</span><span class="sxs-lookup"><span data-stu-id="a6ec8-118">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="a6ec8-119">关系</span><span class="sxs-lookup"><span data-stu-id="a6ec8-119">Relationships</span></span>
<span data-ttu-id="a6ec8-120">无</span><span class="sxs-lookup"><span data-stu-id="a6ec8-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a6ec8-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a6ec8-121">JSON Representation</span></span>
<span data-ttu-id="a6ec8-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a6ec8-122">Here is a JSON representation of the resource.</span></span>
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




