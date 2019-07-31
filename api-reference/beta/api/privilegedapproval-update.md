---
title: 更新 privilegedapproval
description: 更新 privilegedapproval 对象的属性。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 6103e01ea9832bd7858215576eaeb4319514d6be
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35978803"
---
# <a name="update-privilegedapproval"></a><span data-ttu-id="7c77e-103">更新 privilegedapproval</span><span class="sxs-lookup"><span data-stu-id="7c77e-103">Update privilegedapproval</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c77e-104">更新 privilegedapproval 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7c77e-104">Update the properties of privilegedapproval object.</span></span>
## <a name="permissions"></a><span data-ttu-id="7c77e-105">权限</span><span class="sxs-lookup"><span data-stu-id="7c77e-105">Permissions</span></span>
<span data-ttu-id="7c77e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7c77e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7c77e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="7c77e-108">Permission type</span></span>      | <span data-ttu-id="7c77e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7c77e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7c77e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7c77e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7c77e-111">PrivilegedAccess 的 AzureAD、Directory.accessasuser.all</span><span class="sxs-lookup"><span data-stu-id="7c77e-111">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7c77e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7c77e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c77e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="7c77e-113">Not supported.</span></span>    |
|<span data-ttu-id="7c77e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="7c77e-114">Application</span></span> | <span data-ttu-id="7c77e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7c77e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7c77e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7c77e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedApproval/<id>
```
## <a name="optional-request-headers"></a><span data-ttu-id="7c77e-117">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="7c77e-117">Optional request headers</span></span>
| <span data-ttu-id="7c77e-118">名称</span><span class="sxs-lookup"><span data-stu-id="7c77e-118">Name</span></span>       | <span data-ttu-id="7c77e-119">说明</span><span class="sxs-lookup"><span data-stu-id="7c77e-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="7c77e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c77e-120">Authorization</span></span>  | <span data-ttu-id="7c77e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7c77e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7c77e-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="7c77e-123">Request body</span></span>
<span data-ttu-id="7c77e-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="7c77e-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="7c77e-127">属性</span><span class="sxs-lookup"><span data-stu-id="7c77e-127">Property</span></span>     | <span data-ttu-id="7c77e-128">类型</span><span class="sxs-lookup"><span data-stu-id="7c77e-128">Type</span></span>   |<span data-ttu-id="7c77e-129">说明</span><span class="sxs-lookup"><span data-stu-id="7c77e-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7c77e-130">approvalDuration</span><span class="sxs-lookup"><span data-stu-id="7c77e-130">approvalDuration</span></span>|<span data-ttu-id="7c77e-131">持续时间</span><span class="sxs-lookup"><span data-stu-id="7c77e-131">Duration</span></span>||
|<span data-ttu-id="7c77e-132">approvalState</span><span class="sxs-lookup"><span data-stu-id="7c77e-132">approvalState</span></span>|<span data-ttu-id="7c77e-133">string</span><span class="sxs-lookup"><span data-stu-id="7c77e-133">string</span></span>| <span data-ttu-id="7c77e-134">可取值为：`pending`、`approved`、`denied`、`aborted`、`canceled`。</span><span class="sxs-lookup"><span data-stu-id="7c77e-134">Possible values are: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span></span>|
|<span data-ttu-id="7c77e-135">approvalType</span><span class="sxs-lookup"><span data-stu-id="7c77e-135">approvalType</span></span>|<span data-ttu-id="7c77e-136">String</span><span class="sxs-lookup"><span data-stu-id="7c77e-136">String</span></span>||
|<span data-ttu-id="7c77e-137">approverReason</span><span class="sxs-lookup"><span data-stu-id="7c77e-137">approverReason</span></span>|<span data-ttu-id="7c77e-138">String</span><span class="sxs-lookup"><span data-stu-id="7c77e-138">String</span></span>||
|<span data-ttu-id="7c77e-139">endDateTime</span><span class="sxs-lookup"><span data-stu-id="7c77e-139">endDateTime</span></span>|<span data-ttu-id="7c77e-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c77e-140">DateTimeOffset</span></span>||
|<span data-ttu-id="7c77e-141">requestorReason</span><span class="sxs-lookup"><span data-stu-id="7c77e-141">requestorReason</span></span>|<span data-ttu-id="7c77e-142">String</span><span class="sxs-lookup"><span data-stu-id="7c77e-142">String</span></span>||
|<span data-ttu-id="7c77e-143">roleId</span><span class="sxs-lookup"><span data-stu-id="7c77e-143">roleId</span></span>|<span data-ttu-id="7c77e-144">String</span><span class="sxs-lookup"><span data-stu-id="7c77e-144">String</span></span>||
|<span data-ttu-id="7c77e-145">startDateTime</span><span class="sxs-lookup"><span data-stu-id="7c77e-145">startDateTime</span></span>|<span data-ttu-id="7c77e-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c77e-146">DateTimeOffset</span></span>||
|<span data-ttu-id="7c77e-147">userId</span><span class="sxs-lookup"><span data-stu-id="7c77e-147">userId</span></span>|<span data-ttu-id="7c77e-148">String</span><span class="sxs-lookup"><span data-stu-id="7c77e-148">String</span></span>||

## <a name="response"></a><span data-ttu-id="7c77e-149">响应</span><span class="sxs-lookup"><span data-stu-id="7c77e-149">Response</span></span>

<span data-ttu-id="7c77e-150">如果成功, 此方法将`204 No Content`返回响应代码</span><span class="sxs-lookup"><span data-stu-id="7c77e-150">If successful, this method returns a `204 No Content` response code</span></span>

<span data-ttu-id="7c77e-151">请注意, 需要将租户注册到 PIM。</span><span class="sxs-lookup"><span data-stu-id="7c77e-151">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="7c77e-152">否则, 将返回 HTTP 403 禁止的状态代码。</span><span class="sxs-lookup"><span data-stu-id="7c77e-152">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="7c77e-153">示例</span><span class="sxs-lookup"><span data-stu-id="7c77e-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7c77e-154">请求</span><span class="sxs-lookup"><span data-stu-id="7c77e-154">Request</span></span>
<span data-ttu-id="7c77e-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7c77e-155">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_privilegedapproval"
}-->
```http
PATCH https://graph.microsoft.com/beta/privilegedApproval{request-id}
Content-type: application/json
Content-length: 180

{
  "approvalState": "approvalState-value",
  "approverReason": "approverReason-value"
}
```
##### <a name="response"></a><span data-ttu-id="7c77e-156">响应</span><span class="sxs-lookup"><span data-stu-id="7c77e-156">Response</span></span>
<span data-ttu-id="7c77e-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7c77e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedApproval"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update privilegedapproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
