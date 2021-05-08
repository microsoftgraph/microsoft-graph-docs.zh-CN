---
title: 创建 educationClass
description: 创建新的 educationClass 对象。
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 71dcda18e56b6dfd53fa35943e6da246b5b8d68f
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232180"
---
# <a name="create-educationclass"></a><span data-ttu-id="d4cb3-103">创建 educationClass</span><span class="sxs-lookup"><span data-stu-id="d4cb3-103">Create educationClass</span></span>

<span data-ttu-id="d4cb3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4cb3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d4cb3-105">创建新的 [educationClass](../resources/educationclass.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d4cb3-105">Create a new [educationClass](../resources/educationclass.md) object.</span></span>

> [!NOTE]
> <span data-ttu-id="d4cb3-106">此操作还会创建通用组。</span><span class="sxs-lookup"><span data-stu-id="d4cb3-106">This will also create a universal group.</span></span> <span data-ttu-id="d4cb3-107">使用此 API 创建课程时，它会向组添加特殊属性，这将在使用组创建团队时在 Microsoft Teams 中添加分配和特殊处理等功能。</span><span class="sxs-lookup"><span data-stu-id="d4cb3-107">When you use this API to create a class, it will add special properties to the group, which will add features such as assignments and special handling within Microsoft Teams when teams are created using the group.</span></span> <span data-ttu-id="d4cb3-108">请注意，此 API 仅创建通用组，不会创建团队。</span><span class="sxs-lookup"><span data-stu-id="d4cb3-108">Please note that this API only creates the universal group and does not create a team.</span></span> <span data-ttu-id="d4cb3-109">Microsoft Teams为教师提供用户界面，以使用此 API 创建的组创建自己的班级团队。</span><span class="sxs-lookup"><span data-stu-id="d4cb3-109">Microsoft Teams provides a user interface for teachers to create teams for their own classes using the groups created by this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="d4cb3-110">权限</span><span class="sxs-lookup"><span data-stu-id="d4cb3-110">Permissions</span></span>

<span data-ttu-id="d4cb3-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d4cb3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d4cb3-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="d4cb3-113">Permission type</span></span>                        | <span data-ttu-id="d4cb3-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d4cb3-114">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="d4cb3-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d4cb3-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="d4cb3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d4cb3-116">Not supported.</span></span>                              |
| <span data-ttu-id="d4cb3-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d4cb3-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4cb3-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="d4cb3-118">Not supported.</span></span>                              |
| <span data-ttu-id="d4cb3-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="d4cb3-119">Application</span></span>                            | <span data-ttu-id="d4cb3-120">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4cb3-120">EduRoster.ReadWrite.All</span></span>                     |

## <a name="http-request"></a><span data-ttu-id="d4cb3-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d4cb3-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
POST /education/classes
```

## <a name="request-headers"></a><span data-ttu-id="d4cb3-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="d4cb3-122">Request headers</span></span>

| <span data-ttu-id="d4cb3-123">名称</span><span class="sxs-lookup"><span data-stu-id="d4cb3-123">Name</span></span>          | <span data-ttu-id="d4cb3-124">说明</span><span class="sxs-lookup"><span data-stu-id="d4cb3-124">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="d4cb3-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4cb3-125">Authorization</span></span> | <span data-ttu-id="d4cb3-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d4cb3-p103">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="d4cb3-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d4cb3-128">Content-Type</span></span>  | <span data-ttu-id="d4cb3-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="d4cb3-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d4cb3-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="d4cb3-131">Request body</span></span>

<span data-ttu-id="d4cb3-132">在请求正文中，提供 [educationClass](../resources/educationclass.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d4cb3-132">In the request body, supply a JSON representation of the [educationClass](../resources/educationclass.md) object.</span></span>

<span data-ttu-id="d4cb3-133">下表显示创建 [educationClass](../resources/educationclass.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d4cb3-133">The following table shows the properties that are required when you create the [educationClass](../resources/educationclass.md).</span></span>

| <span data-ttu-id="d4cb3-134">属性</span><span class="sxs-lookup"><span data-stu-id="d4cb3-134">Property</span></span>             | <span data-ttu-id="d4cb3-135">类型</span><span class="sxs-lookup"><span data-stu-id="d4cb3-135">Type</span></span>                                           | <span data-ttu-id="d4cb3-136">说明</span><span class="sxs-lookup"><span data-stu-id="d4cb3-136">Description</span></span>                                                        |
| :------------------- | :--------------------------------------------- | :----------------------------------------------------------------- |
| <span data-ttu-id="d4cb3-137">id</span><span class="sxs-lookup"><span data-stu-id="d4cb3-137">id</span></span>                   | <span data-ttu-id="d4cb3-138">String</span><span class="sxs-lookup"><span data-stu-id="d4cb3-138">String</span></span>                                         | <span data-ttu-id="d4cb3-139">对象标识符。</span><span class="sxs-lookup"><span data-stu-id="d4cb3-139">Object identifier.</span></span> <span data-ttu-id="d4cb3-140">继承自 [实体](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="d4cb3-140">Inherited from [entity](../resources/entity.md)</span></span> |
| <span data-ttu-id="d4cb3-141">displayName</span><span class="sxs-lookup"><span data-stu-id="d4cb3-141">displayName</span></span>          | <span data-ttu-id="d4cb3-142">String</span><span class="sxs-lookup"><span data-stu-id="d4cb3-142">String</span></span>                                         | <span data-ttu-id="d4cb3-143">课程名称。</span><span class="sxs-lookup"><span data-stu-id="d4cb3-143">Name of the class.</span></span>                                                 |
| <span data-ttu-id="d4cb3-144">mailNickname</span><span class="sxs-lookup"><span data-stu-id="d4cb3-144">mailNickname</span></span>         | <span data-ttu-id="d4cb3-145">String</span><span class="sxs-lookup"><span data-stu-id="d4cb3-145">String</span></span>                                         | <span data-ttu-id="d4cb3-146">向所有成员发送电子邮件的邮件名称（如果已启用）。</span><span class="sxs-lookup"><span data-stu-id="d4cb3-146">Mail name for sending email to all members, if this is enabled.</span></span>    |
| <span data-ttu-id="d4cb3-147">说明</span><span class="sxs-lookup"><span data-stu-id="d4cb3-147">description</span></span>          | <span data-ttu-id="d4cb3-148">String</span><span class="sxs-lookup"><span data-stu-id="d4cb3-148">String</span></span>                                         | <span data-ttu-id="d4cb3-149">课程说明。</span><span class="sxs-lookup"><span data-stu-id="d4cb3-149">Description of the class.</span></span>                                          |
| <span data-ttu-id="d4cb3-150">createdBy</span><span class="sxs-lookup"><span data-stu-id="d4cb3-150">createdBy</span></span>            | [<span data-ttu-id="d4cb3-151">identitySet</span><span class="sxs-lookup"><span data-stu-id="d4cb3-151">identitySet</span></span>](../resources/identityset.md)     | <span data-ttu-id="d4cb3-152">创建了课程的实体</span><span class="sxs-lookup"><span data-stu-id="d4cb3-152">Entity who created the class</span></span>                                       |
| <span data-ttu-id="d4cb3-153">classCode</span><span class="sxs-lookup"><span data-stu-id="d4cb3-153">classCode</span></span>            | <span data-ttu-id="d4cb3-154">String</span><span class="sxs-lookup"><span data-stu-id="d4cb3-154">String</span></span>                                         | <span data-ttu-id="d4cb3-155">学校用于标识课程的课程代码。</span><span class="sxs-lookup"><span data-stu-id="d4cb3-155">Class code used by the school to identify the class.</span></span>               |
| <span data-ttu-id="d4cb3-156">externalName</span><span class="sxs-lookup"><span data-stu-id="d4cb3-156">externalName</span></span>         | <span data-ttu-id="d4cb3-157">String</span><span class="sxs-lookup"><span data-stu-id="d4cb3-157">String</span></span>                                         | <span data-ttu-id="d4cb3-158">同步系统中的课程名称。</span><span class="sxs-lookup"><span data-stu-id="d4cb3-158">Name of the class in the syncing system.</span></span>                           |
| <span data-ttu-id="d4cb3-159">externalId</span><span class="sxs-lookup"><span data-stu-id="d4cb3-159">externalId</span></span>           | <span data-ttu-id="d4cb3-160">String</span><span class="sxs-lookup"><span data-stu-id="d4cb3-160">String</span></span>                                         | <span data-ttu-id="d4cb3-161">来自同步系统的课程 ID。</span><span class="sxs-lookup"><span data-stu-id="d4cb3-161">ID of the class from the syncing system.</span></span>                           |
| <span data-ttu-id="d4cb3-162">externalSource</span><span class="sxs-lookup"><span data-stu-id="d4cb3-162">externalSource</span></span>       | <span data-ttu-id="d4cb3-163">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="d4cb3-163">educationExternalSource</span></span>                        | <span data-ttu-id="d4cb3-164">此课程的创建方式。</span><span class="sxs-lookup"><span data-stu-id="d4cb3-164">How this class was created.</span></span> <span data-ttu-id="d4cb3-165">可能的值包括： `sis` 、 `manual`</span><span class="sxs-lookup"><span data-stu-id="d4cb3-165">Possible values are: `sis`, `manual`</span></span>   |
| <span data-ttu-id="d4cb3-166">externalSourceDetail</span><span class="sxs-lookup"><span data-stu-id="d4cb3-166">externalSourceDetail</span></span> | <span data-ttu-id="d4cb3-167">String</span><span class="sxs-lookup"><span data-stu-id="d4cb3-167">String</span></span>                                         | <span data-ttu-id="d4cb3-168">生成此资源的外部源的名称。</span><span class="sxs-lookup"><span data-stu-id="d4cb3-168">The name of the external source this resources was generated from.</span></span> |
| <span data-ttu-id="d4cb3-169">grade</span><span class="sxs-lookup"><span data-stu-id="d4cb3-169">grade</span></span>                | <span data-ttu-id="d4cb3-170">String</span><span class="sxs-lookup"><span data-stu-id="d4cb3-170">String</span></span>                                         | <span data-ttu-id="d4cb3-171">课程的年级。</span><span class="sxs-lookup"><span data-stu-id="d4cb3-171">Grade level of the class.</span></span>                                          |
| <span data-ttu-id="d4cb3-172">term</span><span class="sxs-lookup"><span data-stu-id="d4cb3-172">term</span></span>                 | [<span data-ttu-id="d4cb3-173">educationTerm</span><span class="sxs-lookup"><span data-stu-id="d4cb3-173">educationTerm</span></span>](../resources/educationterm.md) | <span data-ttu-id="d4cb3-174">此课程的学期。</span><span class="sxs-lookup"><span data-stu-id="d4cb3-174">Term for this class.</span></span>                                               |

## <a name="response"></a><span data-ttu-id="d4cb3-175">响应</span><span class="sxs-lookup"><span data-stu-id="d4cb3-175">Response</span></span>

<span data-ttu-id="d4cb3-176">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [educationClass](../resources/educationclass.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d4cb3-176">If successful, this method returns a `201 Created` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d4cb3-177">示例</span><span class="sxs-lookup"><span data-stu-id="d4cb3-177">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d4cb3-178">请求</span><span class="sxs-lookup"><span data-stu-id="d4cb3-178">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_"
}
-->

```http
POST https://graph.microsoft.com/v1.0/education/classes
Content-Type: application/json
Content-length: 533

{
  "@odata.type": "#microsoft.graph.educationClass",
  "displayName": "String",
  "mailNickname": "String",
  "description": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "classCode": "String",
  "externalName": "String",
  "externalId": "String",
  "externalSource": "String",
  "externalSourceDetail": "String",
  "grade": "String",
  "term": {
    "@odata.type": "microsoft.graph.educationTerm"
  }
}
```

### <a name="response"></a><span data-ttu-id="d4cb3-179">响应</span><span class="sxs-lookup"><span data-stu-id="d4cb3-179">Response</span></span>

> <span data-ttu-id="d4cb3-180">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d4cb3-180">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
}
-->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.educationClass",
  "id": "64ef8ce5-8ce5-64ef-e58c-ef64e58cef64",
  "displayName": "String",
  "mailNickname": "String",
  "description": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "classCode": "String",
  "externalName": "String",
  "externalId": "String",
  "externalSource": "String",
  "externalSourceDetail": "String",
  "grade": "String",
  "term": {
    "@odata.type": "microsoft.graph.educationTerm"
  }
}
```
