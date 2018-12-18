---
title: managedAppDiagnosticStatus 资源类型
description: 表示诊断状态。
author: tfitzmac
ms.openlocfilehash: 7f0cd0d5b11c4d902f51dd422add2373e8e8df9e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340682"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="9de8a-103">managedAppDiagnosticStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="9de8a-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="9de8a-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9de8a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9de8a-105">表示诊断状态。</span><span class="sxs-lookup"><span data-stu-id="9de8a-105">Represents diagnostics status.</span></span>
## <a name="properties"></a><span data-ttu-id="9de8a-106">属性</span><span class="sxs-lookup"><span data-stu-id="9de8a-106">Properties</span></span>
|<span data-ttu-id="9de8a-107">属性</span><span class="sxs-lookup"><span data-stu-id="9de8a-107">Property</span></span>|<span data-ttu-id="9de8a-108">类型</span><span class="sxs-lookup"><span data-stu-id="9de8a-108">Type</span></span>|<span data-ttu-id="9de8a-109">说明</span><span class="sxs-lookup"><span data-stu-id="9de8a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9de8a-110">validationName</span><span class="sxs-lookup"><span data-stu-id="9de8a-110">validationName</span></span>|<span data-ttu-id="9de8a-111">String</span><span class="sxs-lookup"><span data-stu-id="9de8a-111">String</span></span>|<span data-ttu-id="9de8a-112">验证友好名称</span><span class="sxs-lookup"><span data-stu-id="9de8a-112">The validation friendly name</span></span>|
|<span data-ttu-id="9de8a-113">状态</span><span class="sxs-lookup"><span data-stu-id="9de8a-113">state</span></span>|<span data-ttu-id="9de8a-114">String</span><span class="sxs-lookup"><span data-stu-id="9de8a-114">String</span></span>|<span data-ttu-id="9de8a-115">操作状态</span><span class="sxs-lookup"><span data-stu-id="9de8a-115">The state of the operation</span></span>|
|<span data-ttu-id="9de8a-116">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="9de8a-116">mitigationInstruction</span></span>|<span data-ttu-id="9de8a-117">String</span><span class="sxs-lookup"><span data-stu-id="9de8a-117">String</span></span>|<span data-ttu-id="9de8a-118">有关如何降低失败验证的说明</span><span class="sxs-lookup"><span data-stu-id="9de8a-118">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="9de8a-119">关系</span><span class="sxs-lookup"><span data-stu-id="9de8a-119">Relationships</span></span>
<span data-ttu-id="9de8a-120">无</span><span class="sxs-lookup"><span data-stu-id="9de8a-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9de8a-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9de8a-121">JSON Representation</span></span>
<span data-ttu-id="9de8a-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9de8a-122">Here is a JSON representation of the resource.</span></span>
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



