---
title: 配置资源类型
description: 指定允许管理 externalConnection 和索引 externalConnection 中的内容的其他应用程序 Id。
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c7808d014ee2ab19fda9eceb6064375cf5904d52
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/19/2019
ms.locfileid: "38704148"
---
# <a name="configuration-resource-type"></a><span data-ttu-id="f830a-103">配置资源类型</span><span class="sxs-lookup"><span data-stu-id="f830a-103">configuration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f830a-104">指定允许管理 externalConnection 和索引[externalConnection](../resources/externalconnection.md)中的内容的其他应用程序 id。</span><span class="sxs-lookup"><span data-stu-id="f830a-104">Specifies additional application IDs that are allowed to manage the externalConnection and to index content in a [externalConnection](../resources/externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="f830a-105">属性</span><span class="sxs-lookup"><span data-stu-id="f830a-105">Properties</span></span>

| <span data-ttu-id="f830a-106">属性</span><span class="sxs-lookup"><span data-stu-id="f830a-106">Property</span></span>       | <span data-ttu-id="f830a-107">类型</span><span class="sxs-lookup"><span data-stu-id="f830a-107">Type</span></span>              | <span data-ttu-id="f830a-108">说明</span><span class="sxs-lookup"><span data-stu-id="f830a-108">Description</span></span> |
|:---------------|:------------------|:------------|
| <span data-ttu-id="f830a-109">authorizedApps</span><span class="sxs-lookup"><span data-stu-id="f830a-109">authorizedApps</span></span> | <span data-ttu-id="f830a-110">String collection</span><span class="sxs-lookup"><span data-stu-id="f830a-110">String collection</span></span> | <span data-ttu-id="f830a-111">允许管理 externalConnection 和索引 externalConnection 中的内容的注册的 Azure Active Directory 应用程序的应用程序 Id 的集合。</span><span class="sxs-lookup"><span data-stu-id="f830a-111">A collection of application IDs for registered Azure Active Directory apps that are allowed to manage the externalConnection and to index content in the externalConnection.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f830a-112">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f830a-112">JSON representation</span></span>

<span data-ttu-id="f830a-113">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f830a-113">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.configuration",
  "baseType": null
}-->

```json
{
  "authorizedApps": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "configuration resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
