---
title: auditProperty 资源类型
description: 包含审核属性的属性的类。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 18e819234fd4ee7065378046f8ec977276a8c9f2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32565798"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="9eba3-103">auditProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="9eba3-103">auditProperty resource type</span></span>

> <span data-ttu-id="9eba3-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9eba3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9eba3-105">包含审核属性的属性的类。</span><span class="sxs-lookup"><span data-stu-id="9eba3-105">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="9eba3-106">属性</span><span class="sxs-lookup"><span data-stu-id="9eba3-106">Properties</span></span>
|<span data-ttu-id="9eba3-107">属性</span><span class="sxs-lookup"><span data-stu-id="9eba3-107">Property</span></span>|<span data-ttu-id="9eba3-108">类型</span><span class="sxs-lookup"><span data-stu-id="9eba3-108">Type</span></span>|<span data-ttu-id="9eba3-109">说明</span><span class="sxs-lookup"><span data-stu-id="9eba3-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9eba3-110">displayName</span><span class="sxs-lookup"><span data-stu-id="9eba3-110">displayName</span></span>|<span data-ttu-id="9eba3-111">String</span><span class="sxs-lookup"><span data-stu-id="9eba3-111">String</span></span>|<span data-ttu-id="9eba3-112">显示名称。</span><span class="sxs-lookup"><span data-stu-id="9eba3-112">Display name.</span></span>|
|<span data-ttu-id="9eba3-113">oldValue</span><span class="sxs-lookup"><span data-stu-id="9eba3-113">oldValue</span></span>|<span data-ttu-id="9eba3-114">String</span><span class="sxs-lookup"><span data-stu-id="9eba3-114">String</span></span>|<span data-ttu-id="9eba3-115">旧值。</span><span class="sxs-lookup"><span data-stu-id="9eba3-115">Old value.</span></span>|
|<span data-ttu-id="9eba3-116">NewValue</span><span class="sxs-lookup"><span data-stu-id="9eba3-116">newValue</span></span>|<span data-ttu-id="9eba3-117">String</span><span class="sxs-lookup"><span data-stu-id="9eba3-117">String</span></span>|<span data-ttu-id="9eba3-118">新值。</span><span class="sxs-lookup"><span data-stu-id="9eba3-118">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9eba3-119">关系</span><span class="sxs-lookup"><span data-stu-id="9eba3-119">Relationships</span></span>
<span data-ttu-id="9eba3-120">无</span><span class="sxs-lookup"><span data-stu-id="9eba3-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9eba3-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9eba3-121">JSON Representation</span></span>
<span data-ttu-id="9eba3-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9eba3-122">Here is a JSON representation of the resource.</span></span>
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



