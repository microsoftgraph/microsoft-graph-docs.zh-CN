---
title: auditProperty 资源类型
description: 包含审核属性的属性的类。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f306fbbf1d93386e4ffd963199c4e6d54296ce26
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439516"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="eee22-103">auditProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="eee22-103">auditProperty resource type</span></span>

<span data-ttu-id="eee22-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eee22-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eee22-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="eee22-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eee22-106">包含审核属性的属性的类。</span><span class="sxs-lookup"><span data-stu-id="eee22-106">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="eee22-107">属性</span><span class="sxs-lookup"><span data-stu-id="eee22-107">Properties</span></span>
|<span data-ttu-id="eee22-108">属性</span><span class="sxs-lookup"><span data-stu-id="eee22-108">Property</span></span>|<span data-ttu-id="eee22-109">类型</span><span class="sxs-lookup"><span data-stu-id="eee22-109">Type</span></span>|<span data-ttu-id="eee22-110">说明</span><span class="sxs-lookup"><span data-stu-id="eee22-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eee22-111">displayName</span><span class="sxs-lookup"><span data-stu-id="eee22-111">displayName</span></span>|<span data-ttu-id="eee22-112">String</span><span class="sxs-lookup"><span data-stu-id="eee22-112">String</span></span>|<span data-ttu-id="eee22-113">显示名称。</span><span class="sxs-lookup"><span data-stu-id="eee22-113">Display name.</span></span>|
|<span data-ttu-id="eee22-114">oldValue</span><span class="sxs-lookup"><span data-stu-id="eee22-114">oldValue</span></span>|<span data-ttu-id="eee22-115">String</span><span class="sxs-lookup"><span data-stu-id="eee22-115">String</span></span>|<span data-ttu-id="eee22-116">旧值。</span><span class="sxs-lookup"><span data-stu-id="eee22-116">Old value.</span></span>|
|<span data-ttu-id="eee22-117">NewValue</span><span class="sxs-lookup"><span data-stu-id="eee22-117">newValue</span></span>|<span data-ttu-id="eee22-118">String</span><span class="sxs-lookup"><span data-stu-id="eee22-118">String</span></span>|<span data-ttu-id="eee22-119">新值。</span><span class="sxs-lookup"><span data-stu-id="eee22-119">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eee22-120">关系</span><span class="sxs-lookup"><span data-stu-id="eee22-120">Relationships</span></span>
<span data-ttu-id="eee22-121">无</span><span class="sxs-lookup"><span data-stu-id="eee22-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eee22-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="eee22-122">JSON Representation</span></span>
<span data-ttu-id="eee22-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eee22-123">Here is a JSON representation of the resource.</span></span>
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







