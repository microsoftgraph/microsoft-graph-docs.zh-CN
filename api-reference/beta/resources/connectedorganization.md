---
title: connectedOrganization 资源类型
description: 在 Azure AD 权利管理中，已连接组织是其他用户可请求访问的目录或域的引用。
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 23deb11dc582228cd398dfc1f88d576b3cb15a86
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444299"
---
# <a name="connectedorganization-resource-type"></a><span data-ttu-id="61d7e-103">connectedOrganization 资源类型</span><span class="sxs-lookup"><span data-stu-id="61d7e-103">connectedOrganization resource type</span></span>

<span data-ttu-id="61d7e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61d7e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="61d7e-105">在 [Azure AD 权利管理](entitlementmanagement-root.md)中，已连接组织是其他用户可请求访问的目录或域的引用。</span><span class="sxs-lookup"><span data-stu-id="61d7e-105">In [Azure AD entitlement management](entitlementmanagement-root.md), a connected organization is a reference to a directory or domain of another organization whose users can request access.</span></span>

## <a name="methods"></a><span data-ttu-id="61d7e-106">Methods</span><span class="sxs-lookup"><span data-stu-id="61d7e-106">Methods</span></span>

|<span data-ttu-id="61d7e-107">方法</span><span class="sxs-lookup"><span data-stu-id="61d7e-107">Method</span></span>|<span data-ttu-id="61d7e-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="61d7e-108">Return type</span></span>|<span data-ttu-id="61d7e-109">说明</span><span class="sxs-lookup"><span data-stu-id="61d7e-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="61d7e-110">列出 connectedOrganizations</span><span class="sxs-lookup"><span data-stu-id="61d7e-110">List connectedOrganizations</span></span>](../api/connectedorganization-list.md) | <span data-ttu-id="61d7e-111">[connectedOrganization](connectedorganization.md) 集合</span><span class="sxs-lookup"><span data-stu-id="61d7e-111">[connectedOrganization](connectedorganization.md) collection</span></span> | <span data-ttu-id="61d7e-112">检索 connectedOrganization 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="61d7e-112">Retrieve a list of connectedOrganization objects.</span></span> |
|[<span data-ttu-id="61d7e-113">创建 connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="61d7e-113">Create connectedOrganization</span></span>](../api/connectedorganization-post.md) | [<span data-ttu-id="61d7e-114">connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="61d7e-114">connectedOrganization</span></span>](connectedorganization.md) | <span data-ttu-id="61d7e-115">创建新的 connectedOrganization 对象。</span><span class="sxs-lookup"><span data-stu-id="61d7e-115">Create a new connectedOrganization object.</span></span> |
|[<span data-ttu-id="61d7e-116">获取 connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="61d7e-116">Get connectedOrganization</span></span>](../api/connectedorganization-get.md) | [<span data-ttu-id="61d7e-117">connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="61d7e-117">connectedOrganization</span></span>](connectedorganization.md) | <span data-ttu-id="61d7e-118">读取 connectedOrganization 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="61d7e-118">Read properties and relationships of a connectedOrganization object.</span></span> |
|[<span data-ttu-id="61d7e-119">更新 connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="61d7e-119">Update connectedOrganization</span></span>](../api/connectedorganization-update.md) | | <span data-ttu-id="61d7e-120">更新 connectedOrganization。</span><span class="sxs-lookup"><span data-stu-id="61d7e-120">Update a connectedOrganization.</span></span> |
|[<span data-ttu-id="61d7e-121">删除 connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="61d7e-121">Delete connectedOrganization</span></span>](../api/connectedorganization-delete.md) |<span data-ttu-id="61d7e-122">无</span><span class="sxs-lookup"><span data-stu-id="61d7e-122">None</span></span> | <span data-ttu-id="61d7e-123">删除 connectedOrganization。</span><span class="sxs-lookup"><span data-stu-id="61d7e-123">Delete a connectedOrganization.</span></span> |
|[<span data-ttu-id="61d7e-124">列出 internalSponsors</span><span class="sxs-lookup"><span data-stu-id="61d7e-124">List internalSponsors</span></span>](../api/connectedorganization-list-internalsponsors.md) | <span data-ttu-id="61d7e-125">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="61d7e-125">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="61d7e-126">检索 connectedOrganization 的内部发起人的列表。</span><span class="sxs-lookup"><span data-stu-id="61d7e-126">Retrieve a list of a connectedOrganization's internal sponsors.</span></span> |
|[<span data-ttu-id="61d7e-127">列出 externalSponsors</span><span class="sxs-lookup"><span data-stu-id="61d7e-127">List externalSponsors</span></span>](../api/connectedorganization-list-externalsponsors.md) | <span data-ttu-id="61d7e-128">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="61d7e-128">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="61d7e-129">检索 connectedOrganization 的外部发起人的列表。</span><span class="sxs-lookup"><span data-stu-id="61d7e-129">Retrieve a list of a connectedOrganization's external sponsors.</span></span> |
|[<span data-ttu-id="61d7e-130">添加 internalSponsors</span><span class="sxs-lookup"><span data-stu-id="61d7e-130">Add internalSponsors</span></span>](../api/connectedorganization-post-internalsponsors.md) | <span data-ttu-id="61d7e-131">无</span><span class="sxs-lookup"><span data-stu-id="61d7e-131">None</span></span> | <span data-ttu-id="61d7e-132">将用户或组添加到 connectedOrganization 的内部发起人。</span><span class="sxs-lookup"><span data-stu-id="61d7e-132">Add a user or group to a connectedOrganization's internal sponsors.</span></span> |
|[<span data-ttu-id="61d7e-133">添加 externalSponsors</span><span class="sxs-lookup"><span data-stu-id="61d7e-133">Add externalSponsors</span></span>](../api/connectedorganization-post-externalsponsors.md) | <span data-ttu-id="61d7e-134">无</span><span class="sxs-lookup"><span data-stu-id="61d7e-134">None</span></span> | <span data-ttu-id="61d7e-135">将用户或组添加到 connectedOrganization 的外部发起人。</span><span class="sxs-lookup"><span data-stu-id="61d7e-135">Add a user or group to a connectedOrganization's external sponsors.</span></span> |
|[<span data-ttu-id="61d7e-136">删除 internalSponsors</span><span class="sxs-lookup"><span data-stu-id="61d7e-136">Remove internalSponsors</span></span>](../api/connectedorganization-delete-internalsponsors.md) | <span data-ttu-id="61d7e-137">无</span><span class="sxs-lookup"><span data-stu-id="61d7e-137">None</span></span> | <span data-ttu-id="61d7e-138">从 connectedOrganization 的内部发起人中删除用户或组。</span><span class="sxs-lookup"><span data-stu-id="61d7e-138">Remove a user or group from a connectedOrganization's internal sponsors.</span></span> |
|[<span data-ttu-id="61d7e-139">删除 externalSponsors</span><span class="sxs-lookup"><span data-stu-id="61d7e-139">Remove externalSponsors</span></span>](../api/connectedorganization-delete-externalsponsors.md) | <span data-ttu-id="61d7e-140">无</span><span class="sxs-lookup"><span data-stu-id="61d7e-140">None</span></span> | <span data-ttu-id="61d7e-141">从 connectedOrganization 的外部发起人中删除用户或组。</span><span class="sxs-lookup"><span data-stu-id="61d7e-141">Remove a user or group from a connectedOrganization's external sponsors.</span></span> |

