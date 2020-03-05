---
title: workforceIntegrationEncryption 资源类型
description: 为劳动力集成定义协议和密码的加密实体。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c2d24371a0a999069d80a9ad86afd48ac9e68d38
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519076"
---
# <a name="workforceintegrationencryption-resource-type"></a><span data-ttu-id="d2faa-103">workforceIntegrationEncryption 资源类型</span><span class="sxs-lookup"><span data-stu-id="d2faa-103">workforceIntegrationEncryption resource type</span></span>

<span data-ttu-id="d2faa-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="d2faa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2faa-105">为[workforceintegration](../resources/workforceintegration.md)定义协议和密码的加密实体。</span><span class="sxs-lookup"><span data-stu-id="d2faa-105">An encryption entity defining the protocol and secret for a [workforceintegration](../resources/workforceintegration.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d2faa-106">属性</span><span class="sxs-lookup"><span data-stu-id="d2faa-106">Properties</span></span>

| <span data-ttu-id="d2faa-107">属性</span><span class="sxs-lookup"><span data-stu-id="d2faa-107">Property</span></span>     | <span data-ttu-id="d2faa-108">类型</span><span class="sxs-lookup"><span data-stu-id="d2faa-108">Type</span></span>        | <span data-ttu-id="d2faa-109">说明</span><span class="sxs-lookup"><span data-stu-id="d2faa-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d2faa-110">协议</span><span class="sxs-lookup"><span data-stu-id="d2faa-110">protocol</span></span>|<span data-ttu-id="d2faa-111">String</span><span class="sxs-lookup"><span data-stu-id="d2faa-111">String</span></span>| <span data-ttu-id="d2faa-112">可取值为：`sharedSecret`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="d2faa-112">Possible values are: `sharedSecret`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="d2faa-113">私钥</span><span class="sxs-lookup"><span data-stu-id="d2faa-113">secret</span></span>|<span data-ttu-id="d2faa-114">String</span><span class="sxs-lookup"><span data-stu-id="d2faa-114">String</span></span>|<span data-ttu-id="d2faa-115">加密共享密钥。</span><span class="sxs-lookup"><span data-stu-id="d2faa-115">Encryption shared secret.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d2faa-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d2faa-116">JSON representation</span></span>

<span data-ttu-id="d2faa-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d2faa-117">The following is a JSON representation of the resource.</span></span>

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
