---
title: serviceInformation 资源类型
description: serviceInformation 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: ba13967a2b4373c1a3599baf2fcc856967fbb00c
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939829"
---
# <a name="serviceinformation-resource-type"></a><span data-ttu-id="cb4ff-103">serviceInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="cb4ff-103">serviceInformation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb4ff-104">表示有关用户已从其帐户中选择要引用的云服务的基本描述性数据。</span><span class="sxs-lookup"><span data-stu-id="cb4ff-104">Represents basic descriptive data about cloud services that a user has chosen to refer to from their account.</span></span>

## <a name="properties"></a><span data-ttu-id="cb4ff-105">属性</span><span class="sxs-lookup"><span data-stu-id="cb4ff-105">Properties</span></span>

| <span data-ttu-id="cb4ff-106">属性</span><span class="sxs-lookup"><span data-stu-id="cb4ff-106">Property</span></span>     | <span data-ttu-id="cb4ff-107">类型</span><span class="sxs-lookup"><span data-stu-id="cb4ff-107">Type</span></span>        | <span data-ttu-id="cb4ff-108">描述</span><span class="sxs-lookup"><span data-stu-id="cb4ff-108">Description</span></span>                                            |
|:-------------|:------------|:-------------------------------------------------------|
|<span data-ttu-id="cb4ff-109">name</span><span class="sxs-lookup"><span data-stu-id="cb4ff-109">name</span></span>          | <span data-ttu-id="cb4ff-110">字符串</span><span class="sxs-lookup"><span data-stu-id="cb4ff-110">String</span></span>      | <span data-ttu-id="cb4ff-111">云服务的名称（例如，Twitter、Instagram）。</span><span class="sxs-lookup"><span data-stu-id="cb4ff-111">The name of the cloud service (for example, Twitter, Instagram).</span></span> |
|<span data-ttu-id="cb4ff-112">webUrl</span><span class="sxs-lookup"><span data-stu-id="cb4ff-112">webUrl</span></span>        | <span data-ttu-id="cb4ff-113">String</span><span class="sxs-lookup"><span data-stu-id="cb4ff-113">String</span></span>      | <span data-ttu-id="cb4ff-114">包含要引用的服务的 URL。</span><span class="sxs-lookup"><span data-stu-id="cb4ff-114">Contains the URL for the service being referenced.</span></span>     |

## <a name="json-representation"></a><span data-ttu-id="cb4ff-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cb4ff-115">JSON representation</span></span>

<span data-ttu-id="cb4ff-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cb4ff-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.serviceInformation",
  "baseType": null
}-->

```json
{
  "name": "String",
  "webUrl": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "serviceInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
