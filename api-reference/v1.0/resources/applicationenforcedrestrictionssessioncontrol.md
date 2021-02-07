---
title: applicationEnforcedRestrictionsSessionControl 资源类型
description: 强制实施应用程序限制的会话控制。
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 130644ebf0d72b4870dc78e64455c2dfab446ae5
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134965"
---
# <a name="applicationenforcedrestrictionssessioncontrol-resource-type"></a><span data-ttu-id="3493b-103">applicationEnforcedRestrictionsSessionControl 资源类型</span><span class="sxs-lookup"><span data-stu-id="3493b-103">applicationEnforcedRestrictionsSessionControl resource type</span></span>

<span data-ttu-id="3493b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3493b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3493b-105">强制实施应用程序限制的会话控制。</span><span class="sxs-lookup"><span data-stu-id="3493b-105">Session control to enforce application restrictions.</span></span> <span data-ttu-id="3493b-106">继承自 [条件访问会话控件](conditionalaccesssessioncontrol.md)。</span><span class="sxs-lookup"><span data-stu-id="3493b-106">Inherits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="3493b-107">属性</span><span class="sxs-lookup"><span data-stu-id="3493b-107">Properties</span></span>

| <span data-ttu-id="3493b-108">属性</span><span class="sxs-lookup"><span data-stu-id="3493b-108">Property</span></span>     | <span data-ttu-id="3493b-109">类型</span><span class="sxs-lookup"><span data-stu-id="3493b-109">Type</span></span>        | <span data-ttu-id="3493b-110">说明</span><span class="sxs-lookup"><span data-stu-id="3493b-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3493b-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="3493b-111">isEnabled</span></span>     |<span data-ttu-id="3493b-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="3493b-112">Boolean</span></span>      | <span data-ttu-id="3493b-113">指定是否启用会话控件。</span><span class="sxs-lookup"><span data-stu-id="3493b-113">Specifies whether the session control is enabled or not.</span></span> |

## <a name="relationships"></a><span data-ttu-id="3493b-114">关系</span><span class="sxs-lookup"><span data-stu-id="3493b-114">Relationships</span></span>

<span data-ttu-id="3493b-115">无。</span><span class="sxs-lookup"><span data-stu-id="3493b-115">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3493b-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3493b-116">JSON representation</span></span>

<span data-ttu-id="3493b-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3493b-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applicationEnforcedRestrictionsSessionControl",
  "baseType": "microsoft.graph.conditionalAccessSessionControl"
}-->

```json
{
  "isEnabled": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applicationEnforcedRestrictionsSessionControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

