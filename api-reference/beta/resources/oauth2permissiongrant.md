---
title: oAuth2PermissionGrant 资源类型
description: 代表已被授予对 （由服务主体） 应用程序的 OAuth 2.0 范围 （委派权限） 为用户或管理员同意过程的一部分。
localization_priority: Normal
ms.openlocfilehash: 5d3d900395843f39645f61d1b984e3ed4f79d476
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576967"
---
# <a name="oauth2permissiongrant-resource-type"></a><span data-ttu-id="2eb44-103">oAuth2PermissionGrant 资源类型</span><span class="sxs-lookup"><span data-stu-id="2eb44-103">oAuth2PermissionGrant resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2eb44-104">代表已被授予对 （由服务主体） 应用程序的 OAuth 2.0 范围 （委派权限） 为用户或管理员同意过程的一部分。</span><span class="sxs-lookup"><span data-stu-id="2eb44-104">Represents the OAuth 2.0 scopes (delegated permissions) that have been granted to an application (represented by a service principal) as part of the user or admin consent process.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2eb44-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2eb44-105">JSON representation</span></span>

<span data-ttu-id="2eb44-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2eb44-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="2eb44-107">属性</span><span class="sxs-lookup"><span data-stu-id="2eb44-107">Properties</span></span>
| <span data-ttu-id="2eb44-108">属性</span><span class="sxs-lookup"><span data-stu-id="2eb44-108">Property</span></span>     | <span data-ttu-id="2eb44-109">类型</span><span class="sxs-lookup"><span data-stu-id="2eb44-109">Type</span></span>   |<span data-ttu-id="2eb44-110">说明</span><span class="sxs-lookup"><span data-stu-id="2eb44-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2eb44-111">clientId</span><span class="sxs-lookup"><span data-stu-id="2eb44-111">clientId</span></span>|<span data-ttu-id="2eb44-112">String</span><span class="sxs-lookup"><span data-stu-id="2eb44-112">String</span></span>| <span data-ttu-id="2eb44-113">服务主体的 id 授予同意以访问 （由 resourceId 属性） 的资源时模拟用户。</span><span class="sxs-lookup"><span data-stu-id="2eb44-113">The id of the service principal granted consent to impersonate the user when accessing the resource (represented by the resourceId property).</span></span> |
|<span data-ttu-id="2eb44-114">consentType</span><span class="sxs-lookup"><span data-stu-id="2eb44-114">consentType</span></span>|<span data-ttu-id="2eb44-115">String</span><span class="sxs-lookup"><span data-stu-id="2eb44-115">String</span></span>| <span data-ttu-id="2eb44-116">指示由 （代表组织） 管理员或个人是否提供同意。</span><span class="sxs-lookup"><span data-stu-id="2eb44-116">Indicates if consent was provided by the administrator (on behalf of the organization) or by an individual.</span></span> <span data-ttu-id="2eb44-117">可能的值为*AllPrincipals*或*主体*。</span><span class="sxs-lookup"><span data-stu-id="2eb44-117">The possible values are *AllPrincipals* or *Principal*.</span></span> |
|<span data-ttu-id="2eb44-118">expiryTime</span><span class="sxs-lookup"><span data-stu-id="2eb44-118">expiryTime</span></span>|<span data-ttu-id="2eb44-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2eb44-119">DateTimeOffset</span></span>| <span data-ttu-id="2eb44-120">目前，到期时间值将被忽略。</span><span class="sxs-lookup"><span data-stu-id="2eb44-120">Currently, the expiry time value is ignored.</span></span> |
|<span data-ttu-id="2eb44-121">id</span><span class="sxs-lookup"><span data-stu-id="2eb44-121">id</span></span>|<span data-ttu-id="2eb44-122">String</span><span class="sxs-lookup"><span data-stu-id="2eb44-122">String</span></span>| <span data-ttu-id="2eb44-123">唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="2eb44-123">Unique identifier.</span></span> <span data-ttu-id="2eb44-124">只读。</span><span class="sxs-lookup"><span data-stu-id="2eb44-124">Read-only.</span></span>|
|<span data-ttu-id="2eb44-125">principalId</span><span class="sxs-lookup"><span data-stu-id="2eb44-125">principalId</span></span>|<span data-ttu-id="2eb44-126">String</span><span class="sxs-lookup"><span data-stu-id="2eb44-126">String</span></span>| <span data-ttu-id="2eb44-127">如果 consentType *AllPrincipals*此值为 null，并同意应用于组织中的所有用户。</span><span class="sxs-lookup"><span data-stu-id="2eb44-127">If consentType is *AllPrincipals* this value is null, and the consent applies to all users in the organization.</span></span> <span data-ttu-id="2eb44-128">如果*主体*consentType，此属性将指定的用户的授予许可，并且仅适用于该用户的 id。</span><span class="sxs-lookup"><span data-stu-id="2eb44-128">If consentType is *Principal*, then this property specifies the id of the user that granted consent and applies only for that user.</span></span> |
|<span data-ttu-id="2eb44-129">resourceId</span><span class="sxs-lookup"><span data-stu-id="2eb44-129">resourceId</span></span>|<span data-ttu-id="2eb44-130">String</span><span class="sxs-lookup"><span data-stu-id="2eb44-130">String</span></span>| <span data-ttu-id="2eb44-131">指定已向其授予访问的资源服务主体的 id。</span><span class="sxs-lookup"><span data-stu-id="2eb44-131">Specifies the id of the resource service principal to which access has been granted.</span></span> |
|<span data-ttu-id="2eb44-132">scope</span><span class="sxs-lookup"><span data-stu-id="2eb44-132">scope</span></span>|<span data-ttu-id="2eb44-133">String</span><span class="sxs-lookup"><span data-stu-id="2eb44-133">String</span></span>| <span data-ttu-id="2eb44-134">OAuth 2.0 访问令牌中指定资源应用程序应产生预期[范围](/graph/permissions-reference)声明的值。</span><span class="sxs-lookup"><span data-stu-id="2eb44-134">Specifies the value of the [scope](/graph/permissions-reference) claim that the resource application should expect in the OAuth 2.0 access token.</span></span> <span data-ttu-id="2eb44-135">例如， *User.Read*</span><span class="sxs-lookup"><span data-stu-id="2eb44-135">For example, *User.Read*</span></span> |
|<span data-ttu-id="2eb44-136">startTime</span><span class="sxs-lookup"><span data-stu-id="2eb44-136">startTime</span></span>|<span data-ttu-id="2eb44-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2eb44-137">DateTimeOffset</span></span>| <span data-ttu-id="2eb44-138">目前，开始时间值将被忽略。</span><span class="sxs-lookup"><span data-stu-id="2eb44-138">Currently, the start time value is ignored.</span></span> |

