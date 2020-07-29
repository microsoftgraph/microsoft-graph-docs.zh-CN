---
title: connectedOrganization 资源类型
description: 在 Azure AD 权限管理中，连接的组织是对其他组织的目录或域的引用，用户可以请求访问它。
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: cb82ac88f1f81bf7d2f3238657818d0782ed6b60
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/29/2020
ms.locfileid: "46510148"
---
# <a name="connectedorganization-resource-type"></a><span data-ttu-id="29f91-103">connectedOrganization 资源类型</span><span class="sxs-lookup"><span data-stu-id="29f91-103">connectedOrganization resource type</span></span>

<span data-ttu-id="29f91-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29f91-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29f91-105">在[AZURE AD 权限管理](entitlementmanagement-root.md)中，连接的组织是对其他组织的目录或域的引用，用户可以请求访问它。</span><span class="sxs-lookup"><span data-stu-id="29f91-105">In [Azure AD entitlement management](entitlementmanagement-root.md), a connected organization is a reference to a directory or domain of another organization whose users can request access.</span></span>

## <a name="methods"></a><span data-ttu-id="29f91-106">方法</span><span class="sxs-lookup"><span data-stu-id="29f91-106">Methods</span></span>

|<span data-ttu-id="29f91-107">方法</span><span class="sxs-lookup"><span data-stu-id="29f91-107">Method</span></span>|<span data-ttu-id="29f91-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="29f91-108">Return type</span></span>|<span data-ttu-id="29f91-109">说明</span><span class="sxs-lookup"><span data-stu-id="29f91-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="29f91-110">列出 connectedOrganizations</span><span class="sxs-lookup"><span data-stu-id="29f91-110">List connectedOrganizations</span></span>](../api/connectedorganization-list.md) | <span data-ttu-id="29f91-111">[connectedOrganization](connectedorganization.md)集合</span><span class="sxs-lookup"><span data-stu-id="29f91-111">[connectedOrganization](connectedorganization.md) collection</span></span> | <span data-ttu-id="29f91-112">检索 connectedOrganization 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="29f91-112">Retrieve a list of connectedOrganization objects.</span></span> |
|[<span data-ttu-id="29f91-113">创建 connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="29f91-113">Create connectedOrganization</span></span>](../api/connectedorganization-post.md) | [<span data-ttu-id="29f91-114">connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="29f91-114">connectedOrganization</span></span>](connectedorganization.md) | <span data-ttu-id="29f91-115">创建新的 connectedOrganization 对象。</span><span class="sxs-lookup"><span data-stu-id="29f91-115">Create a new connectedOrganization object.</span></span> |
|[<span data-ttu-id="29f91-116">获取 connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="29f91-116">Get connectedOrganization</span></span>](../api/connectedorganization-get.md) | [<span data-ttu-id="29f91-117">connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="29f91-117">connectedOrganization</span></span>](connectedorganization.md) | <span data-ttu-id="29f91-118">读取 connectedOrganization 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="29f91-118">Read properties and relationships of a connectedOrganization object.</span></span> |
|[<span data-ttu-id="29f91-119">更新 connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="29f91-119">Update connectedOrganization</span></span>](../api/connectedorganization-update.md) | | <span data-ttu-id="29f91-120">更新 connectedOrganization。</span><span class="sxs-lookup"><span data-stu-id="29f91-120">Update a connectedOrganization.</span></span> |
|[<span data-ttu-id="29f91-121">删除 connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="29f91-121">Delete connectedOrganization</span></span>](../api/connectedorganization-delete.md) |<span data-ttu-id="29f91-122">无</span><span class="sxs-lookup"><span data-stu-id="29f91-122">None</span></span> | <span data-ttu-id="29f91-123">删除 connectedOrganization。</span><span class="sxs-lookup"><span data-stu-id="29f91-123">Delete a connectedOrganization.</span></span> |

## <a name="properties"></a><span data-ttu-id="29f91-124">属性</span><span class="sxs-lookup"><span data-stu-id="29f91-124">Properties</span></span>

