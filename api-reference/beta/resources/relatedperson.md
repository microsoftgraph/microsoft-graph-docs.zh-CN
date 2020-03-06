---
title: relatedPerson 资源类型
description: relatedPerson 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 507746674f17a7bf8255ccddc53ea14fe2ca5a26
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521178"
---
# <a name="relatedperson-resource-type"></a><span data-ttu-id="6ca06-103">relatedPerson 资源类型</span><span class="sxs-lookup"><span data-stu-id="6ca06-103">relatedPerson resource type</span></span>

<span data-ttu-id="6ca06-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ca06-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ca06-105">表示有关与用户的[配置文件](profile.md)中给定实体内的信息相关的人员的信息。</span><span class="sxs-lookup"><span data-stu-id="6ca06-105">Represents information about people related to information within a given entity in a [profile](profile.md) for a user.</span></span>

## <a name="properties"></a><span data-ttu-id="6ca06-106">属性</span><span class="sxs-lookup"><span data-stu-id="6ca06-106">Properties</span></span>

| <span data-ttu-id="6ca06-107">属性</span><span class="sxs-lookup"><span data-stu-id="6ca06-107">Property</span></span>        | <span data-ttu-id="6ca06-108">类型</span><span class="sxs-lookup"><span data-stu-id="6ca06-108">Type</span></span>        | <span data-ttu-id="6ca06-109">说明</span><span class="sxs-lookup"><span data-stu-id="6ca06-109">Description</span></span>                                               |
|:----------------|:------------|:----------------------------------------------------------|
|<span data-ttu-id="6ca06-110">displayName</span><span class="sxs-lookup"><span data-stu-id="6ca06-110">displayName</span></span>      |<span data-ttu-id="6ca06-111">String</span><span class="sxs-lookup"><span data-stu-id="6ca06-111">String</span></span>       | <span data-ttu-id="6ca06-112">人员的姓名。</span><span class="sxs-lookup"><span data-stu-id="6ca06-112">Name of the person.</span></span>                                        |
|<span data-ttu-id="6ca06-113">关系</span><span class="sxs-lookup"><span data-stu-id="6ca06-113">relationship</span></span>     |<span data-ttu-id="6ca06-114">字符串</span><span class="sxs-lookup"><span data-stu-id="6ca06-114">String</span></span>       | <span data-ttu-id="6ca06-115">可取值为：`manager`、`colleague`、`directReport`、`dotLineReport`、`assistant`、`dotLineManager`、`alternateContact`、`friend`、`spouse`、`sibling`、`child`、`parent`、`sponsor`、`emergencyContact`、`other`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="6ca06-115">Possible values are: `manager`, `colleague`, `directReport`, `dotLineReport`, `assistant`, `dotLineManager`, `alternateContact`, `friend`, `spouse`, `sibling`, `child`, `parent`, `sponsor`, `emergencyContact`, `other`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="6ca06-116">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6ca06-116">userPrincipalName</span></span>|<span data-ttu-id="6ca06-117">字符串</span><span class="sxs-lookup"><span data-stu-id="6ca06-117">String</span></span>       | <span data-ttu-id="6ca06-118">组织内的人员的电子邮件地址或引用。</span><span class="sxs-lookup"><span data-stu-id="6ca06-118">Email address or reference to person within organization.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6ca06-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6ca06-119">JSON representation</span></span>

<span data-ttu-id="6ca06-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6ca06-120">The following is a JSON representation of the resource.</span></span>

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
