---
title: auditResource 资源类型
description: 包含审核资源的属性的类。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4778e01076e2af1c18edb16a2587f65396cc6466
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977247"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="b6d44-103">auditResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="b6d44-103">auditResource resource type</span></span>

> <span data-ttu-id="b6d44-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b6d44-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b6d44-105">包含审核资源的属性的类。</span><span class="sxs-lookup"><span data-stu-id="b6d44-105">A class containing the properties for Audit Resource.</span></span>
## <a name="properties"></a><span data-ttu-id="b6d44-106">属性</span><span class="sxs-lookup"><span data-stu-id="b6d44-106">Properties</span></span>
|<span data-ttu-id="b6d44-107">属性</span><span class="sxs-lookup"><span data-stu-id="b6d44-107">Property</span></span>|<span data-ttu-id="b6d44-108">类型</span><span class="sxs-lookup"><span data-stu-id="b6d44-108">Type</span></span>|<span data-ttu-id="b6d44-109">说明</span><span class="sxs-lookup"><span data-stu-id="b6d44-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6d44-110">displayName</span><span class="sxs-lookup"><span data-stu-id="b6d44-110">displayName</span></span>|<span data-ttu-id="b6d44-111">String</span><span class="sxs-lookup"><span data-stu-id="b6d44-111">String</span></span>|<span data-ttu-id="b6d44-112">显示名称。</span><span class="sxs-lookup"><span data-stu-id="b6d44-112">Display name.</span></span>|
|<span data-ttu-id="b6d44-113">ModifiedProperties</span><span class="sxs-lookup"><span data-stu-id="b6d44-113">modifiedProperties</span></span>|<span data-ttu-id="b6d44-114">[auditProperty](../resources/intune-auditing-auditproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b6d44-114">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="b6d44-115">已修改属性列表。</span><span class="sxs-lookup"><span data-stu-id="b6d44-115">List of modified properties.</span></span>|
|<span data-ttu-id="b6d44-116">type</span><span class="sxs-lookup"><span data-stu-id="b6d44-116">type</span></span>|<span data-ttu-id="b6d44-117">String</span><span class="sxs-lookup"><span data-stu-id="b6d44-117">String</span></span>|<span data-ttu-id="b6d44-118">审核资源的类型。</span><span class="sxs-lookup"><span data-stu-id="b6d44-118">Audit resource's type.</span></span>|
|<span data-ttu-id="b6d44-119">resourceId</span><span class="sxs-lookup"><span data-stu-id="b6d44-119">resourceId</span></span>|<span data-ttu-id="b6d44-120">String</span><span class="sxs-lookup"><span data-stu-id="b6d44-120">String</span></span>|<span data-ttu-id="b6d44-121">审核资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="b6d44-121">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b6d44-122">关系</span><span class="sxs-lookup"><span data-stu-id="b6d44-122">Relationships</span></span>
<span data-ttu-id="b6d44-123">无</span><span class="sxs-lookup"><span data-stu-id="b6d44-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b6d44-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b6d44-124">JSON Representation</span></span>
<span data-ttu-id="b6d44-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b6d44-125">Here is a JSON representation of the resource.</span></span>
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



