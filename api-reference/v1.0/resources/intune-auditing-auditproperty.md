---
title: auditProperty 资源类型
description: 包含审核属性的属性的类。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e91f3771be981f6ff410e8774f6a8ac9fbc121dd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870915"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="98e6d-103">auditProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="98e6d-103">auditProperty resource type</span></span>

> <span data-ttu-id="98e6d-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="98e6d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="98e6d-105">包含审核属性的属性的类。</span><span class="sxs-lookup"><span data-stu-id="98e6d-105">A class containing the properties for Audit Property.</span></span>
## <a name="properties"></a><span data-ttu-id="98e6d-106">属性</span><span class="sxs-lookup"><span data-stu-id="98e6d-106">Properties</span></span>
|<span data-ttu-id="98e6d-107">属性</span><span class="sxs-lookup"><span data-stu-id="98e6d-107">Property</span></span>|<span data-ttu-id="98e6d-108">类型</span><span class="sxs-lookup"><span data-stu-id="98e6d-108">Type</span></span>|<span data-ttu-id="98e6d-109">说明</span><span class="sxs-lookup"><span data-stu-id="98e6d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98e6d-110">displayName</span><span class="sxs-lookup"><span data-stu-id="98e6d-110">displayName</span></span>|<span data-ttu-id="98e6d-111">String</span><span class="sxs-lookup"><span data-stu-id="98e6d-111">String</span></span>|<span data-ttu-id="98e6d-112">显示名称。</span><span class="sxs-lookup"><span data-stu-id="98e6d-112">Display name.</span></span>|
|<span data-ttu-id="98e6d-113">oldValue</span><span class="sxs-lookup"><span data-stu-id="98e6d-113">oldValue</span></span>|<span data-ttu-id="98e6d-114">String</span><span class="sxs-lookup"><span data-stu-id="98e6d-114">String</span></span>|<span data-ttu-id="98e6d-115">旧值。</span><span class="sxs-lookup"><span data-stu-id="98e6d-115">Old value.</span></span>|
|<span data-ttu-id="98e6d-116">NewValue</span><span class="sxs-lookup"><span data-stu-id="98e6d-116">newValue</span></span>|<span data-ttu-id="98e6d-117">String</span><span class="sxs-lookup"><span data-stu-id="98e6d-117">String</span></span>|<span data-ttu-id="98e6d-118">新值。</span><span class="sxs-lookup"><span data-stu-id="98e6d-118">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="98e6d-119">关系</span><span class="sxs-lookup"><span data-stu-id="98e6d-119">Relationships</span></span>
<span data-ttu-id="98e6d-120">无</span><span class="sxs-lookup"><span data-stu-id="98e6d-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="98e6d-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="98e6d-121">JSON Representation</span></span>
<span data-ttu-id="98e6d-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="98e6d-122">Here is a JSON representation of the resource.</span></span>
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



