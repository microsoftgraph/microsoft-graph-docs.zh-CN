---
title: workforceIntegrationEncryption 资源类型
description: 为劳动力集成定义协议和密码的加密实体。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: fb974b80b03edc36a0f974633c8f95ca384182e6
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154148"
---
# <a name="workforceintegrationencryption-resource-type"></a><span data-ttu-id="0ee69-103">workforceIntegrationEncryption 资源类型</span><span class="sxs-lookup"><span data-stu-id="0ee69-103">workforceIntegrationEncryption resource type</span></span>

<span data-ttu-id="0ee69-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ee69-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0ee69-105">为[workforceintegration](../resources/workforceintegration.md)定义协议和密码的加密实体。</span><span class="sxs-lookup"><span data-stu-id="0ee69-105">An encryption entity defining the protocol and secret for a [workforceintegration](../resources/workforceintegration.md).</span></span>

## <a name="properties"></a><span data-ttu-id="0ee69-106">属性</span><span class="sxs-lookup"><span data-stu-id="0ee69-106">Properties</span></span>

| <span data-ttu-id="0ee69-107">属性</span><span class="sxs-lookup"><span data-stu-id="0ee69-107">Property</span></span>     | <span data-ttu-id="0ee69-108">类型</span><span class="sxs-lookup"><span data-stu-id="0ee69-108">Type</span></span>        | <span data-ttu-id="0ee69-109">Description</span><span class="sxs-lookup"><span data-stu-id="0ee69-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0ee69-110">协议</span><span class="sxs-lookup"><span data-stu-id="0ee69-110">protocol</span></span>|<span data-ttu-id="0ee69-111">String</span><span class="sxs-lookup"><span data-stu-id="0ee69-111">String</span></span>| <span data-ttu-id="0ee69-112">可取值为：`sharedSecret`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="0ee69-112">Possible values are: `sharedSecret`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="0ee69-113">私钥</span><span class="sxs-lookup"><span data-stu-id="0ee69-113">secret</span></span>|<span data-ttu-id="0ee69-114">字符串</span><span class="sxs-lookup"><span data-stu-id="0ee69-114">String</span></span>|<span data-ttu-id="0ee69-115">加密共享密钥。</span><span class="sxs-lookup"><span data-stu-id="0ee69-115">Encryption shared secret.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0ee69-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0ee69-116">JSON representation</span></span>

<span data-ttu-id="0ee69-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0ee69-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workforceIntegrationEncryption",
  "baseType": null
}-->

```json
{
  "protocol": "String",
  "secret": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workforceIntegrationEncryption resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
