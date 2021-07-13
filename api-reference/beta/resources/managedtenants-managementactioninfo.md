---
title: managementActionInfo 资源类型
description: 表示管理操作的引用信息。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: cde8e52b8329d03169eb5953dd92b897b3b8272e
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402285"
---
# <a name="managementactioninfo-resource-type"></a><span data-ttu-id="daf5e-103">managementActionInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="daf5e-103">managementActionInfo resource type</span></span>

<span data-ttu-id="daf5e-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="daf5e-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="daf5e-105">表示管理操作的引用信息。</span><span class="sxs-lookup"><span data-stu-id="daf5e-105">Represents reference information for a management action.</span></span>

## <a name="properties"></a><span data-ttu-id="daf5e-106">属性</span><span class="sxs-lookup"><span data-stu-id="daf5e-106">Properties</span></span>
|<span data-ttu-id="daf5e-107">属性</span><span class="sxs-lookup"><span data-stu-id="daf5e-107">Property</span></span>|<span data-ttu-id="daf5e-108">类型</span><span class="sxs-lookup"><span data-stu-id="daf5e-108">Type</span></span>|<span data-ttu-id="daf5e-109">说明</span><span class="sxs-lookup"><span data-stu-id="daf5e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="daf5e-110">managementActionId</span><span class="sxs-lookup"><span data-stu-id="daf5e-110">managementActionId</span></span>|<span data-ttu-id="daf5e-111">String</span><span class="sxs-lookup"><span data-stu-id="daf5e-111">String</span></span>|<span data-ttu-id="daf5e-112">管理操作标识符。</span><span class="sxs-lookup"><span data-stu-id="daf5e-112">The identifier for the management action.</span></span> <span data-ttu-id="daf5e-113">必填。</span><span class="sxs-lookup"><span data-stu-id="daf5e-113">Required.</span></span> <span data-ttu-id="daf5e-114">只读。</span><span class="sxs-lookup"><span data-stu-id="daf5e-114">Read-only.</span></span>|
|<span data-ttu-id="daf5e-115">managementTemplateId</span><span class="sxs-lookup"><span data-stu-id="daf5e-115">managementTemplateId</span></span>|<span data-ttu-id="daf5e-116">String</span><span class="sxs-lookup"><span data-stu-id="daf5e-116">String</span></span>|<span data-ttu-id="daf5e-117">管理模板的标识符。</span><span class="sxs-lookup"><span data-stu-id="daf5e-117">The identifier for the management template.</span></span> <span data-ttu-id="daf5e-118">必填。</span><span class="sxs-lookup"><span data-stu-id="daf5e-118">Required.</span></span> <span data-ttu-id="daf5e-119">只读。</span><span class="sxs-lookup"><span data-stu-id="daf5e-119">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="daf5e-120">关系</span><span class="sxs-lookup"><span data-stu-id="daf5e-120">Relationships</span></span>
<span data-ttu-id="daf5e-121">无。</span><span class="sxs-lookup"><span data-stu-id="daf5e-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="daf5e-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="daf5e-122">JSON representation</span></span>
<span data-ttu-id="daf5e-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="daf5e-123">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.managementActionInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managementActionInfo",
  "managementTemplateId": "String",
  "managementActionId": "String"
}
```
