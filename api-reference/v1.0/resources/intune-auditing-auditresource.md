---
title: auditResource 资源类型
description: 包含审核资源的属性的类。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7f8fc3a96b3d17759e1e65eaa17c6571e4cec347
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844735"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="bbb05-103">auditResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="bbb05-103">auditResource resource type</span></span>

> <span data-ttu-id="bbb05-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="bbb05-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bbb05-105">包含审核资源的属性的类。</span><span class="sxs-lookup"><span data-stu-id="bbb05-105">A class containing the properties for Audit Resource.</span></span>
## <a name="properties"></a><span data-ttu-id="bbb05-106">属性</span><span class="sxs-lookup"><span data-stu-id="bbb05-106">Properties</span></span>
|<span data-ttu-id="bbb05-107">属性</span><span class="sxs-lookup"><span data-stu-id="bbb05-107">Property</span></span>|<span data-ttu-id="bbb05-108">类型</span><span class="sxs-lookup"><span data-stu-id="bbb05-108">Type</span></span>|<span data-ttu-id="bbb05-109">说明</span><span class="sxs-lookup"><span data-stu-id="bbb05-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bbb05-110">displayName</span><span class="sxs-lookup"><span data-stu-id="bbb05-110">displayName</span></span>|<span data-ttu-id="bbb05-111">String</span><span class="sxs-lookup"><span data-stu-id="bbb05-111">String</span></span>|<span data-ttu-id="bbb05-112">显示名称。</span><span class="sxs-lookup"><span data-stu-id="bbb05-112">Display name.</span></span>|
|<span data-ttu-id="bbb05-113">ModifiedProperties</span><span class="sxs-lookup"><span data-stu-id="bbb05-113">modifiedProperties</span></span>|<span data-ttu-id="bbb05-114">[auditProperty](../resources/intune-auditing-auditproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bbb05-114">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="bbb05-115">已修改属性列表。</span><span class="sxs-lookup"><span data-stu-id="bbb05-115">List of modified properties.</span></span>|
|<span data-ttu-id="bbb05-116">type</span><span class="sxs-lookup"><span data-stu-id="bbb05-116">type</span></span>|<span data-ttu-id="bbb05-117">String</span><span class="sxs-lookup"><span data-stu-id="bbb05-117">String</span></span>|<span data-ttu-id="bbb05-118">审核资源的类型。</span><span class="sxs-lookup"><span data-stu-id="bbb05-118">Audit resource's type.</span></span>|
|<span data-ttu-id="bbb05-119">resourceId</span><span class="sxs-lookup"><span data-stu-id="bbb05-119">resourceId</span></span>|<span data-ttu-id="bbb05-120">String</span><span class="sxs-lookup"><span data-stu-id="bbb05-120">String</span></span>|<span data-ttu-id="bbb05-121">审核资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="bbb05-121">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bbb05-122">关系</span><span class="sxs-lookup"><span data-stu-id="bbb05-122">Relationships</span></span>
<span data-ttu-id="bbb05-123">无</span><span class="sxs-lookup"><span data-stu-id="bbb05-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bbb05-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bbb05-124">JSON Representation</span></span>
<span data-ttu-id="bbb05-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bbb05-125">Here is a JSON representation of the resource.</span></span>
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