## <a name="properties"></a><span data-ttu-id="61d7e-142">属性</span><span class="sxs-lookup"><span data-stu-id="61d7e-142">Properties</span></span>

|<span data-ttu-id="61d7e-143">属性</span><span class="sxs-lookup"><span data-stu-id="61d7e-143">Property</span></span>|<span data-ttu-id="61d7e-144">类型</span><span class="sxs-lookup"><span data-stu-id="61d7e-144">Type</span></span>|<span data-ttu-id="61d7e-145">说明</span><span class="sxs-lookup"><span data-stu-id="61d7e-145">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61d7e-146">createdBy</span><span class="sxs-lookup"><span data-stu-id="61d7e-146">createdBy</span></span>|<span data-ttu-id="61d7e-147">String</span><span class="sxs-lookup"><span data-stu-id="61d7e-147">String</span></span>|<span data-ttu-id="61d7e-148">创建此资源的用户的 UPN。</span><span class="sxs-lookup"><span data-stu-id="61d7e-148">UPN of the user who created this resource.</span></span> <span data-ttu-id="61d7e-149">只读。</span><span class="sxs-lookup"><span data-stu-id="61d7e-149">Read-only.</span></span>|
|<span data-ttu-id="61d7e-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="61d7e-150">createdDateTime</span></span>|<span data-ttu-id="61d7e-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61d7e-151">DateTimeOffset</span></span>|<span data-ttu-id="61d7e-152">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="61d7e-152">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="61d7e-153">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="61d7e-153">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="61d7e-154">只读。</span><span class="sxs-lookup"><span data-stu-id="61d7e-154">Read-only.</span></span>|
|<span data-ttu-id="61d7e-155">说明</span><span class="sxs-lookup"><span data-stu-id="61d7e-155">description</span></span>|<span data-ttu-id="61d7e-156">String</span><span class="sxs-lookup"><span data-stu-id="61d7e-156">String</span></span>|<span data-ttu-id="61d7e-157">已连接组织的说明。</span><span class="sxs-lookup"><span data-stu-id="61d7e-157">The description of the connected organization.</span></span>|
|<span data-ttu-id="61d7e-158">displayName</span><span class="sxs-lookup"><span data-stu-id="61d7e-158">displayName</span></span>|<span data-ttu-id="61d7e-159">String</span><span class="sxs-lookup"><span data-stu-id="61d7e-159">String</span></span>|<span data-ttu-id="61d7e-160">显示名称组织的成员。</span><span class="sxs-lookup"><span data-stu-id="61d7e-160">The display name of the connected organization.</span></span>|
|<span data-ttu-id="61d7e-161">id</span><span class="sxs-lookup"><span data-stu-id="61d7e-161">id</span></span>|<span data-ttu-id="61d7e-162">String</span><span class="sxs-lookup"><span data-stu-id="61d7e-162">String</span></span>| <span data-ttu-id="61d7e-163">只读。</span><span class="sxs-lookup"><span data-stu-id="61d7e-163">Read-only.</span></span>|
|<span data-ttu-id="61d7e-164">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="61d7e-164">modifiedBy</span></span>|<span data-ttu-id="61d7e-165">String</span><span class="sxs-lookup"><span data-stu-id="61d7e-165">String</span></span>|<span data-ttu-id="61d7e-166">上次修改此资源的用户的 UPN。</span><span class="sxs-lookup"><span data-stu-id="61d7e-166">UPN of the user who last modified this resource.</span></span> <span data-ttu-id="61d7e-167">只读。</span><span class="sxs-lookup"><span data-stu-id="61d7e-167">Read-only.</span></span>|
|<span data-ttu-id="61d7e-168">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="61d7e-168">modifiedDateTime</span></span>|<span data-ttu-id="61d7e-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61d7e-169">DateTimeOffset</span></span>|<span data-ttu-id="61d7e-170">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="61d7e-170">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="61d7e-171">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="61d7e-171">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="61d7e-172">只读。</span><span class="sxs-lookup"><span data-stu-id="61d7e-172">Read-only.</span></span>|
|<span data-ttu-id="61d7e-173">state</span><span class="sxs-lookup"><span data-stu-id="61d7e-173">state</span></span>|<span data-ttu-id="61d7e-174">connectedOrganizationState</span><span class="sxs-lookup"><span data-stu-id="61d7e-174">connectedOrganizationState</span></span>|<span data-ttu-id="61d7e-175">已连接组织的状态定义具有请求者作用域类型的分配策略 `AllConfiguredConnectedOrganizationSubjects` 是否适用。</span><span class="sxs-lookup"><span data-stu-id="61d7e-175">The state of a connected organization defines whether assignment policies with requestor scope type `AllConfiguredConnectedOrganizationSubjects` are applicable or not.</span></span> <span data-ttu-id="61d7e-176">可取值为：`configured`、`proposed`。</span><span class="sxs-lookup"><span data-stu-id="61d7e-176">Possible values are: `configured`, `proposed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="61d7e-177">关系</span><span class="sxs-lookup"><span data-stu-id="61d7e-177">Relationships</span></span>

|<span data-ttu-id="61d7e-178">关系</span><span class="sxs-lookup"><span data-stu-id="61d7e-178">Relationship</span></span>|<span data-ttu-id="61d7e-179">类型</span><span class="sxs-lookup"><span data-stu-id="61d7e-179">Type</span></span>|<span data-ttu-id="61d7e-180">说明</span><span class="sxs-lookup"><span data-stu-id="61d7e-180">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61d7e-181">identitySources</span><span class="sxs-lookup"><span data-stu-id="61d7e-181">identitySources</span></span>|<span data-ttu-id="61d7e-182">[identitySource](identitySource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="61d7e-182">[identitySource](identitySource.md) collection</span></span>| <span data-ttu-id="61d7e-183">此连接组织中的身份源[，azureActiveDirectoryTenant、domainIdentitySource](azureactivedirectorytenant.md)或[externalDomainFederation 之一](externaldomainfederation.md)。 [](domainidentitysource.md)</span><span class="sxs-lookup"><span data-stu-id="61d7e-183">The identity sources in this connected organization, one of [azureActiveDirectoryTenant](azureactivedirectorytenant.md), [domainIdentitySource](domainidentitysource.md) or [externalDomainFederation](externaldomainfederation.md).</span></span> <span data-ttu-id="61d7e-184">只读。</span><span class="sxs-lookup"><span data-stu-id="61d7e-184">Read-only.</span></span> <span data-ttu-id="61d7e-185">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="61d7e-185">Nullable.</span></span>|
|<span data-ttu-id="61d7e-186">internalSponsors</span><span class="sxs-lookup"><span data-stu-id="61d7e-186">internalSponsors</span></span>| <span data-ttu-id="61d7e-187">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="61d7e-187">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="61d7e-188">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="61d7e-188">Nullable.</span></span>|
|<span data-ttu-id="61d7e-189">externalSponsors</span><span class="sxs-lookup"><span data-stu-id="61d7e-189">externalSponsors</span></span>| <span data-ttu-id="61d7e-190">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="61d7e-190">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="61d7e-191">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="61d7e-191">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="61d7e-192">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="61d7e-192">JSON representation</span></span>

<span data-ttu-id="61d7e-193">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="61d7e-193">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.connectedOrganization",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdBy": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedBy": "String",
  "modifiedDateTime": "String (timestamp)",
  "identitySources": [
    {
      "@odata.type": "microsoft.graph.azureActiveDirectoryTenant",
      "tenantId": "String (identifier)",
      "displayName": "String"
    }
  ],
  "state": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "connectedOrganization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


