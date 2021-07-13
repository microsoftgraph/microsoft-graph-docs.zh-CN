---
title: managementTemplateDetailedInfo 资源类型
description: 表示管理模板的详细信息。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: e98d2ca41bc972a5dca33c575363b1bac27d87a5
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402360"
---
# <a name="managementtemplatedetailedinfo-resource-type"></a><span data-ttu-id="17725-103">managementTemplateDetailedInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="17725-103">managementTemplateDetailedInfo resource type</span></span>

<span data-ttu-id="17725-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="17725-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17725-105">表示管理模板的详细信息。</span><span class="sxs-lookup"><span data-stu-id="17725-105">Represents detailed information for the management template.</span></span>

## <a name="properties"></a><span data-ttu-id="17725-106">属性</span><span class="sxs-lookup"><span data-stu-id="17725-106">Properties</span></span>
|<span data-ttu-id="17725-107">属性</span><span class="sxs-lookup"><span data-stu-id="17725-107">Property</span></span>|<span data-ttu-id="17725-108">类型</span><span class="sxs-lookup"><span data-stu-id="17725-108">Type</span></span>|<span data-ttu-id="17725-109">说明</span><span class="sxs-lookup"><span data-stu-id="17725-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17725-110">category</span><span class="sxs-lookup"><span data-stu-id="17725-110">category</span></span>|<span data-ttu-id="17725-111">managementCategory</span><span class="sxs-lookup"><span data-stu-id="17725-111">managementCategory</span></span>|<span data-ttu-id="17725-112">管理模板的管理类别。</span><span class="sxs-lookup"><span data-stu-id="17725-112">The management category for the management template.</span></span> <span data-ttu-id="17725-113">可取值为：`custom`、`devices`、`identity`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="17725-113">Possible values are: `custom`, `devices`, `identity`, `unknownFutureValue`.</span></span> <span data-ttu-id="17725-114">必填。</span><span class="sxs-lookup"><span data-stu-id="17725-114">Required.</span></span> <span data-ttu-id="17725-115">只读。</span><span class="sxs-lookup"><span data-stu-id="17725-115">Read-only.</span></span>|
|<span data-ttu-id="17725-116">displayName</span><span class="sxs-lookup"><span data-stu-id="17725-116">displayName</span></span>|<span data-ttu-id="17725-117">String</span><span class="sxs-lookup"><span data-stu-id="17725-117">String</span></span>|<span data-ttu-id="17725-118">管理显示名称的表单。</span><span class="sxs-lookup"><span data-stu-id="17725-118">The display name for the management template.</span></span> <span data-ttu-id="17725-119">必填。</span><span class="sxs-lookup"><span data-stu-id="17725-119">Required.</span></span> <span data-ttu-id="17725-120">只读。</span><span class="sxs-lookup"><span data-stu-id="17725-120">Read-only.</span></span>|
|<span data-ttu-id="17725-121">managementTemplateId</span><span class="sxs-lookup"><span data-stu-id="17725-121">managementTemplateId</span></span>|<span data-ttu-id="17725-122">String</span><span class="sxs-lookup"><span data-stu-id="17725-122">String</span></span>|<span data-ttu-id="17725-123">管理模板的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="17725-123">The unique identifier for the management template.</span></span> <span data-ttu-id="17725-124">必填。</span><span class="sxs-lookup"><span data-stu-id="17725-124">Required.</span></span> <span data-ttu-id="17725-125">只读。</span><span class="sxs-lookup"><span data-stu-id="17725-125">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="17725-126">关系</span><span class="sxs-lookup"><span data-stu-id="17725-126">Relationships</span></span>
<span data-ttu-id="17725-127">无。</span><span class="sxs-lookup"><span data-stu-id="17725-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="17725-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="17725-128">JSON representation</span></span>
<span data-ttu-id="17725-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="17725-129">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.managementTemplateDetailedInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managementTemplateDetailedInfo",
  "managementTemplateId": "String",
  "displayName": "String",
  "category": "String"
}
```
