---
title: managementIntentInfo 资源类型
description: 表示管理意图的关系信息。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 9bc58ff4c850661b968e7b540de9038074406ac5
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402280"
---
# <a name="managementintentinfo-resource-type"></a><span data-ttu-id="8933a-103">managementIntentInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="8933a-103">managementIntentInfo resource type</span></span>

<span data-ttu-id="8933a-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="8933a-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8933a-105">表示管理意图的关系信息。</span><span class="sxs-lookup"><span data-stu-id="8933a-105">Represents relationship information for a management intent.</span></span>

## <a name="properties"></a><span data-ttu-id="8933a-106">属性</span><span class="sxs-lookup"><span data-stu-id="8933a-106">Properties</span></span>
|<span data-ttu-id="8933a-107">属性</span><span class="sxs-lookup"><span data-stu-id="8933a-107">Property</span></span>|<span data-ttu-id="8933a-108">类型</span><span class="sxs-lookup"><span data-stu-id="8933a-108">Type</span></span>|<span data-ttu-id="8933a-109">说明</span><span class="sxs-lookup"><span data-stu-id="8933a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8933a-110">managementIntentDisplayName</span><span class="sxs-lookup"><span data-stu-id="8933a-110">managementIntentDisplayName</span></span>|<span data-ttu-id="8933a-111">String</span><span class="sxs-lookup"><span data-stu-id="8933a-111">String</span></span>|<span data-ttu-id="8933a-112">管理显示名称定义。</span><span class="sxs-lookup"><span data-stu-id="8933a-112">The display name for the management intent.</span></span> <span data-ttu-id="8933a-113">可选。</span><span class="sxs-lookup"><span data-stu-id="8933a-113">Optional.</span></span> <span data-ttu-id="8933a-114">只读。</span><span class="sxs-lookup"><span data-stu-id="8933a-114">Read-only.</span></span>|
|<span data-ttu-id="8933a-115">managementIntentId</span><span class="sxs-lookup"><span data-stu-id="8933a-115">managementIntentId</span></span>|<span data-ttu-id="8933a-116">String</span><span class="sxs-lookup"><span data-stu-id="8933a-116">String</span></span>|<span data-ttu-id="8933a-117">管理意图的标识符。</span><span class="sxs-lookup"><span data-stu-id="8933a-117">The identifier for the management intent.</span></span> <span data-ttu-id="8933a-118">必填。</span><span class="sxs-lookup"><span data-stu-id="8933a-118">Required.</span></span> <span data-ttu-id="8933a-119">只读。</span><span class="sxs-lookup"><span data-stu-id="8933a-119">Read-only.</span></span>|
|<span data-ttu-id="8933a-120">managementTemplates</span><span class="sxs-lookup"><span data-stu-id="8933a-120">managementTemplates</span></span>|<span data-ttu-id="8933a-121">[microsoft.graph.managedTenants.managementTemplateDetailedInfo](../resources/managedtenants-managementtemplatedetailedinfo.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8933a-121">[microsoft.graph.managedTenants.managementTemplateDetailedInfo](../resources/managedtenants-managementtemplatedetailedinfo.md) collection</span></span>|<span data-ttu-id="8933a-122">与管理意图关联的管理模板信息的集合。</span><span class="sxs-lookup"><span data-stu-id="8933a-122">The collection of management template information associated with the management intent.</span></span> <span data-ttu-id="8933a-123">可选。</span><span class="sxs-lookup"><span data-stu-id="8933a-123">Optional.</span></span> <span data-ttu-id="8933a-124">只读。</span><span class="sxs-lookup"><span data-stu-id="8933a-124">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8933a-125">关系</span><span class="sxs-lookup"><span data-stu-id="8933a-125">Relationships</span></span>
<span data-ttu-id="8933a-126">无。</span><span class="sxs-lookup"><span data-stu-id="8933a-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8933a-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8933a-127">JSON representation</span></span>
<span data-ttu-id="8933a-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8933a-128">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.managementIntentInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managementIntentInfo",
  "managementIntentId": "String",
  "managementIntentDisplayName": "String",
  "managementTemplates": [
    {
      "@odata.type": "microsoft.graph.managedTenants.managementTemplateDetailedInfo"
    }
  ]
}
```
