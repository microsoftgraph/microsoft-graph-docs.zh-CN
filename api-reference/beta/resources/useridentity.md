---
title: userIdentity 类型
description: 表示访问评审审阅者的 Azure AD 用户标识。
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 94c0af9a5909966471594ab4c23003282f416849
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52750362"
---
# <a name="useridentity-type"></a><span data-ttu-id="097d5-103">userIdentity 类型</span><span class="sxs-lookup"><span data-stu-id="097d5-103">userIdentity type</span></span>

<span data-ttu-id="097d5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="097d5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="097d5-105">对于 Azure AD [访问评审](accessreviews-root.md)，此类型表示访问评审的创建者或审阅者的 Azure AD 用户标识。</span><span class="sxs-lookup"><span data-stu-id="097d5-105">For the Azure AD [access reviews](accessreviews-root.md), this type represents an Azure AD user identity for a creator or reviewer of an access review.</span></span>
<span data-ttu-id="097d5-106">在 Azure AD 审核日志，这表示启动或受审核活动影响的用户信息。</span><span class="sxs-lookup"><span data-stu-id="097d5-106">In the context of an Azure AD audit log, this represents the user information that initiated or was affected by an audit activity.</span></span>

<span data-ttu-id="097d5-107">此类型继承自 [标识，](identity.md) 并且具有一个附加属性，即用户的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="097d5-107">This type inherits from [identity](identity.md) and has one additional property, the user principal name of the user.</span></span>

## <a name="methods"></a><span data-ttu-id="097d5-108">Methods</span><span class="sxs-lookup"><span data-stu-id="097d5-108">Methods</span></span>

<span data-ttu-id="097d5-109">无。</span><span class="sxs-lookup"><span data-stu-id="097d5-109">None.</span></span>  <span data-ttu-id="097d5-110">创建 [accessReview](../api/accessreview-create.md)时，将在请求正文中包括此类型的对象。</span><span class="sxs-lookup"><span data-stu-id="097d5-110">You would include objects of this type in the body of a request when [creating an accessReview](../api/accessreview-create.md).</span></span>

## <a name="properties"></a><span data-ttu-id="097d5-111">属性</span><span class="sxs-lookup"><span data-stu-id="097d5-111">Properties</span></span>

| <span data-ttu-id="097d5-112">属性</span><span class="sxs-lookup"><span data-stu-id="097d5-112">Property</span></span>          | <span data-ttu-id="097d5-113">类型</span><span class="sxs-lookup"><span data-stu-id="097d5-113">Type</span></span>   | <span data-ttu-id="097d5-114">说明</span><span class="sxs-lookup"><span data-stu-id="097d5-114">Description</span></span>                                                                            |
|:------------------|:-------|:---------------------------------------------------------------------------------------|
| <span data-ttu-id="097d5-115">displayName</span><span class="sxs-lookup"><span data-stu-id="097d5-115">displayName</span></span>       | <span data-ttu-id="097d5-116">String</span><span class="sxs-lookup"><span data-stu-id="097d5-116">String</span></span> | <span data-ttu-id="097d5-117">此身份的显示名称。</span><span class="sxs-lookup"><span data-stu-id="097d5-117">The identity's display name.</span></span> <span data-ttu-id="097d5-118">请注意，这可能并不总是可用或最新的。</span><span class="sxs-lookup"><span data-stu-id="097d5-118">Note that this may not always be available or up-to-date.</span></span> |
| <span data-ttu-id="097d5-119">id</span><span class="sxs-lookup"><span data-stu-id="097d5-119">id</span></span>                | <span data-ttu-id="097d5-120">String</span><span class="sxs-lookup"><span data-stu-id="097d5-120">String</span></span> | <span data-ttu-id="097d5-121">身份的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="097d5-121">Unique identifier for the identity.</span></span> <span data-ttu-id="097d5-122">可为空。</span><span class="sxs-lookup"><span data-stu-id="097d5-122">Nullable.</span></span>                                                   |
| <span data-ttu-id="097d5-123">ipAddress</span><span class="sxs-lookup"><span data-stu-id="097d5-123">ipAddress</span></span>         | <span data-ttu-id="097d5-124">String</span><span class="sxs-lookup"><span data-stu-id="097d5-124">String</span></span> | <span data-ttu-id="097d5-125">指示仅与用户一起执行活动 (审核日志使用的) 。</span><span class="sxs-lookup"><span data-stu-id="097d5-125">Indicates the client IP address used by user performing the activity (audit log only).</span></span> |
| <span data-ttu-id="097d5-126">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="097d5-126">userPrincipalName</span></span> | <span data-ttu-id="097d5-127">String</span><span class="sxs-lookup"><span data-stu-id="097d5-127">String</span></span> | <span data-ttu-id="097d5-128">用户的 userPrincipalName 属性。</span><span class="sxs-lookup"><span data-stu-id="097d5-128">The userPrincipalName attribute of the user.</span></span>                                           |

