---
title: connectedOrganization 资源类型
description: 在 Azure AD 权限管理中，连接的组织是对其他组织的目录或域的引用，用户可以请求访问它。
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f5d53e3a24ad8e99c22d61bc6a4d519888c4aafd
ms.sourcegitcommit: ae2e4b8963edcdcc8ce572c06a531db4769d7779
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/29/2020
ms.locfileid: "47311288"
---
# <a name="connectedorganization-resource-type"></a><span data-ttu-id="4f1be-103">connectedOrganization 资源类型</span><span class="sxs-lookup"><span data-stu-id="4f1be-103">connectedOrganization resource type</span></span>

<span data-ttu-id="4f1be-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f1be-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f1be-105">在 [AZURE AD 权限管理](entitlementmanagement-root.md)中，连接的组织是对其他组织的目录或域的引用，用户可以请求访问它。</span><span class="sxs-lookup"><span data-stu-id="4f1be-105">In [Azure AD entitlement management](entitlementmanagement-root.md), a connected organization is a reference to a directory or domain of another organization whose users can request access.</span></span>

## <a name="methods"></a><span data-ttu-id="4f1be-106">方法</span><span class="sxs-lookup"><span data-stu-id="4f1be-106">Methods</span></span>

|<span data-ttu-id="4f1be-107">方法</span><span class="sxs-lookup"><span data-stu-id="4f1be-107">Method</span></span>|<span data-ttu-id="4f1be-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="4f1be-108">Return type</span></span>|<span data-ttu-id="4f1be-109">说明</span><span class="sxs-lookup"><span data-stu-id="4f1be-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4f1be-110">列出 connectedOrganizations</span><span class="sxs-lookup"><span data-stu-id="4f1be-110">List connectedOrganizations</span></span>](../api/connectedorganization-list.md) | <span data-ttu-id="4f1be-111">[connectedOrganization](connectedorganization.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4f1be-111">[connectedOrganization](connectedorganization.md) collection</span></span> | <span data-ttu-id="4f1be-112">检索 connectedOrganization 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="4f1be-112">Retrieve a list of connectedOrganization objects.</span></span> |
|[<span data-ttu-id="4f1be-113">创建 connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="4f1be-113">Create connectedOrganization</span></span>](../api/connectedorganization-post.md) | [<span data-ttu-id="4f1be-114">connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="4f1be-114">connectedOrganization</span></span>](connectedorganization.md) | <span data-ttu-id="4f1be-115">创建新的 connectedOrganization 对象。</span><span class="sxs-lookup"><span data-stu-id="4f1be-115">Create a new connectedOrganization object.</span></span> |
|[<span data-ttu-id="4f1be-116">获取 connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="4f1be-116">Get connectedOrganization</span></span>](../api/connectedorganization-get.md) | [<span data-ttu-id="4f1be-117">connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="4f1be-117">connectedOrganization</span></span>](connectedorganization.md) | <span data-ttu-id="4f1be-118">读取 connectedOrganization 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4f1be-118">Read properties and relationships of a connectedOrganization object.</span></span> |
|[<span data-ttu-id="4f1be-119">更新 connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="4f1be-119">Update connectedOrganization</span></span>](../api/connectedorganization-update.md) | | <span data-ttu-id="4f1be-120">更新 connectedOrganization。</span><span class="sxs-lookup"><span data-stu-id="4f1be-120">Update a connectedOrganization.</span></span> |
|[<span data-ttu-id="4f1be-121">删除 connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="4f1be-121">Delete connectedOrganization</span></span>](../api/connectedorganization-delete.md) |<span data-ttu-id="4f1be-122">无</span><span class="sxs-lookup"><span data-stu-id="4f1be-122">None</span></span> | <span data-ttu-id="4f1be-123">删除 connectedOrganization。</span><span class="sxs-lookup"><span data-stu-id="4f1be-123">Delete a connectedOrganization.</span></span> |
|[<span data-ttu-id="4f1be-124">列出 internalSponsors</span><span class="sxs-lookup"><span data-stu-id="4f1be-124">List internalSponsors</span></span>](../api/connectedorganization-list-internalsponsors.md) | <span data-ttu-id="4f1be-125">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="4f1be-125">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="4f1be-126">检索 connectedOrganization 的内部发起人列表。</span><span class="sxs-lookup"><span data-stu-id="4f1be-126">Retrieve a list of a connectedOrganization's internal sponsors.</span></span> |
|[<span data-ttu-id="4f1be-127">列出 externalSponsors</span><span class="sxs-lookup"><span data-stu-id="4f1be-127">List externalSponsors</span></span>](../api/connectedorganization-list-externalsponsors.md) | <span data-ttu-id="4f1be-128">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="4f1be-128">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="4f1be-129">检索 connectedOrganization 的外部发起人列表。</span><span class="sxs-lookup"><span data-stu-id="4f1be-129">Retrieve a list of a connectedOrganization's external sponsors.</span></span> |
|[<span data-ttu-id="4f1be-130">添加 internalSponsors</span><span class="sxs-lookup"><span data-stu-id="4f1be-130">Add internalSponsors</span></span>](../api/connectedorganization-post-internalsponsors.md) | <span data-ttu-id="4f1be-131">无</span><span class="sxs-lookup"><span data-stu-id="4f1be-131">None</span></span> | <span data-ttu-id="4f1be-132">将用户或组添加到 connectedOrganization 的内部发起人。</span><span class="sxs-lookup"><span data-stu-id="4f1be-132">Add a user or group to a connectedOrganization's internal sponsors.</span></span> |
|[<span data-ttu-id="4f1be-133">添加 externalSponsors</span><span class="sxs-lookup"><span data-stu-id="4f1be-133">Add externalSponsors</span></span>](../api/connectedorganization-post-externalsponsors.md) | <span data-ttu-id="4f1be-134">无</span><span class="sxs-lookup"><span data-stu-id="4f1be-134">None</span></span> | <span data-ttu-id="4f1be-135">将用户或组添加到 connectedOrganization 的外部发起人。</span><span class="sxs-lookup"><span data-stu-id="4f1be-135">Add a user or group to a connectedOrganization's external sponsors.</span></span> |
|[<span data-ttu-id="4f1be-136">删除 internalSponsors</span><span class="sxs-lookup"><span data-stu-id="4f1be-136">Remove internalSponsors</span></span>](../api/connectedorganization-delete-internalsponsors.md) | <span data-ttu-id="4f1be-137">无</span><span class="sxs-lookup"><span data-stu-id="4f1be-137">None</span></span> | <span data-ttu-id="4f1be-138">从 connectedOrganization 的内部发起人中删除用户或组。</span><span class="sxs-lookup"><span data-stu-id="4f1be-138">Remove a user or group from a connectedOrganization's internal sponsors.</span></span> |
|[<span data-ttu-id="4f1be-139">删除 externalSponsors</span><span class="sxs-lookup"><span data-stu-id="4f1be-139">Remove externalSponsors</span></span>](../api/connectedorganization-delete-externalsponsors.md) | <span data-ttu-id="4f1be-140">无</span><span class="sxs-lookup"><span data-stu-id="4f1be-140">None</span></span> | <span data-ttu-id="4f1be-141">从 connectedOrganization 的外部发起人中删除用户或组。</span><span class="sxs-lookup"><span data-stu-id="4f1be-141">Remove a user or group from a connectedOrganization's external sponsors.</span></span> |

