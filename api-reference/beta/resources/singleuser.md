---
title: singleUser 复杂类型
description: 标识租户中将允许其成为请求者、审批者或审阅者的用户。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8e1982eef048e1f68f579df7f2ebc6b0975f2f0b
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761042"
---
# <a name="singleuser-complex-type"></a><span data-ttu-id="7d9fa-103">singleUser 复杂类型</span><span class="sxs-lookup"><span data-stu-id="7d9fa-103">singleUser complex type</span></span>

<span data-ttu-id="7d9fa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d9fa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d9fa-105">在访问包分配策略的请求、审批和分配审阅 [设置中使用](accesspackageassignmentpolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="7d9fa-105">Used in the request, approval, and assignment review settings of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="7d9fa-106">该值指示此用户集标识租户中将允许其成为请求者、审批者或审阅者  `@odata.type` `#microsoft.graph.singleUser` 的特定用户。</span><span class="sxs-lookup"><span data-stu-id="7d9fa-106">The  `@odata.type` value `#microsoft.graph.singleUser` indicates that this user set identifies a specific user in the tenant who will be allowed as a requestor, approver, or reviewer.</span></span>

## <a name="properties"></a><span data-ttu-id="7d9fa-107">属性</span><span class="sxs-lookup"><span data-stu-id="7d9fa-107">Properties</span></span>

<span data-ttu-id="7d9fa-108">此类型具有以下属性：</span><span class="sxs-lookup"><span data-stu-id="7d9fa-108">This type has the following properties:</span></span>

| <span data-ttu-id="7d9fa-109">属性</span><span class="sxs-lookup"><span data-stu-id="7d9fa-109">Property</span></span>                     | <span data-ttu-id="7d9fa-110">类型</span><span class="sxs-lookup"><span data-stu-id="7d9fa-110">Type</span></span>                      | <span data-ttu-id="7d9fa-111">说明</span><span class="sxs-lookup"><span data-stu-id="7d9fa-111">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="7d9fa-112">id</span><span class="sxs-lookup"><span data-stu-id="7d9fa-112">id</span></span> |<span data-ttu-id="7d9fa-113">String</span><span class="sxs-lookup"><span data-stu-id="7d9fa-113">String</span></span> | <span data-ttu-id="7d9fa-114">Azure AD 中的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="7d9fa-114">The ID of the user in Azure AD.</span></span> |
| <span data-ttu-id="7d9fa-115">说明</span><span class="sxs-lookup"><span data-stu-id="7d9fa-115">description</span></span> |<span data-ttu-id="7d9fa-116">String</span><span class="sxs-lookup"><span data-stu-id="7d9fa-116">String</span></span> | <span data-ttu-id="7d9fa-117">Azure AD 中的用户名。</span><span class="sxs-lookup"><span data-stu-id="7d9fa-117">The name of the user in Azure AD.</span></span> <span data-ttu-id="7d9fa-118">只读。</span><span class="sxs-lookup"><span data-stu-id="7d9fa-118">Read only.</span></span> |
| <span data-ttu-id="7d9fa-119">isBackup</span><span class="sxs-lookup"><span data-stu-id="7d9fa-119">isBackup</span></span> | <span data-ttu-id="7d9fa-120">布尔</span><span class="sxs-lookup"><span data-stu-id="7d9fa-120">Boolean</span></span> | <span data-ttu-id="7d9fa-121">对于 **审批阶段中的 singleUser，** 指示用户是否是备份回退审批者。</span><span class="sxs-lookup"><span data-stu-id="7d9fa-121">For a **singleUser** in an approval stage, indicates whether the user is a backup fallback approver.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7d9fa-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7d9fa-122">JSON representation</span></span>

<span data-ttu-id="7d9fa-123">以下是类型的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7d9fa-123">The following is a JSON representation of the type.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.singleUser",
  "baseType": "microsoft.graph.userSet"
}-->

```json
{
  "isBackup": false,
  "id": "string (identifier)",
  "description": "string"
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "singleUser complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