## <a name="relationships"></a><span data-ttu-id="2eb44-139">关系</span><span class="sxs-lookup"><span data-stu-id="2eb44-139">Relationships</span></span>
<span data-ttu-id="2eb44-140">无</span><span class="sxs-lookup"><span data-stu-id="2eb44-140">None</span></span>


## <a name="methods"></a><span data-ttu-id="2eb44-141">方法</span><span class="sxs-lookup"><span data-stu-id="2eb44-141">Methods</span></span>

| <span data-ttu-id="2eb44-142">方法</span><span class="sxs-lookup"><span data-stu-id="2eb44-142">Method</span></span>           | <span data-ttu-id="2eb44-143">返回类型</span><span class="sxs-lookup"><span data-stu-id="2eb44-143">Return Type</span></span>    |<span data-ttu-id="2eb44-144">说明</span><span class="sxs-lookup"><span data-stu-id="2eb44-144">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2eb44-145">获取 oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="2eb44-145">Get oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-get.md) | [<span data-ttu-id="2eb44-146">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="2eb44-146">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) |<span data-ttu-id="2eb44-147">读取属性和 oAuth2PermissionGrant 对象的关系。</span><span class="sxs-lookup"><span data-stu-id="2eb44-147">Read properties and relationships of oAuth2PermissionGrant object.</span></span>|
|[<span data-ttu-id="2eb44-148">列表 oAuth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="2eb44-148">List oAuth2PermissionGrants</span></span>](../api/oauth2permissiongrant-list.md) | <span data-ttu-id="2eb44-149">[oAuth2PermissionGrant](oauth2permissiongrant.md)集合</span><span class="sxs-lookup"><span data-stu-id="2eb44-149">[oAuth2PermissionGrant](oauth2permissiongrant.md) collection</span></span> | <span data-ttu-id="2eb44-150">检索 oauth2PermissionGrant 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="2eb44-150">Retrieve a list of oauth2PermissionGrant objects.</span></span> |
|[<span data-ttu-id="2eb44-151">更新 oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="2eb44-151">Update oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-update.md) | [<span data-ttu-id="2eb44-152">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="2eb44-152">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) |<span data-ttu-id="2eb44-153">更新 oAuth2PermissionGrant 对象。</span><span class="sxs-lookup"><span data-stu-id="2eb44-153">Update oAuth2PermissionGrant object.</span></span> |
|[<span data-ttu-id="2eb44-154">删除 oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="2eb44-154">Delete oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-delete.md) | <span data-ttu-id="2eb44-155">无</span><span class="sxs-lookup"><span data-stu-id="2eb44-155">None</span></span> |<span data-ttu-id="2eb44-156">删除 oAuth2PermissionGrant 对象。</span><span class="sxs-lookup"><span data-stu-id="2eb44-156">Delete oAuth2PermissionGrant object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oAuth2PermissionGrant resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/oauth2permissiongrant.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
