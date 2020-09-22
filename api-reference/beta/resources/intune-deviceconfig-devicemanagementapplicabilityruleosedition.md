---
title: deviceManagementApplicabilityRuleOsEdition 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a2e145f54116272687683789e67cbab3e6429bf4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985942"
---
# <a name="devicemanagementapplicabilityruleosedition-resource-type"></a><span data-ttu-id="d81e1-103">deviceManagementApplicabilityRuleOsEdition 资源类型</span><span class="sxs-lookup"><span data-stu-id="d81e1-103">deviceManagementApplicabilityRuleOsEdition resource type</span></span>

<span data-ttu-id="d81e1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d81e1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d81e1-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d81e1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d81e1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d81e1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d81e1-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d81e1-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="d81e1-108">属性</span><span class="sxs-lookup"><span data-stu-id="d81e1-108">Properties</span></span>
|<span data-ttu-id="d81e1-109">属性</span><span class="sxs-lookup"><span data-stu-id="d81e1-109">Property</span></span>|<span data-ttu-id="d81e1-110">类型</span><span class="sxs-lookup"><span data-stu-id="d81e1-110">Type</span></span>|<span data-ttu-id="d81e1-111">说明</span><span class="sxs-lookup"><span data-stu-id="d81e1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d81e1-112">osEditionTypes</span><span class="sxs-lookup"><span data-stu-id="d81e1-112">osEditionTypes</span></span>|<span data-ttu-id="d81e1-113">[windows10EditionType](../resources/intune-deviceconfig-windows10editiontype.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d81e1-113">[windows10EditionType](../resources/intune-deviceconfig-windows10editiontype.md) collection</span></span>|<span data-ttu-id="d81e1-114">适用性规则 OS 版本类型。</span><span class="sxs-lookup"><span data-stu-id="d81e1-114">Applicability rule OS edition type.</span></span>|
|<span data-ttu-id="d81e1-115">name</span><span class="sxs-lookup"><span data-stu-id="d81e1-115">name</span></span>|<span data-ttu-id="d81e1-116">String</span><span class="sxs-lookup"><span data-stu-id="d81e1-116">String</span></span>|<span data-ttu-id="d81e1-117">对象的名称。</span><span class="sxs-lookup"><span data-stu-id="d81e1-117">Name for object.</span></span>|
|<span data-ttu-id="d81e1-118">ruleType</span><span class="sxs-lookup"><span data-stu-id="d81e1-118">ruleType</span></span>|[<span data-ttu-id="d81e1-119">deviceManagementApplicabilityRuleType</span><span class="sxs-lookup"><span data-stu-id="d81e1-119">deviceManagementApplicabilityRuleType</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruletype.md)|<span data-ttu-id="d81e1-120">适用性规则类型。</span><span class="sxs-lookup"><span data-stu-id="d81e1-120">Applicability Rule type.</span></span> <span data-ttu-id="d81e1-121">可取值为：`include`、`exclude`。</span><span class="sxs-lookup"><span data-stu-id="d81e1-121">Possible values are: `include`, `exclude`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d81e1-122">关系</span><span class="sxs-lookup"><span data-stu-id="d81e1-122">Relationships</span></span>
<span data-ttu-id="d81e1-123">无</span><span class="sxs-lookup"><span data-stu-id="d81e1-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d81e1-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d81e1-124">JSON Representation</span></span>
<span data-ttu-id="d81e1-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d81e1-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
  "osEditionTypes": [
    "String"
  ],
  "name": "String",
  "ruleType": "String"
}
```






