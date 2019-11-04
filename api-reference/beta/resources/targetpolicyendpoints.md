---
title: targetPolicyEndpoints 资源类型
description: 表示面向用户通知的平台。
localization_priority: Normal
ms.prod: notifications
doc_type: resourcePageType
author: merzink
ms.openlocfilehash: 9c1911900f4945d6f4b75d62c62457791fbb5c6a
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939465"
---
# <a name="targetpolicyendpoints-resource-type"></a><span data-ttu-id="f9ab6-103">targetPolicyEndpoints 资源类型</span><span class="sxs-lookup"><span data-stu-id="f9ab6-103">targetPolicyEndpoints resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9ab6-104">表示可定向到的平台，用于接收发送给用户的通知。</span><span class="sxs-lookup"><span data-stu-id="f9ab6-104">Represents the platforms that can be targeted to receive notifications sent to the user.</span></span>  <span data-ttu-id="f9ab6-105">其中包括 Windows、iOS、Android 和 Web。</span><span class="sxs-lookup"><span data-stu-id="f9ab6-105">These include Windows, iOS, Android and Web.</span></span> 


## <a name="properties"></a><span data-ttu-id="f9ab6-106">属性</span><span class="sxs-lookup"><span data-stu-id="f9ab6-106">Properties</span></span>

| <span data-ttu-id="f9ab6-107">属性</span><span class="sxs-lookup"><span data-stu-id="f9ab6-107">Property</span></span>     | <span data-ttu-id="f9ab6-108">类型</span><span class="sxs-lookup"><span data-stu-id="f9ab6-108">Type</span></span>        | <span data-ttu-id="f9ab6-109">描述</span><span class="sxs-lookup"><span data-stu-id="f9ab6-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f9ab6-110">platformTypes</span><span class="sxs-lookup"><span data-stu-id="f9ab6-110">platformTypes</span></span>|<span data-ttu-id="f9ab6-111">String collection</span><span class="sxs-lookup"><span data-stu-id="f9ab6-111">String collection</span></span>|<span data-ttu-id="f9ab6-112">使用将通知分发筛选到特定平台或平台。</span><span class="sxs-lookup"><span data-stu-id="f9ab6-112">Use to filter the notification distribution to a specific platform or platforms.</span></span> <span data-ttu-id="f9ab6-113">有效值为`Windows`、 `iOS` `Android`和。 `WebPush`</span><span class="sxs-lookup"><span data-stu-id="f9ab6-113">Valid values are `Windows`, `iOS`, `Android` and `WebPush`.</span></span> <span data-ttu-id="f9ab6-114">默认情况下，将启用所有推送终结点类型（Windows、iOS、Android 和 WebPush）。</span><span class="sxs-lookup"><span data-stu-id="f9ab6-114">By default, all push endpoint types (Windows, iOS, Android and WebPush) are enabled.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f9ab6-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f9ab6-115">JSON representation</span></span>

<span data-ttu-id="f9ab6-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f9ab6-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetPolicyEndpoints",
  "baseType": null
}-->

```json
{
  "platformTypes": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetPolicyEndpoints resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->