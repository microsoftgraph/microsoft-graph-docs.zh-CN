---
title: oAuth2PermissionGrant 资源类型
description: 代表已被授予对 （由服务主体） 应用程序的 OAuth 2.0 范围 （委派权限） 为用户或管理员同意过程的一部分。
ms.openlocfilehash: 8fc5154ddba1b78976dc3e24c6712f9fc8944f43
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042678"
---
# <a name="oauth2permissiongrant-resource-type"></a><span data-ttu-id="0ecf2-103">oAuth2PermissionGrant 资源类型</span><span class="sxs-lookup"><span data-stu-id="0ecf2-103">oAuth2PermissionGrant resource type</span></span>

> <span data-ttu-id="0ecf2-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0ecf2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0ecf2-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0ecf2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0ecf2-106">代表已被授予对 （由服务主体） 应用程序的 OAuth 2.0 范围 （委派权限） 为用户或管理员同意过程的一部分。</span><span class="sxs-lookup"><span data-stu-id="0ecf2-106">Represents the OAuth 2.0 scopes (delegated permissions) that have been granted to an application (represented by a service principal) as part of the user or admin consent process.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0ecf2-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0ecf2-107">JSON representation</span></span>

<span data-ttu-id="0ecf2-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0ecf2-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.oAuth2Permissiongrant"
}-->

```json
{
  "clientId": "string",
  "consentType": "string",
  "expiryTime": "String (timestamp)",
  "id": "string (identifier)",
  "principalId": "string",
  "resourceId": "string",
  "scope": "string",
  "startTime": "String (timestamp)"
}

```
## <a name="properties"></a><span data-ttu-id="0ecf2-109">属性</span><span class="sxs-lookup"><span data-stu-id="0ecf2-109">Properties</span></span>
| <span data-ttu-id="0ecf2-110">属性</span><span class="sxs-lookup"><span data-stu-id="0ecf2-110">Property</span></span>     | <span data-ttu-id="0ecf2-111">类型</span><span class="sxs-lookup"><span data-stu-id="0ecf2-111">Type</span></span>   |<span data-ttu-id="0ecf2-112">说明</span><span class="sxs-lookup"><span data-stu-id="0ecf2-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0ecf2-113">clientId</span><span class="sxs-lookup"><span data-stu-id="0ecf2-113">clientId</span></span>|<span data-ttu-id="0ecf2-114">字符串</span><span class="sxs-lookup"><span data-stu-id="0ecf2-114">String</span></span>| <span data-ttu-id="0ecf2-115">服务主体的 id 授予同意以访问 （由 resourceId 属性） 的资源时模拟用户。</span><span class="sxs-lookup"><span data-stu-id="0ecf2-115">The id of the service principal granted consent to impersonate the user when accessing the resource (represented by the resourceId property).</span></span> |
|<span data-ttu-id="0ecf2-116">consentType</span><span class="sxs-lookup"><span data-stu-id="0ecf2-116">consentType</span></span>|<span data-ttu-id="0ecf2-117">字符串</span><span class="sxs-lookup"><span data-stu-id="0ecf2-117">String</span></span>| <span data-ttu-id="0ecf2-118">指示由 （代表组织） 管理员或个人是否提供同意。</span><span class="sxs-lookup"><span data-stu-id="0ecf2-118">Indicates if consent was provided by the administrator (on behalf of the organization) or by an individual.</span></span> <span data-ttu-id="0ecf2-119">可能的值为*AllPrincipals*或*主体*。</span><span class="sxs-lookup"><span data-stu-id="0ecf2-119">The possible values are *AllPrincipals* or *Principal*.</span></span> |
|<span data-ttu-id="0ecf2-120">expiryTime</span><span class="sxs-lookup"><span data-stu-id="0ecf2-120">expiryTime</span></span>|<span data-ttu-id="0ecf2-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ecf2-121">DateTimeOffset</span></span>| <span data-ttu-id="0ecf2-122">目前，到期时间值将被忽略。</span><span class="sxs-lookup"><span data-stu-id="0ecf2-122">Currently, the expiry time value is ignored.</span></span> |
|<span data-ttu-id="0ecf2-123">id</span><span class="sxs-lookup"><span data-stu-id="0ecf2-123">id</span></span>|<span data-ttu-id="0ecf2-124">字符串</span><span class="sxs-lookup"><span data-stu-id="0ecf2-124">String</span></span>| <span data-ttu-id="0ecf2-125">唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="0ecf2-125">Unique identifier.</span></span> <span data-ttu-id="0ecf2-126">只读。</span><span class="sxs-lookup"><span data-stu-id="0ecf2-126">Read-only.</span></span>|
|<span data-ttu-id="0ecf2-127">principalId</span><span class="sxs-lookup"><span data-stu-id="0ecf2-127">principalId</span></span>|<span data-ttu-id="0ecf2-128">字符串</span><span class="sxs-lookup"><span data-stu-id="0ecf2-128">String</span></span>| <span data-ttu-id="0ecf2-129">如果 consentType *AllPrincipals*此值为 null，并同意应用于组织中的所有用户。</span><span class="sxs-lookup"><span data-stu-id="0ecf2-129">If consentType is *AllPrincipals* this value is null, and the consent applies to all users in the organization.</span></span> <span data-ttu-id="0ecf2-130">如果*主体*consentType，此属性将指定的用户的授予许可，并且仅适用于该用户的 id。</span><span class="sxs-lookup"><span data-stu-id="0ecf2-130">If consentType is *Principal*, then this property specifies the id of the user that granted consent and applies only for that user.</span></span> |
|<span data-ttu-id="0ecf2-131">resourceId</span><span class="sxs-lookup"><span data-stu-id="0ecf2-131">resourceId</span></span>|<span data-ttu-id="0ecf2-132">String</span><span class="sxs-lookup"><span data-stu-id="0ecf2-132">String</span></span>| <span data-ttu-id="0ecf2-133">指定已向其授予访问的资源服务主体的 id。</span><span class="sxs-lookup"><span data-stu-id="0ecf2-133">Specifies the id of the resource service principal to which access has been granted.</span></span> |
|<span data-ttu-id="0ecf2-134">scope</span><span class="sxs-lookup"><span data-stu-id="0ecf2-134">scope</span></span>|<span data-ttu-id="0ecf2-135">字符串</span><span class="sxs-lookup"><span data-stu-id="0ecf2-135">String</span></span>| <span data-ttu-id="0ecf2-136">OAuth 2.0 访问令牌中指定资源应用程序应产生预期[范围](/graph/permissions-reference)声明的值。</span><span class="sxs-lookup"><span data-stu-id="0ecf2-136">Specifies the value of the [scope](/graph/permissions-reference) claim that the resource application should expect in the OAuth 2.0 access token.</span></span> <span data-ttu-id="0ecf2-137">例如， *User.Read*</span><span class="sxs-lookup"><span data-stu-id="0ecf2-137">For example, *User.Read*</span></span> |
|<span data-ttu-id="0ecf2-138">startTime</span><span class="sxs-lookup"><span data-stu-id="0ecf2-138">startTime</span></span>|<span data-ttu-id="0ecf2-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ecf2-139">DateTimeOffset</span></span>| <span data-ttu-id="0ecf2-140">目前，开始时间值将被忽略。</span><span class="sxs-lookup"><span data-stu-id="0ecf2-140">Currently, the start time value is ignored.</span></span> |

