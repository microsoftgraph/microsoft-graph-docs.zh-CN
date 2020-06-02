---
title: clientUserAgent 资源类型
description: ClientUserAgent 类型
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8a21133cfe70f7c887f8d0ecbc782f1b872d0940
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44491951"
---
# <a name="clientuseragent-resource-type"></a><span data-ttu-id="7b807-103">clientUserAgent 资源类型</span><span class="sxs-lookup"><span data-stu-id="7b807-103">clientUserAgent resource type</span></span>

<span data-ttu-id="7b807-104">命名空间：microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="7b807-104">Namespace: microsoft.graph.callRecords</span></span>

<span data-ttu-id="7b807-105">表示呼叫中终结点的客户端用户代理。</span><span class="sxs-lookup"><span data-stu-id="7b807-105">Represents a client user agent of an endpoint in a call.</span></span> <span data-ttu-id="7b807-106">继承自[userAgent](callrecords-useragent.md)类型。</span><span class="sxs-lookup"><span data-stu-id="7b807-106">Inherits from the [userAgent](callrecords-useragent.md) type.</span></span>

## <a name="properties"></a><span data-ttu-id="7b807-107">属性</span><span class="sxs-lookup"><span data-stu-id="7b807-107">Properties</span></span>

| <span data-ttu-id="7b807-108">属性</span><span class="sxs-lookup"><span data-stu-id="7b807-108">Property</span></span>     | <span data-ttu-id="7b807-109">类型</span><span class="sxs-lookup"><span data-stu-id="7b807-109">Type</span></span>        | <span data-ttu-id="7b807-110">Description</span><span class="sxs-lookup"><span data-stu-id="7b807-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7b807-111">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="7b807-111">applicationVersion</span></span>|<span data-ttu-id="7b807-112">String</span><span class="sxs-lookup"><span data-stu-id="7b807-112">String</span></span>|<span data-ttu-id="7b807-113">标识此终结点使用的应用程序软件的版本。</span><span class="sxs-lookup"><span data-stu-id="7b807-113">Identifies the version of application software used by this endpoint.</span></span>|
|<span data-ttu-id="7b807-114">headerValue</span><span class="sxs-lookup"><span data-stu-id="7b807-114">headerValue</span></span>|<span data-ttu-id="7b807-115">String</span><span class="sxs-lookup"><span data-stu-id="7b807-115">String</span></span>|<span data-ttu-id="7b807-116">此终结点报告的用户代理标头值。</span><span class="sxs-lookup"><span data-stu-id="7b807-116">User-agent header value reported by this endpoint.</span></span>|
|<span data-ttu-id="7b807-117">platform</span><span class="sxs-lookup"><span data-stu-id="7b807-117">platform</span></span>|<span data-ttu-id="7b807-118">callRecords。 clientPlatform</span><span class="sxs-lookup"><span data-stu-id="7b807-118">microsoft.graph.callRecords.clientPlatform</span></span>|<span data-ttu-id="7b807-119">标识此终结点使用的平台。</span><span class="sxs-lookup"><span data-stu-id="7b807-119">Identifies the platform used by this endpoint.</span></span> <span data-ttu-id="7b807-120">可取值为：`unknown`、`windows`、`macOS`、`iOS`、`android`、`web`、`ipPhone`、`roomSystem`、`surfaceHub`、`holoLens`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="7b807-120">Possible values are: `unknown`, `windows`, `macOS`, `iOS`, `android`, `web`, `ipPhone`, `roomSystem`, `surfaceHub`, `holoLens`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="7b807-121">productFamily</span><span class="sxs-lookup"><span data-stu-id="7b807-121">productFamily</span></span>|<span data-ttu-id="7b807-122">callRecords。 productFamily</span><span class="sxs-lookup"><span data-stu-id="7b807-122">microsoft.graph.callRecords.productFamily</span></span>|<span data-ttu-id="7b807-123">标识此终结点使用的应用程序软件系列。</span><span class="sxs-lookup"><span data-stu-id="7b807-123">Identifies the family of application software used by this endpoint.</span></span> <span data-ttu-id="7b807-124">可取值为：`unknown`、`teams`、`skypeForBusiness`、`lync`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="7b807-124">Possible values are: `unknown`, `teams`, `skypeForBusiness`, `lync`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7b807-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7b807-125">JSON representation</span></span>

<span data-ttu-id="7b807-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7b807-126">The following is a JSON representation of the resource.</span></span>

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