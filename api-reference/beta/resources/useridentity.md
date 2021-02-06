---
title: userIdentity 类型
description: 表示访问评审审阅者的 Azure AD 用户标识。
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 5451216ea41e6de286b5ecc0de2bed1b7ce7c8cf
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132970"
---
# <a name="useridentity-type"></a><span data-ttu-id="f735a-103">userIdentity 类型</span><span class="sxs-lookup"><span data-stu-id="f735a-103">userIdentity type</span></span>

<span data-ttu-id="f735a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f735a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f735a-105">对于 Azure AD [访问评审](accessreviews-root.md)，此类型表示访问评审的创建者或审阅者的 Azure AD 用户标识。</span><span class="sxs-lookup"><span data-stu-id="f735a-105">For the Azure AD [access reviews](accessreviews-root.md), this type represents an Azure AD user identity for a creator or reviewer of an access review.</span></span>
<span data-ttu-id="f735a-106">在 Azure AD 审核日志中，这表示启动或受审核活动影响的用户信息。</span><span class="sxs-lookup"><span data-stu-id="f735a-106">In the context of an Azure AD audit log, this represents the user information that initiated or was affected by an audit activity.</span></span>

<span data-ttu-id="f735a-107">此类型继承自 [标识，](identity.md) 并且具有一个附加属性，即用户的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="f735a-107">This type inherits from [identity](identity.md) and has one additional property, the user principal name of the user.</span></span>

## <a name="methods"></a><span data-ttu-id="f735a-108">方法</span><span class="sxs-lookup"><span data-stu-id="f735a-108">Methods</span></span>

<span data-ttu-id="f735a-109">无。</span><span class="sxs-lookup"><span data-stu-id="f735a-109">None.</span></span>  <span data-ttu-id="f735a-110">在创建 [accessReview](../api/accessreview-create.md)时，将在请求正文中包括此类型的对象。</span><span class="sxs-lookup"><span data-stu-id="f735a-110">You would include objects of this type in the body of a request when [creating an accessReview](../api/accessreview-create.md).</span></span>

## <a name="properties"></a><span data-ttu-id="f735a-111">属性</span><span class="sxs-lookup"><span data-stu-id="f735a-111">Properties</span></span>

| <span data-ttu-id="f735a-112">属性</span><span class="sxs-lookup"><span data-stu-id="f735a-112">Property</span></span> | <span data-ttu-id="f735a-113">类型</span><span class="sxs-lookup"><span data-stu-id="f735a-113">Type</span></span> | <span data-ttu-id="f735a-114">说明</span><span class="sxs-lookup"><span data-stu-id="f735a-114">Description</span></span>|
|:---------------|:--------|:----------|
| `displayName` | `String` | <span data-ttu-id="f735a-115">此身份的显示名称。</span><span class="sxs-lookup"><span data-stu-id="f735a-115">The identity's display name.</span></span> <span data-ttu-id="f735a-116">请注意，这并不总是可用或最新的。</span><span class="sxs-lookup"><span data-stu-id="f735a-116">Note that this may not always be available or up-to-date.</span></span>    |
| `id`          | `String` | <span data-ttu-id="f735a-117">身份的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f735a-117">Unique identifier for the identity.</span></span>  |
| `ipAddress`| `String`| <span data-ttu-id="f735a-118">指示仅执行活动的用户使用的 (审核日志 IP) 。</span><span class="sxs-lookup"><span data-stu-id="f735a-118">Indicates the client IP address used by user performing the activity (audit log only).</span></span>|
| `userPrincipalName`|`String` | <span data-ttu-id="f735a-119">用户的 userPrincipalName 属性。</span><span class="sxs-lookup"><span data-stu-id="f735a-119">The userPrincipalName attribute of the user.</span></span> |

## <a name="remarks"></a><span data-ttu-id="f735a-120">注解</span><span class="sxs-lookup"><span data-stu-id="f735a-120">Remarks</span></span>

<span data-ttu-id="f735a-p104">在某些情况下，角色唯一标识符可能不可用。在这种情况下，将返回身份的 **displayName** 属性，但 **id** 属性将从资源中丢失。</span><span class="sxs-lookup"><span data-stu-id="f735a-p104">In some circumstances, the unique identifier for the actor may not be available. In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.</span></span>

## <a name="relationships"></a><span data-ttu-id="f735a-123">关系</span><span class="sxs-lookup"><span data-stu-id="f735a-123">Relationships</span></span>

<span data-ttu-id="f735a-124">无。</span><span class="sxs-lookup"><span data-stu-id="f735a-124">None.</span></span>

## <a name="see-also"></a><span data-ttu-id="f735a-125">另请参阅</span><span class="sxs-lookup"><span data-stu-id="f735a-125">See also</span></span>

| <span data-ttu-id="f735a-126">方法</span><span class="sxs-lookup"><span data-stu-id="f735a-126">Method</span></span>                                                                | <span data-ttu-id="f735a-127">返回类型</span><span class="sxs-lookup"><span data-stu-id="f735a-127">Return Type</span></span>                                | <span data-ttu-id="f735a-128">说明</span><span class="sxs-lookup"><span data-stu-id="f735a-128">Description</span></span>                             |
|:----------------------------------------------------------------------|:-------------------------------------------|:----------------------------------------|
| [<span data-ttu-id="f735a-129">获取 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="f735a-129">Get accessReview reviewers</span></span>](../api/accessreview-listreviewers.md)    | <span data-ttu-id="f735a-130">[userIdentity](useridentity.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f735a-130">[userIdentity](useridentity.md) collection</span></span> | <span data-ttu-id="f735a-131">获取 accessReview 的审阅者。</span><span class="sxs-lookup"><span data-stu-id="f735a-131">Get the reviewers of an accessReview.</span></span>   |
| [<span data-ttu-id="f735a-132">添加 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="f735a-132">Add accessReview reviewer</span></span>](../api/accessreview-addreviewer.md)       | <span data-ttu-id="f735a-133">无。</span><span class="sxs-lookup"><span data-stu-id="f735a-133">None.</span></span>                                      | <span data-ttu-id="f735a-134">将审阅者添加到 accessReview。</span><span class="sxs-lookup"><span data-stu-id="f735a-134">Add a reviewer to an accessReview.</span></span>      |
| [<span data-ttu-id="f735a-135">删除 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="f735a-135">Remove accessReview reviewer</span></span>](../api/accessreview-removereviewer.md) | <span data-ttu-id="f735a-136">无。</span><span class="sxs-lookup"><span data-stu-id="f735a-136">None.</span></span>                                      | <span data-ttu-id="f735a-137">从 accessReview 中删除审阅者。</span><span class="sxs-lookup"><span data-stu-id="f735a-137">Remove a reviewer from an accessReview.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f735a-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f735a-138">JSON representation</span></span>

<span data-ttu-id="f735a-139">下面是类型的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f735a-139">Here is a JSON representation of the type.</span></span>

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


