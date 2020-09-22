---
title: internalSponsors 复杂类型
description: 标识将允许作为审批者的租户中另一个用户的关系。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 56ae53e1b55be0a56a4c021449b8c5f4eb1a7c05
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058381"
---
# <a name="internalsponsors-complex-type"></a><span data-ttu-id="33758-103">internalSponsors 复杂类型</span><span class="sxs-lookup"><span data-stu-id="33758-103">internalSponsors complex type</span></span>

<span data-ttu-id="33758-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33758-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33758-105">在 [访问包分配策略](accesspackageassignmentpolicy.md)的审批阶段中使用。</span><span class="sxs-lookup"><span data-stu-id="33758-105">Used in the approval stage of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="33758-106">它是 [userSet](userset.md)的一个子类型，其中 `@odata.type` 值 `#microsoft.graph.internalSponsors` 表示请求用户的连接的组织内部发起人将成为审批者。</span><span class="sxs-lookup"><span data-stu-id="33758-106">It is a subtype of [userSet](userset.md), in which the `@odata.type` value `#microsoft.graph.internalSponsors` indicates that a requesting user's connected organization internal sponsors are to be the approver.</span></span> <span data-ttu-id="33758-107">此审批者仅适用于来自属于已连接组织的用户的请求。</span><span class="sxs-lookup"><span data-stu-id="33758-107">This approver is only applicable to requests from users who are part of a connected organization.</span></span>  <span data-ttu-id="33758-108">在使用 internalSponsors 创建访问包分配策略审批阶段时，还应包括另一个审批者（如单个用户或组成员），以防所连接的组织没有内部赞助者。</span><span class="sxs-lookup"><span data-stu-id="33758-108">When creating an access package assignment policy approval stage with internalSponsors, also include another approver, such as a single user or group member, in case the connected organization does not have an internal sponsor.</span></span>

## <a name="properties"></a><span data-ttu-id="33758-109">属性</span><span class="sxs-lookup"><span data-stu-id="33758-109">Properties</span></span>

| <span data-ttu-id="33758-110">属性</span><span class="sxs-lookup"><span data-stu-id="33758-110">Property</span></span>                     | <span data-ttu-id="33758-111">类型</span><span class="sxs-lookup"><span data-stu-id="33758-111">Type</span></span>                      | <span data-ttu-id="33758-112">说明</span><span class="sxs-lookup"><span data-stu-id="33758-112">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="33758-113">isBackup</span><span class="sxs-lookup"><span data-stu-id="33758-113">isBackup</span></span> | <span data-ttu-id="33758-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="33758-114">Boolean</span></span> | <span data-ttu-id="33758-115">指示发起人是否为备份回退审批者。</span><span class="sxs-lookup"><span data-stu-id="33758-115">Indicates whether the sponsor is a backup fallback approver.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="33758-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="33758-116">JSON representation</span></span>

<span data-ttu-id="33758-117">以下是类型的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="33758-117">The following is a JSON representation of the type.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.internalSponsors",
  "baseType": "microsoft.graph.userSet"
}-->

```json
{
  "@odata.type": "#microsoft.graph.internalSponsors",
  "isBackup": false
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "internalSponsor complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