|<span data-ttu-id="29f91-125">属性</span><span class="sxs-lookup"><span data-stu-id="29f91-125">Property</span></span>|<span data-ttu-id="29f91-126">类型</span><span class="sxs-lookup"><span data-stu-id="29f91-126">Type</span></span>|<span data-ttu-id="29f91-127">说明</span><span class="sxs-lookup"><span data-stu-id="29f91-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29f91-128">createdBy</span><span class="sxs-lookup"><span data-stu-id="29f91-128">createdBy</span></span>|<span data-ttu-id="29f91-129">字符串</span><span class="sxs-lookup"><span data-stu-id="29f91-129">String</span></span>|<span data-ttu-id="29f91-130">创建此资源的用户的 UPN。</span><span class="sxs-lookup"><span data-stu-id="29f91-130">UPN of the user who created this resource.</span></span> <span data-ttu-id="29f91-131">只读。</span><span class="sxs-lookup"><span data-stu-id="29f91-131">Read-only.</span></span>|
|<span data-ttu-id="29f91-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="29f91-132">createdDateTime</span></span>|<span data-ttu-id="29f91-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29f91-133">DateTimeOffset</span></span>|<span data-ttu-id="29f91-134">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="29f91-134">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="29f91-135">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="29f91-135">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="29f91-136">只读。</span><span class="sxs-lookup"><span data-stu-id="29f91-136">Read-only.</span></span>|
|<span data-ttu-id="29f91-137">说明</span><span class="sxs-lookup"><span data-stu-id="29f91-137">description</span></span>|<span data-ttu-id="29f91-138">String</span><span class="sxs-lookup"><span data-stu-id="29f91-138">String</span></span>|<span data-ttu-id="29f91-139">所连接的组织的说明。</span><span class="sxs-lookup"><span data-stu-id="29f91-139">The description of the connected organization.</span></span>|
|<span data-ttu-id="29f91-140">displayName</span><span class="sxs-lookup"><span data-stu-id="29f91-140">displayName</span></span>|<span data-ttu-id="29f91-141">String</span><span class="sxs-lookup"><span data-stu-id="29f91-141">String</span></span>|<span data-ttu-id="29f91-142">所连接的组织的显示名称。</span><span class="sxs-lookup"><span data-stu-id="29f91-142">The display name of the connected organization.</span></span>|
|<span data-ttu-id="29f91-143">id</span><span class="sxs-lookup"><span data-stu-id="29f91-143">id</span></span>|<span data-ttu-id="29f91-144">字符串</span><span class="sxs-lookup"><span data-stu-id="29f91-144">String</span></span>| <span data-ttu-id="29f91-145">只读。</span><span class="sxs-lookup"><span data-stu-id="29f91-145">Read-only.</span></span>|
|<span data-ttu-id="29f91-146">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="29f91-146">modifiedBy</span></span>|<span data-ttu-id="29f91-147">字符串</span><span class="sxs-lookup"><span data-stu-id="29f91-147">String</span></span>|<span data-ttu-id="29f91-148">上次修改此资源的用户的 UPN。</span><span class="sxs-lookup"><span data-stu-id="29f91-148">UPN of the user who last modified this resource.</span></span> <span data-ttu-id="29f91-149">只读。</span><span class="sxs-lookup"><span data-stu-id="29f91-149">Read-only.</span></span>|
|<span data-ttu-id="29f91-150">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="29f91-150">modifiedDateTime</span></span>|<span data-ttu-id="29f91-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29f91-151">DateTimeOffset</span></span>|<span data-ttu-id="29f91-152">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="29f91-152">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="29f91-153">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="29f91-153">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="29f91-154">只读。</span><span class="sxs-lookup"><span data-stu-id="29f91-154">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="29f91-155">关系</span><span class="sxs-lookup"><span data-stu-id="29f91-155">Relationships</span></span>

|<span data-ttu-id="29f91-156">关系</span><span class="sxs-lookup"><span data-stu-id="29f91-156">Relationship</span></span>|<span data-ttu-id="29f91-157">类型</span><span class="sxs-lookup"><span data-stu-id="29f91-157">Type</span></span>|<span data-ttu-id="29f91-158">说明</span><span class="sxs-lookup"><span data-stu-id="29f91-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29f91-159">identitySources</span><span class="sxs-lookup"><span data-stu-id="29f91-159">identitySources</span></span>|<span data-ttu-id="29f91-160">[identitySource](identitySource.md)集合</span><span class="sxs-lookup"><span data-stu-id="29f91-160">[identitySource](identitySource.md) collection</span></span>| <span data-ttu-id="29f91-161">此连接组织中的标识源、 [azureActiveDirectoryTenant](azureactivedirectorytenant.md)、 [domainIdentitySource](domainidentitysource.md)或[externalDomainFederation](externaldomainfederation.md)之一。</span><span class="sxs-lookup"><span data-stu-id="29f91-161">The identity sources in this connected organization, one of [azureActiveDirectoryTenant](azureactivedirectorytenant.md), [domainIdentitySource](domainidentitysource.md) or [externalDomainFederation](externaldomainfederation.md).</span></span> <span data-ttu-id="29f91-162">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="29f91-162">Read-only.</span></span> <span data-ttu-id="29f91-163">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="29f91-163">Nullable.</span></span>|
|<span data-ttu-id="29f91-164">internalSponsors</span><span class="sxs-lookup"><span data-stu-id="29f91-164">internalSponsors</span></span>| <span data-ttu-id="29f91-165">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="29f91-165">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="29f91-166">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="29f91-166">Nullable.</span></span>|
|<span data-ttu-id="29f91-167">externalSponsors</span><span class="sxs-lookup"><span data-stu-id="29f91-167">externalSponsors</span></span>| <span data-ttu-id="29f91-168">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="29f91-168">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="29f91-169">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="29f91-169">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="29f91-170">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="29f91-170">JSON representation</span></span>

<span data-ttu-id="29f91-171">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="29f91-171">The following is a JSON representation of the resource.</span></span>

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
  ]
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
