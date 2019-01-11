---
title: auditProperty 资源类型
description: 包含审核属性的属性的类。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b0a04d924560e712a0656584693940b127210645
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812864"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="009e0-103">auditProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="009e0-103">auditProperty resource type</span></span>

> <span data-ttu-id="009e0-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="009e0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="009e0-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="009e0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="009e0-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="009e0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="009e0-107">包含审核属性的属性的类。</span><span class="sxs-lookup"><span data-stu-id="009e0-107">A class containing the properties for Audit Property.</span></span>
## <a name="properties"></a><span data-ttu-id="009e0-108">属性</span><span class="sxs-lookup"><span data-stu-id="009e0-108">Properties</span></span>
|<span data-ttu-id="009e0-109">属性</span><span class="sxs-lookup"><span data-stu-id="009e0-109">Property</span></span>|<span data-ttu-id="009e0-110">类型</span><span class="sxs-lookup"><span data-stu-id="009e0-110">Type</span></span>|<span data-ttu-id="009e0-111">说明</span><span class="sxs-lookup"><span data-stu-id="009e0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="009e0-112">displayName</span><span class="sxs-lookup"><span data-stu-id="009e0-112">displayName</span></span>|<span data-ttu-id="009e0-113">String</span><span class="sxs-lookup"><span data-stu-id="009e0-113">String</span></span>|<span data-ttu-id="009e0-114">显示名称。</span><span class="sxs-lookup"><span data-stu-id="009e0-114">Display name.</span></span>|
|<span data-ttu-id="009e0-115">oldValue</span><span class="sxs-lookup"><span data-stu-id="009e0-115">oldValue</span></span>|<span data-ttu-id="009e0-116">String</span><span class="sxs-lookup"><span data-stu-id="009e0-116">String</span></span>|<span data-ttu-id="009e0-117">旧值。</span><span class="sxs-lookup"><span data-stu-id="009e0-117">Old value.</span></span>|
|<span data-ttu-id="009e0-118">NewValue</span><span class="sxs-lookup"><span data-stu-id="009e0-118">newValue</span></span>|<span data-ttu-id="009e0-119">String</span><span class="sxs-lookup"><span data-stu-id="009e0-119">String</span></span>|<span data-ttu-id="009e0-120">新值。</span><span class="sxs-lookup"><span data-stu-id="009e0-120">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="009e0-121">关系</span><span class="sxs-lookup"><span data-stu-id="009e0-121">Relationships</span></span>
<span data-ttu-id="009e0-122">无</span><span class="sxs-lookup"><span data-stu-id="009e0-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="009e0-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="009e0-123">JSON Representation</span></span>
<span data-ttu-id="009e0-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="009e0-124">Here is a JSON representation of the resource.</span></span>
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





