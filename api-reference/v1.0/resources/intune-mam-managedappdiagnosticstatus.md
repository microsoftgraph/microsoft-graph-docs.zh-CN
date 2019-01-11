---
title: managedAppDiagnosticStatus 资源类型
description: 表示诊断状态。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f471a71c10a225f2bb5af77399932402f154538d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872119"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="d8564-103">managedAppDiagnosticStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="d8564-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="d8564-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d8564-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d8564-105">表示诊断状态。</span><span class="sxs-lookup"><span data-stu-id="d8564-105">Represents diagnostics status.</span></span>
## <a name="properties"></a><span data-ttu-id="d8564-106">属性</span><span class="sxs-lookup"><span data-stu-id="d8564-106">Properties</span></span>
|<span data-ttu-id="d8564-107">属性</span><span class="sxs-lookup"><span data-stu-id="d8564-107">Property</span></span>|<span data-ttu-id="d8564-108">类型</span><span class="sxs-lookup"><span data-stu-id="d8564-108">Type</span></span>|<span data-ttu-id="d8564-109">说明</span><span class="sxs-lookup"><span data-stu-id="d8564-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8564-110">validationName</span><span class="sxs-lookup"><span data-stu-id="d8564-110">validationName</span></span>|<span data-ttu-id="d8564-111">String</span><span class="sxs-lookup"><span data-stu-id="d8564-111">String</span></span>|<span data-ttu-id="d8564-112">验证友好名称</span><span class="sxs-lookup"><span data-stu-id="d8564-112">The validation friendly name</span></span>|
|<span data-ttu-id="d8564-113">状态</span><span class="sxs-lookup"><span data-stu-id="d8564-113">state</span></span>|<span data-ttu-id="d8564-114">String</span><span class="sxs-lookup"><span data-stu-id="d8564-114">String</span></span>|<span data-ttu-id="d8564-115">操作状态</span><span class="sxs-lookup"><span data-stu-id="d8564-115">The state of the operation</span></span>|
|<span data-ttu-id="d8564-116">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="d8564-116">mitigationInstruction</span></span>|<span data-ttu-id="d8564-117">String</span><span class="sxs-lookup"><span data-stu-id="d8564-117">String</span></span>|<span data-ttu-id="d8564-118">有关如何降低失败验证的说明</span><span class="sxs-lookup"><span data-stu-id="d8564-118">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="d8564-119">关系</span><span class="sxs-lookup"><span data-stu-id="d8564-119">Relationships</span></span>
<span data-ttu-id="d8564-120">无</span><span class="sxs-lookup"><span data-stu-id="d8564-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d8564-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d8564-121">JSON Representation</span></span>
<span data-ttu-id="d8564-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d8564-122">Here is a JSON representation of the resource.</span></span>
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



