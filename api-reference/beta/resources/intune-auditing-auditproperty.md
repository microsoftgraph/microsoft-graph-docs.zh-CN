---
title: auditProperty 资源类型
description: 包含审核属性的属性的类。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 666879bd6a4554be85c52c54c1d9ef3f1a406886
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49295556"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="32e15-103">auditProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="32e15-103">auditProperty resource type</span></span>

<span data-ttu-id="32e15-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32e15-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="32e15-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="32e15-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="32e15-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="32e15-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32e15-107">包含审核属性的属性的类。</span><span class="sxs-lookup"><span data-stu-id="32e15-107">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="32e15-108">属性</span><span class="sxs-lookup"><span data-stu-id="32e15-108">Properties</span></span>
|<span data-ttu-id="32e15-109">属性</span><span class="sxs-lookup"><span data-stu-id="32e15-109">Property</span></span>|<span data-ttu-id="32e15-110">类型</span><span class="sxs-lookup"><span data-stu-id="32e15-110">Type</span></span>|<span data-ttu-id="32e15-111">说明</span><span class="sxs-lookup"><span data-stu-id="32e15-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32e15-112">displayName</span><span class="sxs-lookup"><span data-stu-id="32e15-112">displayName</span></span>|<span data-ttu-id="32e15-113">字符串</span><span class="sxs-lookup"><span data-stu-id="32e15-113">String</span></span>|<span data-ttu-id="32e15-114">显示名称。</span><span class="sxs-lookup"><span data-stu-id="32e15-114">Display name.</span></span>|
|<span data-ttu-id="32e15-115">oldValue</span><span class="sxs-lookup"><span data-stu-id="32e15-115">oldValue</span></span>|<span data-ttu-id="32e15-116">String</span><span class="sxs-lookup"><span data-stu-id="32e15-116">String</span></span>|<span data-ttu-id="32e15-117">旧值。</span><span class="sxs-lookup"><span data-stu-id="32e15-117">Old value.</span></span>|
|<span data-ttu-id="32e15-118">NewValue</span><span class="sxs-lookup"><span data-stu-id="32e15-118">newValue</span></span>|<span data-ttu-id="32e15-119">String</span><span class="sxs-lookup"><span data-stu-id="32e15-119">String</span></span>|<span data-ttu-id="32e15-120">新值。</span><span class="sxs-lookup"><span data-stu-id="32e15-120">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="32e15-121">关系</span><span class="sxs-lookup"><span data-stu-id="32e15-121">Relationships</span></span>
<span data-ttu-id="32e15-122">无</span><span class="sxs-lookup"><span data-stu-id="32e15-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="32e15-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="32e15-123">JSON Representation</span></span>
<span data-ttu-id="32e15-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="32e15-124">Here is a JSON representation of the resource.</span></span>
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




