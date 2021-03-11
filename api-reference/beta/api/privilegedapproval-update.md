---
title: 更新 privilegedapproval
description: 更新 privilegedapproval 对象的属性。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: a04f33c283cd82715cb1e0d63917cea7cb373329
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720457"
---
# <a name="update-privilegedapproval"></a><span data-ttu-id="3b1bb-103">更新 privilegedapproval</span><span class="sxs-lookup"><span data-stu-id="3b1bb-103">Update privilegedapproval</span></span>

<span data-ttu-id="3b1bb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b1bb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b1bb-105">更新 privilegedapproval 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3b1bb-105">Update the properties of privilegedapproval object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3b1bb-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="3b1bb-106">Permissions</span></span>
<span data-ttu-id="3b1bb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3b1bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="3b1bb-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3b1bb-109">Permission type</span></span>      | <span data-ttu-id="3b1bb-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3b1bb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3b1bb-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3b1bb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3b1bb-112">PrivilegedAccess.ReadWrite.AzureAD、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3b1bb-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3b1bb-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3b1bb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3b1bb-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3b1bb-114">Not supported.</span></span>    |
|<span data-ttu-id="3b1bb-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3b1bb-115">Application</span></span> | <span data-ttu-id="3b1bb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3b1bb-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3b1bb-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3b1bb-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedApproval/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="3b1bb-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="3b1bb-118">Optional request headers</span></span>
| <span data-ttu-id="3b1bb-119">名称</span><span class="sxs-lookup"><span data-stu-id="3b1bb-119">Name</span></span>       | <span data-ttu-id="3b1bb-120">说明</span><span class="sxs-lookup"><span data-stu-id="3b1bb-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="3b1bb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b1bb-121">Authorization</span></span>  | <span data-ttu-id="3b1bb-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3b1bb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3b1bb-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="3b1bb-124">Request body</span></span>
<span data-ttu-id="3b1bb-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="3b1bb-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3b1bb-128">属性</span><span class="sxs-lookup"><span data-stu-id="3b1bb-128">Property</span></span>     | <span data-ttu-id="3b1bb-129">类型</span><span class="sxs-lookup"><span data-stu-id="3b1bb-129">Type</span></span>   |<span data-ttu-id="3b1bb-130">说明</span><span class="sxs-lookup"><span data-stu-id="3b1bb-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3b1bb-131">approvalDuration</span><span class="sxs-lookup"><span data-stu-id="3b1bb-131">approvalDuration</span></span>|<span data-ttu-id="3b1bb-132">持续时间</span><span class="sxs-lookup"><span data-stu-id="3b1bb-132">Duration</span></span>||
|<span data-ttu-id="3b1bb-133">approvalState</span><span class="sxs-lookup"><span data-stu-id="3b1bb-133">approvalState</span></span>|<span data-ttu-id="3b1bb-134">string</span><span class="sxs-lookup"><span data-stu-id="3b1bb-134">string</span></span>| <span data-ttu-id="3b1bb-135">可取值为：`pending`、`approved`、`denied`、`aborted`、`canceled`。</span><span class="sxs-lookup"><span data-stu-id="3b1bb-135">Possible values are: `pending`, `approved`, `denied`, `aborted`, `canceled`.</span></span>|
|<span data-ttu-id="3b1bb-136">approvalType</span><span class="sxs-lookup"><span data-stu-id="3b1bb-136">approvalType</span></span>|<span data-ttu-id="3b1bb-137">String</span><span class="sxs-lookup"><span data-stu-id="3b1bb-137">String</span></span>||
|<span data-ttu-id="3b1bb-138">approverReason</span><span class="sxs-lookup"><span data-stu-id="3b1bb-138">approverReason</span></span>|<span data-ttu-id="3b1bb-139">String</span><span class="sxs-lookup"><span data-stu-id="3b1bb-139">String</span></span>||
|<span data-ttu-id="3b1bb-140">endDateTime</span><span class="sxs-lookup"><span data-stu-id="3b1bb-140">endDateTime</span></span>|<span data-ttu-id="3b1bb-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b1bb-141">DateTimeOffset</span></span>||
|<span data-ttu-id="3b1bb-142">requestorReason</span><span class="sxs-lookup"><span data-stu-id="3b1bb-142">requestorReason</span></span>|<span data-ttu-id="3b1bb-143">String</span><span class="sxs-lookup"><span data-stu-id="3b1bb-143">String</span></span>||
|<span data-ttu-id="3b1bb-144">roleId</span><span class="sxs-lookup"><span data-stu-id="3b1bb-144">roleId</span></span>|<span data-ttu-id="3b1bb-145">String</span><span class="sxs-lookup"><span data-stu-id="3b1bb-145">String</span></span>||
|<span data-ttu-id="3b1bb-146">startDateTime</span><span class="sxs-lookup"><span data-stu-id="3b1bb-146">startDateTime</span></span>|<span data-ttu-id="3b1bb-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b1bb-147">DateTimeOffset</span></span>||
|<span data-ttu-id="3b1bb-148">userId</span><span class="sxs-lookup"><span data-stu-id="3b1bb-148">userId</span></span>|<span data-ttu-id="3b1bb-149">String</span><span class="sxs-lookup"><span data-stu-id="3b1bb-149">String</span></span>||

## <a name="response"></a><span data-ttu-id="3b1bb-150">响应</span><span class="sxs-lookup"><span data-stu-id="3b1bb-150">Response</span></span>

<span data-ttu-id="3b1bb-151">如果成功，此方法将返回 `204 No Content` 响应代码</span><span class="sxs-lookup"><span data-stu-id="3b1bb-151">If successful, this method returns a `204 No Content` response code</span></span>

<span data-ttu-id="3b1bb-152">请注意，租户需要注册到 PIM。</span><span class="sxs-lookup"><span data-stu-id="3b1bb-152">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="3b1bb-153">否则，将返回 HTTP 403 禁止状态代码。</span><span class="sxs-lookup"><span data-stu-id="3b1bb-153">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="3b1bb-154">示例</span><span class="sxs-lookup"><span data-stu-id="3b1bb-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3b1bb-155">请求</span><span class="sxs-lookup"><span data-stu-id="3b1bb-155">Request</span></span>
<span data-ttu-id="3b1bb-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3b1bb-156">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_privilegedapproval"
}-->
```http
PATCH https://graph.microsoft.com/beta/privilegedApproval/{requestId}
Content-type: application/json
Content-length: 180

{
  "approvalState": "approvalState-value",
  "approverReason": "approverReason-value"
}
```
##### <a name="response"></a><span data-ttu-id="3b1bb-157">响应</span><span class="sxs-lookup"><span data-stu-id="3b1bb-157">Response</span></span>
<span data-ttu-id="3b1bb-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3b1bb-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


