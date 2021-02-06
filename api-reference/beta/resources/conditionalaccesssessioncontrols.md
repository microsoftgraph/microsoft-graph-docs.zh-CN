---
title: conditionalAccessSessionControls 资源类型
description: 表示登录后强制执行的复杂会话控件类型。
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: bf50399a26999c35730e2ce0c171c1be8777841d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134887"
---
# <a name="conditionalaccesssessioncontrols-resource-type"></a><span data-ttu-id="e44a4-103">conditionalAccessSessionControls 资源类型</span><span class="sxs-lookup"><span data-stu-id="e44a4-103">conditionalAccessSessionControls resource type</span></span>

<span data-ttu-id="e44a4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e44a4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e44a4-105">表示登录后强制执行的会话控件。</span><span class="sxs-lookup"><span data-stu-id="e44a4-105">Represents session controls that are enforced after sign-in.</span></span>
<span data-ttu-id="e44a4-106">所有会话控件都继承自 [conditionalAccessSessionControl](conditionalaccesssessioncontrol.md)。</span><span class="sxs-lookup"><span data-stu-id="e44a4-106">All the session controls inherit from [conditionalAccessSessionControl](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e44a4-107">属性</span><span class="sxs-lookup"><span data-stu-id="e44a4-107">Properties</span></span>

| <span data-ttu-id="e44a4-108">属性</span><span class="sxs-lookup"><span data-stu-id="e44a4-108">Property</span></span>     | <span data-ttu-id="e44a4-109">类型</span><span class="sxs-lookup"><span data-stu-id="e44a4-109">Type</span></span>        | <span data-ttu-id="e44a4-110">说明</span><span class="sxs-lookup"><span data-stu-id="e44a4-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e44a4-111">applicationEnforcedRestrictions</span><span class="sxs-lookup"><span data-stu-id="e44a4-111">applicationEnforcedRestrictions</span></span>|[<span data-ttu-id="e44a4-112">applicationEnforcedRestrictionsSessionControl</span><span class="sxs-lookup"><span data-stu-id="e44a4-112">applicationEnforcedRestrictionsSessionControl</span></span>](applicationenforcedrestrictionssessioncontrol.md)| <span data-ttu-id="e44a4-113">强制实施应用程序限制的会话控制。</span><span class="sxs-lookup"><span data-stu-id="e44a4-113">Session control to enforce application restrictions.</span></span> <span data-ttu-id="e44a4-114">只有 Exchange Online 和 Sharepoint Online 支持此会话控制。</span><span class="sxs-lookup"><span data-stu-id="e44a4-114">Only Exchange Online and Sharepoint Online support this session control.</span></span> |
|<span data-ttu-id="e44a4-115">cloudAppSecurity</span><span class="sxs-lookup"><span data-stu-id="e44a4-115">cloudAppSecurity</span></span>|[<span data-ttu-id="e44a4-116">cloudAppSecuritySessionControl</span><span class="sxs-lookup"><span data-stu-id="e44a4-116">cloudAppSecuritySessionControl</span></span>](cloudappsecuritysessioncontrol.md)| <span data-ttu-id="e44a4-117">应用云应用安全性的会话控制。</span><span class="sxs-lookup"><span data-stu-id="e44a4-117">Session control to apply cloud app security.</span></span>|
|<span data-ttu-id="e44a4-118">persistentBrowser</span><span class="sxs-lookup"><span data-stu-id="e44a4-118">persistentBrowser</span></span>|[<span data-ttu-id="e44a4-119">persistentBrowserSessionControl</span><span class="sxs-lookup"><span data-stu-id="e44a4-119">persistentBrowserSessionControl</span></span>](persistentbrowsersessioncontrol.md)| <span data-ttu-id="e44a4-120">用于定义是否保留 Cookie 的会话控件。</span><span class="sxs-lookup"><span data-stu-id="e44a4-120">Session control to define whether to persist cookies or not.</span></span> <span data-ttu-id="e44a4-121">应选择所有应用，使此会话控件正常工作。</span><span class="sxs-lookup"><span data-stu-id="e44a4-121">All apps should be selected for this session control to work correctly.</span></span> |
|<span data-ttu-id="e44a4-122">signInFrequency</span><span class="sxs-lookup"><span data-stu-id="e44a4-122">signInFrequency</span></span>|[<span data-ttu-id="e44a4-123">signInFrequencySessionControl</span><span class="sxs-lookup"><span data-stu-id="e44a4-123">signInFrequencySessionControl</span></span>](signinfrequencysessioncontrol.md)| <span data-ttu-id="e44a4-124">强制登录频率的会话控制。</span><span class="sxs-lookup"><span data-stu-id="e44a4-124">Session control to enforce signin frequency.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e44a4-125">关系</span><span class="sxs-lookup"><span data-stu-id="e44a4-125">Relationships</span></span>

<span data-ttu-id="e44a4-126">无。</span><span class="sxs-lookup"><span data-stu-id="e44a4-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e44a4-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e44a4-127">JSON representation</span></span>

<span data-ttu-id="e44a4-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e44a4-128">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "applicationEnforcedRestrictions",
    "persistentBrowser",
    "cloudAppSecurity",
    "signInFrequency"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessSessionControls",
  "baseType": null
}-->

```json
{
  "applicationEnforcedRestrictions": {"@odata.type": "microsoft.graph.applicationEnforcedRestrictionsSessionControl"},
  "cloudAppSecurity": {"@odata.type": "microsoft.graph.cloudAppSecuritySessionControl"},
  "persistentBrowser": {"@odata.type": "microsoft.graph.persistentBrowserSessionControl"},
  "signInFrequency": {"@odata.type": "microsoft.graph.signInFrequencySessionControl"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessSessionControls resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

