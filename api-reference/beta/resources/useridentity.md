---
title: userIdentity 类型
description: '对于 Azure AD 访问审核, 此类型表示访问审核的审阅者的 Azure AD 用户标识。  '
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 21342efd10f5e6f66db795a781eb3f0e333975a2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007450"
---
# <a name="useridentity-type"></a><span data-ttu-id="0981a-103">userIdentity 类型</span><span class="sxs-lookup"><span data-stu-id="0981a-103">userIdentity type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0981a-104">对于 Azure AD[访问审核](accessreviews-root.md), 此类型表示访问评审的创建者或审阅者的 Azure ad 用户标识。</span><span class="sxs-lookup"><span data-stu-id="0981a-104">For the Azure AD [access reviews](accessreviews-root.md), this type represents an Azure AD user identity for a creator or reviewer of an access review.</span></span>  
<span data-ttu-id="0981a-105">在 Azure AD 审核日志的上下文中, 这表示已启动或受审核活动影响的用户信息。</span><span class="sxs-lookup"><span data-stu-id="0981a-105">In the context of an Azure AD audit log, this represents the user information that initiated or was affected by an audit activity.</span></span>

<span data-ttu-id="0981a-106">此类型继承自[标识](identity.md), 并且具有一个附加属性 (用户的用户主体名称)。</span><span class="sxs-lookup"><span data-stu-id="0981a-106">This type inherits from [identity](identity.md) and has one additional property, the user principal name of the user.</span></span>

## <a name="methods"></a><span data-ttu-id="0981a-107">方法</span><span class="sxs-lookup"><span data-stu-id="0981a-107">Methods</span></span>

<span data-ttu-id="0981a-108">无。</span><span class="sxs-lookup"><span data-stu-id="0981a-108">None.</span></span>  <span data-ttu-id="0981a-109">[创建 accessReview](../api/accessreview-create.md)时, 您可以在请求的正文中包含此类型的对象。</span><span class="sxs-lookup"><span data-stu-id="0981a-109">You would include objects of this type in the body of a request when [creating an accessReview](../api/accessreview-create.md).</span></span>

## <a name="properties"></a><span data-ttu-id="0981a-110">属性</span><span class="sxs-lookup"><span data-stu-id="0981a-110">Properties</span></span>
| <span data-ttu-id="0981a-111">属性</span><span class="sxs-lookup"><span data-stu-id="0981a-111">Property</span></span>     | <span data-ttu-id="0981a-112">类型</span><span class="sxs-lookup"><span data-stu-id="0981a-112">Type</span></span>   |<span data-ttu-id="0981a-113">说明</span><span class="sxs-lookup"><span data-stu-id="0981a-113">Description</span></span>|
|:---------------|:--------|:----------|
| `displayName` | `String` | <span data-ttu-id="0981a-114">此身份的显示名称。</span><span class="sxs-lookup"><span data-stu-id="0981a-114">The identity's display name.</span></span> <span data-ttu-id="0981a-115">请注意, 这可能并不总是可用, 也不是最新的。</span><span class="sxs-lookup"><span data-stu-id="0981a-115">Note that this may not always be available or up-to-date.</span></span>    |
| `id`          | `String` | <span data-ttu-id="0981a-116">身份的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="0981a-116">Unique identifier for the identity.</span></span>  |
| `ipAddress`| `String`| <span data-ttu-id="0981a-117">指示执行活动的用户使用的客户端 IP 地址 (仅限审核日志)。</span><span class="sxs-lookup"><span data-stu-id="0981a-117">Indicates the client IP address used by user performing the activity (audit log only).</span></span>|
| `userPrincipalName`|`String` | <span data-ttu-id="0981a-118">用户的 userPrincipalName 属性。</span><span class="sxs-lookup"><span data-stu-id="0981a-118">The userPrincipalName attribute of the user.</span></span> |

## <a name="remarks"></a><span data-ttu-id="0981a-119">注解</span><span class="sxs-lookup"><span data-stu-id="0981a-119">Remarks</span></span>

<span data-ttu-id="0981a-p103">在某些情况下，角色唯一标识符可能不可用。在这种情况下，将返回身份的 **displayName** 属性，但 **id** 属性将从资源中丢失。</span><span class="sxs-lookup"><span data-stu-id="0981a-p103">In some circumstances, the unique identifier for the actor may not be available. In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.</span></span>

## <a name="relationships"></a><span data-ttu-id="0981a-122">关系</span><span class="sxs-lookup"><span data-stu-id="0981a-122">Relationships</span></span>

<span data-ttu-id="0981a-123">无。</span><span class="sxs-lookup"><span data-stu-id="0981a-123">None.</span></span>

## <a name="see-also"></a><span data-ttu-id="0981a-124">另请参阅</span><span class="sxs-lookup"><span data-stu-id="0981a-124">See also</span></span>

| <span data-ttu-id="0981a-125">方法</span><span class="sxs-lookup"><span data-stu-id="0981a-125">Method</span></span>           | <span data-ttu-id="0981a-126">返回类型</span><span class="sxs-lookup"><span data-stu-id="0981a-126">Return Type</span></span>    |<span data-ttu-id="0981a-127">说明</span><span class="sxs-lookup"><span data-stu-id="0981a-127">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0981a-128">获取 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="0981a-128">Get accessReview reviewers</span></span>](../api/accessreview-listreviewers.md) |       <span data-ttu-id="0981a-129">[userIdentity](useridentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="0981a-129">[userIdentity](useridentity.md) collection</span></span>| <span data-ttu-id="0981a-130">获取 accessReview 的审阅者。</span><span class="sxs-lookup"><span data-stu-id="0981a-130">Get the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="0981a-131">添加 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="0981a-131">Add accessReview reviewer</span></span>](../api/accessreview-addreviewer.md) |      <span data-ttu-id="0981a-132">无。</span><span class="sxs-lookup"><span data-stu-id="0981a-132">None.</span></span>   |   <span data-ttu-id="0981a-133">向 accessReview 添加审阅者。</span><span class="sxs-lookup"><span data-stu-id="0981a-133">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="0981a-134">删除 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="0981a-134">Remove accessReview reviewer</span></span>](../api/accessreview-removereviewer.md) | <span data-ttu-id="0981a-135">无。</span><span class="sxs-lookup"><span data-stu-id="0981a-135">None.</span></span>  |   <span data-ttu-id="0981a-136">从 accessReview 中删除审阅者。</span><span class="sxs-lookup"><span data-stu-id="0981a-136">Remove a reviewer from an accessReview.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0981a-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0981a-137">JSON representation</span></span>

<span data-ttu-id="0981a-138">下面是类型的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0981a-138">Here is a JSON representation of the type.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
"displayName", "thumbnails"
  ],
  "@odata.type": "microsoft.graph.userIdentity"
}-->

```json
{
  "displayName": "string",
  "id": "string",
  "userPrincipalName": "String",
  "ipAddress": "string"
}

```

<!--
{
  "type": "#page.annotation",
  "description": "userIdentity type",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