## <a name="properties"></a><span data-ttu-id="4f1be-142">属性</span><span class="sxs-lookup"><span data-stu-id="4f1be-142">Properties</span></span>

|<span data-ttu-id="4f1be-143">属性</span><span class="sxs-lookup"><span data-stu-id="4f1be-143">Property</span></span>|<span data-ttu-id="4f1be-144">类型</span><span class="sxs-lookup"><span data-stu-id="4f1be-144">Type</span></span>|<span data-ttu-id="4f1be-145">说明</span><span class="sxs-lookup"><span data-stu-id="4f1be-145">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f1be-146">createdBy</span><span class="sxs-lookup"><span data-stu-id="4f1be-146">createdBy</span></span>|<span data-ttu-id="4f1be-147">String</span><span class="sxs-lookup"><span data-stu-id="4f1be-147">String</span></span>|<span data-ttu-id="4f1be-148">创建此资源的用户的 UPN。</span><span class="sxs-lookup"><span data-stu-id="4f1be-148">UPN of the user who created this resource.</span></span> <span data-ttu-id="4f1be-149">只读。</span><span class="sxs-lookup"><span data-stu-id="4f1be-149">Read-only.</span></span>|
|<span data-ttu-id="4f1be-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4f1be-150">createdDateTime</span></span>|<span data-ttu-id="4f1be-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f1be-151">DateTimeOffset</span></span>|<span data-ttu-id="4f1be-152">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="4f1be-152">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4f1be-153">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="4f1be-153">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="4f1be-154">只读。</span><span class="sxs-lookup"><span data-stu-id="4f1be-154">Read-only.</span></span>|
|<span data-ttu-id="4f1be-155">说明</span><span class="sxs-lookup"><span data-stu-id="4f1be-155">description</span></span>|<span data-ttu-id="4f1be-156">String</span><span class="sxs-lookup"><span data-stu-id="4f1be-156">String</span></span>|<span data-ttu-id="4f1be-157">所连接的组织的说明。</span><span class="sxs-lookup"><span data-stu-id="4f1be-157">The description of the connected organization.</span></span>|
|<span data-ttu-id="4f1be-158">displayName</span><span class="sxs-lookup"><span data-stu-id="4f1be-158">displayName</span></span>|<span data-ttu-id="4f1be-159">String</span><span class="sxs-lookup"><span data-stu-id="4f1be-159">String</span></span>|<span data-ttu-id="4f1be-160">所连接的组织的显示名称。</span><span class="sxs-lookup"><span data-stu-id="4f1be-160">The display name of the connected organization.</span></span>|
|<span data-ttu-id="4f1be-161">id</span><span class="sxs-lookup"><span data-stu-id="4f1be-161">id</span></span>|<span data-ttu-id="4f1be-162">String</span><span class="sxs-lookup"><span data-stu-id="4f1be-162">String</span></span>| <span data-ttu-id="4f1be-163">只读。</span><span class="sxs-lookup"><span data-stu-id="4f1be-163">Read-only.</span></span>|
|<span data-ttu-id="4f1be-164">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="4f1be-164">modifiedBy</span></span>|<span data-ttu-id="4f1be-165">String</span><span class="sxs-lookup"><span data-stu-id="4f1be-165">String</span></span>|<span data-ttu-id="4f1be-166">上次修改此资源的用户的 UPN。</span><span class="sxs-lookup"><span data-stu-id="4f1be-166">UPN of the user who last modified this resource.</span></span> <span data-ttu-id="4f1be-167">只读。</span><span class="sxs-lookup"><span data-stu-id="4f1be-167">Read-only.</span></span>|
|<span data-ttu-id="4f1be-168">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4f1be-168">modifiedDateTime</span></span>|<span data-ttu-id="4f1be-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f1be-169">DateTimeOffset</span></span>|<span data-ttu-id="4f1be-170">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="4f1be-170">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4f1be-171">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="4f1be-171">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="4f1be-172">只读。</span><span class="sxs-lookup"><span data-stu-id="4f1be-172">Read-only.</span></span>|
|<span data-ttu-id="4f1be-173">state</span><span class="sxs-lookup"><span data-stu-id="4f1be-173">state</span></span>|<span data-ttu-id="4f1be-174">connectedOrganizationState</span><span class="sxs-lookup"><span data-stu-id="4f1be-174">connectedOrganizationState</span></span>|<span data-ttu-id="4f1be-175">已连接组织的状态定义了请求者范围类型的工作分配策略是否 `AllConfiguredConnectedOrganizationSubjects` 适用。</span><span class="sxs-lookup"><span data-stu-id="4f1be-175">The state of a connected organization defines whether assignment policies with requestor scope type `AllConfiguredConnectedOrganizationSubjects` are applicable or not.</span></span> <span data-ttu-id="4f1be-176">可取值为：`configured`、`proposed`。</span><span class="sxs-lookup"><span data-stu-id="4f1be-176">Possible values are: `configured`, `proposed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4f1be-177">关系</span><span class="sxs-lookup"><span data-stu-id="4f1be-177">Relationships</span></span>

|<span data-ttu-id="4f1be-178">关系</span><span class="sxs-lookup"><span data-stu-id="4f1be-178">Relationship</span></span>|<span data-ttu-id="4f1be-179">类型</span><span class="sxs-lookup"><span data-stu-id="4f1be-179">Type</span></span>|<span data-ttu-id="4f1be-180">说明</span><span class="sxs-lookup"><span data-stu-id="4f1be-180">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f1be-181">identitySources</span><span class="sxs-lookup"><span data-stu-id="4f1be-181">identitySources</span></span>|<span data-ttu-id="4f1be-182">[identitySource](identitySource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4f1be-182">[identitySource](identitySource.md) collection</span></span>| <span data-ttu-id="4f1be-183">此连接组织中的标识源、 [azureActiveDirectoryTenant](azureactivedirectorytenant.md)、 [domainIdentitySource](domainidentitysource.md) 或 [externalDomainFederation](externaldomainfederation.md)之一。</span><span class="sxs-lookup"><span data-stu-id="4f1be-183">The identity sources in this connected organization, one of [azureActiveDirectoryTenant](azureactivedirectorytenant.md), [domainIdentitySource](domainidentitysource.md) or [externalDomainFederation](externaldomainfederation.md).</span></span> <span data-ttu-id="4f1be-184">只读。</span><span class="sxs-lookup"><span data-stu-id="4f1be-184">Read-only.</span></span> <span data-ttu-id="4f1be-185">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="4f1be-185">Nullable.</span></span>|
|<span data-ttu-id="4f1be-186">internalSponsors</span><span class="sxs-lookup"><span data-stu-id="4f1be-186">internalSponsors</span></span>| <span data-ttu-id="4f1be-187">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="4f1be-187">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="4f1be-188">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="4f1be-188">Nullable.</span></span>|
|<span data-ttu-id="4f1be-189">externalSponsors</span><span class="sxs-lookup"><span data-stu-id="4f1be-189">externalSponsors</span></span>| <span data-ttu-id="4f1be-190">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="4f1be-190">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="4f1be-191">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="4f1be-191">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4f1be-192">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4f1be-192">JSON representation</span></span>

<span data-ttu-id="4f1be-193">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4f1be-193">The following is a JSON representation of the resource.</span></span>

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
