---
title: auditProperty 资源类型
description: 包含审核属性的属性的类。
ms.openlocfilehash: eaffa5552d611ac2ef8bb236009b9520d1134586
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011073"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="c6b2b-103">auditProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="c6b2b-103">auditProperty resource type</span></span>

> <span data-ttu-id="c6b2b-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c6b2b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c6b2b-105">包含审核属性的属性的类。</span><span class="sxs-lookup"><span data-stu-id="c6b2b-105">A class containing the properties for Audit Property.</span></span>
## <a name="properties"></a><span data-ttu-id="c6b2b-106">属性</span><span class="sxs-lookup"><span data-stu-id="c6b2b-106">Properties</span></span>
|<span data-ttu-id="c6b2b-107">属性</span><span class="sxs-lookup"><span data-stu-id="c6b2b-107">Property</span></span>|<span data-ttu-id="c6b2b-108">类型</span><span class="sxs-lookup"><span data-stu-id="c6b2b-108">Type</span></span>|<span data-ttu-id="c6b2b-109">说明</span><span class="sxs-lookup"><span data-stu-id="c6b2b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6b2b-110">displayName</span><span class="sxs-lookup"><span data-stu-id="c6b2b-110">displayName</span></span>|<span data-ttu-id="c6b2b-111">String</span><span class="sxs-lookup"><span data-stu-id="c6b2b-111">String</span></span>|<span data-ttu-id="c6b2b-112">显示名称。</span><span class="sxs-lookup"><span data-stu-id="c6b2b-112">Display name.</span></span>|
|<span data-ttu-id="c6b2b-113">oldValue</span><span class="sxs-lookup"><span data-stu-id="c6b2b-113">oldValue</span></span>|<span data-ttu-id="c6b2b-114">String</span><span class="sxs-lookup"><span data-stu-id="c6b2b-114">String</span></span>|<span data-ttu-id="c6b2b-115">旧值。</span><span class="sxs-lookup"><span data-stu-id="c6b2b-115">Old value.</span></span>|
|<span data-ttu-id="c6b2b-116">NewValue</span><span class="sxs-lookup"><span data-stu-id="c6b2b-116">newValue</span></span>|<span data-ttu-id="c6b2b-117">String</span><span class="sxs-lookup"><span data-stu-id="c6b2b-117">String</span></span>|<span data-ttu-id="c6b2b-118">新值。</span><span class="sxs-lookup"><span data-stu-id="c6b2b-118">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c6b2b-119">关系</span><span class="sxs-lookup"><span data-stu-id="c6b2b-119">Relationships</span></span>
<span data-ttu-id="c6b2b-120">无</span><span class="sxs-lookup"><span data-stu-id="c6b2b-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c6b2b-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c6b2b-121">JSON Representation</span></span>
<span data-ttu-id="c6b2b-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c6b2b-122">Here is a JSON representation of the resource.</span></span>
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



