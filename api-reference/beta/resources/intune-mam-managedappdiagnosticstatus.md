---
title: managedAppDiagnosticStatus 资源类型
description: 表示诊断状态。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 665ca55c67f5facb22eaf976e81737fed3dacf76
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407359"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="5c3d7-103">managedAppDiagnosticStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="5c3d7-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="5c3d7-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="5c3d7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5c3d7-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5c3d7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5c3d7-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5c3d7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c3d7-107">表示诊断状态。</span><span class="sxs-lookup"><span data-stu-id="5c3d7-107">Represents diagnostics status.</span></span>

## <a name="properties"></a><span data-ttu-id="5c3d7-108">属性</span><span class="sxs-lookup"><span data-stu-id="5c3d7-108">Properties</span></span>
|<span data-ttu-id="5c3d7-109">属性</span><span class="sxs-lookup"><span data-stu-id="5c3d7-109">Property</span></span>|<span data-ttu-id="5c3d7-110">类型</span><span class="sxs-lookup"><span data-stu-id="5c3d7-110">Type</span></span>|<span data-ttu-id="5c3d7-111">说明</span><span class="sxs-lookup"><span data-stu-id="5c3d7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c3d7-112">validationName</span><span class="sxs-lookup"><span data-stu-id="5c3d7-112">validationName</span></span>|<span data-ttu-id="5c3d7-113">String</span><span class="sxs-lookup"><span data-stu-id="5c3d7-113">String</span></span>|<span data-ttu-id="5c3d7-114">验证友好名称</span><span class="sxs-lookup"><span data-stu-id="5c3d7-114">The validation friendly name</span></span>|
|<span data-ttu-id="5c3d7-115">状态</span><span class="sxs-lookup"><span data-stu-id="5c3d7-115">state</span></span>|<span data-ttu-id="5c3d7-116">String</span><span class="sxs-lookup"><span data-stu-id="5c3d7-116">String</span></span>|<span data-ttu-id="5c3d7-117">操作状态</span><span class="sxs-lookup"><span data-stu-id="5c3d7-117">The state of the operation</span></span>|
|<span data-ttu-id="5c3d7-118">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="5c3d7-118">mitigationInstruction</span></span>|<span data-ttu-id="5c3d7-119">String</span><span class="sxs-lookup"><span data-stu-id="5c3d7-119">String</span></span>|<span data-ttu-id="5c3d7-120">有关如何降低失败验证的说明</span><span class="sxs-lookup"><span data-stu-id="5c3d7-120">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="5c3d7-121">关系</span><span class="sxs-lookup"><span data-stu-id="5c3d7-121">Relationships</span></span>
<span data-ttu-id="5c3d7-122">无</span><span class="sxs-lookup"><span data-stu-id="5c3d7-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5c3d7-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5c3d7-123">JSON Representation</span></span>
<span data-ttu-id="5c3d7-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5c3d7-124">Here is a JSON representation of the resource.</span></span>
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




