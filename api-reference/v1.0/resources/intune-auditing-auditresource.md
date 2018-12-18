---
title: auditResource 资源类型
description: 包含审核资源的属性的类。
author: tfitzmac
ms.openlocfilehash: 5cfc23a80b2247b9f561d802ce844091c623ef62
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302658"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="97bc6-103">auditResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="97bc6-103">auditResource resource type</span></span>

> <span data-ttu-id="97bc6-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="97bc6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="97bc6-105">包含审核资源的属性的类。</span><span class="sxs-lookup"><span data-stu-id="97bc6-105">A class containing the properties for Audit Resource.</span></span>
## <a name="properties"></a><span data-ttu-id="97bc6-106">属性</span><span class="sxs-lookup"><span data-stu-id="97bc6-106">Properties</span></span>
|<span data-ttu-id="97bc6-107">属性</span><span class="sxs-lookup"><span data-stu-id="97bc6-107">Property</span></span>|<span data-ttu-id="97bc6-108">类型</span><span class="sxs-lookup"><span data-stu-id="97bc6-108">Type</span></span>|<span data-ttu-id="97bc6-109">说明</span><span class="sxs-lookup"><span data-stu-id="97bc6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97bc6-110">displayName</span><span class="sxs-lookup"><span data-stu-id="97bc6-110">displayName</span></span>|<span data-ttu-id="97bc6-111">String</span><span class="sxs-lookup"><span data-stu-id="97bc6-111">String</span></span>|<span data-ttu-id="97bc6-112">显示名称。</span><span class="sxs-lookup"><span data-stu-id="97bc6-112">Display name.</span></span>|
|<span data-ttu-id="97bc6-113">ModifiedProperties</span><span class="sxs-lookup"><span data-stu-id="97bc6-113">modifiedProperties</span></span>|<span data-ttu-id="97bc6-114">[auditProperty](../resources/intune-auditing-auditproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="97bc6-114">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="97bc6-115">已修改属性列表。</span><span class="sxs-lookup"><span data-stu-id="97bc6-115">List of modified properties.</span></span>|
|<span data-ttu-id="97bc6-116">type</span><span class="sxs-lookup"><span data-stu-id="97bc6-116">type</span></span>|<span data-ttu-id="97bc6-117">String</span><span class="sxs-lookup"><span data-stu-id="97bc6-117">String</span></span>|<span data-ttu-id="97bc6-118">审核资源的类型。</span><span class="sxs-lookup"><span data-stu-id="97bc6-118">Audit resource's type.</span></span>|
|<span data-ttu-id="97bc6-119">resourceId</span><span class="sxs-lookup"><span data-stu-id="97bc6-119">resourceId</span></span>|<span data-ttu-id="97bc6-120">String</span><span class="sxs-lookup"><span data-stu-id="97bc6-120">String</span></span>|<span data-ttu-id="97bc6-121">审核资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="97bc6-121">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="97bc6-122">关系</span><span class="sxs-lookup"><span data-stu-id="97bc6-122">Relationships</span></span>
<span data-ttu-id="97bc6-123">无</span><span class="sxs-lookup"><span data-stu-id="97bc6-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="97bc6-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="97bc6-124">JSON Representation</span></span>
<span data-ttu-id="97bc6-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="97bc6-125">Here is a JSON representation of the resource.</span></span>
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



