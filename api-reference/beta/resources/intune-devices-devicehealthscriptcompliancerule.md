---
title: deviceHealthScriptComplianceRule 资源类型
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8098582bd3e1b91a7e80af141e31847d2d3155cc
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36371473"
---
# <a name="devicehealthscriptcompliancerule-resource-type"></a><span data-ttu-id="689cf-103">deviceHealthScriptComplianceRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="689cf-103">deviceHealthScriptComplianceRule resource type</span></span>

> <span data-ttu-id="689cf-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="689cf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="689cf-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="689cf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="689cf-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="689cf-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="689cf-107">属性</span><span class="sxs-lookup"><span data-stu-id="689cf-107">Properties</span></span>
|<span data-ttu-id="689cf-108">属性</span><span class="sxs-lookup"><span data-stu-id="689cf-108">Property</span></span>|<span data-ttu-id="689cf-109">类型</span><span class="sxs-lookup"><span data-stu-id="689cf-109">Type</span></span>|<span data-ttu-id="689cf-110">说明</span><span class="sxs-lookup"><span data-stu-id="689cf-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="689cf-111">detectionType</span><span class="sxs-lookup"><span data-stu-id="689cf-111">detectionType</span></span>|[<span data-ttu-id="689cf-112">deviceHealthScriptDetectionType</span><span class="sxs-lookup"><span data-stu-id="689cf-112">deviceHealthScriptDetectionType</span></span>](../resources/intune-devices-devicehealthscriptdetectiontype.md)|<span data-ttu-id="689cf-113">尚未记录。</span><span class="sxs-lookup"><span data-stu-id="689cf-113">Not yet documented.</span></span> <span data-ttu-id="689cf-114">可取值为：`notConfigured`、`string`。</span><span class="sxs-lookup"><span data-stu-id="689cf-114">Possible values are: `notConfigured`, `string`.</span></span>|
|<span data-ttu-id="689cf-115">operator</span><span class="sxs-lookup"><span data-stu-id="689cf-115">operator</span></span>|[<span data-ttu-id="689cf-116">deviceHealthScriptComplianceRuleOperator</span><span class="sxs-lookup"><span data-stu-id="689cf-116">deviceHealthScriptComplianceRuleOperator</span></span>](../resources/intune-devices-devicehealthscriptcomplianceruleoperator.md)|<span data-ttu-id="689cf-117">尚未记录。</span><span class="sxs-lookup"><span data-stu-id="689cf-117">Not yet documented.</span></span> <span data-ttu-id="689cf-118">可取值为：`notConfigured`、`equal`、`notEqual`。</span><span class="sxs-lookup"><span data-stu-id="689cf-118">Possible values are: `notConfigured`, `equal`, `notEqual`.</span></span>|
|<span data-ttu-id="689cf-119">detectionValue</span><span class="sxs-lookup"><span data-stu-id="689cf-119">detectionValue</span></span>|<span data-ttu-id="689cf-120">String</span><span class="sxs-lookup"><span data-stu-id="689cf-120">String</span></span>|<span data-ttu-id="689cf-121">尚未记录</span><span class="sxs-lookup"><span data-stu-id="689cf-121">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="689cf-122">关系</span><span class="sxs-lookup"><span data-stu-id="689cf-122">Relationships</span></span>
<span data-ttu-id="689cf-123">无</span><span class="sxs-lookup"><span data-stu-id="689cf-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="689cf-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="689cf-124">JSON Representation</span></span>
<span data-ttu-id="689cf-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="689cf-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptComplianceRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptComplianceRule",
  "detectionType": "String",
  "operator": "String",
  "detectionValue": "String"
}
```



