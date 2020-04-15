---
title: auditResource 资源类型
description: 包含审核资源的属性的类。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 35d4385ca16569e1b7e0177995c32ae22e5a0aa0
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439485"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="ff34e-103">auditResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="ff34e-103">auditResource resource type</span></span>

<span data-ttu-id="ff34e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff34e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ff34e-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ff34e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff34e-106">包含审核资源的属性的类。</span><span class="sxs-lookup"><span data-stu-id="ff34e-106">A class containing the properties for Audit Resource.</span></span>

## <a name="properties"></a><span data-ttu-id="ff34e-107">属性</span><span class="sxs-lookup"><span data-stu-id="ff34e-107">Properties</span></span>
|<span data-ttu-id="ff34e-108">属性</span><span class="sxs-lookup"><span data-stu-id="ff34e-108">Property</span></span>|<span data-ttu-id="ff34e-109">类型</span><span class="sxs-lookup"><span data-stu-id="ff34e-109">Type</span></span>|<span data-ttu-id="ff34e-110">说明</span><span class="sxs-lookup"><span data-stu-id="ff34e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff34e-111">displayName</span><span class="sxs-lookup"><span data-stu-id="ff34e-111">displayName</span></span>|<span data-ttu-id="ff34e-112">String</span><span class="sxs-lookup"><span data-stu-id="ff34e-112">String</span></span>|<span data-ttu-id="ff34e-113">显示名称。</span><span class="sxs-lookup"><span data-stu-id="ff34e-113">Display name.</span></span>|
|<span data-ttu-id="ff34e-114">ModifiedProperties</span><span class="sxs-lookup"><span data-stu-id="ff34e-114">modifiedProperties</span></span>|<span data-ttu-id="ff34e-115">[auditProperty](../resources/intune-auditing-auditproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ff34e-115">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="ff34e-116">已修改属性列表。</span><span class="sxs-lookup"><span data-stu-id="ff34e-116">List of modified properties.</span></span>|
|<span data-ttu-id="ff34e-117">type</span><span class="sxs-lookup"><span data-stu-id="ff34e-117">type</span></span>|<span data-ttu-id="ff34e-118">字符串</span><span class="sxs-lookup"><span data-stu-id="ff34e-118">String</span></span>|<span data-ttu-id="ff34e-119">审核资源的类型。</span><span class="sxs-lookup"><span data-stu-id="ff34e-119">Audit resource's type.</span></span>|
|<span data-ttu-id="ff34e-120">resourceId</span><span class="sxs-lookup"><span data-stu-id="ff34e-120">resourceId</span></span>|<span data-ttu-id="ff34e-121">String</span><span class="sxs-lookup"><span data-stu-id="ff34e-121">String</span></span>|<span data-ttu-id="ff34e-122">审核资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="ff34e-122">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff34e-123">关系</span><span class="sxs-lookup"><span data-stu-id="ff34e-123">Relationships</span></span>
<span data-ttu-id="ff34e-124">无</span><span class="sxs-lookup"><span data-stu-id="ff34e-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ff34e-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ff34e-125">JSON Representation</span></span>
<span data-ttu-id="ff34e-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ff34e-126">Here is a JSON representation of the resource.</span></span>
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







