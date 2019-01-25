---
title: 更新 serviceprincipal
description: 更新 serviceprincipal 对象的属性。
localization_priority: Normal
ms.openlocfilehash: a562bca03881923cfc21d32eadee2a7f7053fa9b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511658"
---
# <a name="update-serviceprincipal"></a><span data-ttu-id="40859-103">更新 serviceprincipal</span><span class="sxs-lookup"><span data-stu-id="40859-103">Update serviceprincipal</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40859-104">更新 serviceprincipal 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="40859-104">Update the properties of serviceprincipal object.</span></span>
## <a name="permissions"></a><span data-ttu-id="40859-105">权限</span><span class="sxs-lookup"><span data-stu-id="40859-105">Permissions</span></span>
<span data-ttu-id="40859-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="40859-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40859-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="40859-108">Permission type</span></span>      | <span data-ttu-id="40859-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="40859-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="40859-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="40859-110">Delegated (work or school account)</span></span> | <span data-ttu-id="40859-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="40859-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="40859-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="40859-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40859-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="40859-113">Not supported.</span></span>    |
|<span data-ttu-id="40859-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="40859-114">Application</span></span> | <span data-ttu-id="40859-115">Application.ReadWrite.OwnedBy Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40859-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="40859-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="40859-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /servicePrincipals/{id}
```
## <a name="request-headers"></a><span data-ttu-id="40859-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="40859-117">Request headers</span></span>
| <span data-ttu-id="40859-118">名称</span><span class="sxs-lookup"><span data-stu-id="40859-118">Name</span></span>       | <span data-ttu-id="40859-119">类型</span><span class="sxs-lookup"><span data-stu-id="40859-119">Type</span></span> | <span data-ttu-id="40859-120">说明</span><span class="sxs-lookup"><span data-stu-id="40859-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="40859-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="40859-121">Authorization</span></span>  | <span data-ttu-id="40859-122">string</span><span class="sxs-lookup"><span data-stu-id="40859-122">string</span></span>  | <span data-ttu-id="40859-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="40859-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="40859-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="40859-125">Request body</span></span>
<span data-ttu-id="40859-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="40859-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="40859-129">属性</span><span class="sxs-lookup"><span data-stu-id="40859-129">Property</span></span>     | <span data-ttu-id="40859-130">类型</span><span class="sxs-lookup"><span data-stu-id="40859-130">Type</span></span>   |<span data-ttu-id="40859-131">说明</span><span class="sxs-lookup"><span data-stu-id="40859-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="40859-132">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="40859-132">accountEnabled</span></span>|<span data-ttu-id="40859-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="40859-133">Boolean</span></span>|                <span data-ttu-id="40859-134">**true**如果已启用的服务主体帐户;否则为**false**。</span><span class="sxs-lookup"><span data-stu-id="40859-134">**true** if the service principal account is enabled; otherwise, **false**.</span></span>            |
|<span data-ttu-id="40859-135">AppDisplayName</span><span class="sxs-lookup"><span data-stu-id="40859-135">appDisplayName</span></span>|<span data-ttu-id="40859-136">String</span><span class="sxs-lookup"><span data-stu-id="40859-136">String</span></span>|<span data-ttu-id="40859-137">通过关联的应用程序公开的显示名称。</span><span class="sxs-lookup"><span data-stu-id="40859-137">The display name exposed by the associated application.</span></span>|
|<span data-ttu-id="40859-138">appId</span><span class="sxs-lookup"><span data-stu-id="40859-138">appId</span></span>|<span data-ttu-id="40859-139">String</span><span class="sxs-lookup"><span data-stu-id="40859-139">String</span></span>|<span data-ttu-id="40859-140">关联的应用程序 （其**appId**属性） 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="40859-140">The unique identifier for the associated application (its **appId** property).</span></span>|
|<span data-ttu-id="40859-141">appRoleAssignmentRequired</span><span class="sxs-lookup"><span data-stu-id="40859-141">appRoleAssignmentRequired</span></span>|<span data-ttu-id="40859-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="40859-142">Boolean</span></span>|<span data-ttu-id="40859-143">指定 Azure AD 将问题的用户或访问令牌对应用程序之前是否需要向用户或组**appRoleAssignment** 。</span><span class="sxs-lookup"><span data-stu-id="40859-143">Specifies whether an **appRoleAssignment** to a user or group is required before Azure AD will issue a user or access token to the application.</span></span>                            <span data-ttu-id="40859-144">**说明**： 需要 1.5 版或更高版本，不可为空。</span><span class="sxs-lookup"><span data-stu-id="40859-144">**Notes**: Requires version 1.5 or newer, not nullable.</span></span>            |
|<span data-ttu-id="40859-145">appRoles</span><span class="sxs-lookup"><span data-stu-id="40859-145">appRoles</span></span>|<span data-ttu-id="40859-146">appRole</span><span class="sxs-lookup"><span data-stu-id="40859-146">appRole</span></span>|<span data-ttu-id="40859-147">由关联的应用程序公开应用程序角色。</span><span class="sxs-lookup"><span data-stu-id="40859-147">The application roles exposed by the associated application.</span></span> <span data-ttu-id="40859-148">有关详细信息看到**appRoles**属性定义应用程序实体**注释**： 需要 1.5 版或更高版本，不可为空。</span><span class="sxs-lookup"><span data-stu-id="40859-148">For more information see the **appRoles** property definition on the application entity                            **Notes**: Requires version 1.5 or newer, not nullable.</span></span>            |
|<span data-ttu-id="40859-149">displayName</span><span class="sxs-lookup"><span data-stu-id="40859-149">displayName</span></span>|<span data-ttu-id="40859-150">字符串</span><span class="sxs-lookup"><span data-stu-id="40859-150">String</span></span>|<span data-ttu-id="40859-151">服务主体的显示名。</span><span class="sxs-lookup"><span data-stu-id="40859-151">The display name for the service principal.</span></span>|
|<span data-ttu-id="40859-152">errorUrl</span><span class="sxs-lookup"><span data-stu-id="40859-152">errorUrl</span></span>|<span data-ttu-id="40859-153">String</span><span class="sxs-lookup"><span data-stu-id="40859-153">String</span></span>|            |
|<span data-ttu-id="40859-154">HomePage</span><span class="sxs-lookup"><span data-stu-id="40859-154">homepage</span></span>|<span data-ttu-id="40859-155">String</span><span class="sxs-lookup"><span data-stu-id="40859-155">String</span></span>|<span data-ttu-id="40859-156">关联的应用程序的主页的 URL。</span><span class="sxs-lookup"><span data-stu-id="40859-156">The URL to the homepage of the associated application.</span></span>|
|<span data-ttu-id="40859-157">keyCredentials</span><span class="sxs-lookup"><span data-stu-id="40859-157">keyCredentials</span></span>|<span data-ttu-id="40859-158">keyCredential</span><span class="sxs-lookup"><span data-stu-id="40859-158">keyCredential</span></span>|<span data-ttu-id="40859-159">关键凭据与主体服务相关联的集合。</span><span class="sxs-lookup"><span data-stu-id="40859-159">The collection of key credentials associated with the service principal.</span></span>                            <span data-ttu-id="40859-160">**注意：** 不可为 null。</span><span class="sxs-lookup"><span data-stu-id="40859-160">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="40859-161">logoutUrl</span><span class="sxs-lookup"><span data-stu-id="40859-161">logoutUrl</span></span>|<span data-ttu-id="40859-162">String</span><span class="sxs-lookup"><span data-stu-id="40859-162">String</span></span>| <span data-ttu-id="40859-163">指定将由 Microsoft 的授权服务的用户使用[前信道](https://openid.net/specs/openid-connect-frontchannel-1_0.html)、[后通道](https://openid.net/specs/openid-connect-backchannel-1_0.html)或 SAML 注销协议的注销 URL。</span><span class="sxs-lookup"><span data-stu-id="40859-163">Specifies the URL that will be used by Microsoft's authorization service to logout an user using [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) or SAML logout protocols.</span></span> |
|<span data-ttu-id="40859-164">oauth2Permissions</span><span class="sxs-lookup"><span data-stu-id="40859-164">oauth2Permissions</span></span>|<span data-ttu-id="40859-165">oAuth2Permission</span><span class="sxs-lookup"><span data-stu-id="40859-165">oAuth2Permission</span></span>|<span data-ttu-id="40859-166">由关联的应用程序公开 OAuth 2.0 权限。</span><span class="sxs-lookup"><span data-stu-id="40859-166">The OAuth 2.0 permissions exposed by the associated application.</span></span> <span data-ttu-id="40859-167">有关详细信息请参阅应用程序在实体上的**oauth2Permissions**属性定义。</span><span class="sxs-lookup"><span data-stu-id="40859-167">For more information see the **oauth2Permissions** property definition on the application entity.</span></span>                            <span data-ttu-id="40859-168">**说明**： 需要 1.5 版或更高版本，不可为空。</span><span class="sxs-lookup"><span data-stu-id="40859-168">**Notes**: Requires version 1.5 or newer, not nullable.</span></span>            |
|<span data-ttu-id="40859-169">passwordCredentials</span><span class="sxs-lookup"><span data-stu-id="40859-169">passwordCredentials</span></span>|<span data-ttu-id="40859-170">passwordCredential</span><span class="sxs-lookup"><span data-stu-id="40859-170">passwordCredential</span></span>|<span data-ttu-id="40859-171">密码凭据的服务主体相关联的集合。</span><span class="sxs-lookup"><span data-stu-id="40859-171">The collection of password credentials associated with the service principal.</span></span>                            <span data-ttu-id="40859-172">**注意：** 不可为 null。</span><span class="sxs-lookup"><span data-stu-id="40859-172">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="40859-173">preferredTokenSigningKeyThumbprint</span><span class="sxs-lookup"><span data-stu-id="40859-173">preferredTokenSigningKeyThumbprint</span></span>|<span data-ttu-id="40859-174">String</span><span class="sxs-lookup"><span data-stu-id="40859-174">String</span></span>|<span data-ttu-id="40859-175">保留以仅供内部使用。</span><span class="sxs-lookup"><span data-stu-id="40859-175">Reserved for internal use only.</span></span> <span data-ttu-id="40859-176">不要编写或否则依赖于此属性。</span><span class="sxs-lookup"><span data-stu-id="40859-176">Do not write or otherwise rely on this property.</span></span> <span data-ttu-id="40859-177">可能会在将来版本中删除。</span><span class="sxs-lookup"><span data-stu-id="40859-177">May be removed in future versions.</span></span>                            <span data-ttu-id="40859-178">**说明**： 要求 1.5 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="40859-178">**Notes**: Requires version 1.5 or newer.</span></span>            |
|<span data-ttu-id="40859-179">publisherName</span><span class="sxs-lookup"><span data-stu-id="40859-179">publisherName</span></span>|<span data-ttu-id="40859-180">String</span><span class="sxs-lookup"><span data-stu-id="40859-180">String</span></span>|<span data-ttu-id="40859-181">在其中指定关联的应用程序租户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="40859-181">The display name of the tenant in which the associated application is specified.</span></span>|
|<span data-ttu-id="40859-182">replyUrls</span><span class="sxs-lookup"><span data-stu-id="40859-182">replyUrls</span></span>|<span data-ttu-id="40859-183">String</span><span class="sxs-lookup"><span data-stu-id="40859-183">String</span></span>|<span data-ttu-id="40859-184">用户令牌发送到的登录关联的应用程序或重定向 Uri 的 OAuth 2.0 授权代码和访问令牌发送到关联的应用程序的 Url。</span><span class="sxs-lookup"><span data-stu-id="40859-184">The URLs that user tokens are sent to for sign in with the associated application, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to for the associated application.</span></span>                            <span data-ttu-id="40859-185">**注意：** 不可为 null。</span><span class="sxs-lookup"><span data-stu-id="40859-185">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="40859-186">samlMetadataUrl</span><span class="sxs-lookup"><span data-stu-id="40859-186">samlMetadataUrl</span></span>|<span data-ttu-id="40859-187">String</span><span class="sxs-lookup"><span data-stu-id="40859-187">String</span></span>|            |
|<span data-ttu-id="40859-188">servicePrincipalNames</span><span class="sxs-lookup"><span data-stu-id="40859-188">servicePrincipalNames</span></span>|<span data-ttu-id="40859-189">String</span><span class="sxs-lookup"><span data-stu-id="40859-189">String</span></span>|<span data-ttu-id="40859-190">标识关联的应用程序的 Uri。</span><span class="sxs-lookup"><span data-stu-id="40859-190">The URIs that identify the associated application.</span></span> <span data-ttu-id="40859-191">有关详细信息，请参阅[应用程序对象和服务主体对象](https://msdn.microsoft.com/library/azure/dn132633.aspx)。</span><span class="sxs-lookup"><span data-stu-id="40859-191">For more information see, [Application Objects and Service Principal Objects](https://msdn.microsoft.com/library/azure/dn132633.aspx).</span></span>                            <span data-ttu-id="40859-192">**说明**： 不可为空， **any**运算符，则需要为多值属性; 筛选器表达式有关详细信息，请参阅[支持的查询，筛选器和分页选项](https://msdn.microsoft.com/library/azure/dn727074.aspx)。</span><span class="sxs-lookup"><span data-stu-id="40859-192">**Notes**: not nullable, the **any** operator is required for filter expressions on multi-valued properties; for more information, see [Supported Queries, Filters, and Paging Options](https://msdn.microsoft.com/library/azure/dn727074.aspx).</span></span>            |
|<span data-ttu-id="40859-193">标记</span><span class="sxs-lookup"><span data-stu-id="40859-193">tags</span></span>|<span data-ttu-id="40859-194">String</span><span class="sxs-lookup"><span data-stu-id="40859-194">String</span></span>|                                        <span data-ttu-id="40859-195">**注意：** 不可为 null。</span><span class="sxs-lookup"><span data-stu-id="40859-195">**Notes**: not nullable.</span></span>            |

## <a name="response"></a><span data-ttu-id="40859-196">响应</span><span class="sxs-lookup"><span data-stu-id="40859-196">Response</span></span>

<span data-ttu-id="40859-197">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[servicePrincipal](../resources/serviceprincipal.md)对象。</span><span class="sxs-lookup"><span data-stu-id="40859-197">If successful, this method returns a `200 OK` response code and updated [servicePrincipal](../resources/serviceprincipal.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="40859-198">示例</span><span class="sxs-lookup"><span data-stu-id="40859-198">Example</span></span>
##### <a name="request"></a><span data-ttu-id="40859-199">请求</span><span class="sxs-lookup"><span data-stu-id="40859-199">Request</span></span>
<span data-ttu-id="40859-200">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="40859-200">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="40859-201">响应</span><span class="sxs-lookup"><span data-stu-id="40859-201">Response</span></span>
<span data-ttu-id="40859-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="40859-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update serviceprincipal",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/serviceprincipal-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
