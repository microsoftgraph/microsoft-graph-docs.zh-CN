---
title: 更新应用程序
description: 更新应用程序对象的属性。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ecdf1d7f4f291b415e83b3926f8f82ea81f73390
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990703"
---
# <a name="update-application"></a><span data-ttu-id="00850-103">更新应用程序</span><span class="sxs-lookup"><span data-stu-id="00850-103">Update application</span></span>

> <span data-ttu-id="00850-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="00850-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="00850-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="00850-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="00850-106">更新应用程序对象的属性。</span><span class="sxs-lookup"><span data-stu-id="00850-106">Update the properties of application object.</span></span>
## <a name="permissions"></a><span data-ttu-id="00850-107">权限</span><span class="sxs-lookup"><span data-stu-id="00850-107">Permissions</span></span>
<span data-ttu-id="00850-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="00850-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="00850-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="00850-110">Permission type</span></span>      | <span data-ttu-id="00850-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="00850-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="00850-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="00850-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="00850-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="00850-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="00850-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="00850-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00850-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="00850-115">Not supported.</span></span>    |
|<span data-ttu-id="00850-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="00850-116">Application</span></span> | <span data-ttu-id="00850-117">Application.ReadWrite.OwnedBy Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00850-117">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="00850-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="00850-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /applications/{id}
```
## <a name="request-headers"></a><span data-ttu-id="00850-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="00850-119">Request headers</span></span>
| <span data-ttu-id="00850-120">名称</span><span class="sxs-lookup"><span data-stu-id="00850-120">Name</span></span>       | <span data-ttu-id="00850-121">类型</span><span class="sxs-lookup"><span data-stu-id="00850-121">Type</span></span> | <span data-ttu-id="00850-122">说明</span><span class="sxs-lookup"><span data-stu-id="00850-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="00850-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="00850-123">Authorization</span></span>  | <span data-ttu-id="00850-124">string</span><span class="sxs-lookup"><span data-stu-id="00850-124">string</span></span>  | <span data-ttu-id="00850-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="00850-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="00850-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="00850-127">Request body</span></span>
<span data-ttu-id="00850-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="00850-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="00850-131">属性</span><span class="sxs-lookup"><span data-stu-id="00850-131">Property</span></span>     | <span data-ttu-id="00850-132">类型</span><span class="sxs-lookup"><span data-stu-id="00850-132">Type</span></span>   |<span data-ttu-id="00850-133">说明</span><span class="sxs-lookup"><span data-stu-id="00850-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="00850-134">allowPublicClient</span><span class="sxs-lookup"><span data-stu-id="00850-134">allowPublicClient</span></span>|<span data-ttu-id="00850-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="00850-135">Boolean</span></span>| <span data-ttu-id="00850-136">指定应用程序可用作公共客户端。</span><span class="sxs-lookup"><span data-stu-id="00850-136">Specifies if the application can act as a public client.</span></span> <span data-ttu-id="00850-137">例如，移动设备上运行安装的应用程序。</span><span class="sxs-lookup"><span data-stu-id="00850-137">For example,  an installed application running on a mobile device.</span></span> <span data-ttu-id="00850-138">默认值为 *false*。</span><span class="sxs-lookup"><span data-stu-id="00850-138">Default value is *false*.</span></span> |
|<span data-ttu-id="00850-139">api</span><span class="sxs-lookup"><span data-stu-id="00850-139">api</span></span>|[<span data-ttu-id="00850-140">api</span><span class="sxs-lookup"><span data-stu-id="00850-140">api</span></span>](../resources/api.md)| <span data-ttu-id="00850-141">指定 API 应用程序的设置。</span><span class="sxs-lookup"><span data-stu-id="00850-141">Specifies settings for an API application.</span></span> |
|<span data-ttu-id="00850-142">appRoles</span><span class="sxs-lookup"><span data-stu-id="00850-142">appRoles</span></span>|<span data-ttu-id="00850-143">[appRole](../resources/approle.md)集合</span><span class="sxs-lookup"><span data-stu-id="00850-143">[appRole](../resources/approle.md) collection</span></span>|<span data-ttu-id="00850-144">声明应用程序可能的应用程序角色的集合。</span><span class="sxs-lookup"><span data-stu-id="00850-144">The collection of application roles that an application may declare.</span></span> <span data-ttu-id="00850-145">这些角色可以分配给用户、 组或服务主体。</span><span class="sxs-lookup"><span data-stu-id="00850-145">These roles can be assigned to users, groups, or service principals.</span></span> <span data-ttu-id="00850-146">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="00850-146">Not nullable.</span></span>|
|<span data-ttu-id="00850-147">applicationAliases</span><span class="sxs-lookup"><span data-stu-id="00850-147">applicationAliases</span></span>|<span data-ttu-id="00850-148">String 集合</span><span class="sxs-lookup"><span data-stu-id="00850-148">String collection</span></span>| <span data-ttu-id="00850-149">标识应用程序的 Uri。</span><span class="sxs-lookup"><span data-stu-id="00850-149">The URIs that identify the application.</span></span> <span data-ttu-id="00850-150">有关详细信息，请参阅[应用程序对象和服务主体对象](https://azure.microsoft.com/documentation/articles/active-directory-application-objects/)。</span><span class="sxs-lookup"><span data-stu-id="00850-150">For more information see, [Application Objects and Service Principal Objects](https://azure.microsoft.com/documentation/articles/active-directory-application-objects/).</span></span> <span data-ttu-id="00850-151">*Any*运算符，则需要为多值属性的筛选器表达式。</span><span class="sxs-lookup"><span data-stu-id="00850-151">The *any* operator is required for filter expressions on multi-valued properties.</span></span> <span data-ttu-id="00850-152">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="00850-152">Not nullable.</span></span> |
|<span data-ttu-id="00850-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="00850-153">createdDateTime</span></span>|<span data-ttu-id="00850-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00850-154">DateTimeOffset</span></span>| <span data-ttu-id="00850-155">日期和时间注册应用程序。</span><span class="sxs-lookup"><span data-stu-id="00850-155">The date and time the application was registered.</span></span> |
|<span data-ttu-id="00850-156">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="00850-156">deletedDateTime</span></span>|<span data-ttu-id="00850-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00850-157">DateTimeOffset</span></span>| <span data-ttu-id="00850-158">日期和时间的应用程序已删除。</span><span class="sxs-lookup"><span data-stu-id="00850-158">The date and time the application was deleted.</span></span> |
|<span data-ttu-id="00850-159">displayName</span><span class="sxs-lookup"><span data-stu-id="00850-159">displayName</span></span>|<span data-ttu-id="00850-160">字符串</span><span class="sxs-lookup"><span data-stu-id="00850-160">String</span></span>|<span data-ttu-id="00850-161">应用程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="00850-161">The display name for the application.</span></span> |
|<span data-ttu-id="00850-162">id</span><span class="sxs-lookup"><span data-stu-id="00850-162">id</span></span>|<span data-ttu-id="00850-163">字符串</span><span class="sxs-lookup"><span data-stu-id="00850-163">String</span></span>|<span data-ttu-id="00850-164">应用程序的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="00850-164">The unique identifier for the application.</span></span> <span data-ttu-id="00850-165">继承自 [directoryObject](../resources/directoryobject.md)。</span><span class="sxs-lookup"><span data-stu-id="00850-165">Inherited from [directoryObject](../resources/directoryobject.md).</span></span> <span data-ttu-id="00850-166">键。</span><span class="sxs-lookup"><span data-stu-id="00850-166">Key.</span></span> <span data-ttu-id="00850-167">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="00850-167">Not nullable.</span></span> <span data-ttu-id="00850-168">只读。</span><span class="sxs-lookup"><span data-stu-id="00850-168">Read-only.</span></span> |
|<span data-ttu-id="00850-169">信息</span><span class="sxs-lookup"><span data-stu-id="00850-169">info</span></span>|[<span data-ttu-id="00850-170">informationalUrl</span><span class="sxs-lookup"><span data-stu-id="00850-170">informationalUrl</span></span>](../resources/informationalurl.md)| <span data-ttu-id="00850-171">应用程序的基本配置文件信息。</span><span class="sxs-lookup"><span data-stu-id="00850-171">Basic profile information of the application.</span></span> | <span data-ttu-id="00850-172">指定安装客户端，如桌面或移动设备的设置。</span><span class="sxs-lookup"><span data-stu-id="00850-172">Specifies settings for installed clients such as desktop or mobile devices.</span></span> |
|<span data-ttu-id="00850-173">keyCredentials</span><span class="sxs-lookup"><span data-stu-id="00850-173">keyCredentials</span></span>|<span data-ttu-id="00850-174">[keyCredential](../resources/keycredential.md)集合</span><span class="sxs-lookup"><span data-stu-id="00850-174">[keyCredential](../resources/keycredential.md) collection</span></span>|<span data-ttu-id="00850-175">不应用程序关联的关键凭据集合可以为 null。</span><span class="sxs-lookup"><span data-stu-id="00850-175">The collection of key credentials associated with the application Not nullable.</span></span> |
|<span data-ttu-id="00850-176">logo</span><span class="sxs-lookup"><span data-stu-id="00850-176">logo</span></span>|<span data-ttu-id="00850-177">Stream</span><span class="sxs-lookup"><span data-stu-id="00850-177">Stream</span></span>|<span data-ttu-id="00850-178">主应用程序徽标。</span><span class="sxs-lookup"><span data-stu-id="00850-178">The main logo for the application.</span></span> <span data-ttu-id="00850-179">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="00850-179">Not nullable.</span></span> |
|<span data-ttu-id="00850-180">orgRestrictions</span><span class="sxs-lookup"><span data-stu-id="00850-180">orgRestrictions</span></span>|<span data-ttu-id="00850-181">String 集合</span><span class="sxs-lookup"><span data-stu-id="00850-181">String collection</span></span>| <span data-ttu-id="00850-182">应用程序所使用的受限组织 tenantIds。</span><span class="sxs-lookup"><span data-stu-id="00850-182">The organizational tenantIds to which the application is restricted.</span></span>  <span data-ttu-id="00850-183">如果集合为空，该应用程序是多租户 （不受限制）。</span><span class="sxs-lookup"><span data-stu-id="00850-183">If the collection is empty, the application is multi-tenant (not restricted).</span></span> <span data-ttu-id="00850-184">如果集合包含 tenantIds，应用程序仅限于组织 tenantIds 集合中。</span><span class="sxs-lookup"><span data-stu-id="00850-184">If the collection contains tenantIds, the application is restricted to the organizational tenantIds in the collection.</span></span> <span data-ttu-id="00850-185">指定其他租户但未注册应用程序其中 tenantId 意味着应用程序自身的 tenantId 为间接包含。</span><span class="sxs-lookup"><span data-stu-id="00850-185">Specifying other tenants but not the tenantId where the application is registered implies that the application's own tenantId is indirectly included.</span></span> |
|<span data-ttu-id="00850-186">passwordCredentials</span><span class="sxs-lookup"><span data-stu-id="00850-186">passwordCredentials</span></span>|<span data-ttu-id="00850-187">[passwordCredential](../resources/passwordcredential.md)集合</span><span class="sxs-lookup"><span data-stu-id="00850-187">[passwordCredential](../resources/passwordcredential.md) collection</span></span>|<span data-ttu-id="00850-188">应用程序关联的密码凭据的集合。</span><span class="sxs-lookup"><span data-stu-id="00850-188">The collection of password credentials associated with the application.</span></span> <span data-ttu-id="00850-189">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="00850-189">Not nullable.</span></span>|
|<span data-ttu-id="00850-190">preAuthorizedApplications</span><span class="sxs-lookup"><span data-stu-id="00850-190">preAuthorizedApplications</span></span>|<span data-ttu-id="00850-191">[preAuthorizedApplication](../resources/preauthorizedapplication.md)集合</span><span class="sxs-lookup"><span data-stu-id="00850-191">[preAuthorizedApplication](../resources/preauthorizedapplication.md) collection</span></span>| <span data-ttu-id="00850-192">列出应用程序和隐式同意请求的权限。</span><span class="sxs-lookup"><span data-stu-id="00850-192">Lists applications and requested permissions for implicit consent.</span></span> <span data-ttu-id="00850-193">需要管理员可以提供了到应用程序的许可。</span><span class="sxs-lookup"><span data-stu-id="00850-193">Requires an admin to have provided consent to the application.</span></span> <span data-ttu-id="00850-194">preAuthorizedApplications 不需要用户同意所请求的权限。</span><span class="sxs-lookup"><span data-stu-id="00850-194">preAuthorizedApplications do not require the user to consent to the requested permissions.</span></span> <span data-ttu-id="00850-195">PreAuthorizedApplications 中列出的权限不需要用户同意。</span><span class="sxs-lookup"><span data-stu-id="00850-195">Permissions listed in preAuthorizedApplications do not require user consent.</span></span> <span data-ttu-id="00850-196">但是，preAuthorizedApplications 中未列出任何其他请求的权限要求用户同意。</span><span class="sxs-lookup"><span data-stu-id="00850-196">However, any additional requested permissions not listed in preAuthorizedApplications require user consent.</span></span> |
|<span data-ttu-id="00850-197">requiredResourceAccess</span><span class="sxs-lookup"><span data-stu-id="00850-197">requiredResourceAccess</span></span>|<span data-ttu-id="00850-198">[requiredResourceAccess](../resources/requiredresourceaccess.md)集合</span><span class="sxs-lookup"><span data-stu-id="00850-198">[requiredResourceAccess](../resources/requiredresourceaccess.md) collection</span></span>|<span data-ttu-id="00850-199">指定此应用程序需要访问和一组的 OAuth 权限范围和应用程序角色它需要在每个这些资源的资源。</span><span class="sxs-lookup"><span data-stu-id="00850-199">Specifies resources that this application requires access to and the set of OAuth permission scopes and application roles that it needs under each of those resources.</span></span> <span data-ttu-id="00850-200">此预配置完所需的资源访问驱动器的同意体验。</span><span class="sxs-lookup"><span data-stu-id="00850-200">This pre-configuration of required resource access drives the consent experience.</span></span> <span data-ttu-id="00850-201">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="00850-201">Not nullable.</span></span>|
|<span data-ttu-id="00850-202">标记前添加的标记</span><span class="sxs-lookup"><span data-stu-id="00850-202">tags</span></span>|<span data-ttu-id="00850-203">String 集合</span><span class="sxs-lookup"><span data-stu-id="00850-203">String collection</span></span>| <span data-ttu-id="00850-204">用于分类和确定应用程序的自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="00850-204">Custom strings that can be used to categorize and identify the application.</span></span> |
|<span data-ttu-id="00850-205">web</span><span class="sxs-lookup"><span data-stu-id="00850-205">web</span></span>|[<span data-ttu-id="00850-206">web</span><span class="sxs-lookup"><span data-stu-id="00850-206">web</span></span>](../resources/web.md)| <span data-ttu-id="00850-207">指定 web 应用程序的设置。</span><span class="sxs-lookup"><span data-stu-id="00850-207">Specifies settings for a web application.</span></span> |

## <a name="response"></a><span data-ttu-id="00850-208">响应</span><span class="sxs-lookup"><span data-stu-id="00850-208">Response</span></span>

<span data-ttu-id="00850-209">如果成功，此方法返回`204 No Content`响应代码和不响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="00850-209">If successful, this method returns a `204 No Content` response code and does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="00850-210">示例</span><span class="sxs-lookup"><span data-stu-id="00850-210">Example</span></span>
##### <a name="request"></a><span data-ttu-id="00850-211">请求</span><span class="sxs-lookup"><span data-stu-id="00850-211">Request</span></span>
<span data-ttu-id="00850-212">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="00850-212">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="00850-213">响应</span><span class="sxs-lookup"><span data-stu-id="00850-213">Response</span></span>
<span data-ttu-id="00850-214">注意：为简洁起见，可能会截断此处展示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="00850-214">Note: The response object shown here may be truncated for brevity.</span></span> 
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
<!-- {
  "type": "#page.annotation",
  "description": "Update application",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
