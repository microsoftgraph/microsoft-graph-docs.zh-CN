---
title: conditionalAccessSessionControls 资源类型
description: 表示登录后强制实施的会话控件的复杂类型。
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 78c9ab3c3b5a55623ba13e1f7ce6d28a9425ded5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057008"
---
# <a name="conditionalaccesssessioncontrols-resource-type"></a><span data-ttu-id="33b26-103">conditionalAccessSessionControls 资源类型</span><span class="sxs-lookup"><span data-stu-id="33b26-103">conditionalAccessSessionControls resource type</span></span>

<span data-ttu-id="33b26-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33b26-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="33b26-105">表示登录后强制实施的会话控件。</span><span class="sxs-lookup"><span data-stu-id="33b26-105">Represents session controls that are enforced after sign-in.</span></span>
<span data-ttu-id="33b26-106">所有会话控件都继承自 [conditionalAccessSessionControl](conditionalaccesssessioncontrol.md)。</span><span class="sxs-lookup"><span data-stu-id="33b26-106">All the session controls inherit from [conditionalAccessSessionControl](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="33b26-107">属性</span><span class="sxs-lookup"><span data-stu-id="33b26-107">Properties</span></span>

| <span data-ttu-id="33b26-108">属性</span><span class="sxs-lookup"><span data-stu-id="33b26-108">Property</span></span>     | <span data-ttu-id="33b26-109">类型</span><span class="sxs-lookup"><span data-stu-id="33b26-109">Type</span></span>        | <span data-ttu-id="33b26-110">说明</span><span class="sxs-lookup"><span data-stu-id="33b26-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="33b26-111">applicationEnforcedRestrictions</span><span class="sxs-lookup"><span data-stu-id="33b26-111">applicationEnforcedRestrictions</span></span>|[<span data-ttu-id="33b26-112">applicationEnforcedRestrictionsSessionControl</span><span class="sxs-lookup"><span data-stu-id="33b26-112">applicationEnforcedRestrictionsSessionControl</span></span>](applicationenforcedrestrictionssessioncontrol.md)| <span data-ttu-id="33b26-113">实施应用程序限制的会话控制。</span><span class="sxs-lookup"><span data-stu-id="33b26-113">Session control to enforce application restrictions.</span></span> <span data-ttu-id="33b26-114">仅 Exchange Online 和 Sharepoint Online 支持此会话控制。</span><span class="sxs-lookup"><span data-stu-id="33b26-114">Only Exchange Online and Sharepoint Online support this session control.</span></span> |
|<span data-ttu-id="33b26-115">cloudAppSecurity</span><span class="sxs-lookup"><span data-stu-id="33b26-115">cloudAppSecurity</span></span>|[<span data-ttu-id="33b26-116">cloudAppSecuritySessionControl</span><span class="sxs-lookup"><span data-stu-id="33b26-116">cloudAppSecuritySessionControl</span></span>](cloudappsecuritysessioncontrol.md)| <span data-ttu-id="33b26-117">应用云应用安全性的会话控制。</span><span class="sxs-lookup"><span data-stu-id="33b26-117">Session control to apply cloud app security.</span></span>|
|<span data-ttu-id="33b26-118">persistentBrowser</span><span class="sxs-lookup"><span data-stu-id="33b26-118">persistentBrowser</span></span>|[<span data-ttu-id="33b26-119">persistentBrowserSessionControl</span><span class="sxs-lookup"><span data-stu-id="33b26-119">persistentBrowserSessionControl</span></span>](persistentbrowsersessioncontrol.md)| <span data-ttu-id="33b26-120">用于定义是否保持 cookie 的会话控制。</span><span class="sxs-lookup"><span data-stu-id="33b26-120">Session control to define whether to persist cookies or not.</span></span> <span data-ttu-id="33b26-121">应选择所有应用程序以使此会话控件正常工作。</span><span class="sxs-lookup"><span data-stu-id="33b26-121">All apps should be selected for this session control to work correctly.</span></span> |
|<span data-ttu-id="33b26-122">signInFrequency</span><span class="sxs-lookup"><span data-stu-id="33b26-122">signInFrequency</span></span>|[<span data-ttu-id="33b26-123">signInFrequencySessionControl</span><span class="sxs-lookup"><span data-stu-id="33b26-123">signInFrequencySessionControl</span></span>](signinfrequencysessioncontrol.md)| <span data-ttu-id="33b26-124">用于强制登录频率的会话控制。</span><span class="sxs-lookup"><span data-stu-id="33b26-124">Session control to enforce signin frequency.</span></span>|

## <a name="relationships"></a><span data-ttu-id="33b26-125">关系</span><span class="sxs-lookup"><span data-stu-id="33b26-125">Relationships</span></span>

<span data-ttu-id="33b26-126">无。</span><span class="sxs-lookup"><span data-stu-id="33b26-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="33b26-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="33b26-127">JSON representation</span></span>

<span data-ttu-id="33b26-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="33b26-128">The following is a JSON representation of the resource.</span></span>

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

