---
title: auditProperty 资源类型
description: 包含审核属性的属性的类。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4c252e7912f3f34e300e1f412db63133ea3acbd8
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949358"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="9d191-103">auditProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="9d191-103">auditProperty resource type</span></span>

> <span data-ttu-id="9d191-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9d191-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9d191-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9d191-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d191-106">包含审核属性的属性的类。</span><span class="sxs-lookup"><span data-stu-id="9d191-106">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="9d191-107">属性</span><span class="sxs-lookup"><span data-stu-id="9d191-107">Properties</span></span>
|<span data-ttu-id="9d191-108">属性</span><span class="sxs-lookup"><span data-stu-id="9d191-108">Property</span></span>|<span data-ttu-id="9d191-109">类型</span><span class="sxs-lookup"><span data-stu-id="9d191-109">Type</span></span>|<span data-ttu-id="9d191-110">说明</span><span class="sxs-lookup"><span data-stu-id="9d191-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d191-111">displayName</span><span class="sxs-lookup"><span data-stu-id="9d191-111">displayName</span></span>|<span data-ttu-id="9d191-112">String</span><span class="sxs-lookup"><span data-stu-id="9d191-112">String</span></span>|<span data-ttu-id="9d191-113">显示名称。</span><span class="sxs-lookup"><span data-stu-id="9d191-113">Display name.</span></span>|
|<span data-ttu-id="9d191-114">oldValue</span><span class="sxs-lookup"><span data-stu-id="9d191-114">oldValue</span></span>|<span data-ttu-id="9d191-115">String</span><span class="sxs-lookup"><span data-stu-id="9d191-115">String</span></span>|<span data-ttu-id="9d191-116">旧值。</span><span class="sxs-lookup"><span data-stu-id="9d191-116">Old value.</span></span>|
|<span data-ttu-id="9d191-117">NewValue</span><span class="sxs-lookup"><span data-stu-id="9d191-117">newValue</span></span>|<span data-ttu-id="9d191-118">String</span><span class="sxs-lookup"><span data-stu-id="9d191-118">String</span></span>|<span data-ttu-id="9d191-119">新值。</span><span class="sxs-lookup"><span data-stu-id="9d191-119">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9d191-120">关系</span><span class="sxs-lookup"><span data-stu-id="9d191-120">Relationships</span></span>
<span data-ttu-id="9d191-121">无</span><span class="sxs-lookup"><span data-stu-id="9d191-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9d191-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9d191-122">JSON Representation</span></span>
<span data-ttu-id="9d191-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9d191-123">Here is a JSON representation of the resource.</span></span>
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




