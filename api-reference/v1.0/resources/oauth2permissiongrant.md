---
title: oAuth2PermissionGrant 资源类型
description: 表示已授予应用程序的委派权限（OAuth 2.0 作用域），这通常是由用户或管理员的同意过程造成的。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: f04bf5b3e59f4554e5320d9b97a3b8ba88e22152
ms.sourcegitcommit: 7a6231aeb570ff45d01b3db3df07a411f9f60fd1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2020
ms.locfileid: "44383635"
---
# <a name="oauth2permissiongrant-resource-type"></a><span data-ttu-id="507cd-103">oAuth2PermissionGrant 资源类型</span><span class="sxs-lookup"><span data-stu-id="507cd-103">oAuth2PermissionGrant resource type</span></span>

<span data-ttu-id="507cd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="507cd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="507cd-105">表示已授予应用程序的服务主体的委派权限。</span><span class="sxs-lookup"><span data-stu-id="507cd-105">Represents the delegated permissions that have been granted to an application's service principal.</span></span>

<span data-ttu-id="507cd-106">委派权限授予可因用户同意应用程序的访问 API 的请求而创建，或直接创建。</span><span class="sxs-lookup"><span data-stu-id="507cd-106">Delegated permissions grants can be created as a result of a user consenting the an application's request to access an API, or created directly.</span></span>

<span data-ttu-id="507cd-107">委派权限有时称为 "OAuth 2.0 作用域" 或 "作用域"。</span><span class="sxs-lookup"><span data-stu-id="507cd-107">Delegated permissions are sometimes referred to as "OAuth 2.0 scopes" or "scopes".</span></span>

## <a name="methods"></a><span data-ttu-id="507cd-108">方法</span><span class="sxs-lookup"><span data-stu-id="507cd-108">Methods</span></span>

| <span data-ttu-id="507cd-109">方法</span><span class="sxs-lookup"><span data-stu-id="507cd-109">Method</span></span> | <span data-ttu-id="507cd-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="507cd-110">Return Type</span></span> | <span data-ttu-id="507cd-111">说明</span><span class="sxs-lookup"><span data-stu-id="507cd-111">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="507cd-112">列出 oAuth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="507cd-112">List oAuth2PermissionGrants</span></span>](../api/oauth2permissiongrant-list.md) | <span data-ttu-id="507cd-113">[oAuth2PermissionGrant](oauth2permissiongrant.md) 集合</span><span class="sxs-lookup"><span data-stu-id="507cd-113">[oAuth2PermissionGrant](oauth2permissiongrant.md) collection</span></span> | <span data-ttu-id="507cd-114">检索委派权限授予的列表。</span><span class="sxs-lookup"><span data-stu-id="507cd-114">Retrieve a list of delegated permission grants.</span></span> |
| [<span data-ttu-id="507cd-115">获取 oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="507cd-115">Get oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-get.md) | [<span data-ttu-id="507cd-116">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="507cd-116">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md)  | <span data-ttu-id="507cd-117">阅读单个委派权限授予。</span><span class="sxs-lookup"><span data-stu-id="507cd-117">Read a single delegated permission grant.</span></span>|
| [<span data-ttu-id="507cd-118">创建 oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="507cd-118">Create oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-post.md) | [<span data-ttu-id="507cd-119">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="507cd-119">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) | <span data-ttu-id="507cd-120">创建委派权限授予。</span><span class="sxs-lookup"><span data-stu-id="507cd-120">Create a delegated permission grant.</span></span> |
| [<span data-ttu-id="507cd-121">更新 oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="507cd-121">Update oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-update.md) | <span data-ttu-id="507cd-122">无</span><span class="sxs-lookup"><span data-stu-id="507cd-122">None</span></span> | <span data-ttu-id="507cd-123">更新 oAuth2PermissionGrant 对象。</span><span class="sxs-lookup"><span data-stu-id="507cd-123">Update oAuth2PermissionGrant object.</span></span> |
| [<span data-ttu-id="507cd-124">删除 oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="507cd-124">Delete oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-delete.md) | <span data-ttu-id="507cd-125">无</span><span class="sxs-lookup"><span data-stu-id="507cd-125">None</span></span>  | <span data-ttu-id="507cd-126">删除委派权限授予。</span><span class="sxs-lookup"><span data-stu-id="507cd-126">Delete a delegated permission grant.</span></span> |

