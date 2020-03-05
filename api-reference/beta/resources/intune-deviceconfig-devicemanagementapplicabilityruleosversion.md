---
title: deviceManagementApplicabilityRuleOsVersion 资源类型
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ef729e66f5198acae1f7a123bfc4911de76c784d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526602"
---
# <a name="devicemanagementapplicabilityruleosversion-resource-type"></a><span data-ttu-id="73b1a-103">deviceManagementApplicabilityRuleOsVersion 资源类型</span><span class="sxs-lookup"><span data-stu-id="73b1a-103">deviceManagementApplicabilityRuleOsVersion resource type</span></span>

<span data-ttu-id="73b1a-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="73b1a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="73b1a-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="73b1a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="73b1a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="73b1a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73b1a-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="73b1a-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="73b1a-108">属性</span><span class="sxs-lookup"><span data-stu-id="73b1a-108">Properties</span></span>
|<span data-ttu-id="73b1a-109">属性</span><span class="sxs-lookup"><span data-stu-id="73b1a-109">Property</span></span>|<span data-ttu-id="73b1a-110">类型</span><span class="sxs-lookup"><span data-stu-id="73b1a-110">Type</span></span>|<span data-ttu-id="73b1a-111">说明</span><span class="sxs-lookup"><span data-stu-id="73b1a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73b1a-112">minOSVersion</span><span class="sxs-lookup"><span data-stu-id="73b1a-112">minOSVersion</span></span>|<span data-ttu-id="73b1a-113">String</span><span class="sxs-lookup"><span data-stu-id="73b1a-113">String</span></span>|<span data-ttu-id="73b1a-114">适用性规则的最小 OS 版本。</span><span class="sxs-lookup"><span data-stu-id="73b1a-114">Min OS version for Applicability Rule.</span></span>|
|<span data-ttu-id="73b1a-115">maxOSVersion</span><span class="sxs-lookup"><span data-stu-id="73b1a-115">maxOSVersion</span></span>|<span data-ttu-id="73b1a-116">String</span><span class="sxs-lookup"><span data-stu-id="73b1a-116">String</span></span>|<span data-ttu-id="73b1a-117">适用性规则的最大 OS 版本。</span><span class="sxs-lookup"><span data-stu-id="73b1a-117">Max OS version for Applicability Rule.</span></span>|
|<span data-ttu-id="73b1a-118">name</span><span class="sxs-lookup"><span data-stu-id="73b1a-118">name</span></span>|<span data-ttu-id="73b1a-119">String</span><span class="sxs-lookup"><span data-stu-id="73b1a-119">String</span></span>|<span data-ttu-id="73b1a-120">对象的名称。</span><span class="sxs-lookup"><span data-stu-id="73b1a-120">Name for object.</span></span>|
|<span data-ttu-id="73b1a-121">ruleType</span><span class="sxs-lookup"><span data-stu-id="73b1a-121">ruleType</span></span>|[<span data-ttu-id="73b1a-122">deviceManagementApplicabilityRuleType</span><span class="sxs-lookup"><span data-stu-id="73b1a-122">deviceManagementApplicabilityRuleType</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruletype.md)|<span data-ttu-id="73b1a-123">适用性规则类型。</span><span class="sxs-lookup"><span data-stu-id="73b1a-123">Applicability Rule type.</span></span> <span data-ttu-id="73b1a-124">可取值为：`include`、`exclude`。</span><span class="sxs-lookup"><span data-stu-id="73b1a-124">Possible values are: `include`, `exclude`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="73b1a-125">关系</span><span class="sxs-lookup"><span data-stu-id="73b1a-125">Relationships</span></span>
<span data-ttu-id="73b1a-126">无</span><span class="sxs-lookup"><span data-stu-id="73b1a-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="73b1a-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="73b1a-127">JSON Representation</span></span>
<span data-ttu-id="73b1a-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="73b1a-128">Here is a JSON representation of the resource.</span></span>
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



