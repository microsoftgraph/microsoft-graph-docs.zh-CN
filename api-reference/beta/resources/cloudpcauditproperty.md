---
title: cloudPcAuditProperty 资源类型
description: 表示审核属性。这将显示已编辑的属性名称、旧值和新值。
author: ecmadao
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 1f73733f0ace4526d3cbae226c963887d5af37ce
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211290"
---
# <a name="cloudpcauditproperty-resource-type"></a><span data-ttu-id="8a3df-104">cloudPcAuditProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="8a3df-104">cloudPcAuditProperty resource type</span></span>

<span data-ttu-id="8a3df-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a3df-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a3df-106">表示审核属性。</span><span class="sxs-lookup"><span data-stu-id="8a3df-106">Represents the audit property.</span></span><span data-ttu-id="8a3df-107">这将显示已编辑的属性名称、旧值和新值。</span><span class="sxs-lookup"><span data-stu-id="8a3df-107"> This shows the edited property name, the old value, and the new value.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a><span data-ttu-id="8a3df-108">属性</span><span class="sxs-lookup"><span data-stu-id="8a3df-108">Properties</span></span>
|<span data-ttu-id="8a3df-109">属性</span><span class="sxs-lookup"><span data-stu-id="8a3df-109">Property</span></span>|<span data-ttu-id="8a3df-110">类型</span><span class="sxs-lookup"><span data-stu-id="8a3df-110">Type</span></span>|<span data-ttu-id="8a3df-111">说明</span><span class="sxs-lookup"><span data-stu-id="8a3df-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a3df-112">displayName</span><span class="sxs-lookup"><span data-stu-id="8a3df-112">displayName</span></span>|<span data-ttu-id="8a3df-113">String</span><span class="sxs-lookup"><span data-stu-id="8a3df-113">String</span></span>|<span data-ttu-id="8a3df-114">显示名称。</span><span class="sxs-lookup"><span data-stu-id="8a3df-114">Display name.</span></span>|
|<span data-ttu-id="8a3df-115">oldValue</span><span class="sxs-lookup"><span data-stu-id="8a3df-115">oldValue</span></span>|<span data-ttu-id="8a3df-116">String</span><span class="sxs-lookup"><span data-stu-id="8a3df-116">String</span></span>|<span data-ttu-id="8a3df-117">旧值。</span><span class="sxs-lookup"><span data-stu-id="8a3df-117">Old value.</span></span>|
|<span data-ttu-id="8a3df-118">NewValue</span><span class="sxs-lookup"><span data-stu-id="8a3df-118">newValue</span></span>|<span data-ttu-id="8a3df-119">String</span><span class="sxs-lookup"><span data-stu-id="8a3df-119">String</span></span>|<span data-ttu-id="8a3df-120">新值。</span><span class="sxs-lookup"><span data-stu-id="8a3df-120">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8a3df-121">关系</span><span class="sxs-lookup"><span data-stu-id="8a3df-121">Relationships</span></span>

<span data-ttu-id="8a3df-122">无。</span><span class="sxs-lookup"><span data-stu-id="8a3df-122">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8a3df-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8a3df-123">JSON Representation</span></span>

<span data-ttu-id="8a3df-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8a3df-124">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcAuditProperty"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcAuditProperty",
  "displayName": "String",
  "oldValue": "String",
  "newValue": "String"
}
```
