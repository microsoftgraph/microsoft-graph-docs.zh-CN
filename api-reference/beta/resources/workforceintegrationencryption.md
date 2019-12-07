---
title: workforceIntegrationEncryption 资源类型
description: 为劳动力集成定义协议和密码的加密实体。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 52fb72380ce74acad429aa3da6f9ad4e60102e06
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895616"
---
# <a name="workforceintegrationencryption-resource-type"></a><span data-ttu-id="60f06-103">workforceIntegrationEncryption 资源类型</span><span class="sxs-lookup"><span data-stu-id="60f06-103">workforceIntegrationEncryption resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60f06-104">为[workforceintegration](../resources/workforceintegration.md)定义协议和密码的加密实体。</span><span class="sxs-lookup"><span data-stu-id="60f06-104">An encryption entity defining the protocol and secret for a [workforceintegration](../resources/workforceintegration.md).</span></span>

## <a name="properties"></a><span data-ttu-id="60f06-105">属性</span><span class="sxs-lookup"><span data-stu-id="60f06-105">Properties</span></span>

| <span data-ttu-id="60f06-106">属性</span><span class="sxs-lookup"><span data-stu-id="60f06-106">Property</span></span>     | <span data-ttu-id="60f06-107">类型</span><span class="sxs-lookup"><span data-stu-id="60f06-107">Type</span></span>        | <span data-ttu-id="60f06-108">说明</span><span class="sxs-lookup"><span data-stu-id="60f06-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="60f06-109">协议</span><span class="sxs-lookup"><span data-stu-id="60f06-109">protocol</span></span>|<span data-ttu-id="60f06-110">String</span><span class="sxs-lookup"><span data-stu-id="60f06-110">String</span></span>| <span data-ttu-id="60f06-111">可取值为：`sharedSecret`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="60f06-111">Possible values are: `sharedSecret`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="60f06-112">私钥</span><span class="sxs-lookup"><span data-stu-id="60f06-112">secret</span></span>|<span data-ttu-id="60f06-113">字符串</span><span class="sxs-lookup"><span data-stu-id="60f06-113">String</span></span>|<span data-ttu-id="60f06-114">加密共享密钥。</span><span class="sxs-lookup"><span data-stu-id="60f06-114">Encryption shared secret.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="60f06-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="60f06-115">JSON representation</span></span>

<span data-ttu-id="60f06-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="60f06-116">The following is a JSON representation of the resource.</span></span>

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
