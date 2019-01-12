---
title: managedAppDiagnosticStatus 资源类型
description: 表示诊断状态。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3a5204a4704eefc2d4e7c8e0d5b3b709e1750667
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937479"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="ed981-103">managedAppDiagnosticStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="ed981-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="ed981-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ed981-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ed981-105">表示诊断状态。</span><span class="sxs-lookup"><span data-stu-id="ed981-105">Represents diagnostics status.</span></span>
## <a name="properties"></a><span data-ttu-id="ed981-106">属性</span><span class="sxs-lookup"><span data-stu-id="ed981-106">Properties</span></span>
|<span data-ttu-id="ed981-107">属性</span><span class="sxs-lookup"><span data-stu-id="ed981-107">Property</span></span>|<span data-ttu-id="ed981-108">类型</span><span class="sxs-lookup"><span data-stu-id="ed981-108">Type</span></span>|<span data-ttu-id="ed981-109">说明</span><span class="sxs-lookup"><span data-stu-id="ed981-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed981-110">validationName</span><span class="sxs-lookup"><span data-stu-id="ed981-110">validationName</span></span>|<span data-ttu-id="ed981-111">String</span><span class="sxs-lookup"><span data-stu-id="ed981-111">String</span></span>|<span data-ttu-id="ed981-112">验证友好名称</span><span class="sxs-lookup"><span data-stu-id="ed981-112">The validation friendly name</span></span>|
|<span data-ttu-id="ed981-113">状态</span><span class="sxs-lookup"><span data-stu-id="ed981-113">state</span></span>|<span data-ttu-id="ed981-114">String</span><span class="sxs-lookup"><span data-stu-id="ed981-114">String</span></span>|<span data-ttu-id="ed981-115">操作状态</span><span class="sxs-lookup"><span data-stu-id="ed981-115">The state of the operation</span></span>|
|<span data-ttu-id="ed981-116">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="ed981-116">mitigationInstruction</span></span>|<span data-ttu-id="ed981-117">String</span><span class="sxs-lookup"><span data-stu-id="ed981-117">String</span></span>|<span data-ttu-id="ed981-118">有关如何降低失败验证的说明</span><span class="sxs-lookup"><span data-stu-id="ed981-118">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="ed981-119">关系</span><span class="sxs-lookup"><span data-stu-id="ed981-119">Relationships</span></span>
<span data-ttu-id="ed981-120">无</span><span class="sxs-lookup"><span data-stu-id="ed981-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ed981-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ed981-121">JSON Representation</span></span>
<span data-ttu-id="ed981-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ed981-122">Here is a JSON representation of the resource.</span></span>
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



