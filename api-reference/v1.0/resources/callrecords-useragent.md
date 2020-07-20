---
title: userAgent 资源类型
description: UserAgent 类型
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 795332d58359d0a0a5dd2776f6c93923fe1bafd8
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44492010"
---
# <a name="useragent-resource-type"></a><span data-ttu-id="b56b9-103">userAgent 资源类型</span><span class="sxs-lookup"><span data-stu-id="b56b9-103">userAgent resource type</span></span>

<span data-ttu-id="b56b9-104">命名空间：microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="b56b9-104">Namespace: microsoft.graph.callRecords</span></span>

<span data-ttu-id="b56b9-105">表示调用中终结点的用户代理。</span><span class="sxs-lookup"><span data-stu-id="b56b9-105">Represents the user agent of an endpoint in a call.</span></span>
<span data-ttu-id="b56b9-106">[ClientUserAgent](callrecords-clientuseragent.md)和[serviceUserAgent](callrecords-serviceuseragent.md)）类型继承自此类型。</span><span class="sxs-lookup"><span data-stu-id="b56b9-106">The [clientUserAgent](callrecords-clientuseragent.md) and [serviceUserAgent](callrecords-serviceuseragent.md)) types inherit from this type.</span></span>

## <a name="properties"></a><span data-ttu-id="b56b9-107">属性</span><span class="sxs-lookup"><span data-stu-id="b56b9-107">Properties</span></span>

| <span data-ttu-id="b56b9-108">属性</span><span class="sxs-lookup"><span data-stu-id="b56b9-108">Property</span></span>     | <span data-ttu-id="b56b9-109">类型</span><span class="sxs-lookup"><span data-stu-id="b56b9-109">Type</span></span>        | <span data-ttu-id="b56b9-110">Description</span><span class="sxs-lookup"><span data-stu-id="b56b9-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b56b9-111">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="b56b9-111">applicationVersion</span></span>|<span data-ttu-id="b56b9-112">String</span><span class="sxs-lookup"><span data-stu-id="b56b9-112">String</span></span>|<span data-ttu-id="b56b9-113">标识此终结点使用的应用程序软件的版本。</span><span class="sxs-lookup"><span data-stu-id="b56b9-113">Identifies the version of application software used by this endpoint.</span></span>|
|<span data-ttu-id="b56b9-114">headerValue</span><span class="sxs-lookup"><span data-stu-id="b56b9-114">headerValue</span></span>|<span data-ttu-id="b56b9-115">String</span><span class="sxs-lookup"><span data-stu-id="b56b9-115">String</span></span>|<span data-ttu-id="b56b9-116">此终结点报告的用户代理标头值。</span><span class="sxs-lookup"><span data-stu-id="b56b9-116">User-agent header value reported by this endpoint.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b56b9-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b56b9-117">JSON representation</span></span>

<span data-ttu-id="b56b9-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b56b9-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.userAgent",
  "baseType": null
}-->

```json
{
  "applicationVersion": "String",
  "headerValue": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userAgent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->