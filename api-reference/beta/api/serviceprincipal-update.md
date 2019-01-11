---
title: 更新 serviceprincipal
description: 更新 serviceprincipal 对象的属性。
localization_priority: Normal
ms.openlocfilehash: a8d4eebe64ac9c0c658ae9c43e2e92045be67424
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813025"
---
# <a name="update-serviceprincipal"></a><span data-ttu-id="b7235-103">更新 serviceprincipal</span><span class="sxs-lookup"><span data-stu-id="b7235-103">Update serviceprincipal</span></span>

> <span data-ttu-id="b7235-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b7235-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b7235-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b7235-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b7235-106">更新 serviceprincipal 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b7235-106">Update the properties of serviceprincipal object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b7235-107">权限</span><span class="sxs-lookup"><span data-stu-id="b7235-107">Permissions</span></span>
<span data-ttu-id="b7235-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b7235-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7235-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b7235-110">Permission type</span></span>      | <span data-ttu-id="b7235-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b7235-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b7235-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b7235-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b7235-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b7235-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b7235-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b7235-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7235-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b7235-115">Not supported.</span></span>    |
|<span data-ttu-id="b7235-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b7235-116">Application</span></span> | <span data-ttu-id="b7235-117">Application.ReadWrite.OwnedBy Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7235-117">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b7235-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b7235-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /servicePrincipals/{id}
```
## <a name="request-headers"></a><span data-ttu-id="b7235-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b7235-119">Request headers</span></span>
| <span data-ttu-id="b7235-120">名称</span><span class="sxs-lookup"><span data-stu-id="b7235-120">Name</span></span>       | <span data-ttu-id="b7235-121">类型</span><span class="sxs-lookup"><span data-stu-id="b7235-121">Type</span></span> | <span data-ttu-id="b7235-122">说明</span><span class="sxs-lookup"><span data-stu-id="b7235-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b7235-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b7235-123">Authorization</span></span>  | <span data-ttu-id="b7235-124">string</span><span class="sxs-lookup"><span data-stu-id="b7235-124">string</span></span>  | <span data-ttu-id="b7235-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b7235-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b7235-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b7235-127">Request body</span></span>
<span data-ttu-id="b7235-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="b7235-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b7235-131">属性</span><span class="sxs-lookup"><span data-stu-id="b7235-131">Property</span></span>     | <span data-ttu-id="b7235-132">类型</span><span class="sxs-lookup"><span data-stu-id="b7235-132">Type</span></span>   |<span data-ttu-id="b7235-133">说明</span><span class="sxs-lookup"><span data-stu-id="b7235-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b7235-134">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="b7235-134">accountEnabled</span></span>|<span data-ttu-id="b7235-135">布尔</span><span class="sxs-lookup"><span data-stu-id="b7235-135">Boolean</span></span>|                <span data-ttu-id="b7235-136">**true**如果已启用的服务主体帐户;否则为**false**。</span><span class="sxs-lookup"><span data-stu-id="b7235-136">**true** if the service principal account is enabled; otherwise, **false**.</span></span>            |
|<span data-ttu-id="b7235-137">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="b7235-137">appDisplayName</span></span>|<span data-ttu-id="b7235-138">字符串</span><span class="sxs-lookup"><span data-stu-id="b7235-138">String</span></span>|<span data-ttu-id="b7235-139">通过关联的应用程序公开的显示名称。</span><span class="sxs-lookup"><span data-stu-id="b7235-139">The display name exposed by the associated application.</span></span>|
|<span data-ttu-id="b7235-140">appId</span><span class="sxs-lookup"><span data-stu-id="b7235-140">appId</span></span>|<span data-ttu-id="b7235-141">String</span><span class="sxs-lookup"><span data-stu-id="b7235-141">String</span></span>|<span data-ttu-id="b7235-142">关联的应用程序 （其**appId**属性） 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="b7235-142">The unique identifier for the associated application (its **appId** property).</span></span>|
|<span data-ttu-id="b7235-143">appRoleAssignmentRequired</span><span class="sxs-lookup"><span data-stu-id="b7235-143">appRoleAssignmentRequired</span></span>|<span data-ttu-id="b7235-144">布尔</span><span class="sxs-lookup"><span data-stu-id="b7235-144">Boolean</span></span>|<span data-ttu-id="b7235-145">指定 Azure AD 将问题的用户或访问令牌对应用程序之前是否需要向用户或组**appRoleAssignment** 。</span><span class="sxs-lookup"><span data-stu-id="b7235-145">Specifies whether an **appRoleAssignment** to a user or group is required before Azure AD will issue a user or access token to the application.</span></span>                            <span data-ttu-id="b7235-146">**说明**： 需要 1.5 版或更高版本，不可为空。</span><span class="sxs-lookup"><span data-stu-id="b7235-146">**Notes**: Requires version 1.5 or newer, not nullable.</span></span>            |
|<span data-ttu-id="b7235-147">appRoles</span><span class="sxs-lookup"><span data-stu-id="b7235-147">appRoles</span></span>|<span data-ttu-id="b7235-148">appRole</span><span class="sxs-lookup"><span data-stu-id="b7235-148">appRole</span></span>|<span data-ttu-id="b7235-149">由关联的应用程序公开应用程序角色。</span><span class="sxs-lookup"><span data-stu-id="b7235-149">The application roles exposed by the associated application.</span></span> <span data-ttu-id="b7235-150">有关详细信息看到**appRoles**属性定义应用程序实体**注释**： 需要 1.5 版或更高版本，不可为空。</span><span class="sxs-lookup"><span data-stu-id="b7235-150">For more information see the **appRoles** property definition on the application entity                            **Notes**: Requires version 1.5 or newer, not nullable.</span></span>            |
|<span data-ttu-id="b7235-151">displayName</span><span class="sxs-lookup"><span data-stu-id="b7235-151">displayName</span></span>|<span data-ttu-id="b7235-152">字符串</span><span class="sxs-lookup"><span data-stu-id="b7235-152">String</span></span>|<span data-ttu-id="b7235-153">服务主体的显示名。</span><span class="sxs-lookup"><span data-stu-id="b7235-153">The display name for the service principal.</span></span>|
|<span data-ttu-id="b7235-154">errorUrl</span><span class="sxs-lookup"><span data-stu-id="b7235-154">errorUrl</span></span>|<span data-ttu-id="b7235-155">字符串</span><span class="sxs-lookup"><span data-stu-id="b7235-155">String</span></span>|            |
|<span data-ttu-id="b7235-156">主页</span><span class="sxs-lookup"><span data-stu-id="b7235-156">homepage</span></span>|<span data-ttu-id="b7235-157">字符串</span><span class="sxs-lookup"><span data-stu-id="b7235-157">String</span></span>|<span data-ttu-id="b7235-158">关联的应用程序的主页的 URL。</span><span class="sxs-lookup"><span data-stu-id="b7235-158">The URL to the homepage of the associated application.</span></span>|
|<span data-ttu-id="b7235-159">keyCredentials</span><span class="sxs-lookup"><span data-stu-id="b7235-159">keyCredentials</span></span>|<span data-ttu-id="b7235-160">keyCredential</span><span class="sxs-lookup"><span data-stu-id="b7235-160">keyCredential</span></span>|<span data-ttu-id="b7235-161">关键凭据与主体服务相关联的集合。</span><span class="sxs-lookup"><span data-stu-id="b7235-161">The collection of key credentials associated with the service principal.</span></span>                            <span data-ttu-id="b7235-162">**注意：** 不可为 null。</span><span class="sxs-lookup"><span data-stu-id="b7235-162">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="b7235-163">logoutUrl</span><span class="sxs-lookup"><span data-stu-id="b7235-163">logoutUrl</span></span>|<span data-ttu-id="b7235-164">字符串</span><span class="sxs-lookup"><span data-stu-id="b7235-164">String</span></span>| <span data-ttu-id="b7235-165">指定将由 Microsoft 的授权服务的用户使用[前信道](https://openid.net/specs/openid-connect-frontchannel-1_0.html)、[后通道](https://openid.net/specs/openid-connect-backchannel-1_0.html)或 SAML 注销协议的注销 URL。</span><span class="sxs-lookup"><span data-stu-id="b7235-165">Specifies the URL that will be used by Microsoft's authorization service to logout an user using [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) or SAML logout protocols.</span></span> |
|<span data-ttu-id="b7235-166">oauth2Permissions</span><span class="sxs-lookup"><span data-stu-id="b7235-166">oauth2Permissions</span></span>|<span data-ttu-id="b7235-167">oAuth2Permission</span><span class="sxs-lookup"><span data-stu-id="b7235-167">oAuth2Permission</span></span>|<span data-ttu-id="b7235-168">由关联的应用程序公开 OAuth 2.0 权限。</span><span class="sxs-lookup"><span data-stu-id="b7235-168">The OAuth 2.0 permissions exposed by the associated application.</span></span> <span data-ttu-id="b7235-169">有关详细信息请参阅应用程序在实体上的**oauth2Permissions**属性定义。</span><span class="sxs-lookup"><span data-stu-id="b7235-169">For more information see the **oauth2Permissions** property definition on the application entity.</span></span>                            <span data-ttu-id="b7235-170">**说明**： 需要 1.5 版或更高版本，不可为空。</span><span class="sxs-lookup"><span data-stu-id="b7235-170">**Notes**: Requires version 1.5 or newer, not nullable.</span></span>            |
|<span data-ttu-id="b7235-171">passwordCredentials</span><span class="sxs-lookup"><span data-stu-id="b7235-171">passwordCredentials</span></span>|<span data-ttu-id="b7235-172">passwordCredential</span><span class="sxs-lookup"><span data-stu-id="b7235-172">passwordCredential</span></span>|<span data-ttu-id="b7235-173">密码凭据的服务主体相关联的集合。</span><span class="sxs-lookup"><span data-stu-id="b7235-173">The collection of password credentials associated with the service principal.</span></span>                            <span data-ttu-id="b7235-174">**注意：** 不可为 null。</span><span class="sxs-lookup"><span data-stu-id="b7235-174">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="b7235-175">preferredTokenSigningKeyThumbprint</span><span class="sxs-lookup"><span data-stu-id="b7235-175">preferredTokenSigningKeyThumbprint</span></span>|<span data-ttu-id="b7235-176">字符串</span><span class="sxs-lookup"><span data-stu-id="b7235-176">String</span></span>|<span data-ttu-id="b7235-177">保留以仅供内部使用。</span><span class="sxs-lookup"><span data-stu-id="b7235-177">Reserved for internal use only.</span></span> <span data-ttu-id="b7235-178">不要编写或否则依赖于此属性。</span><span class="sxs-lookup"><span data-stu-id="b7235-178">Do not write or otherwise rely on this property.</span></span> <span data-ttu-id="b7235-179">可能会在将来版本中删除。</span><span class="sxs-lookup"><span data-stu-id="b7235-179">May be removed in future versions.</span></span>                            <span data-ttu-id="b7235-180">**说明**： 要求 1.5 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="b7235-180">**Notes**: Requires version 1.5 or newer.</span></span>            |
|<span data-ttu-id="b7235-181">publisherName</span><span class="sxs-lookup"><span data-stu-id="b7235-181">publisherName</span></span>|<span data-ttu-id="b7235-182">String</span><span class="sxs-lookup"><span data-stu-id="b7235-182">String</span></span>|<span data-ttu-id="b7235-183">在其中指定关联的应用程序租户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="b7235-183">The display name of the tenant in which the associated application is specified.</span></span>|
|<span data-ttu-id="b7235-184">replyUrls</span><span class="sxs-lookup"><span data-stu-id="b7235-184">replyUrls</span></span>|<span data-ttu-id="b7235-185">字符串</span><span class="sxs-lookup"><span data-stu-id="b7235-185">String</span></span>|<span data-ttu-id="b7235-186">用户令牌发送到的登录关联的应用程序或重定向 Uri 的 OAuth 2.0 授权代码和访问令牌发送到关联的应用程序的 Url。</span><span class="sxs-lookup"><span data-stu-id="b7235-186">The URLs that user tokens are sent to for sign in with the associated application, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to for the associated application.</span></span>                            <span data-ttu-id="b7235-187">**注意：** 不可为 null。</span><span class="sxs-lookup"><span data-stu-id="b7235-187">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="b7235-188">samlMetadataUrl</span><span class="sxs-lookup"><span data-stu-id="b7235-188">samlMetadataUrl</span></span>|<span data-ttu-id="b7235-189">字符串</span><span class="sxs-lookup"><span data-stu-id="b7235-189">String</span></span>|            |
|<span data-ttu-id="b7235-190">servicePrincipalNames</span><span class="sxs-lookup"><span data-stu-id="b7235-190">servicePrincipalNames</span></span>|<span data-ttu-id="b7235-191">字符串</span><span class="sxs-lookup"><span data-stu-id="b7235-191">String</span></span>|<span data-ttu-id="b7235-192">标识关联的应用程序的 Uri。</span><span class="sxs-lookup"><span data-stu-id="b7235-192">The URIs that identify the associated application.</span></span> <span data-ttu-id="b7235-193">有关详细信息，请参阅[应用程序对象和服务主体对象](https://msdn.microsoft.com/library/azure/dn132633.aspx)。</span><span class="sxs-lookup"><span data-stu-id="b7235-193">For more information see, [Application Objects and Service Principal Objects](https://msdn.microsoft.com/library/azure/dn132633.aspx).</span></span>                            <span data-ttu-id="b7235-194">**说明**： 不可为空， **any**运算符，则需要为多值属性; 筛选器表达式有关详细信息，请参阅[支持的查询，筛选器和分页选项](https://msdn.microsoft.com/library/azure/dn727074.aspx)。</span><span class="sxs-lookup"><span data-stu-id="b7235-194">**Notes**: not nullable, the **any** operator is required for filter expressions on multi-valued properties; for more information, see [Supported Queries, Filters, and Paging Options](https://msdn.microsoft.com/library/azure/dn727074.aspx).</span></span>            |
|<span data-ttu-id="b7235-195">标记前添加的标记</span><span class="sxs-lookup"><span data-stu-id="b7235-195">tags</span></span>|<span data-ttu-id="b7235-196">String</span><span class="sxs-lookup"><span data-stu-id="b7235-196">String</span></span>|                                        <span data-ttu-id="b7235-197">**注意：** 不可为 null。</span><span class="sxs-lookup"><span data-stu-id="b7235-197">**Notes**: not nullable.</span></span>            |

## <a name="response"></a><span data-ttu-id="b7235-198">响应</span><span class="sxs-lookup"><span data-stu-id="b7235-198">Response</span></span>

<span data-ttu-id="b7235-199">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[servicePrincipal](../resources/serviceprincipal.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b7235-199">If successful, this method returns a `200 OK` response code and updated [servicePrincipal](../resources/serviceprincipal.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b7235-200">示例</span><span class="sxs-lookup"><span data-stu-id="b7235-200">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b7235-201">请求</span><span class="sxs-lookup"><span data-stu-id="b7235-201">Request</span></span>
<span data-ttu-id="b7235-202">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b7235-202">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_serviceprincipal"
}-->
```http
PATCH https://graph.microsoft.com/beta/servicePrincipals/{id}
Content-type: application/json
Content-length: 391

{
  "accountEnabled": true,
  "addIns": [
    {
      "id": "id-value",
      "type": "type-value",
      "properties": [
        {
          "key": "key-value",
          "value": "value-value"
        }
      ]
    }
  ],
  "appDisplayName": "appDisplayName-value",
  "appId": "appId-value",
  "appOwnerOrganizationId": "appOwnerOrganizationId-value",
  "appRoleAssignmentRequired": true
}
```
##### <a name="response"></a><span data-ttu-id="b7235-203">响应</span><span class="sxs-lookup"><span data-stu-id="b7235-203">Response</span></span>
<span data-ttu-id="b7235-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b7235-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.serviceprincipal"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 391

{
  "accountEnabled": true,
  "addIns": [
    {
      "id": "id-value",
      "type": "type-value",
      "properties": [
        {
          "key": "key-value",
          "value": "value-value"
        }
      ]
    }
  ],
  "appDisplayName": "appDisplayName-value",
  "appId": "appId-value",
  "appOwnerOrganizationId": "appOwnerOrganizationId-value",
  "appRoleAssignmentRequired": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update serviceprincipal",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