## <a name="properties"></a><span data-ttu-id="507cd-127">属性</span><span class="sxs-lookup"><span data-stu-id="507cd-127">Properties</span></span>

| <span data-ttu-id="507cd-128">属性</span><span class="sxs-lookup"><span data-stu-id="507cd-128">Property</span></span> | <span data-ttu-id="507cd-129">类型</span><span class="sxs-lookup"><span data-stu-id="507cd-129">Type</span></span> | <span data-ttu-id="507cd-130">说明</span><span class="sxs-lookup"><span data-stu-id="507cd-130">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="507cd-131">id</span><span class="sxs-lookup"><span data-stu-id="507cd-131">id</span></span> | <span data-ttu-id="507cd-132">String</span><span class="sxs-lookup"><span data-stu-id="507cd-132">String</span></span> | <span data-ttu-id="507cd-133">**OAuth2PermissionGrant**的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="507cd-133">Unique identifier for the **oAuth2PermissionGrant**.</span></span> <span data-ttu-id="507cd-134">只读。</span><span class="sxs-lookup"><span data-stu-id="507cd-134">Read-only.</span></span>|
| <span data-ttu-id="507cd-135">clientId</span><span class="sxs-lookup"><span data-stu-id="507cd-135">clientId</span></span> | <span data-ttu-id="507cd-136">字符串</span><span class="sxs-lookup"><span data-stu-id="507cd-136">String</span></span> | <span data-ttu-id="507cd-137">授权在访问 API 时代表登录用户执行操作的应用程序的客户端[服务主体](serviceprincipal.md)的**id** 。</span><span class="sxs-lookup"><span data-stu-id="507cd-137">The **id** of the client [service principal](serviceprincipal.md) for the application which is authorized to act on behalf of a signed-in user when accessing an API.</span></span> <span data-ttu-id="507cd-138">必填。</span><span class="sxs-lookup"><span data-stu-id="507cd-138">Required.</span></span> <span data-ttu-id="507cd-139">支持 `$filter` （ `eq` 仅限）。</span><span class="sxs-lookup"><span data-stu-id="507cd-139">Supports `$filter` (`eq` only).</span></span> |
| <span data-ttu-id="507cd-140">consentType</span><span class="sxs-lookup"><span data-stu-id="507cd-140">consentType</span></span> | <span data-ttu-id="507cd-141">String</span><span class="sxs-lookup"><span data-stu-id="507cd-141">String</span></span> | <span data-ttu-id="507cd-142">指示是否向客户端应用程序授予了授权以模拟所有用户或仅模拟特定用户。</span><span class="sxs-lookup"><span data-stu-id="507cd-142">Indicates if authorization is granted for the client application to impersonate all users or only a specific user.</span></span> <span data-ttu-id="507cd-143">*AllPrincipals*表示模拟所有用户的授权。</span><span class="sxs-lookup"><span data-stu-id="507cd-143">*AllPrincipals* indicates authorization to impersonate all users.</span></span> <span data-ttu-id="507cd-144">*主体*指示模拟特定用户的授权。</span><span class="sxs-lookup"><span data-stu-id="507cd-144">*Principal* indicates authorization to impersonate a specific user.</span></span> <span data-ttu-id="507cd-145">管理员可以授予代表所有用户的同意。</span><span class="sxs-lookup"><span data-stu-id="507cd-145">Consent on behalf of all users can be granted by an administrator.</span></span> <span data-ttu-id="507cd-146">在某些情况下，对于某些委派权限，非管理员用户可能有权代表自己同意代表自己。</span><span class="sxs-lookup"><span data-stu-id="507cd-146">Non-admin users may be authorized to consent on behalf of themselves in some cases, for some delegated permissions.</span></span> <span data-ttu-id="507cd-147">必填。</span><span class="sxs-lookup"><span data-stu-id="507cd-147">Required.</span></span> <span data-ttu-id="507cd-148">支持 `$filter` （ `eq` 仅限）。</span><span class="sxs-lookup"><span data-stu-id="507cd-148">Supports `$filter` (`eq` only).</span></span> |
| <span data-ttu-id="507cd-149">principalId</span><span class="sxs-lookup"><span data-stu-id="507cd-149">principalId</span></span> | <span data-ttu-id="507cd-150">String</span><span class="sxs-lookup"><span data-stu-id="507cd-150">String</span></span> | <span data-ttu-id="507cd-151">当**consentType**为*Principal*时，代表其授权客户端访问该资源的[用户](user.md)的**id** 。</span><span class="sxs-lookup"><span data-stu-id="507cd-151">The **id** of the [user](user.md) on behalf of whom the client is authorized to access the resource, when **consentType** is *Principal*.</span></span> <span data-ttu-id="507cd-152">如果**consentType**为*AllPrincipals* ，则此值为 null。</span><span class="sxs-lookup"><span data-stu-id="507cd-152">If **consentType** is *AllPrincipals* this value is null.</span></span> <span data-ttu-id="507cd-153">当**consentType**为*Principal*时是必需的。</span><span class="sxs-lookup"><span data-stu-id="507cd-153">Required when **consentType** is *Principal*.</span></span> |
| <span data-ttu-id="507cd-154">resourceId</span><span class="sxs-lookup"><span data-stu-id="507cd-154">resourceId</span></span> | <span data-ttu-id="507cd-155">String</span><span class="sxs-lookup"><span data-stu-id="507cd-155">String</span></span> | <span data-ttu-id="507cd-156">向其授予访问权限的资源[服务主体](serviceprincipal.md)的**id** 。</span><span class="sxs-lookup"><span data-stu-id="507cd-156">The **id** of the resource [service principal](serviceprincipal.md) to which access is authorized.</span></span> <span data-ttu-id="507cd-157">这将标识客户端授权尝试代表已登录用户呼叫的 API。</span><span class="sxs-lookup"><span data-stu-id="507cd-157">This identifies the API which the client is authorized to attempt to call on behalf of a signed-in user.</span></span> |
| <span data-ttu-id="507cd-158">scope</span><span class="sxs-lookup"><span data-stu-id="507cd-158">scope</span></span> | <span data-ttu-id="507cd-159">String</span><span class="sxs-lookup"><span data-stu-id="507cd-159">String</span></span> | <span data-ttu-id="507cd-160">应包含在资源应用程序（API）的访问令牌中的委派权限的声明值列表（以空格分隔）。</span><span class="sxs-lookup"><span data-stu-id="507cd-160">A space-separated list of the claim values for delegated permissions which should be included in access tokens for the resource application (the API).</span></span> <span data-ttu-id="507cd-161">例如，`openid User.Read GroupMember.Read.All`。</span><span class="sxs-lookup"><span data-stu-id="507cd-161">For example, `openid User.Read GroupMember.Read.All`.</span></span> <span data-ttu-id="507cd-162">每个声明值都应与 API 定义的某个委派权限的**值**字段相匹配，这些权限在资源[服务主体](serviceprincipal.md)的**publishedPermissionScopes**属性中列出。</span><span class="sxs-lookup"><span data-stu-id="507cd-162">Each claim value should match the **value** field of one of the delegated permissions defined by the API, listed in the **publishedPermissionScopes** property of the resource [service principal](serviceprincipal.md).</span></span> |

## <a name="relationships"></a><span data-ttu-id="507cd-163">关系</span><span class="sxs-lookup"><span data-stu-id="507cd-163">Relationships</span></span>

<span data-ttu-id="507cd-164">无。</span><span class="sxs-lookup"><span data-stu-id="507cd-164">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="507cd-165">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="507cd-165">JSON representation</span></span>

<span data-ttu-id="507cd-166">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="507cd-166">The following is a JSON representation of the resource.</span></span>

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
  "id": "string (identifier)",
  "principalId": "string",
  "resourceId": "string",
  "scope": "string"
}
```


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
