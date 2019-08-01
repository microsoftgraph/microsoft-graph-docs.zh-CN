---
title: auditResource 资源类型
description: 包含审核资源的属性的类。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 14ecd6e4772e6d694707bd047899bd6b75720252
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028859"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="3264a-103">auditResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="3264a-103">auditResource resource type</span></span>

> <span data-ttu-id="3264a-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3264a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3264a-105">包含审核资源的属性的类。</span><span class="sxs-lookup"><span data-stu-id="3264a-105">A class containing the properties for Audit Resource.</span></span>

## <a name="properties"></a><span data-ttu-id="3264a-106">属性</span><span class="sxs-lookup"><span data-stu-id="3264a-106">Properties</span></span>
|<span data-ttu-id="3264a-107">属性</span><span class="sxs-lookup"><span data-stu-id="3264a-107">Property</span></span>|<span data-ttu-id="3264a-108">类型</span><span class="sxs-lookup"><span data-stu-id="3264a-108">Type</span></span>|<span data-ttu-id="3264a-109">说明</span><span class="sxs-lookup"><span data-stu-id="3264a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3264a-110">displayName</span><span class="sxs-lookup"><span data-stu-id="3264a-110">displayName</span></span>|<span data-ttu-id="3264a-111">String</span><span class="sxs-lookup"><span data-stu-id="3264a-111">String</span></span>|<span data-ttu-id="3264a-112">显示名称。</span><span class="sxs-lookup"><span data-stu-id="3264a-112">Display name.</span></span>|
|<span data-ttu-id="3264a-113">ModifiedProperties</span><span class="sxs-lookup"><span data-stu-id="3264a-113">modifiedProperties</span></span>|<span data-ttu-id="3264a-114">[auditProperty](../resources/intune-auditing-auditproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3264a-114">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="3264a-115">已修改属性列表。</span><span class="sxs-lookup"><span data-stu-id="3264a-115">List of modified properties.</span></span>|
|<span data-ttu-id="3264a-116">type</span><span class="sxs-lookup"><span data-stu-id="3264a-116">type</span></span>|<span data-ttu-id="3264a-117">字符串</span><span class="sxs-lookup"><span data-stu-id="3264a-117">String</span></span>|<span data-ttu-id="3264a-118">审核资源的类型。</span><span class="sxs-lookup"><span data-stu-id="3264a-118">Audit resource's type.</span></span>|
|<span data-ttu-id="3264a-119">resourceId</span><span class="sxs-lookup"><span data-stu-id="3264a-119">resourceId</span></span>|<span data-ttu-id="3264a-120">String</span><span class="sxs-lookup"><span data-stu-id="3264a-120">String</span></span>|<span data-ttu-id="3264a-121">审核资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="3264a-121">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3264a-122">关系</span><span class="sxs-lookup"><span data-stu-id="3264a-122">Relationships</span></span>
<span data-ttu-id="3264a-123">无</span><span class="sxs-lookup"><span data-stu-id="3264a-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3264a-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3264a-124">JSON Representation</span></span>
<span data-ttu-id="3264a-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3264a-125">Here is a JSON representation of the resource.</span></span>
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



