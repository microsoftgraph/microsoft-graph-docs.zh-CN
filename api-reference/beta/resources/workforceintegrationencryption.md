---
title: workforceIntegrationEncryption 资源类型
description: 为劳动力集成定义协议和密码的加密实体。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 15feb2097a3a7bf36092070cc2af4841d2aa3839
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48019392"
---
# <a name="workforceintegrationencryption-resource-type"></a><span data-ttu-id="7d260-103">workforceIntegrationEncryption 资源类型</span><span class="sxs-lookup"><span data-stu-id="7d260-103">workforceIntegrationEncryption resource type</span></span>

<span data-ttu-id="7d260-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d260-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d260-105">为 [workforceintegration](../resources/workforceintegration.md)定义协议和密码的加密实体。</span><span class="sxs-lookup"><span data-stu-id="7d260-105">An encryption entity defining the protocol and secret for a [workforceintegration](../resources/workforceintegration.md).</span></span>

## <a name="properties"></a><span data-ttu-id="7d260-106">属性</span><span class="sxs-lookup"><span data-stu-id="7d260-106">Properties</span></span>

| <span data-ttu-id="7d260-107">属性</span><span class="sxs-lookup"><span data-stu-id="7d260-107">Property</span></span>     | <span data-ttu-id="7d260-108">类型</span><span class="sxs-lookup"><span data-stu-id="7d260-108">Type</span></span>        | <span data-ttu-id="7d260-109">说明</span><span class="sxs-lookup"><span data-stu-id="7d260-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7d260-110">协议</span><span class="sxs-lookup"><span data-stu-id="7d260-110">protocol</span></span>|<span data-ttu-id="7d260-111">String</span><span class="sxs-lookup"><span data-stu-id="7d260-111">String</span></span>| <span data-ttu-id="7d260-112">可取值为：`sharedSecret`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="7d260-112">Possible values are: `sharedSecret`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="7d260-113">私钥</span><span class="sxs-lookup"><span data-stu-id="7d260-113">secret</span></span>|<span data-ttu-id="7d260-114">String</span><span class="sxs-lookup"><span data-stu-id="7d260-114">String</span></span>|<span data-ttu-id="7d260-115">加密共享密钥。</span><span class="sxs-lookup"><span data-stu-id="7d260-115">Encryption shared secret.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7d260-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7d260-116">JSON representation</span></span>

<span data-ttu-id="7d260-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7d260-117">The following is a JSON representation of the resource.</span></span>

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


