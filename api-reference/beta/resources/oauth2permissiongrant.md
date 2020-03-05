---
title: oAuth2PermissionGrant 资源类型
description: 表示已授予应用程序（由服务主体表示）作为用户或管理员同意过程的一部分的 OAuth 2.0 作用域（委派权限）。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: e43866c73b8ad92e56a6e907c5ef8c660ef56e22
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522531"
---
# <a name="oauth2permissiongrant-resource-type"></a><span data-ttu-id="9e953-103">oAuth2PermissionGrant 资源类型</span><span class="sxs-lookup"><span data-stu-id="9e953-103">oAuth2PermissionGrant resource type</span></span>

<span data-ttu-id="9e953-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="9e953-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e953-105">表示已授予应用程序（由服务主体表示）作为用户或管理员同意过程的一部分的 OAuth 2.0 作用域（委派权限）。</span><span class="sxs-lookup"><span data-stu-id="9e953-105">Represents the OAuth 2.0 scopes (delegated permissions) that have been granted to an application (represented by a service principal) as part of the user or admin consent process.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9e953-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9e953-106">JSON representation</span></span>

<span data-ttu-id="9e953-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9e953-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant"
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
## <a name="properties"></a><span data-ttu-id="9e953-108">属性</span><span class="sxs-lookup"><span data-stu-id="9e953-108">Properties</span></span>
| <span data-ttu-id="9e953-109">属性</span><span class="sxs-lookup"><span data-stu-id="9e953-109">Property</span></span>     | <span data-ttu-id="9e953-110">类型</span><span class="sxs-lookup"><span data-stu-id="9e953-110">Type</span></span>   |<span data-ttu-id="9e953-111">说明</span><span class="sxs-lookup"><span data-stu-id="9e953-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9e953-112">clientId</span><span class="sxs-lookup"><span data-stu-id="9e953-112">clientId</span></span>|<span data-ttu-id="9e953-113">字符串</span><span class="sxs-lookup"><span data-stu-id="9e953-113">String</span></span>| <span data-ttu-id="9e953-114">在访问资源（由 resourceId 属性表示）时，授权模拟用户的服务主体的 id。</span><span class="sxs-lookup"><span data-stu-id="9e953-114">The id of the service principal granted consent to impersonate the user when accessing the resource (represented by the resourceId property).</span></span> |
|<span data-ttu-id="9e953-115">consentType</span><span class="sxs-lookup"><span data-stu-id="9e953-115">consentType</span></span>|<span data-ttu-id="9e953-116">String</span><span class="sxs-lookup"><span data-stu-id="9e953-116">String</span></span>| <span data-ttu-id="9e953-117">指示许可是由管理员（代表组织）提供，还是由个人授予。</span><span class="sxs-lookup"><span data-stu-id="9e953-117">Indicates if consent was provided by the administrator (on behalf of the organization) or by an individual.</span></span> <span data-ttu-id="9e953-118">可能的值为*AllPrincipals*或*Principal*。</span><span class="sxs-lookup"><span data-stu-id="9e953-118">The possible values are *AllPrincipals* or *Principal*.</span></span> |
|<span data-ttu-id="9e953-119">expiryTime</span><span class="sxs-lookup"><span data-stu-id="9e953-119">expiryTime</span></span>|<span data-ttu-id="9e953-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e953-120">DateTimeOffset</span></span>| <span data-ttu-id="9e953-121">目前，到期时间值将被忽略。</span><span class="sxs-lookup"><span data-stu-id="9e953-121">Currently, the expiry time value is ignored.</span></span> |
|<span data-ttu-id="9e953-122">id</span><span class="sxs-lookup"><span data-stu-id="9e953-122">id</span></span>|<span data-ttu-id="9e953-123">String</span><span class="sxs-lookup"><span data-stu-id="9e953-123">String</span></span>| <span data-ttu-id="9e953-124">唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="9e953-124">Unique identifier.</span></span> <span data-ttu-id="9e953-125">只读。</span><span class="sxs-lookup"><span data-stu-id="9e953-125">Read-only.</span></span>|
|<span data-ttu-id="9e953-126">principalId</span><span class="sxs-lookup"><span data-stu-id="9e953-126">principalId</span></span>|<span data-ttu-id="9e953-127">String</span><span class="sxs-lookup"><span data-stu-id="9e953-127">String</span></span>| <span data-ttu-id="9e953-128">如果 consentType 为*AllPrincipals* ，则此值为 null，并且同意适用于组织中的所有用户。</span><span class="sxs-lookup"><span data-stu-id="9e953-128">If consentType is *AllPrincipals* this value is null, and the consent applies to all users in the organization.</span></span> <span data-ttu-id="9e953-129">如果 consentType 为*Principal*，则此属性指定授予同意的用户的 id，并且仅适用于该用户。</span><span class="sxs-lookup"><span data-stu-id="9e953-129">If consentType is *Principal*, then this property specifies the id of the user that granted consent and applies only for that user.</span></span> |
|<span data-ttu-id="9e953-130">resourceId</span><span class="sxs-lookup"><span data-stu-id="9e953-130">resourceId</span></span>|<span data-ttu-id="9e953-131">String</span><span class="sxs-lookup"><span data-stu-id="9e953-131">String</span></span>| <span data-ttu-id="9e953-132">指定已向其授予访问权限的资源服务主体的 id。</span><span class="sxs-lookup"><span data-stu-id="9e953-132">Specifies the id of the resource service principal to which access has been granted.</span></span> |
|<span data-ttu-id="9e953-133">scope</span><span class="sxs-lookup"><span data-stu-id="9e953-133">scope</span></span>|<span data-ttu-id="9e953-134">String</span><span class="sxs-lookup"><span data-stu-id="9e953-134">String</span></span>| <span data-ttu-id="9e953-135">指定在 OAuth 2.0 访问令牌中，资源应用程序应预期的[范围](/graph/permissions-reference)声明的值。</span><span class="sxs-lookup"><span data-stu-id="9e953-135">Specifies the value of the [scope](/graph/permissions-reference) claim that the resource application should expect in the OAuth 2.0 access token.</span></span> <span data-ttu-id="9e953-136">例如， *User. Read*</span><span class="sxs-lookup"><span data-stu-id="9e953-136">For example, *User.Read*</span></span> |
|<span data-ttu-id="9e953-137">startTime</span><span class="sxs-lookup"><span data-stu-id="9e953-137">startTime</span></span>|<span data-ttu-id="9e953-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e953-138">DateTimeOffset</span></span>| <span data-ttu-id="9e953-139">目前，开始时间值将被忽略。</span><span class="sxs-lookup"><span data-stu-id="9e953-139">Currently, the start time value is ignored.</span></span> |

