---
title: managedAppDiagnosticStatus 资源类型
description: 表示诊断状态。
author: tfitzmac
ms.openlocfilehash: 1618c65b46654832fc7706f01cb6d6a9f78926e4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314775"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="adf01-103">managedAppDiagnosticStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="adf01-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="adf01-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="adf01-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="adf01-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="adf01-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="adf01-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="adf01-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="adf01-107">表示诊断状态。</span><span class="sxs-lookup"><span data-stu-id="adf01-107">Represents diagnostics status.</span></span>
## <a name="properties"></a><span data-ttu-id="adf01-108">属性</span><span class="sxs-lookup"><span data-stu-id="adf01-108">Properties</span></span>
|<span data-ttu-id="adf01-109">属性</span><span class="sxs-lookup"><span data-stu-id="adf01-109">Property</span></span>|<span data-ttu-id="adf01-110">类型</span><span class="sxs-lookup"><span data-stu-id="adf01-110">Type</span></span>|<span data-ttu-id="adf01-111">说明</span><span class="sxs-lookup"><span data-stu-id="adf01-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="adf01-112">validationName</span><span class="sxs-lookup"><span data-stu-id="adf01-112">validationName</span></span>|<span data-ttu-id="adf01-113">String</span><span class="sxs-lookup"><span data-stu-id="adf01-113">String</span></span>|<span data-ttu-id="adf01-114">验证友好名称</span><span class="sxs-lookup"><span data-stu-id="adf01-114">The validation friendly name</span></span>|
|<span data-ttu-id="adf01-115">状态</span><span class="sxs-lookup"><span data-stu-id="adf01-115">state</span></span>|<span data-ttu-id="adf01-116">String</span><span class="sxs-lookup"><span data-stu-id="adf01-116">String</span></span>|<span data-ttu-id="adf01-117">操作状态</span><span class="sxs-lookup"><span data-stu-id="adf01-117">The state of the operation</span></span>|
|<span data-ttu-id="adf01-118">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="adf01-118">mitigationInstruction</span></span>|<span data-ttu-id="adf01-119">String</span><span class="sxs-lookup"><span data-stu-id="adf01-119">String</span></span>|<span data-ttu-id="adf01-120">有关如何降低失败验证的说明</span><span class="sxs-lookup"><span data-stu-id="adf01-120">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="adf01-121">关系</span><span class="sxs-lookup"><span data-stu-id="adf01-121">Relationships</span></span>
<span data-ttu-id="adf01-122">无</span><span class="sxs-lookup"><span data-stu-id="adf01-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="adf01-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="adf01-123">JSON Representation</span></span>
<span data-ttu-id="adf01-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="adf01-124">Here is a JSON representation of the resource.</span></span>
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