### <a name="remarks"></a><span data-ttu-id="097d5-129">注解</span><span class="sxs-lookup"><span data-stu-id="097d5-129">Remarks</span></span>

<span data-ttu-id="097d5-p105">在某些情况下，角色唯一标识符可能不可用。在这种情况下，将返回身份的 **displayName** 属性，但 **id** 属性将从资源中丢失。</span><span class="sxs-lookup"><span data-stu-id="097d5-p105">In some circumstances, the unique identifier for the actor may not be available. In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.</span></span>

## <a name="relationships"></a><span data-ttu-id="097d5-132">关系</span><span class="sxs-lookup"><span data-stu-id="097d5-132">Relationships</span></span>

<span data-ttu-id="097d5-133">无。</span><span class="sxs-lookup"><span data-stu-id="097d5-133">None.</span></span>

## <a name="see-also"></a><span data-ttu-id="097d5-134">另请参阅</span><span class="sxs-lookup"><span data-stu-id="097d5-134">See also</span></span>

| <span data-ttu-id="097d5-135">方法</span><span class="sxs-lookup"><span data-stu-id="097d5-135">Method</span></span>                                                                | <span data-ttu-id="097d5-136">返回类型</span><span class="sxs-lookup"><span data-stu-id="097d5-136">Return Type</span></span>                                | <span data-ttu-id="097d5-137">Description</span><span class="sxs-lookup"><span data-stu-id="097d5-137">Description</span></span>                             |
|:----------------------------------------------------------------------|:-------------------------------------------|:----------------------------------------|
| [<span data-ttu-id="097d5-138">获取 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="097d5-138">Get accessReview reviewers</span></span>](../api/accessreview-listreviewers.md)    | <span data-ttu-id="097d5-139">[userIdentity](useridentity.md) 集合</span><span class="sxs-lookup"><span data-stu-id="097d5-139">[userIdentity](useridentity.md) collection</span></span> | <span data-ttu-id="097d5-140">获取 accessReview 的审阅者。</span><span class="sxs-lookup"><span data-stu-id="097d5-140">Get the reviewers of an accessReview.</span></span>   |
| [<span data-ttu-id="097d5-141">添加 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="097d5-141">Add accessReview reviewer</span></span>](../api/accessreview-addreviewer.md)       | <span data-ttu-id="097d5-142">无。</span><span class="sxs-lookup"><span data-stu-id="097d5-142">None.</span></span>                                      | <span data-ttu-id="097d5-143">将审阅者添加到 accessReview。</span><span class="sxs-lookup"><span data-stu-id="097d5-143">Add a reviewer to an accessReview.</span></span>      |
| [<span data-ttu-id="097d5-144">删除 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="097d5-144">Remove accessReview reviewer</span></span>](../api/accessreview-removereviewer.md) | <span data-ttu-id="097d5-145">无。</span><span class="sxs-lookup"><span data-stu-id="097d5-145">None.</span></span>                                      | <span data-ttu-id="097d5-146">从 accessReview 中删除审阅者。</span><span class="sxs-lookup"><span data-stu-id="097d5-146">Remove a reviewer from an accessReview.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="097d5-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="097d5-147">JSON representation</span></span>

<span data-ttu-id="097d5-148">下面是类型的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="097d5-148">Here is a JSON representation of the type.</span></span>

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


