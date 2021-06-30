---
title: cloudPcAuditResource 资源类型
description: 表示审核资源。这将显示具有多个已编辑属性的目标已编辑资源实体。
author: ecmadao
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: ebd61a14680c5e5f2917e273456bcce60672149e
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211287"
---
# <a name="cloudpcauditresource-resource-type"></a><span data-ttu-id="da96e-104">cloudPcAuditResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="da96e-104">cloudPcAuditResource resource type</span></span>

<span data-ttu-id="da96e-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da96e-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da96e-106">表示审核资源。</span><span class="sxs-lookup"><span data-stu-id="da96e-106">Represents the audit resource.</span></span><span data-ttu-id="da96e-107">这将显示具有多个已编辑属性的目标已编辑资源实体。</span><span class="sxs-lookup"><span data-stu-id="da96e-107"> This shows the target edited resource entity, with multiple edited properties.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a><span data-ttu-id="da96e-108">属性</span><span class="sxs-lookup"><span data-stu-id="da96e-108">Properties</span></span>
|<span data-ttu-id="da96e-109">属性</span><span class="sxs-lookup"><span data-stu-id="da96e-109">Property</span></span>|<span data-ttu-id="da96e-110">类型</span><span class="sxs-lookup"><span data-stu-id="da96e-110">Type</span></span>|<span data-ttu-id="da96e-111">说明</span><span class="sxs-lookup"><span data-stu-id="da96e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da96e-112">displayName</span><span class="sxs-lookup"><span data-stu-id="da96e-112">displayName</span></span>|<span data-ttu-id="da96e-113">String</span><span class="sxs-lookup"><span data-stu-id="da96e-113">String</span></span>|<span data-ttu-id="da96e-114">资源实体显示名称。</span><span class="sxs-lookup"><span data-stu-id="da96e-114">The resource entity display name.</span></span>|
|<span data-ttu-id="da96e-115">ModifiedProperties</span><span class="sxs-lookup"><span data-stu-id="da96e-115">modifiedProperties</span></span>|<span data-ttu-id="da96e-116">[cloudPcAuditProperty](../resources/cloudpcauditproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="da96e-116">[cloudPcAuditProperty](../resources/cloudpcauditproperty.md) collection</span></span>|<span data-ttu-id="da96e-117">已修改属性的列表。</span><span class="sxs-lookup"><span data-stu-id="da96e-117">A list of modified properties.</span></span>|
|<span data-ttu-id="da96e-118">type</span><span class="sxs-lookup"><span data-stu-id="da96e-118">type</span></span>|<span data-ttu-id="da96e-119">String</span><span class="sxs-lookup"><span data-stu-id="da96e-119">String</span></span>|<span data-ttu-id="da96e-120">审核资源的类型。</span><span class="sxs-lookup"><span data-stu-id="da96e-120">The type of the audit resource.</span></span>|
|<span data-ttu-id="da96e-121">resourceId</span><span class="sxs-lookup"><span data-stu-id="da96e-121">resourceId</span></span>|<span data-ttu-id="da96e-122">String</span><span class="sxs-lookup"><span data-stu-id="da96e-122">String</span></span>|<span data-ttu-id="da96e-123">审核资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="da96e-123">The ID of the audit resource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="da96e-124">关系</span><span class="sxs-lookup"><span data-stu-id="da96e-124">Relationships</span></span>

<span data-ttu-id="da96e-125">无</span><span class="sxs-lookup"><span data-stu-id="da96e-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="da96e-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="da96e-126">JSON Representation</span></span>

<span data-ttu-id="da96e-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="da96e-127">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcAuditResource"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcAuditResource",
  "displayName": "String",
  "modifiedProperties": [
    {
      "@odata.type": "microsoft.graph.cloudPcAuditProperty",
      "displayName": "String",
      "oldValue": "String",
      "newValue": "String"
    }
  ],
  "type": "String",
  "resourceId": "String"
}
```
