---
title: managedAppDiagnosticStatus 资源类型
description: 表示诊断状态。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 210edaf8eb039db928d612337aa7c8e0642c9ee3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987186"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="a09b1-103">managedAppDiagnosticStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="a09b1-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="a09b1-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a09b1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a09b1-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a09b1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a09b1-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a09b1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a09b1-107">表示诊断状态。</span><span class="sxs-lookup"><span data-stu-id="a09b1-107">Represents diagnostics status.</span></span>
## <a name="properties"></a><span data-ttu-id="a09b1-108">属性</span><span class="sxs-lookup"><span data-stu-id="a09b1-108">Properties</span></span>
|<span data-ttu-id="a09b1-109">属性</span><span class="sxs-lookup"><span data-stu-id="a09b1-109">Property</span></span>|<span data-ttu-id="a09b1-110">类型</span><span class="sxs-lookup"><span data-stu-id="a09b1-110">Type</span></span>|<span data-ttu-id="a09b1-111">说明</span><span class="sxs-lookup"><span data-stu-id="a09b1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a09b1-112">validationName</span><span class="sxs-lookup"><span data-stu-id="a09b1-112">validationName</span></span>|<span data-ttu-id="a09b1-113">String</span><span class="sxs-lookup"><span data-stu-id="a09b1-113">String</span></span>|<span data-ttu-id="a09b1-114">验证友好名称</span><span class="sxs-lookup"><span data-stu-id="a09b1-114">The validation friendly name</span></span>|
|<span data-ttu-id="a09b1-115">状态</span><span class="sxs-lookup"><span data-stu-id="a09b1-115">state</span></span>|<span data-ttu-id="a09b1-116">String</span><span class="sxs-lookup"><span data-stu-id="a09b1-116">String</span></span>|<span data-ttu-id="a09b1-117">操作状态</span><span class="sxs-lookup"><span data-stu-id="a09b1-117">The state of the operation</span></span>|
|<span data-ttu-id="a09b1-118">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="a09b1-118">mitigationInstruction</span></span>|<span data-ttu-id="a09b1-119">String</span><span class="sxs-lookup"><span data-stu-id="a09b1-119">String</span></span>|<span data-ttu-id="a09b1-120">有关如何降低失败验证的说明</span><span class="sxs-lookup"><span data-stu-id="a09b1-120">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="a09b1-121">关系</span><span class="sxs-lookup"><span data-stu-id="a09b1-121">Relationships</span></span>
<span data-ttu-id="a09b1-122">无</span><span class="sxs-lookup"><span data-stu-id="a09b1-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a09b1-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a09b1-123">JSON Representation</span></span>
<span data-ttu-id="a09b1-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a09b1-124">Here is a JSON representation of the resource.</span></span>
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





