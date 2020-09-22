---
title: clientUserAgent 资源类型
description: ClientUserAgent 类型
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 1833972fc97559cf10dac75e08ab11b5fe633a81
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071547"
---
# <a name="clientuseragent-resource-type"></a><span data-ttu-id="cbc46-103">clientUserAgent 资源类型</span><span class="sxs-lookup"><span data-stu-id="cbc46-103">clientUserAgent resource type</span></span>

<span data-ttu-id="cbc46-104">命名空间：microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="cbc46-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cbc46-105">表示呼叫中终结点的客户端用户代理。</span><span class="sxs-lookup"><span data-stu-id="cbc46-105">Represents a client user agent of an endpoint in a call.</span></span> <span data-ttu-id="cbc46-106">继承自 [userAgent](callrecords-useragent.md) 类型。</span><span class="sxs-lookup"><span data-stu-id="cbc46-106">Inherits from the [userAgent](callrecords-useragent.md) type.</span></span>

## <a name="properties"></a><span data-ttu-id="cbc46-107">属性</span><span class="sxs-lookup"><span data-stu-id="cbc46-107">Properties</span></span>

| <span data-ttu-id="cbc46-108">属性</span><span class="sxs-lookup"><span data-stu-id="cbc46-108">Property</span></span>     | <span data-ttu-id="cbc46-109">类型</span><span class="sxs-lookup"><span data-stu-id="cbc46-109">Type</span></span>        | <span data-ttu-id="cbc46-110">说明</span><span class="sxs-lookup"><span data-stu-id="cbc46-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cbc46-111">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="cbc46-111">applicationVersion</span></span>|<span data-ttu-id="cbc46-112">String</span><span class="sxs-lookup"><span data-stu-id="cbc46-112">String</span></span>|<span data-ttu-id="cbc46-113">标识此终结点使用的应用程序软件的版本。</span><span class="sxs-lookup"><span data-stu-id="cbc46-113">Identifies the version of application software used by this endpoint.</span></span>|
|<span data-ttu-id="cbc46-114">headerValue</span><span class="sxs-lookup"><span data-stu-id="cbc46-114">headerValue</span></span>|<span data-ttu-id="cbc46-115">String</span><span class="sxs-lookup"><span data-stu-id="cbc46-115">String</span></span>|<span data-ttu-id="cbc46-116">此终结点报告的用户代理标头值。</span><span class="sxs-lookup"><span data-stu-id="cbc46-116">User-agent header value reported by this endpoint.</span></span>|
|<span data-ttu-id="cbc46-117">平台</span><span class="sxs-lookup"><span data-stu-id="cbc46-117">platform</span></span>|<span data-ttu-id="cbc46-118">callRecords。 clientPlatform</span><span class="sxs-lookup"><span data-stu-id="cbc46-118">microsoft.graph.callRecords.clientPlatform</span></span>|<span data-ttu-id="cbc46-119">标识此终结点使用的平台。</span><span class="sxs-lookup"><span data-stu-id="cbc46-119">Identifies the platform used by this endpoint.</span></span> <span data-ttu-id="cbc46-120">可取值为：`unknown`、`windows`、`macOS`、`iOS`、`android`、`web`、`ipPhone`、`roomSystem`、`surfaceHub`、`holoLens`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="cbc46-120">Possible values are: `unknown`, `windows`, `macOS`, `iOS`, `android`, `web`, `ipPhone`, `roomSystem`, `surfaceHub`, `holoLens`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="cbc46-121">productFamily</span><span class="sxs-lookup"><span data-stu-id="cbc46-121">productFamily</span></span>|<span data-ttu-id="cbc46-122">callRecords。 productFamily</span><span class="sxs-lookup"><span data-stu-id="cbc46-122">microsoft.graph.callRecords.productFamily</span></span>|<span data-ttu-id="cbc46-123">标识此终结点使用的应用程序软件系列。</span><span class="sxs-lookup"><span data-stu-id="cbc46-123">Identifies the family of application software used by this endpoint.</span></span> <span data-ttu-id="cbc46-124">可取值为：`unknown`、`teams`、`skypeForBusiness`、`lync`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="cbc46-124">Possible values are: `unknown`, `teams`, `skypeForBusiness`, `lync`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cbc46-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cbc46-125">JSON representation</span></span>

<span data-ttu-id="cbc46-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cbc46-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.clientUserAgent",
  "baseType": "microsoft.graph.callRecords.userAgent"
}-->

```json
{
  "applicationVersion": "String",
  "headerValue": "String",
  "platform": "String",
  "productFamily": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "clientUserAgent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

