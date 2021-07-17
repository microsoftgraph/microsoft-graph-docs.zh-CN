---
title: 配置资源类型
description: 指定允许管理 externalConnection 和为 externalConnection 中的内容编制索引的附加应用程序 ID。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 05fbf022c11cf318281831d1b4e8572646875a06
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467647"
---
# <a name="configuration-resource-type"></a><span data-ttu-id="109e9-103">配置资源类型</span><span class="sxs-lookup"><span data-stu-id="109e9-103">configuration resource type</span></span>

<span data-ttu-id="109e9-104">命名空间：microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="109e9-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="109e9-105">指定允许管理 externalConnection 和为 externalConnection 中的内容编制索引的附加[应用程序 ID。](../resources/externalconnectors-externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="109e9-105">Specifies additional application IDs that are allowed to manage the externalConnection and to index content in a [externalConnection](../resources/externalconnectors-externalconnection.md).</span></span>

## <a name="properties"></a><span data-ttu-id="109e9-106">属性</span><span class="sxs-lookup"><span data-stu-id="109e9-106">Properties</span></span>

| <span data-ttu-id="109e9-107">属性</span><span class="sxs-lookup"><span data-stu-id="109e9-107">Property</span></span>       | <span data-ttu-id="109e9-108">类型</span><span class="sxs-lookup"><span data-stu-id="109e9-108">Type</span></span>              | <span data-ttu-id="109e9-109">说明</span><span class="sxs-lookup"><span data-stu-id="109e9-109">Description</span></span> |
|:---------------|:------------------|:------------|
| <span data-ttu-id="109e9-110">authorizedAppIds</span><span class="sxs-lookup"><span data-stu-id="109e9-110">authorizedAppIds</span></span> | <span data-ttu-id="109e9-111">字符串集合</span><span class="sxs-lookup"><span data-stu-id="109e9-111">String collection</span></span> | <span data-ttu-id="109e9-112">允许管理 externalConnection 和为 externalConnection 中的内容编制索引的已注册 Azure Active Directory 应用程序的应用程序 ID 的集合。</span><span class="sxs-lookup"><span data-stu-id="109e9-112">A collection of application IDs for registered Azure Active Directory apps that are allowed to manage the externalConnection and to index content in the externalConnection.</span></span> |

> [!NOTE]
> <span data-ttu-id="109e9-113">属性 `authorizedAppIds` 以前名为 `authorizedApps` 。</span><span class="sxs-lookup"><span data-stu-id="109e9-113">The `authorizedAppIds` property was previously named `authorizedApps`.</span></span>

## <a name="json-representation"></a><span data-ttu-id="109e9-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="109e9-114">JSON representation</span></span>

<span data-ttu-id="109e9-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="109e9-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalConnectors.configuration",
  "baseType": null
}-->

```json
{
  "authorizedAppIds": ["String"]
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
