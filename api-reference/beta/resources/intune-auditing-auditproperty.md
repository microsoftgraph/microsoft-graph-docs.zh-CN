---
title: auditProperty 资源类型
description: 包含审核属性的属性的类。
ms.openlocfilehash: 944928014eee2e47ee0478053196bfbc1a999fc2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044897"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="ff255-103">auditProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="ff255-103">auditProperty resource type</span></span>

> <span data-ttu-id="ff255-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ff255-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ff255-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ff255-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ff255-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ff255-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ff255-107">包含审核属性的属性的类。</span><span class="sxs-lookup"><span data-stu-id="ff255-107">A class containing the properties for Audit Property.</span></span>
## <a name="properties"></a><span data-ttu-id="ff255-108">属性</span><span class="sxs-lookup"><span data-stu-id="ff255-108">Properties</span></span>
|<span data-ttu-id="ff255-109">属性</span><span class="sxs-lookup"><span data-stu-id="ff255-109">Property</span></span>|<span data-ttu-id="ff255-110">类型</span><span class="sxs-lookup"><span data-stu-id="ff255-110">Type</span></span>|<span data-ttu-id="ff255-111">说明</span><span class="sxs-lookup"><span data-stu-id="ff255-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff255-112">displayName</span><span class="sxs-lookup"><span data-stu-id="ff255-112">displayName</span></span>|<span data-ttu-id="ff255-113">String</span><span class="sxs-lookup"><span data-stu-id="ff255-113">String</span></span>|<span data-ttu-id="ff255-114">显示名称。</span><span class="sxs-lookup"><span data-stu-id="ff255-114">Display name.</span></span>|
|<span data-ttu-id="ff255-115">oldValue</span><span class="sxs-lookup"><span data-stu-id="ff255-115">oldValue</span></span>|<span data-ttu-id="ff255-116">String</span><span class="sxs-lookup"><span data-stu-id="ff255-116">String</span></span>|<span data-ttu-id="ff255-117">旧值。</span><span class="sxs-lookup"><span data-stu-id="ff255-117">Old value.</span></span>|
|<span data-ttu-id="ff255-118">NewValue</span><span class="sxs-lookup"><span data-stu-id="ff255-118">newValue</span></span>|<span data-ttu-id="ff255-119">String</span><span class="sxs-lookup"><span data-stu-id="ff255-119">String</span></span>|<span data-ttu-id="ff255-120">新值。</span><span class="sxs-lookup"><span data-stu-id="ff255-120">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff255-121">关系</span><span class="sxs-lookup"><span data-stu-id="ff255-121">Relationships</span></span>
<span data-ttu-id="ff255-122">无</span><span class="sxs-lookup"><span data-stu-id="ff255-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ff255-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ff255-123">JSON Representation</span></span>
<span data-ttu-id="ff255-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ff255-124">Here is a JSON representation of the resource.</span></span>
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





