---
title: internalSponsors 复杂类型
description: 标识将允许作为审批者的租户中另一个用户的关系。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c7ec468638de5e9a49cbf2f664eb7d05e3bef5b1
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331392"
---
# <a name="internalsponsors-complex-type"></a><span data-ttu-id="179a0-103">internalSponsors 复杂类型</span><span class="sxs-lookup"><span data-stu-id="179a0-103">internalSponsors complex type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="179a0-104">在[访问包分配策略](accesspackageassignmentpolicy.md)的审批阶段中使用。</span><span class="sxs-lookup"><span data-stu-id="179a0-104">Used in the approval stage of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="179a0-105">它是[userSet](userset.md)的一个子类型，其中`@odata.type`值`#microsoft.graph.internalSponsors`表示请求用户的连接的组织内部发起人将成为审批者。</span><span class="sxs-lookup"><span data-stu-id="179a0-105">It is a subtype of [userSet](userset.md), in which the `@odata.type` value `#microsoft.graph.internalSponsors` indicates that a requesting user's connected organization internal sponsors are to be the approver.</span></span> <span data-ttu-id="179a0-106">此审批者仅适用于来自属于已连接组织的用户的请求。</span><span class="sxs-lookup"><span data-stu-id="179a0-106">This approver is only applicable to requests from users who are part of a connected organization.</span></span>  <span data-ttu-id="179a0-107">在使用 internalSponsors 创建访问包分配策略审批阶段时，还应包括另一个审批者（如单个用户或组成员），以防所连接的组织没有内部赞助者。</span><span class="sxs-lookup"><span data-stu-id="179a0-107">When creating an access package assignment policy approval stage with internalSponsors, also include another approver, such as a single user or group member, in case the connected organization does not have an internal sponsor.</span></span>

## <a name="properties"></a><span data-ttu-id="179a0-108">属性</span><span class="sxs-lookup"><span data-stu-id="179a0-108">Properties</span></span>

| <span data-ttu-id="179a0-109">属性</span><span class="sxs-lookup"><span data-stu-id="179a0-109">Property</span></span>                     | <span data-ttu-id="179a0-110">类型</span><span class="sxs-lookup"><span data-stu-id="179a0-110">Type</span></span>                      | <span data-ttu-id="179a0-111">说明</span><span class="sxs-lookup"><span data-stu-id="179a0-111">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="179a0-112">isBackup</span><span class="sxs-lookup"><span data-stu-id="179a0-112">isBackup</span></span> | <span data-ttu-id="179a0-113">布尔值</span><span class="sxs-lookup"><span data-stu-id="179a0-113">Boolean</span></span> | <span data-ttu-id="179a0-114">指示发起人是否为备份回退审批者。</span><span class="sxs-lookup"><span data-stu-id="179a0-114">Indicates whether the sponsor is a backup fallback approver.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="179a0-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="179a0-115">JSON representation</span></span>

<span data-ttu-id="179a0-116">以下是类型的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="179a0-116">The following is a JSON representation of the type.</span></span>

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
