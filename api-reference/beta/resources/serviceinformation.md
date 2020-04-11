---
title: serviceInformation 资源类型
description: serviceInformation 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: daca733578e5415fc777bc01a8ef1272cfdcc681
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2020
ms.locfileid: "43228878"
---
# <a name="serviceinformation-resource-type"></a><span data-ttu-id="e395a-103">serviceInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="e395a-103">serviceInformation resource type</span></span>

<span data-ttu-id="e395a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e395a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e395a-105">表示有关用户已从其帐户中选择要引用的云服务的基本描述性数据。</span><span class="sxs-lookup"><span data-stu-id="e395a-105">Represents basic descriptive data about cloud services that a user has chosen to refer to from their account.</span></span>

## <a name="properties"></a><span data-ttu-id="e395a-106">属性</span><span class="sxs-lookup"><span data-stu-id="e395a-106">Properties</span></span>

| <span data-ttu-id="e395a-107">属性</span><span class="sxs-lookup"><span data-stu-id="e395a-107">Property</span></span>     | <span data-ttu-id="e395a-108">类型</span><span class="sxs-lookup"><span data-stu-id="e395a-108">Type</span></span>        | <span data-ttu-id="e395a-109">说明</span><span class="sxs-lookup"><span data-stu-id="e395a-109">Description</span></span>                                                      |
|:-------------|:------------|:-----------------------------------------------------------------|
|<span data-ttu-id="e395a-110">name</span><span class="sxs-lookup"><span data-stu-id="e395a-110">name</span></span>          | <span data-ttu-id="e395a-111">字符串</span><span class="sxs-lookup"><span data-stu-id="e395a-111">String</span></span>      | <span data-ttu-id="e395a-112">云服务的名称（例如，Twitter、Instagram）。</span><span class="sxs-lookup"><span data-stu-id="e395a-112">The name of the cloud service (for example, Twitter, Instagram).</span></span> |
|<span data-ttu-id="e395a-113">WebUrl</span><span class="sxs-lookup"><span data-stu-id="e395a-113">webUrl</span></span>        | <span data-ttu-id="e395a-114">String</span><span class="sxs-lookup"><span data-stu-id="e395a-114">String</span></span>      | <span data-ttu-id="e395a-115">包含要引用的服务的 URL。</span><span class="sxs-lookup"><span data-stu-id="e395a-115">Contains the URL for the service being referenced.</span></span>               |

## <a name="json-representation"></a><span data-ttu-id="e395a-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e395a-116">JSON representation</span></span>

<span data-ttu-id="e395a-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e395a-117">The following is a JSON representation of the resource.</span></span>

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
