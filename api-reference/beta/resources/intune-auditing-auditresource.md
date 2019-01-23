---
title: auditResource 资源类型
description: 包含审核资源的属性的类。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bba8aa9cfe10d17cefdcfe28d25c4d8c2dfa429f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412476"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="3ac3b-103">auditResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="3ac3b-103">auditResource resource type</span></span>

> <span data-ttu-id="3ac3b-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="3ac3b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3ac3b-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3ac3b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3ac3b-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3ac3b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ac3b-107">包含审核资源的属性的类。</span><span class="sxs-lookup"><span data-stu-id="3ac3b-107">A class containing the properties for Audit Resource.</span></span>

## <a name="properties"></a><span data-ttu-id="3ac3b-108">属性</span><span class="sxs-lookup"><span data-stu-id="3ac3b-108">Properties</span></span>
|<span data-ttu-id="3ac3b-109">属性</span><span class="sxs-lookup"><span data-stu-id="3ac3b-109">Property</span></span>|<span data-ttu-id="3ac3b-110">类型</span><span class="sxs-lookup"><span data-stu-id="3ac3b-110">Type</span></span>|<span data-ttu-id="3ac3b-111">说明</span><span class="sxs-lookup"><span data-stu-id="3ac3b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ac3b-112">displayName</span><span class="sxs-lookup"><span data-stu-id="3ac3b-112">displayName</span></span>|<span data-ttu-id="3ac3b-113">String</span><span class="sxs-lookup"><span data-stu-id="3ac3b-113">String</span></span>|<span data-ttu-id="3ac3b-114">显示名称。</span><span class="sxs-lookup"><span data-stu-id="3ac3b-114">Display name.</span></span>|
|<span data-ttu-id="3ac3b-115">ModifiedProperties</span><span class="sxs-lookup"><span data-stu-id="3ac3b-115">modifiedProperties</span></span>|<span data-ttu-id="3ac3b-116">[auditProperty](../resources/intune-auditing-auditproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3ac3b-116">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="3ac3b-117">已修改属性列表。</span><span class="sxs-lookup"><span data-stu-id="3ac3b-117">List of modified properties.</span></span>|
|<span data-ttu-id="3ac3b-118">type</span><span class="sxs-lookup"><span data-stu-id="3ac3b-118">type</span></span>|<span data-ttu-id="3ac3b-119">String</span><span class="sxs-lookup"><span data-stu-id="3ac3b-119">String</span></span>|<span data-ttu-id="3ac3b-120">审核资源的类型。</span><span class="sxs-lookup"><span data-stu-id="3ac3b-120">Audit resource's type.</span></span>|
|<span data-ttu-id="3ac3b-121">resourceId</span><span class="sxs-lookup"><span data-stu-id="3ac3b-121">resourceId</span></span>|<span data-ttu-id="3ac3b-122">String</span><span class="sxs-lookup"><span data-stu-id="3ac3b-122">String</span></span>|<span data-ttu-id="3ac3b-123">审核资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="3ac3b-123">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3ac3b-124">关系</span><span class="sxs-lookup"><span data-stu-id="3ac3b-124">Relationships</span></span>
<span data-ttu-id="3ac3b-125">无</span><span class="sxs-lookup"><span data-stu-id="3ac3b-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3ac3b-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3ac3b-126">JSON Representation</span></span>
<span data-ttu-id="3ac3b-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3ac3b-127">Here is a JSON representation of the resource.</span></span>
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




