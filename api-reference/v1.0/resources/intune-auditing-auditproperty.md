---
title: auditProperty 资源类型
description: 包含审核属性的属性的类。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c63f390e31e83cfed64ee2a28bba4e4af0dfa756
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532728"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="d3da3-103">auditProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="d3da3-103">auditProperty resource type</span></span>

<span data-ttu-id="d3da3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3da3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d3da3-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d3da3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3da3-106">包含审核属性的属性的类。</span><span class="sxs-lookup"><span data-stu-id="d3da3-106">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="d3da3-107">属性</span><span class="sxs-lookup"><span data-stu-id="d3da3-107">Properties</span></span>
|<span data-ttu-id="d3da3-108">属性</span><span class="sxs-lookup"><span data-stu-id="d3da3-108">Property</span></span>|<span data-ttu-id="d3da3-109">类型</span><span class="sxs-lookup"><span data-stu-id="d3da3-109">Type</span></span>|<span data-ttu-id="d3da3-110">说明</span><span class="sxs-lookup"><span data-stu-id="d3da3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3da3-111">displayName</span><span class="sxs-lookup"><span data-stu-id="d3da3-111">displayName</span></span>|<span data-ttu-id="d3da3-112">String</span><span class="sxs-lookup"><span data-stu-id="d3da3-112">String</span></span>|<span data-ttu-id="d3da3-113">显示名称。</span><span class="sxs-lookup"><span data-stu-id="d3da3-113">Display name.</span></span>|
|<span data-ttu-id="d3da3-114">oldValue</span><span class="sxs-lookup"><span data-stu-id="d3da3-114">oldValue</span></span>|<span data-ttu-id="d3da3-115">字符串</span><span class="sxs-lookup"><span data-stu-id="d3da3-115">String</span></span>|<span data-ttu-id="d3da3-116">旧值。</span><span class="sxs-lookup"><span data-stu-id="d3da3-116">Old value.</span></span>|
|<span data-ttu-id="d3da3-117">NewValue</span><span class="sxs-lookup"><span data-stu-id="d3da3-117">newValue</span></span>|<span data-ttu-id="d3da3-118">String</span><span class="sxs-lookup"><span data-stu-id="d3da3-118">String</span></span>|<span data-ttu-id="d3da3-119">新值。</span><span class="sxs-lookup"><span data-stu-id="d3da3-119">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d3da3-120">关系</span><span class="sxs-lookup"><span data-stu-id="d3da3-120">Relationships</span></span>
<span data-ttu-id="d3da3-121">无</span><span class="sxs-lookup"><span data-stu-id="d3da3-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d3da3-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d3da3-122">JSON Representation</span></span>
<span data-ttu-id="d3da3-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d3da3-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditProperty"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditProperty",
  "displayName": "String",
  "oldValue": "String",
  "newValue": "String"
}
```




