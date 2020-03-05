---
title: 配置资源类型
description: 指定允许管理 externalConnection 和索引 externalConnection 中的内容的其他应用程序 Id。
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: be4fa7bd8f4b44842bd6dbc9876d0dd19fe466fd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507497"
---
# <a name="configuration-resource-type"></a><span data-ttu-id="576cd-103">配置资源类型</span><span class="sxs-lookup"><span data-stu-id="576cd-103">configuration resource type</span></span>

<span data-ttu-id="576cd-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="576cd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="576cd-105">指定允许管理 externalConnection 和索引[externalConnection](../resources/externalconnection.md)中的内容的其他应用程序 id。</span><span class="sxs-lookup"><span data-stu-id="576cd-105">Specifies additional application IDs that are allowed to manage the externalConnection and to index content in a [externalConnection](../resources/externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="576cd-106">属性</span><span class="sxs-lookup"><span data-stu-id="576cd-106">Properties</span></span>

| <span data-ttu-id="576cd-107">属性</span><span class="sxs-lookup"><span data-stu-id="576cd-107">Property</span></span>       | <span data-ttu-id="576cd-108">类型</span><span class="sxs-lookup"><span data-stu-id="576cd-108">Type</span></span>              | <span data-ttu-id="576cd-109">说明</span><span class="sxs-lookup"><span data-stu-id="576cd-109">Description</span></span> |
|:---------------|:------------------|:------------|
| <span data-ttu-id="576cd-110">authorizedApps</span><span class="sxs-lookup"><span data-stu-id="576cd-110">authorizedApps</span></span> | <span data-ttu-id="576cd-111">String 集合</span><span class="sxs-lookup"><span data-stu-id="576cd-111">String collection</span></span> | <span data-ttu-id="576cd-112">允许管理 externalConnection 和索引 externalConnection 中的内容的注册的 Azure Active Directory 应用程序的应用程序 Id 的集合。</span><span class="sxs-lookup"><span data-stu-id="576cd-112">A collection of application IDs for registered Azure Active Directory apps that are allowed to manage the externalConnection and to index content in the externalConnection.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="576cd-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="576cd-113">JSON representation</span></span>

<span data-ttu-id="576cd-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="576cd-114">The following is a JSON representation of the resource.</span></span>

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
