---
title: auditProperty 资源类型
description: 包含审核属性的属性的类。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7028a91f92e87009bdf2899abaafc6bcb5aa0fc0
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34991714"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="99f07-103">auditProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="99f07-103">auditProperty resource type</span></span>

> <span data-ttu-id="99f07-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="99f07-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="99f07-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="99f07-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99f07-106">包含审核属性的属性的类。</span><span class="sxs-lookup"><span data-stu-id="99f07-106">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="99f07-107">属性</span><span class="sxs-lookup"><span data-stu-id="99f07-107">Properties</span></span>
|<span data-ttu-id="99f07-108">属性</span><span class="sxs-lookup"><span data-stu-id="99f07-108">Property</span></span>|<span data-ttu-id="99f07-109">类型</span><span class="sxs-lookup"><span data-stu-id="99f07-109">Type</span></span>|<span data-ttu-id="99f07-110">说明</span><span class="sxs-lookup"><span data-stu-id="99f07-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99f07-111">displayName</span><span class="sxs-lookup"><span data-stu-id="99f07-111">displayName</span></span>|<span data-ttu-id="99f07-112">String</span><span class="sxs-lookup"><span data-stu-id="99f07-112">String</span></span>|<span data-ttu-id="99f07-113">显示名称。</span><span class="sxs-lookup"><span data-stu-id="99f07-113">Display name.</span></span>|
|<span data-ttu-id="99f07-114">oldValue</span><span class="sxs-lookup"><span data-stu-id="99f07-114">oldValue</span></span>|<span data-ttu-id="99f07-115">String</span><span class="sxs-lookup"><span data-stu-id="99f07-115">String</span></span>|<span data-ttu-id="99f07-116">旧值。</span><span class="sxs-lookup"><span data-stu-id="99f07-116">Old value.</span></span>|
|<span data-ttu-id="99f07-117">NewValue</span><span class="sxs-lookup"><span data-stu-id="99f07-117">newValue</span></span>|<span data-ttu-id="99f07-118">String</span><span class="sxs-lookup"><span data-stu-id="99f07-118">String</span></span>|<span data-ttu-id="99f07-119">新值。</span><span class="sxs-lookup"><span data-stu-id="99f07-119">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="99f07-120">关系</span><span class="sxs-lookup"><span data-stu-id="99f07-120">Relationships</span></span>
<span data-ttu-id="99f07-121">无</span><span class="sxs-lookup"><span data-stu-id="99f07-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="99f07-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="99f07-122">JSON Representation</span></span>
<span data-ttu-id="99f07-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="99f07-123">Here is a JSON representation of the resource.</span></span>
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





