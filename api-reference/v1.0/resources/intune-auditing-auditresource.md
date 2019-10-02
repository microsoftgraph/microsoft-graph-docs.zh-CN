---
title: auditResource 资源类型
description: 包含审核资源的属性的类。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bff6bfde2816292b57e31bca81cf085297ee537f
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37355972"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="497ef-103">auditResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="497ef-103">auditResource resource type</span></span>

> <span data-ttu-id="497ef-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="497ef-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="497ef-105">包含审核资源的属性的类。</span><span class="sxs-lookup"><span data-stu-id="497ef-105">A class containing the properties for Audit Resource.</span></span>

## <a name="properties"></a><span data-ttu-id="497ef-106">属性</span><span class="sxs-lookup"><span data-stu-id="497ef-106">Properties</span></span>
|<span data-ttu-id="497ef-107">属性</span><span class="sxs-lookup"><span data-stu-id="497ef-107">Property</span></span>|<span data-ttu-id="497ef-108">类型</span><span class="sxs-lookup"><span data-stu-id="497ef-108">Type</span></span>|<span data-ttu-id="497ef-109">说明</span><span class="sxs-lookup"><span data-stu-id="497ef-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="497ef-110">displayName</span><span class="sxs-lookup"><span data-stu-id="497ef-110">displayName</span></span>|<span data-ttu-id="497ef-111">String</span><span class="sxs-lookup"><span data-stu-id="497ef-111">String</span></span>|<span data-ttu-id="497ef-112">显示名称。</span><span class="sxs-lookup"><span data-stu-id="497ef-112">Display name.</span></span>|
|<span data-ttu-id="497ef-113">ModifiedProperties</span><span class="sxs-lookup"><span data-stu-id="497ef-113">modifiedProperties</span></span>|<span data-ttu-id="497ef-114">[auditProperty](../resources/intune-auditing-auditproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="497ef-114">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="497ef-115">已修改属性列表。</span><span class="sxs-lookup"><span data-stu-id="497ef-115">List of modified properties.</span></span>|
|<span data-ttu-id="497ef-116">type</span><span class="sxs-lookup"><span data-stu-id="497ef-116">type</span></span>|<span data-ttu-id="497ef-117">字符串</span><span class="sxs-lookup"><span data-stu-id="497ef-117">String</span></span>|<span data-ttu-id="497ef-118">审核资源的类型。</span><span class="sxs-lookup"><span data-stu-id="497ef-118">Audit resource's type.</span></span>|
|<span data-ttu-id="497ef-119">resourceId</span><span class="sxs-lookup"><span data-stu-id="497ef-119">resourceId</span></span>|<span data-ttu-id="497ef-120">String</span><span class="sxs-lookup"><span data-stu-id="497ef-120">String</span></span>|<span data-ttu-id="497ef-121">审核资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="497ef-121">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="497ef-122">关系</span><span class="sxs-lookup"><span data-stu-id="497ef-122">Relationships</span></span>
<span data-ttu-id="497ef-123">无</span><span class="sxs-lookup"><span data-stu-id="497ef-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="497ef-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="497ef-124">JSON Representation</span></span>
<span data-ttu-id="497ef-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="497ef-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditResource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditResource",
  "displayName": "String",
  "modifiedProperties": [
    {
      "@odata.type": "microsoft.graph.auditProperty",
      "displayName": "String",
      "oldValue": "String",
      "newValue": "String"
    }
  ],
  "type": "String",
  "resourceId": "String"
}
```




