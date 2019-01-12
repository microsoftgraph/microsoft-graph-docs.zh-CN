---
title: auditResource 资源类型
description: 包含审核资源的属性的类。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ac7da99203631696b8c93fbde62db906143ffe38
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952242"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="1e834-103">auditResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="1e834-103">auditResource resource type</span></span>

> <span data-ttu-id="1e834-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1e834-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1e834-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1e834-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1e834-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1e834-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1e834-107">包含审核资源的属性的类。</span><span class="sxs-lookup"><span data-stu-id="1e834-107">A class containing the properties for Audit Resource.</span></span>
## <a name="properties"></a><span data-ttu-id="1e834-108">属性</span><span class="sxs-lookup"><span data-stu-id="1e834-108">Properties</span></span>
|<span data-ttu-id="1e834-109">属性</span><span class="sxs-lookup"><span data-stu-id="1e834-109">Property</span></span>|<span data-ttu-id="1e834-110">类型</span><span class="sxs-lookup"><span data-stu-id="1e834-110">Type</span></span>|<span data-ttu-id="1e834-111">说明</span><span class="sxs-lookup"><span data-stu-id="1e834-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e834-112">displayName</span><span class="sxs-lookup"><span data-stu-id="1e834-112">displayName</span></span>|<span data-ttu-id="1e834-113">String</span><span class="sxs-lookup"><span data-stu-id="1e834-113">String</span></span>|<span data-ttu-id="1e834-114">显示名称。</span><span class="sxs-lookup"><span data-stu-id="1e834-114">Display name.</span></span>|
|<span data-ttu-id="1e834-115">ModifiedProperties</span><span class="sxs-lookup"><span data-stu-id="1e834-115">modifiedProperties</span></span>|<span data-ttu-id="1e834-116">[auditProperty](../resources/intune-auditing-auditproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1e834-116">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="1e834-117">已修改属性列表。</span><span class="sxs-lookup"><span data-stu-id="1e834-117">List of modified properties.</span></span>|
|<span data-ttu-id="1e834-118">type</span><span class="sxs-lookup"><span data-stu-id="1e834-118">type</span></span>|<span data-ttu-id="1e834-119">String</span><span class="sxs-lookup"><span data-stu-id="1e834-119">String</span></span>|<span data-ttu-id="1e834-120">审核资源的类型。</span><span class="sxs-lookup"><span data-stu-id="1e834-120">Audit resource's type.</span></span>|
|<span data-ttu-id="1e834-121">resourceId</span><span class="sxs-lookup"><span data-stu-id="1e834-121">resourceId</span></span>|<span data-ttu-id="1e834-122">String</span><span class="sxs-lookup"><span data-stu-id="1e834-122">String</span></span>|<span data-ttu-id="1e834-123">审核资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="1e834-123">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1e834-124">关系</span><span class="sxs-lookup"><span data-stu-id="1e834-124">Relationships</span></span>
<span data-ttu-id="1e834-125">无</span><span class="sxs-lookup"><span data-stu-id="1e834-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1e834-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1e834-126">JSON Representation</span></span>
<span data-ttu-id="1e834-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1e834-127">Here is a JSON representation of the resource.</span></span>
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





