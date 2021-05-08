---
title: 创建 educationSchool
description: 创建新的 educationSchool 对象。
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: f9bf1499ef3c1d0106d9daac1bbda8f7ef25926d
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232136"
---
# <a name="create-educationschool"></a><span data-ttu-id="782cd-103">创建 educationSchool</span><span class="sxs-lookup"><span data-stu-id="782cd-103">Create educationSchool</span></span>

<span data-ttu-id="782cd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="782cd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="782cd-105">创建新的 [educationSchool](../resources/educationschool.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="782cd-105">Create a new [educationSchool](../resources/educationschool.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="782cd-106">权限</span><span class="sxs-lookup"><span data-stu-id="782cd-106">Permissions</span></span>

<span data-ttu-id="782cd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="782cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="782cd-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="782cd-109">Permission type</span></span>                        | <span data-ttu-id="782cd-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="782cd-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="782cd-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="782cd-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="782cd-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="782cd-112">Not supported.</span></span>                              |
| <span data-ttu-id="782cd-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="782cd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="782cd-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="782cd-114">Not supported.</span></span>                              |
| <span data-ttu-id="782cd-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="782cd-115">Application</span></span>                            | <span data-ttu-id="782cd-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="782cd-116">EduRoster.ReadWrite.All</span></span>                     |

## <a name="http-request"></a><span data-ttu-id="782cd-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="782cd-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
POST /education/schools
```

## <a name="request-headers"></a><span data-ttu-id="782cd-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="782cd-118">Request headers</span></span>

| <span data-ttu-id="782cd-119">名称</span><span class="sxs-lookup"><span data-stu-id="782cd-119">Name</span></span>          | <span data-ttu-id="782cd-120">说明</span><span class="sxs-lookup"><span data-stu-id="782cd-120">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="782cd-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="782cd-121">Authorization</span></span> | <span data-ttu-id="782cd-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="782cd-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="782cd-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="782cd-124">Content-Type</span></span>  | <span data-ttu-id="782cd-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="782cd-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="782cd-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="782cd-127">Request body</span></span>

<span data-ttu-id="782cd-128">在请求正文中，提供 [educationSchool](../resources/educationschool.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="782cd-128">In the request body, supply a JSON representation of the [educationSchool](../resources/educationschool.md) object.</span></span>

<span data-ttu-id="782cd-129">下表显示创建 [educationSchool 时所需的属性](../resources/educationschool.md)。</span><span class="sxs-lookup"><span data-stu-id="782cd-129">The following table shows the properties that are required when you create the [educationSchool](../resources/educationschool.md).</span></span>

| <span data-ttu-id="782cd-130">属性</span><span class="sxs-lookup"><span data-stu-id="782cd-130">Property</span></span>             | <span data-ttu-id="782cd-131">类型</span><span class="sxs-lookup"><span data-stu-id="782cd-131">Type</span></span>                                               | <span data-ttu-id="782cd-132">说明</span><span class="sxs-lookup"><span data-stu-id="782cd-132">Description</span></span>                                                                                                                                                          |
| :------------------- | :------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="782cd-133">displayName</span><span class="sxs-lookup"><span data-stu-id="782cd-133">displayName</span></span>          | <span data-ttu-id="782cd-134">String</span><span class="sxs-lookup"><span data-stu-id="782cd-134">String</span></span>                                             | <span data-ttu-id="782cd-135">学校的显示名称。</span><span class="sxs-lookup"><span data-stu-id="782cd-135">Display name of the school.</span></span> <span data-ttu-id="782cd-136">继承自 [educationOrganization](../resources/educationorganization.md)。</span><span class="sxs-lookup"><span data-stu-id="782cd-136">Inherited from [educationOrganization](../resources/educationorganization.md).</span></span>                                                           |
| <span data-ttu-id="782cd-137">说明</span><span class="sxs-lookup"><span data-stu-id="782cd-137">description</span></span>          | <span data-ttu-id="782cd-138">String</span><span class="sxs-lookup"><span data-stu-id="782cd-138">String</span></span>                                             | <span data-ttu-id="782cd-139">学校描述。</span><span class="sxs-lookup"><span data-stu-id="782cd-139">Description of the school.</span></span> <span data-ttu-id="782cd-140">继承自 [educationOrganization](../resources/educationorganization.md)。</span><span class="sxs-lookup"><span data-stu-id="782cd-140">Inherited from [educationOrganization](../resources/educationorganization.md).</span></span>                                                            |
| <span data-ttu-id="782cd-141">externalSource</span><span class="sxs-lookup"><span data-stu-id="782cd-141">externalSource</span></span>       | <span data-ttu-id="782cd-142">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="782cd-142">educationExternalSource</span></span>                            | <span data-ttu-id="782cd-143">创建组织的来源。</span><span class="sxs-lookup"><span data-stu-id="782cd-143">Source where this organization was created from.</span></span> <span data-ttu-id="782cd-144">继承自 [educationOrganization](../resources/educationorganization.md)。</span><span class="sxs-lookup"><span data-stu-id="782cd-144">Inherited from [educationOrganization](../resources/educationorganization.md).</span></span> <span data-ttu-id="782cd-145">可能的值是 `sis` ：、'manual。</span><span class="sxs-lookup"><span data-stu-id="782cd-145">Possible values are: `sis`, \`manual.</span></span> |
| <span data-ttu-id="782cd-146">externalSourceDetail</span><span class="sxs-lookup"><span data-stu-id="782cd-146">externalSourceDetail</span></span> | <span data-ttu-id="782cd-147">String</span><span class="sxs-lookup"><span data-stu-id="782cd-147">String</span></span>                                             | <span data-ttu-id="782cd-148">生成此资源的外部源的名称。</span><span class="sxs-lookup"><span data-stu-id="782cd-148">The name of the external source this resources was generated from.</span></span>                                                                                                   |
| <span data-ttu-id="782cd-149">principalEmail</span><span class="sxs-lookup"><span data-stu-id="782cd-149">principalEmail</span></span>       | <span data-ttu-id="782cd-150">String</span><span class="sxs-lookup"><span data-stu-id="782cd-150">String</span></span>                                             | <span data-ttu-id="782cd-151">主体的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="782cd-151">Email address of the principal.</span></span>                                                                                                                                      |
| <span data-ttu-id="782cd-152">principalName</span><span class="sxs-lookup"><span data-stu-id="782cd-152">principalName</span></span>        | <span data-ttu-id="782cd-153">String</span><span class="sxs-lookup"><span data-stu-id="782cd-153">String</span></span>                                             | <span data-ttu-id="782cd-154">主体名称。</span><span class="sxs-lookup"><span data-stu-id="782cd-154">Name of the principal.</span></span>                                                                                                                                               |
| <span data-ttu-id="782cd-155">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="782cd-155">externalPrincipalId</span></span>  | <span data-ttu-id="782cd-156">String</span><span class="sxs-lookup"><span data-stu-id="782cd-156">String</span></span>                                             | <span data-ttu-id="782cd-157">同步系统中主体的 ID。</span><span class="sxs-lookup"><span data-stu-id="782cd-157">ID of principal in syncing system.</span></span>                                                                                                                                   |
| <span data-ttu-id="782cd-158">highestGrade</span><span class="sxs-lookup"><span data-stu-id="782cd-158">highestGrade</span></span>         | <span data-ttu-id="782cd-159">String</span><span class="sxs-lookup"><span data-stu-id="782cd-159">String</span></span>                                             | <span data-ttu-id="782cd-160">教授的最高年级。</span><span class="sxs-lookup"><span data-stu-id="782cd-160">Highest grade taught.</span></span>                                                                                                                                                |
| <span data-ttu-id="782cd-161">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="782cd-161">lowestGrade</span></span>          | <span data-ttu-id="782cd-162">String</span><span class="sxs-lookup"><span data-stu-id="782cd-162">String</span></span>                                             | <span data-ttu-id="782cd-163">教授的最低年级。</span><span class="sxs-lookup"><span data-stu-id="782cd-163">Lowest grade taught.</span></span>                                                                                                                                                 |
| <span data-ttu-id="782cd-164">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="782cd-164">schoolNumber</span></span>         | <span data-ttu-id="782cd-165">String</span><span class="sxs-lookup"><span data-stu-id="782cd-165">String</span></span>                                             | <span data-ttu-id="782cd-166">学校编号。</span><span class="sxs-lookup"><span data-stu-id="782cd-166">School Number.</span></span>                                                                                                                                                       |
| <span data-ttu-id="782cd-167">externalId</span><span class="sxs-lookup"><span data-stu-id="782cd-167">externalId</span></span>           | <span data-ttu-id="782cd-168">String</span><span class="sxs-lookup"><span data-stu-id="782cd-168">String</span></span>                                             | <span data-ttu-id="782cd-169">同步系统中学校的 ID。</span><span class="sxs-lookup"><span data-stu-id="782cd-169">ID of school in syncing system.</span></span>                                                                                                                                      |
| <span data-ttu-id="782cd-170">phone</span><span class="sxs-lookup"><span data-stu-id="782cd-170">phone</span></span>                | <span data-ttu-id="782cd-171">String</span><span class="sxs-lookup"><span data-stu-id="782cd-171">String</span></span>                                             | <span data-ttu-id="782cd-172">学校电话号码。</span><span class="sxs-lookup"><span data-stu-id="782cd-172">Phone number of school.</span></span>                                                                                                                                              |
| <span data-ttu-id="782cd-173">fax</span><span class="sxs-lookup"><span data-stu-id="782cd-173">fax</span></span>                  | <span data-ttu-id="782cd-174">String</span><span class="sxs-lookup"><span data-stu-id="782cd-174">String</span></span>                                             | <span data-ttu-id="782cd-175">学校传真号码。</span><span class="sxs-lookup"><span data-stu-id="782cd-175">Fax number of school.</span></span>                                                                                                                                                |
| <span data-ttu-id="782cd-176">createdBy</span><span class="sxs-lookup"><span data-stu-id="782cd-176">createdBy</span></span>            | [<span data-ttu-id="782cd-177">identitySet</span><span class="sxs-lookup"><span data-stu-id="782cd-177">identitySet</span></span>](../resources/identityset.md)         | <span data-ttu-id="782cd-178">创建了学校的实体。</span><span class="sxs-lookup"><span data-stu-id="782cd-178">Entity who created the school.</span></span>                                                                                                                                       |
| <span data-ttu-id="782cd-179">address</span><span class="sxs-lookup"><span data-stu-id="782cd-179">address</span></span>              | [<span data-ttu-id="782cd-180">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="782cd-180">physicalAddress</span></span>](../resources/physicaladdress.md) | <span data-ttu-id="782cd-181">学校地址。</span><span class="sxs-lookup"><span data-stu-id="782cd-181">Address of the school.</span></span>                                                                                                                                               |

## <a name="response"></a><span data-ttu-id="782cd-182">响应</span><span class="sxs-lookup"><span data-stu-id="782cd-182">Response</span></span>

<span data-ttu-id="782cd-183">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [educationSchool](../resources/educationschool.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="782cd-183">If successful, this method returns a `201 Created` response code and an [educationSchool](../resources/educationschool.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="782cd-184">示例</span><span class="sxs-lookup"><span data-stu-id="782cd-184">Examples</span></span>

### <a name="request"></a><span data-ttu-id="782cd-185">请求</span><span class="sxs-lookup"><span data-stu-id="782cd-185">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_educationschool_from_"
}
-->

```http
POST https://graph.microsoft.com/v1.0/education/schools
Content-Type: application/json
Content-length: 583

{
  "@odata.type": "#microsoft.graph.educationSchool",
  "displayName": "String",
  "description": "String",
  "externalSource": "String",
  "externalSourceDetail": "String",
  "principalEmail": "String",
  "principalName": "String",
  "externalPrincipalId": "String",
  "lowestGrade": "String",
  "highestGrade": "String",
  "schoolNumber": "String",
  "externalId": "String",
  "phone": "String",
  "fax": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "address": {
    "@odata.type": "microsoft.graph.physicalAddress"
  }
}
```

### <a name="response"></a><span data-ttu-id="782cd-186">响应</span><span class="sxs-lookup"><span data-stu-id="782cd-186">Response</span></span>

> <span data-ttu-id="782cd-187">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="782cd-187">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool"
}
-->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.educationSchool",
  "id": "1c23c12e-c12e-1c23-2ec1-231c2ec1231c",
  "displayName": "String",
  "description": "String",
  "externalSource": "String",
  "externalSourceDetail": "String",
  "principalEmail": "String",
  "principalName": "String",
  "externalPrincipalId": "String",
  "lowestGrade": "String",
  "highestGrade": "String",
  "schoolNumber": "String",
  "externalId": "String",
  "phone": "String",
  "fax": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "address": {
    "@odata.type": "microsoft.graph.physicalAddress"
  }
}
```
