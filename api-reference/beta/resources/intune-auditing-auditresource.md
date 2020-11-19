---
title: auditResource 资源类型
description: 包含审核资源的属性的类。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2fc12a0cd27a2645e441b2c820a84769a12bd080
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49295528"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="7e3e3-103">auditResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="7e3e3-103">auditResource resource type</span></span>

<span data-ttu-id="7e3e3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e3e3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7e3e3-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7e3e3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7e3e3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7e3e3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e3e3-107">包含审核资源的属性的类。</span><span class="sxs-lookup"><span data-stu-id="7e3e3-107">A class containing the properties for Audit Resource.</span></span>

## <a name="properties"></a><span data-ttu-id="7e3e3-108">属性</span><span class="sxs-lookup"><span data-stu-id="7e3e3-108">Properties</span></span>
|<span data-ttu-id="7e3e3-109">属性</span><span class="sxs-lookup"><span data-stu-id="7e3e3-109">Property</span></span>|<span data-ttu-id="7e3e3-110">类型</span><span class="sxs-lookup"><span data-stu-id="7e3e3-110">Type</span></span>|<span data-ttu-id="7e3e3-111">说明</span><span class="sxs-lookup"><span data-stu-id="7e3e3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e3e3-112">displayName</span><span class="sxs-lookup"><span data-stu-id="7e3e3-112">displayName</span></span>|<span data-ttu-id="7e3e3-113">字符串</span><span class="sxs-lookup"><span data-stu-id="7e3e3-113">String</span></span>|<span data-ttu-id="7e3e3-114">显示名称。</span><span class="sxs-lookup"><span data-stu-id="7e3e3-114">Display name.</span></span>|
|<span data-ttu-id="7e3e3-115">ModifiedProperties</span><span class="sxs-lookup"><span data-stu-id="7e3e3-115">modifiedProperties</span></span>|<span data-ttu-id="7e3e3-116">[auditProperty](../resources/intune-auditing-auditproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7e3e3-116">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="7e3e3-117">已修改属性列表。</span><span class="sxs-lookup"><span data-stu-id="7e3e3-117">List of modified properties.</span></span>|
|<span data-ttu-id="7e3e3-118">type</span><span class="sxs-lookup"><span data-stu-id="7e3e3-118">type</span></span>|<span data-ttu-id="7e3e3-119">字符串</span><span class="sxs-lookup"><span data-stu-id="7e3e3-119">String</span></span>|<span data-ttu-id="7e3e3-120">审核资源的类型。</span><span class="sxs-lookup"><span data-stu-id="7e3e3-120">Audit resource's type.</span></span>|
|<span data-ttu-id="7e3e3-121">resourceId</span><span class="sxs-lookup"><span data-stu-id="7e3e3-121">resourceId</span></span>|<span data-ttu-id="7e3e3-122">String</span><span class="sxs-lookup"><span data-stu-id="7e3e3-122">String</span></span>|<span data-ttu-id="7e3e3-123">审核资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="7e3e3-123">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7e3e3-124">关系</span><span class="sxs-lookup"><span data-stu-id="7e3e3-124">Relationships</span></span>
<span data-ttu-id="7e3e3-125">无</span><span class="sxs-lookup"><span data-stu-id="7e3e3-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7e3e3-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7e3e3-126">JSON Representation</span></span>
<span data-ttu-id="7e3e3-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7e3e3-127">Here is a JSON representation of the resource.</span></span>
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




