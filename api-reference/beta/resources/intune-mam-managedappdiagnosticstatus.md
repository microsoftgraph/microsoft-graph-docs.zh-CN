---
title: managedAppDiagnosticStatus 资源类型
description: 表示诊断状态。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 907f9940b7cbb4a35f69e0792092e14c99aebdae
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34996293"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="804cd-103">managedAppDiagnosticStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="804cd-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="804cd-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="804cd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="804cd-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="804cd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="804cd-106">表示诊断状态。</span><span class="sxs-lookup"><span data-stu-id="804cd-106">Represents diagnostics status.</span></span>

## <a name="properties"></a><span data-ttu-id="804cd-107">属性</span><span class="sxs-lookup"><span data-stu-id="804cd-107">Properties</span></span>
|<span data-ttu-id="804cd-108">属性</span><span class="sxs-lookup"><span data-stu-id="804cd-108">Property</span></span>|<span data-ttu-id="804cd-109">类型</span><span class="sxs-lookup"><span data-stu-id="804cd-109">Type</span></span>|<span data-ttu-id="804cd-110">说明</span><span class="sxs-lookup"><span data-stu-id="804cd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="804cd-111">validationName</span><span class="sxs-lookup"><span data-stu-id="804cd-111">validationName</span></span>|<span data-ttu-id="804cd-112">String</span><span class="sxs-lookup"><span data-stu-id="804cd-112">String</span></span>|<span data-ttu-id="804cd-113">验证友好名称</span><span class="sxs-lookup"><span data-stu-id="804cd-113">The validation friendly name</span></span>|
|<span data-ttu-id="804cd-114">state</span><span class="sxs-lookup"><span data-stu-id="804cd-114">state</span></span>|<span data-ttu-id="804cd-115">String</span><span class="sxs-lookup"><span data-stu-id="804cd-115">String</span></span>|<span data-ttu-id="804cd-116">操作状态</span><span class="sxs-lookup"><span data-stu-id="804cd-116">The state of the operation</span></span>|
|<span data-ttu-id="804cd-117">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="804cd-117">mitigationInstruction</span></span>|<span data-ttu-id="804cd-118">String</span><span class="sxs-lookup"><span data-stu-id="804cd-118">String</span></span>|<span data-ttu-id="804cd-119">有关如何降低失败验证的说明</span><span class="sxs-lookup"><span data-stu-id="804cd-119">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="804cd-120">关系</span><span class="sxs-lookup"><span data-stu-id="804cd-120">Relationships</span></span>
<span data-ttu-id="804cd-121">无</span><span class="sxs-lookup"><span data-stu-id="804cd-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="804cd-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="804cd-122">JSON Representation</span></span>
<span data-ttu-id="804cd-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="804cd-123">Here is a JSON representation of the resource.</span></span>
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





