---
title: deviceManagementApplicabilityRuleOsVersion 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cdd0e5c7a700932af5c5ffa4dd568c252dcf9848
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724577"
---
# <a name="devicemanagementapplicabilityruleosversion-resource-type"></a><span data-ttu-id="1d9a6-103">deviceManagementApplicabilityRuleOsVersion 资源类型</span><span class="sxs-lookup"><span data-stu-id="1d9a6-103">deviceManagementApplicabilityRuleOsVersion resource type</span></span>

<span data-ttu-id="1d9a6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d9a6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1d9a6-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1d9a6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1d9a6-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1d9a6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d9a6-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="1d9a6-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="1d9a6-108">属性</span><span class="sxs-lookup"><span data-stu-id="1d9a6-108">Properties</span></span>
|<span data-ttu-id="1d9a6-109">属性</span><span class="sxs-lookup"><span data-stu-id="1d9a6-109">Property</span></span>|<span data-ttu-id="1d9a6-110">类型</span><span class="sxs-lookup"><span data-stu-id="1d9a6-110">Type</span></span>|<span data-ttu-id="1d9a6-111">说明</span><span class="sxs-lookup"><span data-stu-id="1d9a6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d9a6-112">minOSVersion</span><span class="sxs-lookup"><span data-stu-id="1d9a6-112">minOSVersion</span></span>|<span data-ttu-id="1d9a6-113">String</span><span class="sxs-lookup"><span data-stu-id="1d9a6-113">String</span></span>|<span data-ttu-id="1d9a6-114">适用性规则的最小 OS 版本。</span><span class="sxs-lookup"><span data-stu-id="1d9a6-114">Min OS version for Applicability Rule.</span></span>|
|<span data-ttu-id="1d9a6-115">maxOSVersion</span><span class="sxs-lookup"><span data-stu-id="1d9a6-115">maxOSVersion</span></span>|<span data-ttu-id="1d9a6-116">String</span><span class="sxs-lookup"><span data-stu-id="1d9a6-116">String</span></span>|<span data-ttu-id="1d9a6-117">适用性规则的最大 OS 版本。</span><span class="sxs-lookup"><span data-stu-id="1d9a6-117">Max OS version for Applicability Rule.</span></span>|
|<span data-ttu-id="1d9a6-118">name</span><span class="sxs-lookup"><span data-stu-id="1d9a6-118">name</span></span>|<span data-ttu-id="1d9a6-119">String</span><span class="sxs-lookup"><span data-stu-id="1d9a6-119">String</span></span>|<span data-ttu-id="1d9a6-120">对象的名称。</span><span class="sxs-lookup"><span data-stu-id="1d9a6-120">Name for object.</span></span>|
|<span data-ttu-id="1d9a6-121">ruleType</span><span class="sxs-lookup"><span data-stu-id="1d9a6-121">ruleType</span></span>|[<span data-ttu-id="1d9a6-122">deviceManagementApplicabilityRuleType</span><span class="sxs-lookup"><span data-stu-id="1d9a6-122">deviceManagementApplicabilityRuleType</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruletype.md)|<span data-ttu-id="1d9a6-123">适用性规则类型。</span><span class="sxs-lookup"><span data-stu-id="1d9a6-123">Applicability Rule type.</span></span> <span data-ttu-id="1d9a6-124">可取值为：`include`、`exclude`。</span><span class="sxs-lookup"><span data-stu-id="1d9a6-124">Possible values are: `include`, `exclude`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1d9a6-125">关系</span><span class="sxs-lookup"><span data-stu-id="1d9a6-125">Relationships</span></span>
<span data-ttu-id="1d9a6-126">无</span><span class="sxs-lookup"><span data-stu-id="1d9a6-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1d9a6-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1d9a6-127">JSON Representation</span></span>
<span data-ttu-id="1d9a6-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1d9a6-128">Here is a JSON representation of the resource.</span></span>
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





