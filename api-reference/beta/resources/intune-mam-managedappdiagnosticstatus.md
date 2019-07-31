---
title: managedAppDiagnosticStatus 资源类型
description: 表示诊断状态。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0804b83f819a2f083493418e0cd1240702c2e425
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35998427"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="40905-103">managedAppDiagnosticStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="40905-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="40905-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="40905-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="40905-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="40905-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40905-106">表示诊断状态。</span><span class="sxs-lookup"><span data-stu-id="40905-106">Represents diagnostics status.</span></span>

## <a name="properties"></a><span data-ttu-id="40905-107">属性</span><span class="sxs-lookup"><span data-stu-id="40905-107">Properties</span></span>
|<span data-ttu-id="40905-108">属性</span><span class="sxs-lookup"><span data-stu-id="40905-108">Property</span></span>|<span data-ttu-id="40905-109">类型</span><span class="sxs-lookup"><span data-stu-id="40905-109">Type</span></span>|<span data-ttu-id="40905-110">说明</span><span class="sxs-lookup"><span data-stu-id="40905-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40905-111">validationName</span><span class="sxs-lookup"><span data-stu-id="40905-111">validationName</span></span>|<span data-ttu-id="40905-112">String</span><span class="sxs-lookup"><span data-stu-id="40905-112">String</span></span>|<span data-ttu-id="40905-113">验证友好名称</span><span class="sxs-lookup"><span data-stu-id="40905-113">The validation friendly name</span></span>|
|<span data-ttu-id="40905-114">state</span><span class="sxs-lookup"><span data-stu-id="40905-114">state</span></span>|<span data-ttu-id="40905-115">String</span><span class="sxs-lookup"><span data-stu-id="40905-115">String</span></span>|<span data-ttu-id="40905-116">操作状态</span><span class="sxs-lookup"><span data-stu-id="40905-116">The state of the operation</span></span>|
|<span data-ttu-id="40905-117">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="40905-117">mitigationInstruction</span></span>|<span data-ttu-id="40905-118">String</span><span class="sxs-lookup"><span data-stu-id="40905-118">String</span></span>|<span data-ttu-id="40905-119">有关如何降低失败验证的说明</span><span class="sxs-lookup"><span data-stu-id="40905-119">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="40905-120">关系</span><span class="sxs-lookup"><span data-stu-id="40905-120">Relationships</span></span>
<span data-ttu-id="40905-121">无</span><span class="sxs-lookup"><span data-stu-id="40905-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="40905-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="40905-122">JSON Representation</span></span>
<span data-ttu-id="40905-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="40905-123">Here is a JSON representation of the resource.</span></span>
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





