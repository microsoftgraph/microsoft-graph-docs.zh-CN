---
title: externalSponsors 复杂类型
description: 标识与租户中将允许其成为审批者的另一个用户的关系。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 361ac6ff85d5b4462b39aa10e4f978ce7d486e40
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761868"
---
# <a name="externalsponsors-complex-type"></a><span data-ttu-id="100d4-103">externalSponsors 复杂类型</span><span class="sxs-lookup"><span data-stu-id="100d4-103">externalSponsors complex type</span></span>

<span data-ttu-id="100d4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="100d4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="100d4-105">在访问包分配策略的 [审批阶段使用](accesspackageassignmentpolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="100d4-105">Used in the approval stage of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="100d4-106">它是 [userSet](userset.md)的子类型，其中值指示请求用户的已连接组织 `@odata.type` 外部发起 `#microsoft.graph.externalSponsors` 人将是审批者。</span><span class="sxs-lookup"><span data-stu-id="100d4-106">It is a subtype of [userSet](userset.md), in which the `@odata.type` value `#microsoft.graph.externalSponsors` indicates that a requesting user's connected organization external sponsors are to be the approver.</span></span> <span data-ttu-id="100d4-107">此审批者仅适用于来自已连接组织一部分的用户的请求。</span><span class="sxs-lookup"><span data-stu-id="100d4-107">This approver is only applicable to requests from users who are part of a connected organization.</span></span>  <span data-ttu-id="100d4-108">使用 externalSponsors 创建访问包分配策略审批阶段时，还应包括另一个审批者，如单个用户或组的成员，以防连接的组织没有外部发起人。</span><span class="sxs-lookup"><span data-stu-id="100d4-108">When creating an access package assignment policy approval stage with externalSponsors, also include another approver, such as a single user or group member, in case the connected organization does not have an external sponsor.</span></span>

## <a name="properties"></a><span data-ttu-id="100d4-109">属性</span><span class="sxs-lookup"><span data-stu-id="100d4-109">Properties</span></span>

| <span data-ttu-id="100d4-110">属性</span><span class="sxs-lookup"><span data-stu-id="100d4-110">Property</span></span>                     | <span data-ttu-id="100d4-111">类型</span><span class="sxs-lookup"><span data-stu-id="100d4-111">Type</span></span>                      | <span data-ttu-id="100d4-112">说明</span><span class="sxs-lookup"><span data-stu-id="100d4-112">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="100d4-113">isBackup</span><span class="sxs-lookup"><span data-stu-id="100d4-113">isBackup</span></span> | <span data-ttu-id="100d4-114">布尔</span><span class="sxs-lookup"><span data-stu-id="100d4-114">Boolean</span></span> | <span data-ttu-id="100d4-115">指示发起人是否是备份回退审批者。</span><span class="sxs-lookup"><span data-stu-id="100d4-115">Indicates whether the sponsor is a backup fallback approver.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="100d4-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="100d4-116">JSON representation</span></span>

<span data-ttu-id="100d4-117">以下是此类型的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="100d4-117">The following is a JSON representation of this type.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalSponsors",
  "baseType": "microsoft.graph.userSet"
}-->

```json
{
  "@odata.type": "#microsoft.graph.externalSponsors",
  "isBackup": false
}
```



<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "externalSponsor complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


