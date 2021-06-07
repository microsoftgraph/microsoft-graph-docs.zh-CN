---
title: auditProperty 资源类型
description: 包含审核属性的属性的类。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 900e493ce77fd47a232626ad73999ce3482d4fe6
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52748900"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="88482-103">auditProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="88482-103">auditProperty resource type</span></span>

<span data-ttu-id="88482-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88482-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="88482-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="88482-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88482-106">包含审核属性的属性的类。</span><span class="sxs-lookup"><span data-stu-id="88482-106">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="88482-107">属性</span><span class="sxs-lookup"><span data-stu-id="88482-107">Properties</span></span>
|<span data-ttu-id="88482-108">属性</span><span class="sxs-lookup"><span data-stu-id="88482-108">Property</span></span>|<span data-ttu-id="88482-109">类型</span><span class="sxs-lookup"><span data-stu-id="88482-109">Type</span></span>|<span data-ttu-id="88482-110">说明</span><span class="sxs-lookup"><span data-stu-id="88482-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88482-111">displayName</span><span class="sxs-lookup"><span data-stu-id="88482-111">displayName</span></span>|<span data-ttu-id="88482-112">String</span><span class="sxs-lookup"><span data-stu-id="88482-112">String</span></span>|<span data-ttu-id="88482-113">显示名称。</span><span class="sxs-lookup"><span data-stu-id="88482-113">Display name.</span></span>|
|<span data-ttu-id="88482-114">oldValue</span><span class="sxs-lookup"><span data-stu-id="88482-114">oldValue</span></span>|<span data-ttu-id="88482-115">String</span><span class="sxs-lookup"><span data-stu-id="88482-115">String</span></span>|<span data-ttu-id="88482-116">旧值。</span><span class="sxs-lookup"><span data-stu-id="88482-116">Old value.</span></span>|
|<span data-ttu-id="88482-117">NewValue</span><span class="sxs-lookup"><span data-stu-id="88482-117">newValue</span></span>|<span data-ttu-id="88482-118">String</span><span class="sxs-lookup"><span data-stu-id="88482-118">String</span></span>|<span data-ttu-id="88482-119">新值。</span><span class="sxs-lookup"><span data-stu-id="88482-119">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="88482-120">关系</span><span class="sxs-lookup"><span data-stu-id="88482-120">Relationships</span></span>
<span data-ttu-id="88482-121">无</span><span class="sxs-lookup"><span data-stu-id="88482-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="88482-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="88482-122">JSON Representation</span></span>
<span data-ttu-id="88482-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="88482-123">Here is a JSON representation of the resource.</span></span>
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




