---
title: auditProperty 资源类型
description: 包含审核属性的属性的类。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 331c786d7fd21687a0581ae56746d9e0b48f7c04
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36335226"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="b96a8-103">auditProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="b96a8-103">auditProperty resource type</span></span>

> <span data-ttu-id="b96a8-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b96a8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b96a8-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b96a8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b96a8-106">包含审核属性的属性的类。</span><span class="sxs-lookup"><span data-stu-id="b96a8-106">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="b96a8-107">属性</span><span class="sxs-lookup"><span data-stu-id="b96a8-107">Properties</span></span>
|<span data-ttu-id="b96a8-108">属性</span><span class="sxs-lookup"><span data-stu-id="b96a8-108">Property</span></span>|<span data-ttu-id="b96a8-109">类型</span><span class="sxs-lookup"><span data-stu-id="b96a8-109">Type</span></span>|<span data-ttu-id="b96a8-110">说明</span><span class="sxs-lookup"><span data-stu-id="b96a8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b96a8-111">displayName</span><span class="sxs-lookup"><span data-stu-id="b96a8-111">displayName</span></span>|<span data-ttu-id="b96a8-112">String</span><span class="sxs-lookup"><span data-stu-id="b96a8-112">String</span></span>|<span data-ttu-id="b96a8-113">显示名称。</span><span class="sxs-lookup"><span data-stu-id="b96a8-113">Display name.</span></span>|
|<span data-ttu-id="b96a8-114">oldValue</span><span class="sxs-lookup"><span data-stu-id="b96a8-114">oldValue</span></span>|<span data-ttu-id="b96a8-115">String</span><span class="sxs-lookup"><span data-stu-id="b96a8-115">String</span></span>|<span data-ttu-id="b96a8-116">旧值。</span><span class="sxs-lookup"><span data-stu-id="b96a8-116">Old value.</span></span>|
|<span data-ttu-id="b96a8-117">NewValue</span><span class="sxs-lookup"><span data-stu-id="b96a8-117">newValue</span></span>|<span data-ttu-id="b96a8-118">String</span><span class="sxs-lookup"><span data-stu-id="b96a8-118">String</span></span>|<span data-ttu-id="b96a8-119">新值。</span><span class="sxs-lookup"><span data-stu-id="b96a8-119">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b96a8-120">关系</span><span class="sxs-lookup"><span data-stu-id="b96a8-120">Relationships</span></span>
<span data-ttu-id="b96a8-121">无</span><span class="sxs-lookup"><span data-stu-id="b96a8-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b96a8-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b96a8-122">JSON Representation</span></span>
<span data-ttu-id="b96a8-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b96a8-123">Here is a JSON representation of the resource.</span></span>
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



