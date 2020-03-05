---
title: targetPolicyEndpoints 资源类型
description: 表示面向用户通知的平台。
localization_priority: Normal
ms.prod: notifications
doc_type: resourcePageType
author: merzink
ms.openlocfilehash: 92ff6d0748e24fd58154f596188f25c51bdc6403
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520000"
---
# <a name="targetpolicyendpoints-resource-type"></a><span data-ttu-id="41f68-103">targetPolicyEndpoints 资源类型</span><span class="sxs-lookup"><span data-stu-id="41f68-103">targetPolicyEndpoints resource type</span></span>

<span data-ttu-id="41f68-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="41f68-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41f68-105">表示可定向到的平台，用于接收发送给用户的通知。</span><span class="sxs-lookup"><span data-stu-id="41f68-105">Represents the platforms that can be targeted to receive notifications sent to the user.</span></span>  <span data-ttu-id="41f68-106">其中包括 Windows、iOS、Android 和 Web。</span><span class="sxs-lookup"><span data-stu-id="41f68-106">These include Windows, iOS, Android and Web.</span></span> 


## <a name="properties"></a><span data-ttu-id="41f68-107">属性</span><span class="sxs-lookup"><span data-stu-id="41f68-107">Properties</span></span>

| <span data-ttu-id="41f68-108">属性</span><span class="sxs-lookup"><span data-stu-id="41f68-108">Property</span></span>     | <span data-ttu-id="41f68-109">类型</span><span class="sxs-lookup"><span data-stu-id="41f68-109">Type</span></span>        | <span data-ttu-id="41f68-110">说明</span><span class="sxs-lookup"><span data-stu-id="41f68-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="41f68-111">platformTypes</span><span class="sxs-lookup"><span data-stu-id="41f68-111">platformTypes</span></span>|<span data-ttu-id="41f68-112">String 集合</span><span class="sxs-lookup"><span data-stu-id="41f68-112">String collection</span></span>|<span data-ttu-id="41f68-113">使用将通知分发筛选到特定平台或平台。</span><span class="sxs-lookup"><span data-stu-id="41f68-113">Use to filter the notification distribution to a specific platform or platforms.</span></span> <span data-ttu-id="41f68-114">有效值为`Windows`、 `iOS` `Android`和。 `WebPush`</span><span class="sxs-lookup"><span data-stu-id="41f68-114">Valid values are `Windows`, `iOS`, `Android` and `WebPush`.</span></span> <span data-ttu-id="41f68-115">默认情况下，将启用所有推送终结点类型（Windows、iOS、Android 和 WebPush）。</span><span class="sxs-lookup"><span data-stu-id="41f68-115">By default, all push endpoint types (Windows, iOS, Android and WebPush) are enabled.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="41f68-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="41f68-116">JSON representation</span></span>

<span data-ttu-id="41f68-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="41f68-117">The following is a JSON representation of the resource.</span></span>

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