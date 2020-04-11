---
title: relatedPerson 资源类型
description: relatedPerson 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: c440be4ad291857fad9540cccad2e43d3a0e7121
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2020
ms.locfileid: "43227686"
---
# <a name="relatedperson-resource-type"></a><span data-ttu-id="506bc-103">relatedPerson 资源类型</span><span class="sxs-lookup"><span data-stu-id="506bc-103">relatedPerson resource type</span></span>

<span data-ttu-id="506bc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="506bc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="506bc-105">表示有关与用户的[配置文件](profile.md)中给定实体内的信息相关的人员的信息。</span><span class="sxs-lookup"><span data-stu-id="506bc-105">Represents information about people related to information within a given entity in a [profile](profile.md) for a user.</span></span>

## <a name="properties"></a><span data-ttu-id="506bc-106">属性</span><span class="sxs-lookup"><span data-stu-id="506bc-106">Properties</span></span>

| <span data-ttu-id="506bc-107">属性</span><span class="sxs-lookup"><span data-stu-id="506bc-107">Property</span></span>        | <span data-ttu-id="506bc-108">类型</span><span class="sxs-lookup"><span data-stu-id="506bc-108">Type</span></span>        | <span data-ttu-id="506bc-109">说明</span><span class="sxs-lookup"><span data-stu-id="506bc-109">Description</span></span>                                                                                                                                                                                                                                     |
|:----------------|:------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="506bc-110">displayName</span><span class="sxs-lookup"><span data-stu-id="506bc-110">displayName</span></span>      |<span data-ttu-id="506bc-111">String</span><span class="sxs-lookup"><span data-stu-id="506bc-111">String</span></span>       | <span data-ttu-id="506bc-112">人员的姓名。</span><span class="sxs-lookup"><span data-stu-id="506bc-112">Name of the person.</span></span>                                                                                                                                                                                                                             |
|<span data-ttu-id="506bc-113">关系</span><span class="sxs-lookup"><span data-stu-id="506bc-113">relationship</span></span>     |<span data-ttu-id="506bc-114">String</span><span class="sxs-lookup"><span data-stu-id="506bc-114">String</span></span>       | <span data-ttu-id="506bc-115">可取值为：`manager`、`colleague`、`directReport`、`dotLineReport`、`assistant`、`dotLineManager`、`alternateContact`、`friend`、`spouse`、`sibling`、`child`、`parent`、`sponsor`、`emergencyContact`、`other`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="506bc-115">Possible values are: `manager`, `colleague`, `directReport`, `dotLineReport`, `assistant`, `dotLineManager`, `alternateContact`, `friend`, `spouse`, `sibling`, `child`, `parent`, `sponsor`, `emergencyContact`, `other`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="506bc-116">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="506bc-116">userPrincipalName</span></span>|<span data-ttu-id="506bc-117">String</span><span class="sxs-lookup"><span data-stu-id="506bc-117">String</span></span>       | <span data-ttu-id="506bc-118">组织内的人员的电子邮件地址或引用。</span><span class="sxs-lookup"><span data-stu-id="506bc-118">Email address or reference to person within organization.</span></span>                                                                                                                                                                                       |

## <a name="json-representation"></a><span data-ttu-id="506bc-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="506bc-119">JSON representation</span></span>

<span data-ttu-id="506bc-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="506bc-120">The following is a JSON representation of the resource.</span></span>

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
