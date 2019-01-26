---
title: 更新应用程序
description: 更新应用程序对象的属性。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9965a46e340063940e1a9af18a89ada7e492bf26
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572211"
---
# <a name="update-application"></a><span data-ttu-id="3c3b7-103">更新应用程序</span><span class="sxs-lookup"><span data-stu-id="3c3b7-103">Update application</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c3b7-104">更新应用程序对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3c3b7-104">Update the properties of application object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3c3b7-105">权限</span><span class="sxs-lookup"><span data-stu-id="3c3b7-105">Permissions</span></span>
<span data-ttu-id="3c3b7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3c3b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="3c3b7-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="3c3b7-108">Permission type</span></span>      | <span data-ttu-id="3c3b7-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3c3b7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3c3b7-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3c3b7-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="3c3b7-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3c3b7-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3c3b7-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3c3b7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c3b7-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="3c3b7-113">Not supported.</span></span>    |
|<span data-ttu-id="3c3b7-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="3c3b7-114">Application</span></span> | <span data-ttu-id="3c3b7-115">Application.ReadWrite.OwnedBy Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c3b7-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3c3b7-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3c3b7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /applications/{id}
```
## <a name="request-headers"></a><span data-ttu-id="3c3b7-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="3c3b7-117">Request headers</span></span>
| <span data-ttu-id="3c3b7-118">名称</span><span class="sxs-lookup"><span data-stu-id="3c3b7-118">Name</span></span>       | <span data-ttu-id="3c3b7-119">类型</span><span class="sxs-lookup"><span data-stu-id="3c3b7-119">Type</span></span> | <span data-ttu-id="3c3b7-120">说明</span><span class="sxs-lookup"><span data-stu-id="3c3b7-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3c3b7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c3b7-121">Authorization</span></span>  | <span data-ttu-id="3c3b7-122">string</span><span class="sxs-lookup"><span data-stu-id="3c3b7-122">string</span></span>  | <span data-ttu-id="3c3b7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3c3b7-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3c3b7-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="3c3b7-125">Request body</span></span>
<span data-ttu-id="3c3b7-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="3c3b7-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3c3b7-129">属性</span><span class="sxs-lookup"><span data-stu-id="3c3b7-129">Property</span></span>     | <span data-ttu-id="3c3b7-130">类型</span><span class="sxs-lookup"><span data-stu-id="3c3b7-130">Type</span></span>   |<span data-ttu-id="3c3b7-131">说明</span><span class="sxs-lookup"><span data-stu-id="3c3b7-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3c3b7-132">allowPublicClient</span><span class="sxs-lookup"><span data-stu-id="3c3b7-132">allowPublicClient</span></span>|<span data-ttu-id="3c3b7-133">布尔值</span><span class="sxs-lookup"><span data-stu-id="3c3b7-133">Boolean</span></span>| <span data-ttu-id="3c3b7-134">指定应用程序可用作公共客户端。</span><span class="sxs-lookup"><span data-stu-id="3c3b7-134">Specifies if the application can act as a public client.</span></span> <span data-ttu-id="3c3b7-135">例如，移动设备上运行安装的应用程序。</span><span class="sxs-lookup"><span data-stu-id="3c3b7-135">For example,  an installed application running on a mobile device.</span></span> <span data-ttu-id="3c3b7-136">默认值为 *false*。</span><span class="sxs-lookup"><span data-stu-id="3c3b7-136">Default value is *false*.</span></span> |
|<span data-ttu-id="3c3b7-137">api</span><span class="sxs-lookup"><span data-stu-id="3c3b7-137">api</span></span>|[<span data-ttu-id="3c3b7-138">api</span><span class="sxs-lookup"><span data-stu-id="3c3b7-138">api</span></span>](../resources/api.md)| <span data-ttu-id="3c3b7-139">指定 API 应用程序的设置。</span><span class="sxs-lookup"><span data-stu-id="3c3b7-139">Specifies settings for an API application.</span></span> |
|<span data-ttu-id="3c3b7-140">appRoles</span><span class="sxs-lookup"><span data-stu-id="3c3b7-140">appRoles</span></span>|<span data-ttu-id="3c3b7-141">[appRole](../resources/approle.md)集合</span><span class="sxs-lookup"><span data-stu-id="3c3b7-141">[appRole](../resources/approle.md) collection</span></span>|<span data-ttu-id="3c3b7-142">声明应用程序可能的应用程序角色的集合。</span><span class="sxs-lookup"><span data-stu-id="3c3b7-142">The collection of application roles that an application may declare.</span></span> <span data-ttu-id="3c3b7-143">这些角色可以分配给用户、 组或服务主体。</span><span class="sxs-lookup"><span data-stu-id="3c3b7-143">These roles can be assigned to users, groups, or service principals.</span></span> <span data-ttu-id="3c3b7-144">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="3c3b7-144">Not nullable.</span></span>|
|<span data-ttu-id="3c3b7-145">applicationAliases</span><span class="sxs-lookup"><span data-stu-id="3c3b7-145">applicationAliases</span></span>|<span data-ttu-id="3c3b7-146">String 集合</span><span class="sxs-lookup"><span data-stu-id="3c3b7-146">String collection</span></span>| <span data-ttu-id="3c3b7-147">标识应用程序的 Uri。</span><span class="sxs-lookup"><span data-stu-id="3c3b7-147">The URIs that identify the application.</span></span> <span data-ttu-id="3c3b7-148">有关详细信息，请参阅[应用程序对象和服务主体对象](https://azure.microsoft.com/documentation/articles/active-directory-application-objects/)。</span><span class="sxs-lookup"><span data-stu-id="3c3b7-148">For more information see, [Application Objects and Service Principal Objects](https://azure.microsoft.com/documentation/articles/active-directory-application-objects/).</span></span> <span data-ttu-id="3c3b7-149">需要多值属性筛选器表达式的 *any* 运算符。</span><span class="sxs-lookup"><span data-stu-id="3c3b7-149">The *any* operator is required for filter expressions on multi-valued properties.</span></span> <span data-ttu-id="3c3b7-150">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="3c3b7-150">Not nullable.</span></span> |
|<span data-ttu-id="3c3b7-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3c3b7-151">createdDateTime</span></span>|<span data-ttu-id="3c3b7-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c3b7-152">DateTimeOffset</span></span>| <span data-ttu-id="3c3b7-153">日期和时间注册应用程序。</span><span class="sxs-lookup"><span data-stu-id="3c3b7-153">The date and time the application was registered.</span></span> |
|<span data-ttu-id="3c3b7-154">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="3c3b7-154">deletedDateTime</span></span>|<span data-ttu-id="3c3b7-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c3b7-155">DateTimeOffset</span></span>| <span data-ttu-id="3c3b7-156">日期和时间的应用程序已删除。</span><span class="sxs-lookup"><span data-stu-id="3c3b7-156">The date and time the application was deleted.</span></span> |
|<span data-ttu-id="3c3b7-157">displayName</span><span class="sxs-lookup"><span data-stu-id="3c3b7-157">displayName</span></span>|<span data-ttu-id="3c3b7-158">String</span><span class="sxs-lookup"><span data-stu-id="3c3b7-158">String</span></span>|<span data-ttu-id="3c3b7-159">应用程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="3c3b7-159">The display name for the application.</span></span> |
|<span data-ttu-id="3c3b7-160">id</span><span class="sxs-lookup"><span data-stu-id="3c3b7-160">id</span></span>|<span data-ttu-id="3c3b7-161">String</span><span class="sxs-lookup"><span data-stu-id="3c3b7-161">String</span></span>|<span data-ttu-id="3c3b7-162">应用程序的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="3c3b7-162">The unique identifier for the application.</span></span> <span data-ttu-id="3c3b7-163">继承自 [directoryObject](../resources/directoryobject.md)。</span><span class="sxs-lookup"><span data-stu-id="3c3b7-163">Inherited from [directoryObject](../resources/directoryobject.md).</span></span> <span data-ttu-id="3c3b7-164">键。</span><span class="sxs-lookup"><span data-stu-id="3c3b7-164">Key.</span></span> <span data-ttu-id="3c3b7-165">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="3c3b7-165">Not nullable.</span></span> <span data-ttu-id="3c3b7-166">只读。</span><span class="sxs-lookup"><span data-stu-id="3c3b7-166">Read-only.</span></span> |
|<span data-ttu-id="3c3b7-167">信息</span><span class="sxs-lookup"><span data-stu-id="3c3b7-167">info</span></span>|[<span data-ttu-id="3c3b7-168">informationalUrl</span><span class="sxs-lookup"><span data-stu-id="3c3b7-168">informationalUrl</span></span>](../resources/informationalurl.md)| <span data-ttu-id="3c3b7-169">应用程序的基本配置文件信息。</span><span class="sxs-lookup"><span data-stu-id="3c3b7-169">Basic profile information of the application.</span></span> | <span data-ttu-id="3c3b7-170">指定安装客户端，如桌面或移动设备的设置。</span><span class="sxs-lookup"><span data-stu-id="3c3b7-170">Specifies settings for installed clients such as desktop or mobile devices.</span></span> |
|<span data-ttu-id="3c3b7-171">keyCredentials</span><span class="sxs-lookup"><span data-stu-id="3c3b7-171">keyCredentials</span></span>|<span data-ttu-id="3c3b7-172">[keyCredential](../resources/keycredential.md)集合</span><span class="sxs-lookup"><span data-stu-id="3c3b7-172">[keyCredential](../resources/keycredential.md) collection</span></span>|<span data-ttu-id="3c3b7-173">不应用程序关联的关键凭据集合可以为 null。</span><span class="sxs-lookup"><span data-stu-id="3c3b7-173">The collection of key credentials associated with the application Not nullable.</span></span> |
|<span data-ttu-id="3c3b7-174">logo</span><span class="sxs-lookup"><span data-stu-id="3c3b7-174">logo</span></span>|<span data-ttu-id="3c3b7-175">Stream</span><span class="sxs-lookup"><span data-stu-id="3c3b7-175">Stream</span></span>|<span data-ttu-id="3c3b7-176">主应用程序徽标。</span><span class="sxs-lookup"><span data-stu-id="3c3b7-176">The main logo for the application.</span></span> <span data-ttu-id="3c3b7-177">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="3c3b7-177">Not nullable.</span></span> |
|<span data-ttu-id="3c3b7-178">orgRestrictions</span><span class="sxs-lookup"><span data-stu-id="3c3b7-178">orgRestrictions</span></span>|<span data-ttu-id="3c3b7-179">String 集合</span><span class="sxs-lookup"><span data-stu-id="3c3b7-179">String collection</span></span>| <span data-ttu-id="3c3b7-180">应用程序所使用的受限组织 tenantIds。</span><span class="sxs-lookup"><span data-stu-id="3c3b7-180">The organizational tenantIds to which the application is restricted.</span></span>  <span data-ttu-id="3c3b7-181">如果集合为空，该应用程序是多租户 （不受限制）。</span><span class="sxs-lookup"><span data-stu-id="3c3b7-181">If the collection is empty, the application is multi-tenant (not restricted).</span></span> <span data-ttu-id="3c3b7-182">如果集合包含 tenantIds，应用程序仅限于组织 tenantIds 集合中。</span><span class="sxs-lookup"><span data-stu-id="3c3b7-182">If the collection contains tenantIds, the application is restricted to the organizational tenantIds in the collection.</span></span> <span data-ttu-id="3c3b7-183">指定其他租户但未注册应用程序其中 tenantId 意味着应用程序自身的 tenantId 为间接包含。</span><span class="sxs-lookup"><span data-stu-id="3c3b7-183">Specifying other tenants but not the tenantId where the application is registered implies that the application's own tenantId is indirectly included.</span></span> |
|<span data-ttu-id="3c3b7-184">passwordCredentials</span><span class="sxs-lookup"><span data-stu-id="3c3b7-184">passwordCredentials</span></span>|<span data-ttu-id="3c3b7-185">[passwordCredential](../resources/passwordcredential.md)集合</span><span class="sxs-lookup"><span data-stu-id="3c3b7-185">[passwordCredential](../resources/passwordcredential.md) collection</span></span>|<span data-ttu-id="3c3b7-186">应用程序关联的密码凭据的集合。</span><span class="sxs-lookup"><span data-stu-id="3c3b7-186">The collection of password credentials associated with the application.</span></span> <span data-ttu-id="3c3b7-187">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="3c3b7-187">Not nullable.</span></span>|
|<span data-ttu-id="3c3b7-188">preAuthorizedApplications</span><span class="sxs-lookup"><span data-stu-id="3c3b7-188">preAuthorizedApplications</span></span>|<span data-ttu-id="3c3b7-189">[preAuthorizedApplication](../resources/preauthorizedapplication.md)集合</span><span class="sxs-lookup"><span data-stu-id="3c3b7-189">[preAuthorizedApplication](../resources/preauthorizedapplication.md) collection</span></span>| <span data-ttu-id="3c3b7-190">列出应用程序和隐式同意请求的权限。</span><span class="sxs-lookup"><span data-stu-id="3c3b7-190">Lists applications and requested permissions for implicit consent.</span></span> <span data-ttu-id="3c3b7-191">需要管理员可以提供了到应用程序的许可。</span><span class="sxs-lookup"><span data-stu-id="3c3b7-191">Requires an admin to have provided consent to the application.</span></span> <span data-ttu-id="3c3b7-192">preAuthorizedApplications 不需要用户同意所请求的权限。</span><span class="sxs-lookup"><span data-stu-id="3c3b7-192">preAuthorizedApplications do not require the user to consent to the requested permissions.</span></span> <span data-ttu-id="3c3b7-193">PreAuthorizedApplications 中列出的权限不需要用户同意。</span><span class="sxs-lookup"><span data-stu-id="3c3b7-193">Permissions listed in preAuthorizedApplications do not require user consent.</span></span> <span data-ttu-id="3c3b7-194">但是，preAuthorizedApplications 中未列出任何其他请求的权限要求用户同意。</span><span class="sxs-lookup"><span data-stu-id="3c3b7-194">However, any additional requested permissions not listed in preAuthorizedApplications require user consent.</span></span> |
|<span data-ttu-id="3c3b7-195">requiredResourceAccess</span><span class="sxs-lookup"><span data-stu-id="3c3b7-195">requiredResourceAccess</span></span>|<span data-ttu-id="3c3b7-196">[requiredResourceAccess](../resources/requiredresourceaccess.md)集合</span><span class="sxs-lookup"><span data-stu-id="3c3b7-196">[requiredResourceAccess](../resources/requiredresourceaccess.md) collection</span></span>|<span data-ttu-id="3c3b7-197">指定此应用程序需要访问和一组的 OAuth 权限范围和应用程序角色它需要在每个这些资源的资源。</span><span class="sxs-lookup"><span data-stu-id="3c3b7-197">Specifies resources that this application requires access to and the set of OAuth permission scopes and application roles that it needs under each of those resources.</span></span> <span data-ttu-id="3c3b7-198">此预配置完所需的资源访问驱动器的同意体验。</span><span class="sxs-lookup"><span data-stu-id="3c3b7-198">This pre-configuration of required resource access drives the consent experience.</span></span> <span data-ttu-id="3c3b7-199">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="3c3b7-199">Not nullable.</span></span>|
|<span data-ttu-id="3c3b7-200">标记</span><span class="sxs-lookup"><span data-stu-id="3c3b7-200">tags</span></span>|<span data-ttu-id="3c3b7-201">String 集合</span><span class="sxs-lookup"><span data-stu-id="3c3b7-201">String collection</span></span>| <span data-ttu-id="3c3b7-202">用于分类和确定应用程序的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="3c3b7-202">Custom strings that can be used to categorize and identify the application.</span></span> |
|<span data-ttu-id="3c3b7-203">web</span><span class="sxs-lookup"><span data-stu-id="3c3b7-203">web</span></span>|[<span data-ttu-id="3c3b7-204">web 应用程序</span><span class="sxs-lookup"><span data-stu-id="3c3b7-204">webApplication</span></span>](../resources/web.md)| <span data-ttu-id="3c3b7-205">指定 web 应用程序的设置。</span><span class="sxs-lookup"><span data-stu-id="3c3b7-205">Specifies settings for a web application.</span></span> |

## <a name="response"></a><span data-ttu-id="3c3b7-206">响应</span><span class="sxs-lookup"><span data-stu-id="3c3b7-206">Response</span></span>

<span data-ttu-id="3c3b7-207">如果成功，此方法返回`204 No Content`响应代码和不响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="3c3b7-207">If successful, this method returns a `204 No Content` response code and does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3c3b7-208">示例</span><span class="sxs-lookup"><span data-stu-id="3c3b7-208">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3c3b7-209">请求</span><span class="sxs-lookup"><span data-stu-id="3c3b7-209">Request</span></span>
<span data-ttu-id="3c3b7-210">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3c3b7-210">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="3c3b7-211">响应</span><span class="sxs-lookup"><span data-stu-id="3c3b7-211">Response</span></span>
<span data-ttu-id="3c3b7-212">注意：为简洁起见，可能会截断此处展示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3c3b7-212">Note: The response object shown here may be truncated for brevity.</span></span> 
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
