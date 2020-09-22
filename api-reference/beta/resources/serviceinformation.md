---
title: serviceInformation 资源类型
description: serviceInformation 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 39382b0fb17795bde26b4e54f629b2e4281f81db
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070441"
---
# <a name="serviceinformation-resource-type"></a><span data-ttu-id="e361e-103">serviceInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="e361e-103">serviceInformation resource type</span></span>

<span data-ttu-id="e361e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e361e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e361e-105">表示有关用户已从其帐户中选择要引用的云服务的基本描述性数据。</span><span class="sxs-lookup"><span data-stu-id="e361e-105">Represents basic descriptive data about cloud services that a user has chosen to refer to from their account.</span></span>

## <a name="properties"></a><span data-ttu-id="e361e-106">属性</span><span class="sxs-lookup"><span data-stu-id="e361e-106">Properties</span></span>

| <span data-ttu-id="e361e-107">属性</span><span class="sxs-lookup"><span data-stu-id="e361e-107">Property</span></span>     | <span data-ttu-id="e361e-108">类型</span><span class="sxs-lookup"><span data-stu-id="e361e-108">Type</span></span>        | <span data-ttu-id="e361e-109">说明</span><span class="sxs-lookup"><span data-stu-id="e361e-109">Description</span></span>                                                      |
|:-------------|:------------|:-----------------------------------------------------------------|
|<span data-ttu-id="e361e-110">名称</span><span class="sxs-lookup"><span data-stu-id="e361e-110">name</span></span>          | <span data-ttu-id="e361e-111">String</span><span class="sxs-lookup"><span data-stu-id="e361e-111">String</span></span>      | <span data-ttu-id="e361e-112">云服务的名称 (例如，Twitter、Instagram) 。</span><span class="sxs-lookup"><span data-stu-id="e361e-112">The name of the cloud service (for example, Twitter, Instagram).</span></span> |
|<span data-ttu-id="e361e-113">webUrl</span><span class="sxs-lookup"><span data-stu-id="e361e-113">webUrl</span></span>        | <span data-ttu-id="e361e-114">String</span><span class="sxs-lookup"><span data-stu-id="e361e-114">String</span></span>      | <span data-ttu-id="e361e-115">包含要引用的服务的 URL。</span><span class="sxs-lookup"><span data-stu-id="e361e-115">Contains the URL for the service being referenced.</span></span>               |

## <a name="json-representation"></a><span data-ttu-id="e361e-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e361e-116">JSON representation</span></span>

<span data-ttu-id="e361e-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e361e-117">The following is a JSON representation of the resource.</span></span>

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


