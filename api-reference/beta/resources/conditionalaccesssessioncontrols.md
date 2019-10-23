---
title: conditionalAccessSessionControls 资源类型
description: 表示登录后强制实施的会话控件的复杂类型。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 317120eb7c4138d955bf8a35030375180d5a1631
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638545"
---
# <a name="conditionalaccesssessioncontrols-resource-type"></a><span data-ttu-id="b2e04-103">conditionalAccessSessionControls 资源类型</span><span class="sxs-lookup"><span data-stu-id="b2e04-103">conditionalAccessSessionControls resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2e04-104">表示登录后强制实施的会话控件。</span><span class="sxs-lookup"><span data-stu-id="b2e04-104">Represents session controls that are enforced after sign-in.</span></span>
<span data-ttu-id="b2e04-105">所有会话控件都继承自[conditionalAccessSessionControl](conditionalaccesssessioncontrol.md)。</span><span class="sxs-lookup"><span data-stu-id="b2e04-105">All the session controls inherit from [conditionalAccessSessionControl](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b2e04-106">属性</span><span class="sxs-lookup"><span data-stu-id="b2e04-106">Properties</span></span>

| <span data-ttu-id="b2e04-107">属性</span><span class="sxs-lookup"><span data-stu-id="b2e04-107">Property</span></span>     | <span data-ttu-id="b2e04-108">类型</span><span class="sxs-lookup"><span data-stu-id="b2e04-108">Type</span></span>        | <span data-ttu-id="b2e04-109">说明</span><span class="sxs-lookup"><span data-stu-id="b2e04-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b2e04-110">applicationEnforcedRestrictions</span><span class="sxs-lookup"><span data-stu-id="b2e04-110">applicationEnforcedRestrictions</span></span>|[<span data-ttu-id="b2e04-111">applicationEnforcedRestrictionsSessionControl</span><span class="sxs-lookup"><span data-stu-id="b2e04-111">applicationEnforcedRestrictionsSessionControl</span></span>](applicationenforcedrestrictionssessioncontrol.md)| <span data-ttu-id="b2e04-112">实施应用程序限制的会话控制。</span><span class="sxs-lookup"><span data-stu-id="b2e04-112">Session control to enforce application restrictions.</span></span> <span data-ttu-id="b2e04-113">仅 Exchange Online 和 Sharepoint Online 支持此会话控制。</span><span class="sxs-lookup"><span data-stu-id="b2e04-113">Only Exchange Online and Sharepoint Online support this session control.</span></span> |
|<span data-ttu-id="b2e04-114">cloudAppSecurity</span><span class="sxs-lookup"><span data-stu-id="b2e04-114">cloudAppSecurity</span></span>|[<span data-ttu-id="b2e04-115">cloudAppSecuritySessionControl</span><span class="sxs-lookup"><span data-stu-id="b2e04-115">cloudAppSecuritySessionControl</span></span>](cloudappsecuritysessioncontrol.md)| <span data-ttu-id="b2e04-116">应用云应用安全性的会话控制。</span><span class="sxs-lookup"><span data-stu-id="b2e04-116">Session control to apply cloud app security.</span></span>|
|<span data-ttu-id="b2e04-117">persistentBrowser</span><span class="sxs-lookup"><span data-stu-id="b2e04-117">persistentBrowser</span></span>|[<span data-ttu-id="b2e04-118">persistentBrowserSessionControl</span><span class="sxs-lookup"><span data-stu-id="b2e04-118">persistentBrowserSessionControl</span></span>](persistentbrowsersessioncontrol.md)| <span data-ttu-id="b2e04-119">用于定义是否保持 cookie 的会话控制。</span><span class="sxs-lookup"><span data-stu-id="b2e04-119">Session control to define whether to persist cookies or not.</span></span> <span data-ttu-id="b2e04-120">应选择所有应用程序以使此会话控件正常工作。</span><span class="sxs-lookup"><span data-stu-id="b2e04-120">All apps should be selected for this session control to work correctly.</span></span> |
|<span data-ttu-id="b2e04-121">signInFrequency</span><span class="sxs-lookup"><span data-stu-id="b2e04-121">signInFrequency</span></span>|[<span data-ttu-id="b2e04-122">signInFrequencySessionControl</span><span class="sxs-lookup"><span data-stu-id="b2e04-122">signInFrequencySessionControl</span></span>](signinfrequencysessioncontrol.md)| <span data-ttu-id="b2e04-123">用于强制登录频率的会话控制。</span><span class="sxs-lookup"><span data-stu-id="b2e04-123">Session control to enforce signin frequency.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b2e04-124">关系</span><span class="sxs-lookup"><span data-stu-id="b2e04-124">Relationships</span></span>

<span data-ttu-id="b2e04-125">无。</span><span class="sxs-lookup"><span data-stu-id="b2e04-125">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b2e04-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b2e04-126">JSON representation</span></span>

<span data-ttu-id="b2e04-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b2e04-127">The following is a JSON representation of the resource.</span></span>

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