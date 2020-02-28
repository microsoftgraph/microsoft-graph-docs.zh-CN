---
title: singleUser 复杂类型
description: 标识租户中将允许作为请求者、审批者或审阅者的用户。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0d4db47278051dd79b697dc352549b95b872e4aa
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331352"
---
# <a name="singleuser-complex-type"></a><span data-ttu-id="05350-103">singleUser 复杂类型</span><span class="sxs-lookup"><span data-stu-id="05350-103">singleUser complex type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05350-104">在[访问包分配策略](accesspackageassignmentpolicy.md)的请求、审批和分配审阅设置中使用。</span><span class="sxs-lookup"><span data-stu-id="05350-104">Used in the request, approval, and assignment review settings of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="05350-105">`@odata.type`该值`#microsoft.graph.singleUser`指示此用户集标识租户中将允许作为请求者、审批者或审阅者的特定用户。</span><span class="sxs-lookup"><span data-stu-id="05350-105">The  `@odata.type` value `#microsoft.graph.singleUser` indicates that this user set identifies a specific user in the tenant who will be allowed as a requestor, approver, or reviewer.</span></span>

## <a name="properties"></a><span data-ttu-id="05350-106">属性</span><span class="sxs-lookup"><span data-stu-id="05350-106">Properties</span></span>

<span data-ttu-id="05350-107">此类型具有以下属性：</span><span class="sxs-lookup"><span data-stu-id="05350-107">This type has the following properties:</span></span>

| <span data-ttu-id="05350-108">属性</span><span class="sxs-lookup"><span data-stu-id="05350-108">Property</span></span>                     | <span data-ttu-id="05350-109">类型</span><span class="sxs-lookup"><span data-stu-id="05350-109">Type</span></span>                      | <span data-ttu-id="05350-110">说明</span><span class="sxs-lookup"><span data-stu-id="05350-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="05350-111">id</span><span class="sxs-lookup"><span data-stu-id="05350-111">id</span></span> |<span data-ttu-id="05350-112">字符串</span><span class="sxs-lookup"><span data-stu-id="05350-112">String</span></span> | <span data-ttu-id="05350-113">Azure AD 中用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="05350-113">The ID of the user in Azure AD.</span></span> |
| <span data-ttu-id="05350-114">说明</span><span class="sxs-lookup"><span data-stu-id="05350-114">description</span></span> |<span data-ttu-id="05350-115">String</span><span class="sxs-lookup"><span data-stu-id="05350-115">String</span></span> | <span data-ttu-id="05350-116">Azure AD 中的用户的名称。</span><span class="sxs-lookup"><span data-stu-id="05350-116">The name of the user in Azure AD.</span></span> <span data-ttu-id="05350-117">只读。</span><span class="sxs-lookup"><span data-stu-id="05350-117">Read only.</span></span> |
| <span data-ttu-id="05350-118">isBackup</span><span class="sxs-lookup"><span data-stu-id="05350-118">isBackup</span></span> | <span data-ttu-id="05350-119">布尔值</span><span class="sxs-lookup"><span data-stu-id="05350-119">Boolean</span></span> | <span data-ttu-id="05350-120">对于审批阶段的**singleUser** ，指示用户是否为备份回退审批者。</span><span class="sxs-lookup"><span data-stu-id="05350-120">For a **singleUser** in an approval stage, indicates whether the user is a backup fallback approver.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="05350-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="05350-121">JSON representation</span></span>

<span data-ttu-id="05350-122">以下是类型的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="05350-122">The following is a JSON representation of the type.</span></span>

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
