---
title: auditProperty 资源类型
description: 包含审核属性的属性的类。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3425c59ae4f30b30b04bd22f74cb1b27ad99191f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416641"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="b86cd-103">auditProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="b86cd-103">auditProperty resource type</span></span>

> <span data-ttu-id="b86cd-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="b86cd-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b86cd-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b86cd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b86cd-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b86cd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b86cd-107">包含审核属性的属性的类。</span><span class="sxs-lookup"><span data-stu-id="b86cd-107">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="b86cd-108">属性</span><span class="sxs-lookup"><span data-stu-id="b86cd-108">Properties</span></span>
|<span data-ttu-id="b86cd-109">属性</span><span class="sxs-lookup"><span data-stu-id="b86cd-109">Property</span></span>|<span data-ttu-id="b86cd-110">类型</span><span class="sxs-lookup"><span data-stu-id="b86cd-110">Type</span></span>|<span data-ttu-id="b86cd-111">说明</span><span class="sxs-lookup"><span data-stu-id="b86cd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b86cd-112">displayName</span><span class="sxs-lookup"><span data-stu-id="b86cd-112">displayName</span></span>|<span data-ttu-id="b86cd-113">String</span><span class="sxs-lookup"><span data-stu-id="b86cd-113">String</span></span>|<span data-ttu-id="b86cd-114">显示名称。</span><span class="sxs-lookup"><span data-stu-id="b86cd-114">Display name.</span></span>|
|<span data-ttu-id="b86cd-115">oldValue</span><span class="sxs-lookup"><span data-stu-id="b86cd-115">oldValue</span></span>|<span data-ttu-id="b86cd-116">String</span><span class="sxs-lookup"><span data-stu-id="b86cd-116">String</span></span>|<span data-ttu-id="b86cd-117">旧值。</span><span class="sxs-lookup"><span data-stu-id="b86cd-117">Old value.</span></span>|
|<span data-ttu-id="b86cd-118">NewValue</span><span class="sxs-lookup"><span data-stu-id="b86cd-118">newValue</span></span>|<span data-ttu-id="b86cd-119">String</span><span class="sxs-lookup"><span data-stu-id="b86cd-119">String</span></span>|<span data-ttu-id="b86cd-120">新值。</span><span class="sxs-lookup"><span data-stu-id="b86cd-120">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b86cd-121">关系</span><span class="sxs-lookup"><span data-stu-id="b86cd-121">Relationships</span></span>
<span data-ttu-id="b86cd-122">无</span><span class="sxs-lookup"><span data-stu-id="b86cd-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b86cd-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b86cd-123">JSON Representation</span></span>
<span data-ttu-id="b86cd-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b86cd-124">Here is a JSON representation of the resource.</span></span>
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




