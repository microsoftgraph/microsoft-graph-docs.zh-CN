---
title: deviceManagementApplicabilityRuleOsEdition 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cff458e69d0394ce3e74f2faab29bec9cfe2ea50
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49283496"
---
# <a name="devicemanagementapplicabilityruleosedition-resource-type"></a><span data-ttu-id="20981-103">deviceManagementApplicabilityRuleOsEdition 资源类型</span><span class="sxs-lookup"><span data-stu-id="20981-103">deviceManagementApplicabilityRuleOsEdition resource type</span></span>

<span data-ttu-id="20981-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20981-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="20981-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="20981-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="20981-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="20981-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20981-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="20981-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="20981-108">属性</span><span class="sxs-lookup"><span data-stu-id="20981-108">Properties</span></span>
|<span data-ttu-id="20981-109">属性</span><span class="sxs-lookup"><span data-stu-id="20981-109">Property</span></span>|<span data-ttu-id="20981-110">类型</span><span class="sxs-lookup"><span data-stu-id="20981-110">Type</span></span>|<span data-ttu-id="20981-111">Description</span><span class="sxs-lookup"><span data-stu-id="20981-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20981-112">osEditionTypes</span><span class="sxs-lookup"><span data-stu-id="20981-112">osEditionTypes</span></span>|<span data-ttu-id="20981-113">[windows10EditionType](../resources/intune-deviceconfig-windows10editiontype.md) 集合</span><span class="sxs-lookup"><span data-stu-id="20981-113">[windows10EditionType](../resources/intune-deviceconfig-windows10editiontype.md) collection</span></span>|<span data-ttu-id="20981-114">适用性规则 OS 版本类型。</span><span class="sxs-lookup"><span data-stu-id="20981-114">Applicability rule OS edition type.</span></span>|
|<span data-ttu-id="20981-115">name</span><span class="sxs-lookup"><span data-stu-id="20981-115">name</span></span>|<span data-ttu-id="20981-116">字符串</span><span class="sxs-lookup"><span data-stu-id="20981-116">String</span></span>|<span data-ttu-id="20981-117">对象的名称。</span><span class="sxs-lookup"><span data-stu-id="20981-117">Name for object.</span></span>|
|<span data-ttu-id="20981-118">ruleType</span><span class="sxs-lookup"><span data-stu-id="20981-118">ruleType</span></span>|[<span data-ttu-id="20981-119">deviceManagementApplicabilityRuleType</span><span class="sxs-lookup"><span data-stu-id="20981-119">deviceManagementApplicabilityRuleType</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruletype.md)|<span data-ttu-id="20981-120">适用性规则类型。</span><span class="sxs-lookup"><span data-stu-id="20981-120">Applicability Rule type.</span></span> <span data-ttu-id="20981-121">可取值为：`include`、`exclude`。</span><span class="sxs-lookup"><span data-stu-id="20981-121">Possible values are: `include`, `exclude`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="20981-122">关系</span><span class="sxs-lookup"><span data-stu-id="20981-122">Relationships</span></span>
<span data-ttu-id="20981-123">无</span><span class="sxs-lookup"><span data-stu-id="20981-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="20981-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="20981-124">JSON Representation</span></span>
<span data-ttu-id="20981-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="20981-125">Here is a JSON representation of the resource.</span></span>
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