## <a name="relationships"></a><span data-ttu-id="0ecf2-141">Relationships</span><span class="sxs-lookup"><span data-stu-id="0ecf2-141">Relationships</span></span>
<span data-ttu-id="0ecf2-142">无</span><span class="sxs-lookup"><span data-stu-id="0ecf2-142">None</span></span>


## <a name="methods"></a><span data-ttu-id="0ecf2-143">方法</span><span class="sxs-lookup"><span data-stu-id="0ecf2-143">Methods</span></span>

| <span data-ttu-id="0ecf2-144">方法</span><span class="sxs-lookup"><span data-stu-id="0ecf2-144">Method</span></span>           | <span data-ttu-id="0ecf2-145">返回类型</span><span class="sxs-lookup"><span data-stu-id="0ecf2-145">Return Type</span></span>    |<span data-ttu-id="0ecf2-146">说明</span><span class="sxs-lookup"><span data-stu-id="0ecf2-146">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0ecf2-147">获取 oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="0ecf2-147">Get oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-get.md) | [<span data-ttu-id="0ecf2-148">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="0ecf2-148">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) |<span data-ttu-id="0ecf2-149">读取属性和 oAuth2PermissionGrant 对象的关系。</span><span class="sxs-lookup"><span data-stu-id="0ecf2-149">Read properties and relationships of oAuth2PermissionGrant object.</span></span>|
|[<span data-ttu-id="0ecf2-150">列表 oAuth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="0ecf2-150">List oAuth2PermissionGrants</span></span>](../api/oauth2permissiongrant-list.md) | <span data-ttu-id="0ecf2-151">[oAuth2PermissionGrant](oauth2permissiongrant.md)集合</span><span class="sxs-lookup"><span data-stu-id="0ecf2-151">[oAuth2PermissionGrant](oauth2permissiongrant.md) collection</span></span> | <span data-ttu-id="0ecf2-152">检索 oauth2PermissionGrant 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="0ecf2-152">Retrieve a list of oauth2PermissionGrant objects.</span></span> |
|[<span data-ttu-id="0ecf2-153">更新 oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="0ecf2-153">Update oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-update.md) | [<span data-ttu-id="0ecf2-154">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="0ecf2-154">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) |<span data-ttu-id="0ecf2-155">更新 oAuth2PermissionGrant 对象。</span><span class="sxs-lookup"><span data-stu-id="0ecf2-155">Update oAuth2PermissionGrant object.</span></span> |
|[<span data-ttu-id="0ecf2-156">删除 oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="0ecf2-156">Delete oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-delete.md) | <span data-ttu-id="0ecf2-157">无</span><span class="sxs-lookup"><span data-stu-id="0ecf2-157">None</span></span> |<span data-ttu-id="0ecf2-158">删除 oAuth2PermissionGrant 对象。</span><span class="sxs-lookup"><span data-stu-id="0ecf2-158">Delete oAuth2PermissionGrant object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "oAuth2PermissionGrant resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->