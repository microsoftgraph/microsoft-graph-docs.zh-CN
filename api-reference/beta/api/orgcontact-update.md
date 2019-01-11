---
title: 更新 orgcontact
description: 更新 orgcontact 对象的属性。
localization_priority: Normal
ms.openlocfilehash: f48795bef6ea1a4833379f54747cbf2c291b2454
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859064"
---
# <a name="update-orgcontact"></a><span data-ttu-id="1565c-103">更新 orgcontact</span><span class="sxs-lookup"><span data-stu-id="1565c-103">Update orgcontact</span></span>

> <span data-ttu-id="1565c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1565c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1565c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1565c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1565c-106">更新 orgcontact 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1565c-106">Update the properties of orgcontact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1565c-107">权限</span><span class="sxs-lookup"><span data-stu-id="1565c-107">Permissions</span></span>
<span data-ttu-id="1565c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1565c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1565c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1565c-110">Permission type</span></span>      | <span data-ttu-id="1565c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1565c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1565c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1565c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1565c-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="1565c-113">Not supported.</span></span>    |
|<span data-ttu-id="1565c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1565c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1565c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1565c-115">Not supported.</span></span>    |
|<span data-ttu-id="1565c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1565c-116">Application</span></span> | <span data-ttu-id="1565c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="1565c-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1565c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1565c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="1565c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="1565c-119">Request headers</span></span>
| <span data-ttu-id="1565c-120">名称</span><span class="sxs-lookup"><span data-stu-id="1565c-120">Name</span></span>       | <span data-ttu-id="1565c-121">类型</span><span class="sxs-lookup"><span data-stu-id="1565c-121">Type</span></span> | <span data-ttu-id="1565c-122">说明</span><span class="sxs-lookup"><span data-stu-id="1565c-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1565c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1565c-123">Authorization</span></span>  | <span data-ttu-id="1565c-124">string</span><span class="sxs-lookup"><span data-stu-id="1565c-124">string</span></span>  | <span data-ttu-id="1565c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1565c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1565c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1565c-127">Request body</span></span>
<span data-ttu-id="1565c-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="1565c-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1565c-131">属性</span><span class="sxs-lookup"><span data-stu-id="1565c-131">Property</span></span>     | <span data-ttu-id="1565c-132">类型</span><span class="sxs-lookup"><span data-stu-id="1565c-132">Type</span></span>   |<span data-ttu-id="1565c-133">说明</span><span class="sxs-lookup"><span data-stu-id="1565c-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1565c-134">city</span><span class="sxs-lookup"><span data-stu-id="1565c-134">city</span></span>|<span data-ttu-id="1565c-135">字符串</span><span class="sxs-lookup"><span data-stu-id="1565c-135">String</span></span>||
|<span data-ttu-id="1565c-136">country</span><span class="sxs-lookup"><span data-stu-id="1565c-136">country</span></span>|<span data-ttu-id="1565c-137">字符串</span><span class="sxs-lookup"><span data-stu-id="1565c-137">String</span></span>||
|<span data-ttu-id="1565c-138">department</span><span class="sxs-lookup"><span data-stu-id="1565c-138">department</span></span>|<span data-ttu-id="1565c-139">字符串</span><span class="sxs-lookup"><span data-stu-id="1565c-139">String</span></span>||
|<span data-ttu-id="1565c-140">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="1565c-140">onPremisesSyncEnabled</span></span>|<span data-ttu-id="1565c-141">布尔</span><span class="sxs-lookup"><span data-stu-id="1565c-141">Boolean</span></span>||
|<span data-ttu-id="1565c-142">displayName</span><span class="sxs-lookup"><span data-stu-id="1565c-142">displayName</span></span>|<span data-ttu-id="1565c-143">字符串</span><span class="sxs-lookup"><span data-stu-id="1565c-143">String</span></span>||
|<span data-ttu-id="1565c-144">givenName</span><span class="sxs-lookup"><span data-stu-id="1565c-144">givenName</span></span>|<span data-ttu-id="1565c-145">字符串</span><span class="sxs-lookup"><span data-stu-id="1565c-145">String</span></span>||
|<span data-ttu-id="1565c-146">jobTitle</span><span class="sxs-lookup"><span data-stu-id="1565c-146">jobTitle</span></span>|<span data-ttu-id="1565c-147">字符串</span><span class="sxs-lookup"><span data-stu-id="1565c-147">String</span></span>||
|<span data-ttu-id="1565c-148">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="1565c-148">onPremisesLastSyncDateTime</span></span>|<span data-ttu-id="1565c-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1565c-149">DateTimeOffset</span></span>||
|<span data-ttu-id="1565c-150">mail</span><span class="sxs-lookup"><span data-stu-id="1565c-150">mail</span></span>|<span data-ttu-id="1565c-151">字符串</span><span class="sxs-lookup"><span data-stu-id="1565c-151">String</span></span>||
|<span data-ttu-id="1565c-152">mailNickname</span><span class="sxs-lookup"><span data-stu-id="1565c-152">mailNickname</span></span>|<span data-ttu-id="1565c-153">字符串</span><span class="sxs-lookup"><span data-stu-id="1565c-153">String</span></span>||
|<span data-ttu-id="1565c-154">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="1565c-154">mobilePhone</span></span>|<span data-ttu-id="1565c-155">String</span><span class="sxs-lookup"><span data-stu-id="1565c-155">String</span></span>||
|<span data-ttu-id="1565c-156">officeLocation</span><span class="sxs-lookup"><span data-stu-id="1565c-156">officeLocation</span></span>|<span data-ttu-id="1565c-157">String</span><span class="sxs-lookup"><span data-stu-id="1565c-157">String</span></span>||
|<span data-ttu-id="1565c-158">postalCode</span><span class="sxs-lookup"><span data-stu-id="1565c-158">postalCode</span></span>|<span data-ttu-id="1565c-159">字符串</span><span class="sxs-lookup"><span data-stu-id="1565c-159">String</span></span>||
|<span data-ttu-id="1565c-160">proxyAddresses</span><span class="sxs-lookup"><span data-stu-id="1565c-160">proxyAddresses</span></span>|<span data-ttu-id="1565c-161">String</span><span class="sxs-lookup"><span data-stu-id="1565c-161">String</span></span>||
|<span data-ttu-id="1565c-162">state</span><span class="sxs-lookup"><span data-stu-id="1565c-162">state</span></span>|<span data-ttu-id="1565c-163">字符串</span><span class="sxs-lookup"><span data-stu-id="1565c-163">String</span></span>||
|<span data-ttu-id="1565c-164">streetAddress</span><span class="sxs-lookup"><span data-stu-id="1565c-164">streetAddress</span></span>|<span data-ttu-id="1565c-165">String</span><span class="sxs-lookup"><span data-stu-id="1565c-165">String</span></span>||
|<span data-ttu-id="1565c-166">surname</span><span class="sxs-lookup"><span data-stu-id="1565c-166">surname</span></span>|<span data-ttu-id="1565c-167">字符串</span><span class="sxs-lookup"><span data-stu-id="1565c-167">String</span></span>||
|<span data-ttu-id="1565c-168">businessPhones</span><span class="sxs-lookup"><span data-stu-id="1565c-168">businessPhones</span></span>|<span data-ttu-id="1565c-169">String</span><span class="sxs-lookup"><span data-stu-id="1565c-169">String</span></span>||

## <a name="response"></a><span data-ttu-id="1565c-170">响应</span><span class="sxs-lookup"><span data-stu-id="1565c-170">Response</span></span>

<span data-ttu-id="1565c-171">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[orgContact](../resources/orgcontact.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1565c-171">If successful, this method returns a `200 OK` response code and updated [orgContact](../resources/orgcontact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1565c-172">示例</span><span class="sxs-lookup"><span data-stu-id="1565c-172">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1565c-173">请求</span><span class="sxs-lookup"><span data-stu-id="1565c-173">Request</span></span>
<span data-ttu-id="1565c-174">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1565c-174">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_orgcontact"
}-->
```http
PATCH https://graph.microsoft.com/beta/contacts/{id}
Content-type: application/json
Content-length: 222

{
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value",
  "companyName": "companyName-value",
  "country": "country-value",
  "department": "department-value",
  "displayName": "displayName-value"
}
```
##### <a name="response"></a><span data-ttu-id="1565c-175">响应</span><span class="sxs-lookup"><span data-stu-id="1565c-175">Response</span></span>
<span data-ttu-id="1565c-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1565c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 222

{
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value",
  "companyName": "companyName-value",
  "country": "country-value",
  "department": "department-value",
  "displayName": "displayName-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update orgcontact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
