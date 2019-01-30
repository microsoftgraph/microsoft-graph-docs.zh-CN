---
title: 更新应用程序
description: 更新应用程序对象的属性。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 335281a0ac37ae3b966f731112223f019a67437d
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642826"
---
# <a name="update-application"></a><span data-ttu-id="9e0b0-103">更新应用程序</span><span class="sxs-lookup"><span data-stu-id="9e0b0-103">Update application</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e0b0-104">更新应用程序对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9e0b0-104">Update the properties of application object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9e0b0-105">权限</span><span class="sxs-lookup"><span data-stu-id="9e0b0-105">Permissions</span></span>
<span data-ttu-id="9e0b0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9e0b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9e0b0-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="9e0b0-108">Permission type</span></span>      | <span data-ttu-id="9e0b0-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9e0b0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9e0b0-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9e0b0-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="9e0b0-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9e0b0-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9e0b0-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9e0b0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e0b0-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="9e0b0-113">Not supported.</span></span>    |
|<span data-ttu-id="9e0b0-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="9e0b0-114">Application</span></span> | <span data-ttu-id="9e0b0-115">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="9e0b0-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9e0b0-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9e0b0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /applications/{id}
```
## <a name="request-headers"></a><span data-ttu-id="9e0b0-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="9e0b0-117">Request headers</span></span>
| <span data-ttu-id="9e0b0-118">名称</span><span class="sxs-lookup"><span data-stu-id="9e0b0-118">Name</span></span>       | <span data-ttu-id="9e0b0-119">类型</span><span class="sxs-lookup"><span data-stu-id="9e0b0-119">Type</span></span> | <span data-ttu-id="9e0b0-120">说明</span><span class="sxs-lookup"><span data-stu-id="9e0b0-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9e0b0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e0b0-121">Authorization</span></span>  | <span data-ttu-id="9e0b0-122">string</span><span class="sxs-lookup"><span data-stu-id="9e0b0-122">string</span></span>  | <span data-ttu-id="9e0b0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9e0b0-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9e0b0-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="9e0b0-125">Request body</span></span>
<span data-ttu-id="9e0b0-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="9e0b0-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9e0b0-129">属性</span><span class="sxs-lookup"><span data-stu-id="9e0b0-129">Property</span></span>     | <span data-ttu-id="9e0b0-130">类型</span><span class="sxs-lookup"><span data-stu-id="9e0b0-130">Type</span></span>   |<span data-ttu-id="9e0b0-131">说明</span><span class="sxs-lookup"><span data-stu-id="9e0b0-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9e0b0-132">allowPublicClient</span><span class="sxs-lookup"><span data-stu-id="9e0b0-132">allowPublicClient</span></span>|<span data-ttu-id="9e0b0-133">布尔值</span><span class="sxs-lookup"><span data-stu-id="9e0b0-133">Boolean</span></span>| <span data-ttu-id="9e0b0-134">指定应用程序可用作公共客户端。</span><span class="sxs-lookup"><span data-stu-id="9e0b0-134">Specifies if the application can act as a public client.</span></span> <span data-ttu-id="9e0b0-135">例如，移动设备上运行安装的应用程序。</span><span class="sxs-lookup"><span data-stu-id="9e0b0-135">For example,  an installed application running on a mobile device.</span></span> <span data-ttu-id="9e0b0-136">默认值为 *false*。</span><span class="sxs-lookup"><span data-stu-id="9e0b0-136">Default value is *false*.</span></span> |
|<span data-ttu-id="9e0b0-137">api</span><span class="sxs-lookup"><span data-stu-id="9e0b0-137">api</span></span>|[<span data-ttu-id="9e0b0-138">api</span><span class="sxs-lookup"><span data-stu-id="9e0b0-138">api</span></span>](../resources/api.md)| <span data-ttu-id="9e0b0-139">指定 API 应用程序的设置。</span><span class="sxs-lookup"><span data-stu-id="9e0b0-139">Specifies settings for an API application.</span></span> |
|<span data-ttu-id="9e0b0-140">appRoles</span><span class="sxs-lookup"><span data-stu-id="9e0b0-140">appRoles</span></span>|<span data-ttu-id="9e0b0-141">[appRole](../resources/approle.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9e0b0-141">[appRole](../resources/approle.md) collection</span></span>|<span data-ttu-id="9e0b0-142">应用程序可声明的应用程序角色的集合。</span><span class="sxs-lookup"><span data-stu-id="9e0b0-142">The collection of application roles that an application may declare.</span></span> <span data-ttu-id="9e0b0-143">这些角色可以分配给用户、组或服务主体。</span><span class="sxs-lookup"><span data-stu-id="9e0b0-143">These roles can be assigned to users, groups, or service principals.</span></span> <span data-ttu-id="9e0b0-144">不可为 Null。</span><span class="sxs-lookup"><span data-stu-id="9e0b0-144">Not nullable.</span></span>|
|<span data-ttu-id="9e0b0-145">applicationAliases</span><span class="sxs-lookup"><span data-stu-id="9e0b0-145">applicationAliases</span></span>|<span data-ttu-id="9e0b0-146">String 集合</span><span class="sxs-lookup"><span data-stu-id="9e0b0-146">String collection</span></span>| <span data-ttu-id="9e0b0-147">用于标识应用程序的 URI。</span><span class="sxs-lookup"><span data-stu-id="9e0b0-147">The URIs that identify the application.</span></span> <span data-ttu-id="9e0b0-148">有关详细信息，请参阅[应用程序对象和服务主体对象](https://azure.microsoft.com/documentation/articles/active-directory-application-objects/)。</span><span class="sxs-lookup"><span data-stu-id="9e0b0-148">For more information see, [Application Objects and Service Principal Objects](https://azure.microsoft.com/documentation/articles/active-directory-application-objects/).</span></span> <span data-ttu-id="9e0b0-149">多值属性筛选器表达式需要 *any* 运算符。</span><span class="sxs-lookup"><span data-stu-id="9e0b0-149">The *any* operator is required for filter expressions on multi-valued properties.</span></span> <span data-ttu-id="9e0b0-150">不可为 Null。</span><span class="sxs-lookup"><span data-stu-id="9e0b0-150">Not nullable.</span></span> |
|<span data-ttu-id="9e0b0-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9e0b0-151">createdDateTime</span></span>|<span data-ttu-id="9e0b0-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e0b0-152">DateTimeOffset</span></span>| <span data-ttu-id="9e0b0-153">注册应用程序的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9e0b0-153">The date and time the application was registered.</span></span> |
|<span data-ttu-id="9e0b0-154">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="9e0b0-154">deletedDateTime</span></span>|<span data-ttu-id="9e0b0-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e0b0-155">DateTimeOffset</span></span>| <span data-ttu-id="9e0b0-156">删除应用程序的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9e0b0-156">The date and time the application was deleted.</span></span> |
|<span data-ttu-id="9e0b0-157">displayName</span><span class="sxs-lookup"><span data-stu-id="9e0b0-157">displayName</span></span>|<span data-ttu-id="9e0b0-158">String</span><span class="sxs-lookup"><span data-stu-id="9e0b0-158">String</span></span>|<span data-ttu-id="9e0b0-159">应用程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="9e0b0-159">The display name for the application.</span></span> |
|<span data-ttu-id="9e0b0-160">id</span><span class="sxs-lookup"><span data-stu-id="9e0b0-160">id</span></span>|<span data-ttu-id="9e0b0-161">String</span><span class="sxs-lookup"><span data-stu-id="9e0b0-161">String</span></span>|<span data-ttu-id="9e0b0-162">应用程序的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="9e0b0-162">The unique identifier for the application.</span></span> <span data-ttu-id="9e0b0-163">继承自 [directoryObject](../resources/directoryobject.md)。</span><span class="sxs-lookup"><span data-stu-id="9e0b0-163">Inherited from [directoryObject](../resources/directoryobject.md).</span></span> <span data-ttu-id="9e0b0-164">键。</span><span class="sxs-lookup"><span data-stu-id="9e0b0-164">Key.</span></span> <span data-ttu-id="9e0b0-165">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="9e0b0-165">Not nullable.</span></span> <span data-ttu-id="9e0b0-166">只读。</span><span class="sxs-lookup"><span data-stu-id="9e0b0-166">Read-only.</span></span> |
|<span data-ttu-id="9e0b0-167">info</span><span class="sxs-lookup"><span data-stu-id="9e0b0-167">info</span></span>|[<span data-ttu-id="9e0b0-168">informationalUrl</span><span class="sxs-lookup"><span data-stu-id="9e0b0-168">informationalUrl</span></span>](../resources/informationalurl.md)| <span data-ttu-id="9e0b0-169">应用程序的基本配置文件信息。</span><span class="sxs-lookup"><span data-stu-id="9e0b0-169">Basic profile information of the application.</span></span> | <span data-ttu-id="9e0b0-170">指定已安装客户端（如台式设备或移动设备）的设置。</span><span class="sxs-lookup"><span data-stu-id="9e0b0-170">Specifies settings for installed clients such as desktop or mobile devices.</span></span> |
|<span data-ttu-id="9e0b0-171">keyCredentials</span><span class="sxs-lookup"><span data-stu-id="9e0b0-171">keyCredentials</span></span>|<span data-ttu-id="9e0b0-172">[keyCredential](../resources/keycredential.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9e0b0-172">[keyCredential](../resources/keycredential.md) collection</span></span>|<span data-ttu-id="9e0b0-173">与应用程序关联的密钥凭据集合，不可为 Null。</span><span class="sxs-lookup"><span data-stu-id="9e0b0-173">The collection of key credentials associated with the application Not nullable.</span></span> |
|<span data-ttu-id="9e0b0-174">logo</span><span class="sxs-lookup"><span data-stu-id="9e0b0-174">logo</span></span>|<span data-ttu-id="9e0b0-175">Stream</span><span class="sxs-lookup"><span data-stu-id="9e0b0-175">Stream</span></span>|<span data-ttu-id="9e0b0-176">应用程序的主徽标。</span><span class="sxs-lookup"><span data-stu-id="9e0b0-176">The main logo for the application.</span></span> <span data-ttu-id="9e0b0-177">不可为 Null。</span><span class="sxs-lookup"><span data-stu-id="9e0b0-177">Not nullable.</span></span> |
|<span data-ttu-id="9e0b0-178">orgRestrictions</span><span class="sxs-lookup"><span data-stu-id="9e0b0-178">orgRestrictions</span></span>|<span data-ttu-id="9e0b0-179">String 集合</span><span class="sxs-lookup"><span data-stu-id="9e0b0-179">String collection</span></span>| <span data-ttu-id="9e0b0-180">应用程序所使用的受限组织 tenantIds。</span><span class="sxs-lookup"><span data-stu-id="9e0b0-180">The organizational tenantIds to which the application is restricted.</span></span>  <span data-ttu-id="9e0b0-181">如果集合为空，该应用程序是多租户 （不受限制）。</span><span class="sxs-lookup"><span data-stu-id="9e0b0-181">If the collection is empty, the application is multi-tenant (not restricted).</span></span> <span data-ttu-id="9e0b0-182">如果集合包含 tenantIds，应用程序仅限于组织 tenantIds 集合中。</span><span class="sxs-lookup"><span data-stu-id="9e0b0-182">If the collection contains tenantIds, the application is restricted to the organizational tenantIds in the collection.</span></span> <span data-ttu-id="9e0b0-183">指定其他租户但未注册应用程序其中 tenantId 意味着应用程序自身的 tenantId 为间接包含。</span><span class="sxs-lookup"><span data-stu-id="9e0b0-183">Specifying other tenants but not the tenantId where the application is registered implies that the application's own tenantId is indirectly included.</span></span> |
|<span data-ttu-id="9e0b0-184">passwordCredentials</span><span class="sxs-lookup"><span data-stu-id="9e0b0-184">passwordCredentials</span></span>|<span data-ttu-id="9e0b0-185">[passwordCredential](../resources/passwordcredential.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9e0b0-185">[passwordCredential](../resources/passwordcredential.md) collection</span></span>|<span data-ttu-id="9e0b0-186">与应用程序关联的密码凭据集合。</span><span class="sxs-lookup"><span data-stu-id="9e0b0-186">The collection of password credentials associated with the application.</span></span> <span data-ttu-id="9e0b0-187">不可为 Null。</span><span class="sxs-lookup"><span data-stu-id="9e0b0-187">Not nullable.</span></span>|
|<span data-ttu-id="9e0b0-188">preAuthorizedApplications</span><span class="sxs-lookup"><span data-stu-id="9e0b0-188">preAuthorizedApplications</span></span>|<span data-ttu-id="9e0b0-189">[preAuthorizedApplication](../resources/preauthorizedapplication.md)集合</span><span class="sxs-lookup"><span data-stu-id="9e0b0-189">[preAuthorizedApplication](../resources/preauthorizedapplication.md) collection</span></span>| <span data-ttu-id="9e0b0-190">列出应用程序和隐式同意请求的权限。</span><span class="sxs-lookup"><span data-stu-id="9e0b0-190">Lists applications and requested permissions for implicit consent.</span></span> <span data-ttu-id="9e0b0-191">需要管理员可以提供了到应用程序的许可。</span><span class="sxs-lookup"><span data-stu-id="9e0b0-191">Requires an admin to have provided consent to the application.</span></span> <span data-ttu-id="9e0b0-192">preAuthorizedApplications 不需要用户同意所请求的权限。</span><span class="sxs-lookup"><span data-stu-id="9e0b0-192">preAuthorizedApplications do not require the user to consent to the requested permissions.</span></span> <span data-ttu-id="9e0b0-193">PreAuthorizedApplications 中列出的权限不需要用户同意。</span><span class="sxs-lookup"><span data-stu-id="9e0b0-193">Permissions listed in preAuthorizedApplications do not require user consent.</span></span> <span data-ttu-id="9e0b0-194">但是，preAuthorizedApplications 中未列出任何其他请求的权限要求用户同意。</span><span class="sxs-lookup"><span data-stu-id="9e0b0-194">However, any additional requested permissions not listed in preAuthorizedApplications require user consent.</span></span> |
|<span data-ttu-id="9e0b0-195">requiredResourceAccess</span><span class="sxs-lookup"><span data-stu-id="9e0b0-195">requiredResourceAccess</span></span>|<span data-ttu-id="9e0b0-196">[requiredResourceAccess](../resources/requiredresourceaccess.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9e0b0-196">[requiredResourceAccess](../resources/requiredresourceaccess.md) collection</span></span>|<span data-ttu-id="9e0b0-197">指定此应用程序需要访问的资源以及在每个资源下所需的 OAuth 权限范围和应用程序角色集。</span><span class="sxs-lookup"><span data-stu-id="9e0b0-197">Specifies resources that this application requires access to and the set of OAuth permission scopes and application roles that it needs under each of those resources.</span></span> <span data-ttu-id="9e0b0-198">这种预配置的所需资源访问权限可驱动同意体验。</span><span class="sxs-lookup"><span data-stu-id="9e0b0-198">This pre-configuration of required resource access drives the consent experience.</span></span> <span data-ttu-id="9e0b0-199">不可为 Null。</span><span class="sxs-lookup"><span data-stu-id="9e0b0-199">Not nullable.</span></span>|
|<span data-ttu-id="9e0b0-200">标记</span><span class="sxs-lookup"><span data-stu-id="9e0b0-200">tags</span></span>|<span data-ttu-id="9e0b0-201">String 集合</span><span class="sxs-lookup"><span data-stu-id="9e0b0-201">String collection</span></span>| <span data-ttu-id="9e0b0-202">可用于分类和标识应用程序的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="9e0b0-202">Custom strings that can be used to categorize and identify the application.</span></span> |
|<span data-ttu-id="9e0b0-203">web</span><span class="sxs-lookup"><span data-stu-id="9e0b0-203">web</span></span>|[<span data-ttu-id="9e0b0-204">web</span><span class="sxs-lookup"><span data-stu-id="9e0b0-204">web</span></span>](../resources/web.md)| <span data-ttu-id="9e0b0-205">指定 Web 应用程序的设置。</span><span class="sxs-lookup"><span data-stu-id="9e0b0-205">Specifies settings for a web application.</span></span> |

## <a name="response"></a><span data-ttu-id="9e0b0-206">响应</span><span class="sxs-lookup"><span data-stu-id="9e0b0-206">Response</span></span>

<span data-ttu-id="9e0b0-207">如果成功，此方法返回`204 No Content`响应代码和不响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="9e0b0-207">If successful, this method returns a `204 No Content` response code and does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9e0b0-208">示例</span><span class="sxs-lookup"><span data-stu-id="9e0b0-208">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9e0b0-209">请求</span><span class="sxs-lookup"><span data-stu-id="9e0b0-209">Request</span></span>
<span data-ttu-id="9e0b0-210">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9e0b0-210">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_application"
}-->
```http
PATCH https://graph.microsoft.com/beta/applications/{id}
Content-type: application/json
Content-length: 72

{
  "allowPublicClient": false,
  "displayName": "New display name"
}
```
##### <a name="response"></a><span data-ttu-id="9e0b0-211">响应</span><span class="sxs-lookup"><span data-stu-id="9e0b0-211">Response</span></span>
<span data-ttu-id="9e0b0-212">注意：为简洁起见，可能会截断此处展示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9e0b0-212">Note: The response object shown here may be truncated for brevity.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update application",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/application-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
