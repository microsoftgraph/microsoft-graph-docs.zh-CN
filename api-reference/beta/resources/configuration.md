---
title: 配置资源类型
description: 指定允许管理 externalConnection 和为 externalConnection 中的内容编制索引的附加应用程序 ID。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 8a82c5e9e4cbd915d5a7e11b9e162bc510628ecf
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366775"
---
# <a name="configuration-resource-type"></a><span data-ttu-id="4365d-103">配置资源类型</span><span class="sxs-lookup"><span data-stu-id="4365d-103">configuration resource type</span></span>

<span data-ttu-id="4365d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4365d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4365d-105">指定允许管理 externalConnection 和为 externalConnection 中的内容编制索引的附加[应用程序 ID。](../resources/externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="4365d-105">Specifies additional application IDs that are allowed to manage the externalConnection and to index content in a [externalConnection](../resources/externalconnection.md).</span></span>

## <a name="properties"></a><span data-ttu-id="4365d-106">属性</span><span class="sxs-lookup"><span data-stu-id="4365d-106">Properties</span></span>

| <span data-ttu-id="4365d-107">属性</span><span class="sxs-lookup"><span data-stu-id="4365d-107">Property</span></span>       | <span data-ttu-id="4365d-108">类型</span><span class="sxs-lookup"><span data-stu-id="4365d-108">Type</span></span>              | <span data-ttu-id="4365d-109">说明</span><span class="sxs-lookup"><span data-stu-id="4365d-109">Description</span></span> |
|:---------------|:------------------|:------------|
| <span data-ttu-id="4365d-110">authorizedApps</span><span class="sxs-lookup"><span data-stu-id="4365d-110">authorizedApps</span></span> | <span data-ttu-id="4365d-111">String collection</span><span class="sxs-lookup"><span data-stu-id="4365d-111">String collection</span></span> | <span data-ttu-id="4365d-112">允许管理 externalConnection 和为 externalConnection 中的内容编制索引的已注册 Azure Active Directory 应用程序的应用程序 ID 的集合。</span><span class="sxs-lookup"><span data-stu-id="4365d-112">A collection of application IDs for registered Azure Active Directory apps that are allowed to manage the externalConnection and to index content in the externalConnection.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4365d-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4365d-113">JSON representation</span></span>

<span data-ttu-id="4365d-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4365d-114">The following is a JSON representation of the resource.</span></span>

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


