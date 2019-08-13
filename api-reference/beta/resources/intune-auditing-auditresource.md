---
title: auditResource 资源类型
description: 包含审核资源的属性的类。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a390f43daca9d86320eea29eb139406ad52476fe
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36335219"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="14152-103">auditResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="14152-103">auditResource resource type</span></span>

> <span data-ttu-id="14152-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="14152-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="14152-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="14152-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14152-106">包含审核资源的属性的类。</span><span class="sxs-lookup"><span data-stu-id="14152-106">A class containing the properties for Audit Resource.</span></span>

## <a name="properties"></a><span data-ttu-id="14152-107">属性</span><span class="sxs-lookup"><span data-stu-id="14152-107">Properties</span></span>
|<span data-ttu-id="14152-108">属性</span><span class="sxs-lookup"><span data-stu-id="14152-108">Property</span></span>|<span data-ttu-id="14152-109">类型</span><span class="sxs-lookup"><span data-stu-id="14152-109">Type</span></span>|<span data-ttu-id="14152-110">说明</span><span class="sxs-lookup"><span data-stu-id="14152-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14152-111">displayName</span><span class="sxs-lookup"><span data-stu-id="14152-111">displayName</span></span>|<span data-ttu-id="14152-112">String</span><span class="sxs-lookup"><span data-stu-id="14152-112">String</span></span>|<span data-ttu-id="14152-113">显示名称。</span><span class="sxs-lookup"><span data-stu-id="14152-113">Display name.</span></span>|
|<span data-ttu-id="14152-114">ModifiedProperties</span><span class="sxs-lookup"><span data-stu-id="14152-114">modifiedProperties</span></span>|<span data-ttu-id="14152-115">[auditProperty](../resources/intune-auditing-auditproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="14152-115">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="14152-116">已修改属性列表。</span><span class="sxs-lookup"><span data-stu-id="14152-116">List of modified properties.</span></span>|
|<span data-ttu-id="14152-117">type</span><span class="sxs-lookup"><span data-stu-id="14152-117">type</span></span>|<span data-ttu-id="14152-118">字符串</span><span class="sxs-lookup"><span data-stu-id="14152-118">String</span></span>|<span data-ttu-id="14152-119">审核资源的类型。</span><span class="sxs-lookup"><span data-stu-id="14152-119">Audit resource's type.</span></span>|
|<span data-ttu-id="14152-120">resourceId</span><span class="sxs-lookup"><span data-stu-id="14152-120">resourceId</span></span>|<span data-ttu-id="14152-121">String</span><span class="sxs-lookup"><span data-stu-id="14152-121">String</span></span>|<span data-ttu-id="14152-122">审核资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="14152-122">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="14152-123">关系</span><span class="sxs-lookup"><span data-stu-id="14152-123">Relationships</span></span>
<span data-ttu-id="14152-124">无</span><span class="sxs-lookup"><span data-stu-id="14152-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="14152-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="14152-125">JSON Representation</span></span>
<span data-ttu-id="14152-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="14152-126">Here is a JSON representation of the resource.</span></span>
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



