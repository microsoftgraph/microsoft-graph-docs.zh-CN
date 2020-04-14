---
title: deviceManagementApplicabilityRuleOsVersion 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 460618d844a01fc913e80022235f38b017091236
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43469273"
---
# <a name="devicemanagementapplicabilityruleosversion-resource-type"></a><span data-ttu-id="ce2ec-103">deviceManagementApplicabilityRuleOsVersion 资源类型</span><span class="sxs-lookup"><span data-stu-id="ce2ec-103">deviceManagementApplicabilityRuleOsVersion resource type</span></span>

<span data-ttu-id="ce2ec-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce2ec-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ce2ec-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ce2ec-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ce2ec-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ce2ec-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce2ec-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ce2ec-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="ce2ec-108">属性</span><span class="sxs-lookup"><span data-stu-id="ce2ec-108">Properties</span></span>
|<span data-ttu-id="ce2ec-109">属性</span><span class="sxs-lookup"><span data-stu-id="ce2ec-109">Property</span></span>|<span data-ttu-id="ce2ec-110">类型</span><span class="sxs-lookup"><span data-stu-id="ce2ec-110">Type</span></span>|<span data-ttu-id="ce2ec-111">说明</span><span class="sxs-lookup"><span data-stu-id="ce2ec-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce2ec-112">minOSVersion</span><span class="sxs-lookup"><span data-stu-id="ce2ec-112">minOSVersion</span></span>|<span data-ttu-id="ce2ec-113">String</span><span class="sxs-lookup"><span data-stu-id="ce2ec-113">String</span></span>|<span data-ttu-id="ce2ec-114">适用性规则的最小 OS 版本。</span><span class="sxs-lookup"><span data-stu-id="ce2ec-114">Min OS version for Applicability Rule.</span></span>|
|<span data-ttu-id="ce2ec-115">maxOSVersion</span><span class="sxs-lookup"><span data-stu-id="ce2ec-115">maxOSVersion</span></span>|<span data-ttu-id="ce2ec-116">String</span><span class="sxs-lookup"><span data-stu-id="ce2ec-116">String</span></span>|<span data-ttu-id="ce2ec-117">适用性规则的最大 OS 版本。</span><span class="sxs-lookup"><span data-stu-id="ce2ec-117">Max OS version for Applicability Rule.</span></span>|
|<span data-ttu-id="ce2ec-118">name</span><span class="sxs-lookup"><span data-stu-id="ce2ec-118">name</span></span>|<span data-ttu-id="ce2ec-119">String</span><span class="sxs-lookup"><span data-stu-id="ce2ec-119">String</span></span>|<span data-ttu-id="ce2ec-120">对象的名称。</span><span class="sxs-lookup"><span data-stu-id="ce2ec-120">Name for object.</span></span>|
|<span data-ttu-id="ce2ec-121">ruleType</span><span class="sxs-lookup"><span data-stu-id="ce2ec-121">ruleType</span></span>|[<span data-ttu-id="ce2ec-122">deviceManagementApplicabilityRuleType</span><span class="sxs-lookup"><span data-stu-id="ce2ec-122">deviceManagementApplicabilityRuleType</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruletype.md)|<span data-ttu-id="ce2ec-123">适用性规则类型。</span><span class="sxs-lookup"><span data-stu-id="ce2ec-123">Applicability Rule type.</span></span> <span data-ttu-id="ce2ec-124">可取值为：`include`、`exclude`。</span><span class="sxs-lookup"><span data-stu-id="ce2ec-124">Possible values are: `include`, `exclude`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ce2ec-125">关系</span><span class="sxs-lookup"><span data-stu-id="ce2ec-125">Relationships</span></span>
<span data-ttu-id="ce2ec-126">无</span><span class="sxs-lookup"><span data-stu-id="ce2ec-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ce2ec-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ce2ec-127">JSON Representation</span></span>
<span data-ttu-id="ce2ec-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ce2ec-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
  "minOSVersion": "String",
  "maxOSVersion": "String",
  "name": "String",
  "ruleType": "String"
}
```



