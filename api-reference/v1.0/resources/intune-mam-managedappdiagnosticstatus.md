---
title: managedAppDiagnosticStatus 资源类型
description: 表示诊断状态。
ms.openlocfilehash: 8a462b49231323288d66a660c769ce7359cb5ab3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010051"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="3268c-103">managedAppDiagnosticStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="3268c-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="3268c-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="3268c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3268c-105">表示诊断状态。</span><span class="sxs-lookup"><span data-stu-id="3268c-105">Represents diagnostics status.</span></span>
## <a name="properties"></a><span data-ttu-id="3268c-106">属性</span><span class="sxs-lookup"><span data-stu-id="3268c-106">Properties</span></span>
|<span data-ttu-id="3268c-107">属性</span><span class="sxs-lookup"><span data-stu-id="3268c-107">Property</span></span>|<span data-ttu-id="3268c-108">类型</span><span class="sxs-lookup"><span data-stu-id="3268c-108">Type</span></span>|<span data-ttu-id="3268c-109">说明</span><span class="sxs-lookup"><span data-stu-id="3268c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3268c-110">validationName</span><span class="sxs-lookup"><span data-stu-id="3268c-110">validationName</span></span>|<span data-ttu-id="3268c-111">String</span><span class="sxs-lookup"><span data-stu-id="3268c-111">String</span></span>|<span data-ttu-id="3268c-112">验证友好名称</span><span class="sxs-lookup"><span data-stu-id="3268c-112">The validation friendly name</span></span>|
|<span data-ttu-id="3268c-113">状态</span><span class="sxs-lookup"><span data-stu-id="3268c-113">state</span></span>|<span data-ttu-id="3268c-114">String</span><span class="sxs-lookup"><span data-stu-id="3268c-114">String</span></span>|<span data-ttu-id="3268c-115">操作状态</span><span class="sxs-lookup"><span data-stu-id="3268c-115">The state of the operation</span></span>|
|<span data-ttu-id="3268c-116">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="3268c-116">mitigationInstruction</span></span>|<span data-ttu-id="3268c-117">String</span><span class="sxs-lookup"><span data-stu-id="3268c-117">String</span></span>|<span data-ttu-id="3268c-118">有关如何降低失败验证的说明</span><span class="sxs-lookup"><span data-stu-id="3268c-118">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="3268c-119">关系</span><span class="sxs-lookup"><span data-stu-id="3268c-119">Relationships</span></span>
<span data-ttu-id="3268c-120">无</span><span class="sxs-lookup"><span data-stu-id="3268c-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3268c-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3268c-121">JSON Representation</span></span>
<span data-ttu-id="3268c-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3268c-122">Here is a JSON representation of the resource.</span></span>
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



