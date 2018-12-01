---
title: userIdentity 类型
description: '为 Azure AD 访问 reviews （英文），此类型的访问评审的审阅者表示 Azure AD 用户标识。  '
ms.openlocfilehash: 6cbbe7aa017572bcd753a57edbf82751ac4986a7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044478"
---
# <a name="useridentity-type"></a><span data-ttu-id="b7ffa-103">userIdentity 类型</span><span class="sxs-lookup"><span data-stu-id="b7ffa-103">userIdentity type</span></span>

> <span data-ttu-id="b7ffa-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b7ffa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b7ffa-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b7ffa-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b7ffa-106">对于[access 会检查](accessreviews-root.md)Azure AD，此类型的访问评审的审阅者代表 Azure AD 用户标识。</span><span class="sxs-lookup"><span data-stu-id="b7ffa-106">For the Azure AD [access reviews](accessreviews-root.md), this type represents an Azure AD user identity for a reviewer of an access review.</span></span>  
<span data-ttu-id="b7ffa-107">在 Azure AD 审核日志的上下文中，这表示启动或审核活动受影响的用户信息。</span><span class="sxs-lookup"><span data-stu-id="b7ffa-107">In the context of an Azure AD audit log, this represents the user information that initiated or was affected by an audit activity.</span></span>

<span data-ttu-id="b7ffa-108">此类型继承自[identity](identity.md)和一个其他属性，用户的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="b7ffa-108">This type inherits from [identity](identity.md) and has one additional property, the user principal name of the user.</span></span>

## <a name="methods"></a><span data-ttu-id="b7ffa-109">方法</span><span class="sxs-lookup"><span data-stu-id="b7ffa-109">Methods</span></span>

<span data-ttu-id="b7ffa-110">无。</span><span class="sxs-lookup"><span data-stu-id="b7ffa-110">None.</span></span>  <span data-ttu-id="b7ffa-111">您将在请求正文中包含此类型的对象时[创建 accessReview](../api/accessreview-create.md)。</span><span class="sxs-lookup"><span data-stu-id="b7ffa-111">You would include objects of this type in the body of a request when [creating an accessReview](../api/accessreview-create.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b7ffa-112">属性</span><span class="sxs-lookup"><span data-stu-id="b7ffa-112">Properties</span></span>
| <span data-ttu-id="b7ffa-113">属性</span><span class="sxs-lookup"><span data-stu-id="b7ffa-113">Property</span></span>     | <span data-ttu-id="b7ffa-114">类型</span><span class="sxs-lookup"><span data-stu-id="b7ffa-114">Type</span></span>   |<span data-ttu-id="b7ffa-115">说明</span><span class="sxs-lookup"><span data-stu-id="b7ffa-115">Description</span></span>|
|:---------------|:--------|:----------|
| `displayName` | `String` | <span data-ttu-id="b7ffa-116">标识的显示名称。</span><span class="sxs-lookup"><span data-stu-id="b7ffa-116">The identity's display name.</span></span> <span data-ttu-id="b7ffa-117">请注意，这可能会始终不可用或最新。</span><span class="sxs-lookup"><span data-stu-id="b7ffa-117">Note that this may not always be available or up-to-date.</span></span>    |
| `id`          | `String` | <span data-ttu-id="b7ffa-118">身份的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="b7ffa-118">Unique identifier for the identity.</span></span>  |
| `ipAddress`| `String`| <span data-ttu-id="b7ffa-119">指示执行活动 （仅用于审核日志） 的用户所使用的客户端 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="b7ffa-119">Indicates the client IP address used by user performing the activity (audit log only).</span></span>|
| `userPrincipalName`|`String` | <span data-ttu-id="b7ffa-120">用户的 userPrincipalName 属性。</span><span class="sxs-lookup"><span data-stu-id="b7ffa-120">The userPrincipalName attribute of the user.</span></span> |

## <a name="remarks"></a><span data-ttu-id="b7ffa-121">注解</span><span class="sxs-lookup"><span data-stu-id="b7ffa-121">Remarks</span></span>

<span data-ttu-id="b7ffa-p104">在某些情况下，角色唯一标识符可能不可用。在这种情况下，将返回身份的 **displayName** 属性，但 **id** 属性将从资源中丢失。</span><span class="sxs-lookup"><span data-stu-id="b7ffa-p104">In some circumstances, the unique identifier for the actor may not be available. In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.</span></span>

## <a name="relationships"></a><span data-ttu-id="b7ffa-124">Relationships</span><span class="sxs-lookup"><span data-stu-id="b7ffa-124">Relationships</span></span>

<span data-ttu-id="b7ffa-125">无。</span><span class="sxs-lookup"><span data-stu-id="b7ffa-125">None.</span></span>

## <a name="see-also"></a><span data-ttu-id="b7ffa-126">另请参阅</span><span class="sxs-lookup"><span data-stu-id="b7ffa-126">See also</span></span>

| <span data-ttu-id="b7ffa-127">方法</span><span class="sxs-lookup"><span data-stu-id="b7ffa-127">Method</span></span>           | <span data-ttu-id="b7ffa-128">返回类型</span><span class="sxs-lookup"><span data-stu-id="b7ffa-128">Return Type</span></span>    |<span data-ttu-id="b7ffa-129">说明</span><span class="sxs-lookup"><span data-stu-id="b7ffa-129">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b7ffa-130">获取 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="b7ffa-130">Get accessReview reviewers</span></span>](../api/accessreview-listreviewers.md) |       <span data-ttu-id="b7ffa-131">[userIdentity](useridentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="b7ffa-131">[userIdentity](useridentity.md) collection</span></span>| <span data-ttu-id="b7ffa-132">要获取 accessReview 审阅的者。</span><span class="sxs-lookup"><span data-stu-id="b7ffa-132">Get the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="b7ffa-133">添加 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="b7ffa-133">Add accessReview reviewer</span></span>](../api/accessreview-addreviewer.md) |      <span data-ttu-id="b7ffa-134">无。</span><span class="sxs-lookup"><span data-stu-id="b7ffa-134">None.</span></span>   |   <span data-ttu-id="b7ffa-135">将审阅者添加到 accessReview。</span><span class="sxs-lookup"><span data-stu-id="b7ffa-135">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="b7ffa-136">删除 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="b7ffa-136">Remove accessReview reviewer</span></span>](../api/accessreview-removereviewer.md) | <span data-ttu-id="b7ffa-137">无。</span><span class="sxs-lookup"><span data-stu-id="b7ffa-137">None.</span></span>  |   <span data-ttu-id="b7ffa-138">删除 accessReview 审阅者。</span><span class="sxs-lookup"><span data-stu-id="b7ffa-138">Remove a reviewer from an accessReview.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b7ffa-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b7ffa-139">JSON representation</span></span>

<span data-ttu-id="b7ffa-140">下面是类型的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b7ffa-140">Here is a JSON representation of the type.</span></span>

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
 "userPrincipalName": "String"
}

```

<!-- {
  "type": "#page.annotation",
  "description": "userIdentity type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
