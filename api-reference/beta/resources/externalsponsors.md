---
title: externalSponsors 复杂类型
description: 标识将允许作为审批者的租户中另一个用户的关系。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4db88b74ae0acb2e817bd575f4e990774533064e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013692"
---
# <a name="externalsponsors-complex-type"></a><span data-ttu-id="2cdcd-103">externalSponsors 复杂类型</span><span class="sxs-lookup"><span data-stu-id="2cdcd-103">externalSponsors complex type</span></span>

<span data-ttu-id="2cdcd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2cdcd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2cdcd-105">在 [访问包分配策略](accesspackageassignmentpolicy.md)的审批阶段中使用。</span><span class="sxs-lookup"><span data-stu-id="2cdcd-105">Used in the approval stage of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="2cdcd-106">它是 [userSet](userset.md)的一个子类型，其中 `@odata.type` 值 `#microsoft.graph.externalSponsors` 表示请求用户的已连接组织的外部发起人是审批者。</span><span class="sxs-lookup"><span data-stu-id="2cdcd-106">It is a subtype of [userSet](userset.md), in which the `@odata.type` value `#microsoft.graph.externalSponsors` indicates that a requesting user's connected organization external sponsors are to be the approver.</span></span> <span data-ttu-id="2cdcd-107">此审批者仅适用于来自属于已连接组织的用户的请求。</span><span class="sxs-lookup"><span data-stu-id="2cdcd-107">This approver is only applicable to requests from users who are part of a connected organization.</span></span>  <span data-ttu-id="2cdcd-108">在使用 externalSponsors 创建访问包分配策略审批阶段时，还应包括另一个审批者（如单个用户或组成员），以防所连接的组织没有外部发起人。</span><span class="sxs-lookup"><span data-stu-id="2cdcd-108">When creating an access package assignment policy approval stage with externalSponsors, also include another approver, such as a single user or group member, in case the connected organization does not have an external sponsor.</span></span>

## <a name="properties"></a><span data-ttu-id="2cdcd-109">属性</span><span class="sxs-lookup"><span data-stu-id="2cdcd-109">Properties</span></span>

| <span data-ttu-id="2cdcd-110">属性</span><span class="sxs-lookup"><span data-stu-id="2cdcd-110">Property</span></span>                     | <span data-ttu-id="2cdcd-111">类型</span><span class="sxs-lookup"><span data-stu-id="2cdcd-111">Type</span></span>                      | <span data-ttu-id="2cdcd-112">说明</span><span class="sxs-lookup"><span data-stu-id="2cdcd-112">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="2cdcd-113">isBackup</span><span class="sxs-lookup"><span data-stu-id="2cdcd-113">isBackup</span></span> | <span data-ttu-id="2cdcd-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="2cdcd-114">Boolean</span></span> | <span data-ttu-id="2cdcd-115">指示发起人是否为备份回退审批者。</span><span class="sxs-lookup"><span data-stu-id="2cdcd-115">Indicates whether the sponsor is a backup fallback approver.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2cdcd-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2cdcd-116">JSON representation</span></span>

<span data-ttu-id="2cdcd-117">以下是此类型的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2cdcd-117">The following is a JSON representation of this type.</span></span>

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


