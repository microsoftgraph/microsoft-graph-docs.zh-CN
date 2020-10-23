---
title: auditProperty 资源类型
description: 包含审核属性的属性的类。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e179c1c7318934c538cef06c3284308c54199059
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48706063"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="cf7ff-103">auditProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="cf7ff-103">auditProperty resource type</span></span>

<span data-ttu-id="cf7ff-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf7ff-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cf7ff-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cf7ff-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cf7ff-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cf7ff-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf7ff-107">包含审核属性的属性的类。</span><span class="sxs-lookup"><span data-stu-id="cf7ff-107">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="cf7ff-108">属性</span><span class="sxs-lookup"><span data-stu-id="cf7ff-108">Properties</span></span>
|<span data-ttu-id="cf7ff-109">属性</span><span class="sxs-lookup"><span data-stu-id="cf7ff-109">Property</span></span>|<span data-ttu-id="cf7ff-110">类型</span><span class="sxs-lookup"><span data-stu-id="cf7ff-110">Type</span></span>|<span data-ttu-id="cf7ff-111">说明</span><span class="sxs-lookup"><span data-stu-id="cf7ff-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf7ff-112">displayName</span><span class="sxs-lookup"><span data-stu-id="cf7ff-112">displayName</span></span>|<span data-ttu-id="cf7ff-113">String</span><span class="sxs-lookup"><span data-stu-id="cf7ff-113">String</span></span>|<span data-ttu-id="cf7ff-114">显示名称。</span><span class="sxs-lookup"><span data-stu-id="cf7ff-114">Display name.</span></span>|
|<span data-ttu-id="cf7ff-115">oldValue</span><span class="sxs-lookup"><span data-stu-id="cf7ff-115">oldValue</span></span>|<span data-ttu-id="cf7ff-116">String</span><span class="sxs-lookup"><span data-stu-id="cf7ff-116">String</span></span>|<span data-ttu-id="cf7ff-117">旧值。</span><span class="sxs-lookup"><span data-stu-id="cf7ff-117">Old value.</span></span>|
|<span data-ttu-id="cf7ff-118">NewValue</span><span class="sxs-lookup"><span data-stu-id="cf7ff-118">newValue</span></span>|<span data-ttu-id="cf7ff-119">String</span><span class="sxs-lookup"><span data-stu-id="cf7ff-119">String</span></span>|<span data-ttu-id="cf7ff-120">新值。</span><span class="sxs-lookup"><span data-stu-id="cf7ff-120">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cf7ff-121">关系</span><span class="sxs-lookup"><span data-stu-id="cf7ff-121">Relationships</span></span>
<span data-ttu-id="cf7ff-122">无</span><span class="sxs-lookup"><span data-stu-id="cf7ff-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cf7ff-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cf7ff-123">JSON Representation</span></span>
<span data-ttu-id="cf7ff-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cf7ff-124">Here is a JSON representation of the resource.</span></span>
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