## <a name="relationships"></a><span data-ttu-id="9e953-140">关系</span><span class="sxs-lookup"><span data-stu-id="9e953-140">Relationships</span></span>
<span data-ttu-id="9e953-141">无</span><span class="sxs-lookup"><span data-stu-id="9e953-141">None</span></span>


## <a name="methods"></a><span data-ttu-id="9e953-142">方法</span><span class="sxs-lookup"><span data-stu-id="9e953-142">Methods</span></span>

| <span data-ttu-id="9e953-143">方法</span><span class="sxs-lookup"><span data-stu-id="9e953-143">Method</span></span>           | <span data-ttu-id="9e953-144">返回类型</span><span class="sxs-lookup"><span data-stu-id="9e953-144">Return Type</span></span>    |<span data-ttu-id="9e953-145">说明</span><span class="sxs-lookup"><span data-stu-id="9e953-145">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9e953-146">获取 oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="9e953-146">Get oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-get.md) | [<span data-ttu-id="9e953-147">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="9e953-147">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) |<span data-ttu-id="9e953-148">读取 oAuth2PermissionGrant 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9e953-148">Read properties and relationships of oAuth2PermissionGrant object.</span></span>|
|[<span data-ttu-id="9e953-149">列出 oAuth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="9e953-149">List oAuth2PermissionGrants</span></span>](../api/oauth2permissiongrant-list.md) | <span data-ttu-id="9e953-150">[oAuth2PermissionGrant](oauth2permissiongrant.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9e953-150">[oAuth2PermissionGrant](oauth2permissiongrant.md) collection</span></span> | <span data-ttu-id="9e953-151">检索 oauth2PermissionGrant 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="9e953-151">Retrieve a list of oauth2PermissionGrant objects.</span></span> |
|[<span data-ttu-id="9e953-152">更新 oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="9e953-152">Update oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-update.md) | [<span data-ttu-id="9e953-153">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="9e953-153">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) |<span data-ttu-id="9e953-154">更新 oAuth2PermissionGrant 对象。</span><span class="sxs-lookup"><span data-stu-id="9e953-154">Update oAuth2PermissionGrant object.</span></span> |
|[<span data-ttu-id="9e953-155">删除 oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="9e953-155">Delete oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-delete.md) | <span data-ttu-id="9e953-156">无</span><span class="sxs-lookup"><span data-stu-id="9e953-156">None</span></span> |<span data-ttu-id="9e953-157">删除 oAuth2PermissionGrant 对象。</span><span class="sxs-lookup"><span data-stu-id="9e953-157">Delete oAuth2PermissionGrant object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oAuth2PermissionGrant resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
