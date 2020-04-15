---
title: managedAppDiagnosticStatus 资源类型
description: 表示诊断状态。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a8c7eb75b2bb8b146c9b227562d7b9cdabe8da41
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43445753"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="c2c38-103">managedAppDiagnosticStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="c2c38-103">managedAppDiagnosticStatus resource type</span></span>

<span data-ttu-id="c2c38-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2c38-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c2c38-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c2c38-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2c38-106">表示诊断状态。</span><span class="sxs-lookup"><span data-stu-id="c2c38-106">Represents diagnostics status.</span></span>

## <a name="properties"></a><span data-ttu-id="c2c38-107">属性</span><span class="sxs-lookup"><span data-stu-id="c2c38-107">Properties</span></span>
|<span data-ttu-id="c2c38-108">属性</span><span class="sxs-lookup"><span data-stu-id="c2c38-108">Property</span></span>|<span data-ttu-id="c2c38-109">类型</span><span class="sxs-lookup"><span data-stu-id="c2c38-109">Type</span></span>|<span data-ttu-id="c2c38-110">说明</span><span class="sxs-lookup"><span data-stu-id="c2c38-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2c38-111">validationName</span><span class="sxs-lookup"><span data-stu-id="c2c38-111">validationName</span></span>|<span data-ttu-id="c2c38-112">String</span><span class="sxs-lookup"><span data-stu-id="c2c38-112">String</span></span>|<span data-ttu-id="c2c38-113">验证友好名称</span><span class="sxs-lookup"><span data-stu-id="c2c38-113">The validation friendly name</span></span>|
|<span data-ttu-id="c2c38-114">state</span><span class="sxs-lookup"><span data-stu-id="c2c38-114">state</span></span>|<span data-ttu-id="c2c38-115">String</span><span class="sxs-lookup"><span data-stu-id="c2c38-115">String</span></span>|<span data-ttu-id="c2c38-116">操作状态</span><span class="sxs-lookup"><span data-stu-id="c2c38-116">The state of the operation</span></span>|
|<span data-ttu-id="c2c38-117">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="c2c38-117">mitigationInstruction</span></span>|<span data-ttu-id="c2c38-118">String</span><span class="sxs-lookup"><span data-stu-id="c2c38-118">String</span></span>|<span data-ttu-id="c2c38-119">有关如何降低失败验证的说明</span><span class="sxs-lookup"><span data-stu-id="c2c38-119">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="c2c38-120">关系</span><span class="sxs-lookup"><span data-stu-id="c2c38-120">Relationships</span></span>
<span data-ttu-id="c2c38-121">无</span><span class="sxs-lookup"><span data-stu-id="c2c38-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c2c38-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c2c38-122">JSON Representation</span></span>
<span data-ttu-id="c2c38-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c2c38-123">Here is a JSON representation of the resource.</span></span>
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







