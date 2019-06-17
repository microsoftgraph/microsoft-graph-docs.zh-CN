---
title: deviceManagementApplicabilityRuleOsEdition 资源类型
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7b3baa84aa90af11f18d6c3dcf8ee1aeafecd240
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "35002516"
---
# <a name="devicemanagementapplicabilityruleosedition-resource-type"></a><span data-ttu-id="7cea4-103">deviceManagementApplicabilityRuleOsEdition 资源类型</span><span class="sxs-lookup"><span data-stu-id="7cea4-103">deviceManagementApplicabilityRuleOsEdition resource type</span></span>

> <span data-ttu-id="7cea4-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7cea4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7cea4-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7cea4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7cea4-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="7cea4-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="7cea4-107">属性</span><span class="sxs-lookup"><span data-stu-id="7cea4-107">Properties</span></span>
|<span data-ttu-id="7cea4-108">属性</span><span class="sxs-lookup"><span data-stu-id="7cea4-108">Property</span></span>|<span data-ttu-id="7cea4-109">类型</span><span class="sxs-lookup"><span data-stu-id="7cea4-109">Type</span></span>|<span data-ttu-id="7cea4-110">说明</span><span class="sxs-lookup"><span data-stu-id="7cea4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7cea4-111">osEditionTypes</span><span class="sxs-lookup"><span data-stu-id="7cea4-111">osEditionTypes</span></span>|<span data-ttu-id="7cea4-112">[windows10EditionType](../resources/intune-deviceconfig-windows10editiontype.md)集合</span><span class="sxs-lookup"><span data-stu-id="7cea4-112">[windows10EditionType](../resources/intune-deviceconfig-windows10editiontype.md) collection</span></span>|<span data-ttu-id="7cea4-113">适用性规则 OS 版本类型。</span><span class="sxs-lookup"><span data-stu-id="7cea4-113">Applicability rule OS edition type.</span></span>|
|<span data-ttu-id="7cea4-114">name</span><span class="sxs-lookup"><span data-stu-id="7cea4-114">name</span></span>|<span data-ttu-id="7cea4-115">String</span><span class="sxs-lookup"><span data-stu-id="7cea4-115">String</span></span>|<span data-ttu-id="7cea4-116">对象的名称。</span><span class="sxs-lookup"><span data-stu-id="7cea4-116">Name for object.</span></span>|
|<span data-ttu-id="7cea4-117">ruleType</span><span class="sxs-lookup"><span data-stu-id="7cea4-117">ruleType</span></span>|[<span data-ttu-id="7cea4-118">deviceManagementApplicabilityRuleType</span><span class="sxs-lookup"><span data-stu-id="7cea4-118">deviceManagementApplicabilityRuleType</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruletype.md)|<span data-ttu-id="7cea4-119">适用性规则类型。</span><span class="sxs-lookup"><span data-stu-id="7cea4-119">Applicability Rule type.</span></span> <span data-ttu-id="7cea4-120">可取值为：`include`、`exclude`。</span><span class="sxs-lookup"><span data-stu-id="7cea4-120">Possible values are: `include`, `exclude`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7cea4-121">关系</span><span class="sxs-lookup"><span data-stu-id="7cea4-121">Relationships</span></span>
<span data-ttu-id="7cea4-122">无</span><span class="sxs-lookup"><span data-stu-id="7cea4-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7cea4-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7cea4-123">JSON Representation</span></span>
<span data-ttu-id="7cea4-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7cea4-124">Here is a JSON representation of the resource.</span></span>
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





