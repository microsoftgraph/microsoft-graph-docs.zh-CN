---
title: auditResource 资源类型
description: 包含审核资源的属性的类。
ms.openlocfilehash: a3825418c1406bbe9fcce7feeba96217342c735e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047072"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="102aa-103">auditResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="102aa-103">auditResource resource type</span></span>

> <span data-ttu-id="102aa-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="102aa-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="102aa-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="102aa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="102aa-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="102aa-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="102aa-107">包含审核资源的属性的类。</span><span class="sxs-lookup"><span data-stu-id="102aa-107">A class containing the properties for Audit Resource.</span></span>
## <a name="properties"></a><span data-ttu-id="102aa-108">属性</span><span class="sxs-lookup"><span data-stu-id="102aa-108">Properties</span></span>
|<span data-ttu-id="102aa-109">属性</span><span class="sxs-lookup"><span data-stu-id="102aa-109">Property</span></span>|<span data-ttu-id="102aa-110">类型</span><span class="sxs-lookup"><span data-stu-id="102aa-110">Type</span></span>|<span data-ttu-id="102aa-111">说明</span><span class="sxs-lookup"><span data-stu-id="102aa-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="102aa-112">displayName</span><span class="sxs-lookup"><span data-stu-id="102aa-112">displayName</span></span>|<span data-ttu-id="102aa-113">String</span><span class="sxs-lookup"><span data-stu-id="102aa-113">String</span></span>|<span data-ttu-id="102aa-114">显示名称。</span><span class="sxs-lookup"><span data-stu-id="102aa-114">Display name.</span></span>|
|<span data-ttu-id="102aa-115">ModifiedProperties</span><span class="sxs-lookup"><span data-stu-id="102aa-115">modifiedProperties</span></span>|<span data-ttu-id="102aa-116">[auditProperty](../resources/intune-auditing-auditproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="102aa-116">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="102aa-117">已修改属性列表。</span><span class="sxs-lookup"><span data-stu-id="102aa-117">List of modified properties.</span></span>|
|<span data-ttu-id="102aa-118">type</span><span class="sxs-lookup"><span data-stu-id="102aa-118">type</span></span>|<span data-ttu-id="102aa-119">String</span><span class="sxs-lookup"><span data-stu-id="102aa-119">String</span></span>|<span data-ttu-id="102aa-120">审核资源的类型。</span><span class="sxs-lookup"><span data-stu-id="102aa-120">Audit resource's type.</span></span>|
|<span data-ttu-id="102aa-121">resourceId</span><span class="sxs-lookup"><span data-stu-id="102aa-121">resourceId</span></span>|<span data-ttu-id="102aa-122">String</span><span class="sxs-lookup"><span data-stu-id="102aa-122">String</span></span>|<span data-ttu-id="102aa-123">审核资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="102aa-123">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="102aa-124">关系</span><span class="sxs-lookup"><span data-stu-id="102aa-124">Relationships</span></span>
<span data-ttu-id="102aa-125">无</span><span class="sxs-lookup"><span data-stu-id="102aa-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="102aa-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="102aa-126">JSON Representation</span></span>
<span data-ttu-id="102aa-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="102aa-127">Here is a JSON representation of the resource.</span></span>
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





