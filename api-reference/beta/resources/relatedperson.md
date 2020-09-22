---
title: relatedPerson 资源类型
description: relatedPerson 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 88d7283d1eac1f3b7bcc7d947fa1961494a58041
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033571"
---
# <a name="relatedperson-resource-type"></a><span data-ttu-id="22852-103">relatedPerson 资源类型</span><span class="sxs-lookup"><span data-stu-id="22852-103">relatedPerson resource type</span></span>

<span data-ttu-id="22852-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22852-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22852-105">表示有关与用户的 [配置文件](profile.md) 中给定实体内的信息相关的人员的信息。</span><span class="sxs-lookup"><span data-stu-id="22852-105">Represents information about people related to information within a given entity in a [profile](profile.md) for a user.</span></span>

## <a name="properties"></a><span data-ttu-id="22852-106">属性</span><span class="sxs-lookup"><span data-stu-id="22852-106">Properties</span></span>

| <span data-ttu-id="22852-107">属性</span><span class="sxs-lookup"><span data-stu-id="22852-107">Property</span></span>        | <span data-ttu-id="22852-108">类型</span><span class="sxs-lookup"><span data-stu-id="22852-108">Type</span></span>        | <span data-ttu-id="22852-109">说明</span><span class="sxs-lookup"><span data-stu-id="22852-109">Description</span></span>                                                                                                                                                                                                                                     |
|:----------------|:------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="22852-110">displayName</span><span class="sxs-lookup"><span data-stu-id="22852-110">displayName</span></span>      |<span data-ttu-id="22852-111">String</span><span class="sxs-lookup"><span data-stu-id="22852-111">String</span></span>       | <span data-ttu-id="22852-112">人员的姓名。</span><span class="sxs-lookup"><span data-stu-id="22852-112">Name of the person.</span></span>                                                                                                                                                                                                                             |
|<span data-ttu-id="22852-113">关系</span><span class="sxs-lookup"><span data-stu-id="22852-113">relationship</span></span>     |<span data-ttu-id="22852-114">String</span><span class="sxs-lookup"><span data-stu-id="22852-114">String</span></span>       | <span data-ttu-id="22852-115">可取值为：`manager`、`colleague`、`directReport`、`dotLineReport`、`assistant`、`dotLineManager`、`alternateContact`、`friend`、`spouse`、`sibling`、`child`、`parent`、`sponsor`、`emergencyContact`、`other`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="22852-115">Possible values are: `manager`, `colleague`, `directReport`, `dotLineReport`, `assistant`, `dotLineManager`, `alternateContact`, `friend`, `spouse`, `sibling`, `child`, `parent`, `sponsor`, `emergencyContact`, `other`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="22852-116">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="22852-116">userPrincipalName</span></span>|<span data-ttu-id="22852-117">String</span><span class="sxs-lookup"><span data-stu-id="22852-117">String</span></span>       | <span data-ttu-id="22852-118">组织内的人员的电子邮件地址或引用。</span><span class="sxs-lookup"><span data-stu-id="22852-118">Email address or reference to person within organization.</span></span>                                                                                                                                                                                       |

## <a name="json-representation"></a><span data-ttu-id="22852-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="22852-119">JSON representation</span></span>

<span data-ttu-id="22852-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="22852-120">The following is a JSON representation of the resource.</span></span>

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


