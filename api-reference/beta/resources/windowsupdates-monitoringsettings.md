---
title: monitoringSettings 资源类型
description: 设置控制部署中的自动监视和响应。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: aff5fa9571628783521dcc5ae0113e767915c2c7
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067854"
---
# <a name="monitoringsettings-resource-type"></a><span data-ttu-id="ee188-103">monitoringSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="ee188-103">monitoringSettings resource type</span></span>

<span data-ttu-id="ee188-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="ee188-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee188-105">设置控制部署中的自动监视和响应。</span><span class="sxs-lookup"><span data-stu-id="ee188-105">Settings controlling automated monitoring and response in a deployment.</span></span>

## <a name="properties"></a><span data-ttu-id="ee188-106">属性</span><span class="sxs-lookup"><span data-stu-id="ee188-106">Properties</span></span>
|<span data-ttu-id="ee188-107">属性</span><span class="sxs-lookup"><span data-stu-id="ee188-107">Property</span></span>|<span data-ttu-id="ee188-108">类型</span><span class="sxs-lookup"><span data-stu-id="ee188-108">Type</span></span>|<span data-ttu-id="ee188-109">说明</span><span class="sxs-lookup"><span data-stu-id="ee188-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee188-110">monitoringRules</span><span class="sxs-lookup"><span data-stu-id="ee188-110">monitoringRules</span></span>|<span data-ttu-id="ee188-111">[microsoft.graph.windowsUpdates.monitoringRule](../resources/windowsupdates-monitoringrule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ee188-111">[microsoft.graph.windowsUpdates.monitoringRule](../resources/windowsupdates-monitoringrule.md) collection</span></span>|<span data-ttu-id="ee188-112">指定监视信号触发对部署的操作时可通过的规则。</span><span class="sxs-lookup"><span data-stu-id="ee188-112">Specifies the rules through which monitoring signals can trigger actions on the deployment.</span></span> <span data-ttu-id="ee188-113">使用"or"组合规则。</span><span class="sxs-lookup"><span data-stu-id="ee188-113">Rules are combined using "or".</span></span>|

## <a name="relationships"></a><span data-ttu-id="ee188-114">关系</span><span class="sxs-lookup"><span data-stu-id="ee188-114">Relationships</span></span>
<span data-ttu-id="ee188-115">无。</span><span class="sxs-lookup"><span data-stu-id="ee188-115">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ee188-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ee188-116">JSON representation</span></span>
<span data-ttu-id="ee188-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ee188-117">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.monitoringSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.monitoringSettings",
  "monitoringRules": [
    {
      "@odata.type": "microsoft.graph.windowsUpdates.monitoringRule"
    }
  ]
}
```

