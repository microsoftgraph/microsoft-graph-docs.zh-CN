---
title: relatedPerson 资源类型
description: relatedPerson 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 6be6300bc901305fb87b04e2482f145b9187f9fb
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939234"
---
# <a name="relatedperson-resource-type"></a><span data-ttu-id="3a607-103">relatedPerson 资源类型</span><span class="sxs-lookup"><span data-stu-id="3a607-103">relatedPerson resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a607-104">表示有关与用户的[配置文件](profile.md)中给定实体内的信息相关的人员的信息。</span><span class="sxs-lookup"><span data-stu-id="3a607-104">Represents information about people related to information within a given entity in a [profile](profile.md) for a user.</span></span>

## <a name="properties"></a><span data-ttu-id="3a607-105">属性</span><span class="sxs-lookup"><span data-stu-id="3a607-105">Properties</span></span>

| <span data-ttu-id="3a607-106">属性</span><span class="sxs-lookup"><span data-stu-id="3a607-106">Property</span></span>        | <span data-ttu-id="3a607-107">类型</span><span class="sxs-lookup"><span data-stu-id="3a607-107">Type</span></span>        | <span data-ttu-id="3a607-108">说明</span><span class="sxs-lookup"><span data-stu-id="3a607-108">Description</span></span>                                               |
|:----------------|:------------|:----------------------------------------------------------|
|<span data-ttu-id="3a607-109">displayName</span><span class="sxs-lookup"><span data-stu-id="3a607-109">displayName</span></span>      |<span data-ttu-id="3a607-110">String</span><span class="sxs-lookup"><span data-stu-id="3a607-110">String</span></span>       | <span data-ttu-id="3a607-111">人员的姓名。</span><span class="sxs-lookup"><span data-stu-id="3a607-111">Name of the person.</span></span>                                        |
|<span data-ttu-id="3a607-112">关系</span><span class="sxs-lookup"><span data-stu-id="3a607-112">relationship</span></span>     |<span data-ttu-id="3a607-113">字符串</span><span class="sxs-lookup"><span data-stu-id="3a607-113">String</span></span>       | <span data-ttu-id="3a607-114">可取值为：`manager`、`colleague`、`directReport`、`dotLineReport`、`assistant`、`dotLineManager`、`alternateContact`、`friend`、`spouse`、`sibling`、`child`、`parent`、`sponsor`、`emergencyContact`、`other`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="3a607-114">Possible values are: `manager`, `colleague`, `directReport`, `dotLineReport`, `assistant`, `dotLineManager`, `alternateContact`, `friend`, `spouse`, `sibling`, `child`, `parent`, `sponsor`, `emergencyContact`, `other`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="3a607-115">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3a607-115">userPrincipalName</span></span>|<span data-ttu-id="3a607-116">字符串</span><span class="sxs-lookup"><span data-stu-id="3a607-116">String</span></span>       | <span data-ttu-id="3a607-117">组织内的人员的电子邮件地址或引用。</span><span class="sxs-lookup"><span data-stu-id="3a607-117">Email address or reference to person within organization.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3a607-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3a607-118">JSON representation</span></span>

<span data-ttu-id="3a607-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3a607-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.relatedPerson",
  "baseType": null
}-->

```json
{
  "displayName": "String",
  "relationship": "String",
  "userPrincipalName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "relatedPerson resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
