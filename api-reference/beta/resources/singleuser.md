---
title: singleUser 复杂类型
description: 标识租户中将允许作为请求者、审批者或审阅者的用户。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fb6b665814281629836f4c5148b567de776ef2ac
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48067123"
---
# <a name="singleuser-complex-type"></a><span data-ttu-id="ef12a-103">singleUser 复杂类型</span><span class="sxs-lookup"><span data-stu-id="ef12a-103">singleUser complex type</span></span>

<span data-ttu-id="ef12a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef12a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef12a-105">在 [访问包分配策略](accesspackageassignmentpolicy.md)的请求、审批和分配审阅设置中使用。</span><span class="sxs-lookup"><span data-stu-id="ef12a-105">Used in the request, approval, and assignment review settings of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="ef12a-106">`@odata.type`该值 `#microsoft.graph.singleUser` 指示此用户集标识租户中将允许作为请求者、审批者或审阅者的特定用户。</span><span class="sxs-lookup"><span data-stu-id="ef12a-106">The  `@odata.type` value `#microsoft.graph.singleUser` indicates that this user set identifies a specific user in the tenant who will be allowed as a requestor, approver, or reviewer.</span></span>

## <a name="properties"></a><span data-ttu-id="ef12a-107">属性</span><span class="sxs-lookup"><span data-stu-id="ef12a-107">Properties</span></span>

<span data-ttu-id="ef12a-108">此类型具有以下属性：</span><span class="sxs-lookup"><span data-stu-id="ef12a-108">This type has the following properties:</span></span>

| <span data-ttu-id="ef12a-109">属性</span><span class="sxs-lookup"><span data-stu-id="ef12a-109">Property</span></span>                     | <span data-ttu-id="ef12a-110">类型</span><span class="sxs-lookup"><span data-stu-id="ef12a-110">Type</span></span>                      | <span data-ttu-id="ef12a-111">说明</span><span class="sxs-lookup"><span data-stu-id="ef12a-111">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="ef12a-112">id</span><span class="sxs-lookup"><span data-stu-id="ef12a-112">id</span></span> |<span data-ttu-id="ef12a-113">String</span><span class="sxs-lookup"><span data-stu-id="ef12a-113">String</span></span> | <span data-ttu-id="ef12a-114">Azure AD 中用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="ef12a-114">The ID of the user in Azure AD.</span></span> |
| <span data-ttu-id="ef12a-115">说明</span><span class="sxs-lookup"><span data-stu-id="ef12a-115">description</span></span> |<span data-ttu-id="ef12a-116">String</span><span class="sxs-lookup"><span data-stu-id="ef12a-116">String</span></span> | <span data-ttu-id="ef12a-117">Azure AD 中的用户的名称。</span><span class="sxs-lookup"><span data-stu-id="ef12a-117">The name of the user in Azure AD.</span></span> <span data-ttu-id="ef12a-118">只读。</span><span class="sxs-lookup"><span data-stu-id="ef12a-118">Read only.</span></span> |
| <span data-ttu-id="ef12a-119">isBackup</span><span class="sxs-lookup"><span data-stu-id="ef12a-119">isBackup</span></span> | <span data-ttu-id="ef12a-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef12a-120">Boolean</span></span> | <span data-ttu-id="ef12a-121">对于审批阶段的 **singleUser** ，指示用户是否为备份回退审批者。</span><span class="sxs-lookup"><span data-stu-id="ef12a-121">For a **singleUser** in an approval stage, indicates whether the user is a backup fallback approver.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ef12a-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ef12a-122">JSON representation</span></span>

<span data-ttu-id="ef12a-123">以下是类型的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ef12a-123">The following is a JSON representation of the type.</span></span>

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


