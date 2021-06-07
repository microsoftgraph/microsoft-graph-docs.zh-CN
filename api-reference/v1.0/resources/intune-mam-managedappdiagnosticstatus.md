---
title: managedAppDiagnosticStatus 资源类型
description: 表示诊断状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 824bcb13741240b1f5bc462312004892ccd5c051
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751319"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="f10d6-103">managedAppDiagnosticStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="f10d6-103">managedAppDiagnosticStatus resource type</span></span>

<span data-ttu-id="f10d6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f10d6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f10d6-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f10d6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f10d6-106">表示诊断状态。</span><span class="sxs-lookup"><span data-stu-id="f10d6-106">Represents diagnostics status.</span></span>

## <a name="properties"></a><span data-ttu-id="f10d6-107">属性</span><span class="sxs-lookup"><span data-stu-id="f10d6-107">Properties</span></span>
|<span data-ttu-id="f10d6-108">属性</span><span class="sxs-lookup"><span data-stu-id="f10d6-108">Property</span></span>|<span data-ttu-id="f10d6-109">类型</span><span class="sxs-lookup"><span data-stu-id="f10d6-109">Type</span></span>|<span data-ttu-id="f10d6-110">说明</span><span class="sxs-lookup"><span data-stu-id="f10d6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f10d6-111">validationName</span><span class="sxs-lookup"><span data-stu-id="f10d6-111">validationName</span></span>|<span data-ttu-id="f10d6-112">String</span><span class="sxs-lookup"><span data-stu-id="f10d6-112">String</span></span>|<span data-ttu-id="f10d6-113">验证友好名称</span><span class="sxs-lookup"><span data-stu-id="f10d6-113">The validation friendly name</span></span>|
|<span data-ttu-id="f10d6-114">state</span><span class="sxs-lookup"><span data-stu-id="f10d6-114">state</span></span>|<span data-ttu-id="f10d6-115">String</span><span class="sxs-lookup"><span data-stu-id="f10d6-115">String</span></span>|<span data-ttu-id="f10d6-116">操作状态</span><span class="sxs-lookup"><span data-stu-id="f10d6-116">The state of the operation</span></span>|
|<span data-ttu-id="f10d6-117">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="f10d6-117">mitigationInstruction</span></span>|<span data-ttu-id="f10d6-118">String</span><span class="sxs-lookup"><span data-stu-id="f10d6-118">String</span></span>|<span data-ttu-id="f10d6-119">有关如何降低失败验证的说明</span><span class="sxs-lookup"><span data-stu-id="f10d6-119">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="f10d6-120">关系</span><span class="sxs-lookup"><span data-stu-id="f10d6-120">Relationships</span></span>
<span data-ttu-id="f10d6-121">无</span><span class="sxs-lookup"><span data-stu-id="f10d6-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f10d6-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f10d6-122">JSON Representation</span></span>
<span data-ttu-id="f10d6-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f10d6-123">Here is a JSON representation of the resource.</span></span>
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




