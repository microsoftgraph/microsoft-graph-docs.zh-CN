---
title: educationSubmission： setUpResourcesFolder
description: 触发创建 SharePoint 资源文件夹，其中应针对给定提交 (Word、Excel 等) 所有基于文件的资源。
localization_priority: Normal
author: sharmas
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: d290f47ccc1dcbfaa5aeae85ed28071e0a15399e
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52546887"
---
# <a name="educationsubmission-setupresourcesfolder"></a><span data-ttu-id="ded41-103">educationSubmission： setUpResourcesFolder</span><span class="sxs-lookup"><span data-stu-id="ded41-103">educationSubmission: setUpResourcesFolder</span></span>

<span data-ttu-id="ded41-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ded41-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ded41-105">触发创建 SharePoint 资源文件夹，其中应针对给定提交 (Word、Excel 等) 所有基于文件的资源。</span><span class="sxs-lookup"><span data-stu-id="ded41-105">Trigger the creation of the SharePoint resource folder where all file-based resources (Word, Excel, and so on) should be uploaded for a given submission.</span></span>

<span data-ttu-id="ded41-106">请注意，文件必须位于此文件夹中才能添加为资源。</span><span class="sxs-lookup"><span data-stu-id="ded41-106">Note that files must be located in this folder in order to be added as resources.</span></span> <span data-ttu-id="ded41-107">只有班级中的学生可以确定要上载到给定提交级别资源文件夹中的文件。</span><span class="sxs-lookup"><span data-stu-id="ded41-107">Only a student in the class can determine what files to upload in a given submission-level resource folder.</span></span> 

## <a name="permissions"></a><span data-ttu-id="ded41-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="ded41-108">Permissions</span></span>
<span data-ttu-id="ded41-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ded41-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ded41-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ded41-111">Permission type</span></span>      | <span data-ttu-id="ded41-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ded41-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ded41-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ded41-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="ded41-114">EduAssignments.ReadBasic、EduAssignments.Read</span><span class="sxs-lookup"><span data-stu-id="ded41-114">EduAssignments.ReadBasic, EduAssignments.Read</span></span>  |
|<span data-ttu-id="ded41-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ded41-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="ded41-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ded41-116">Not supported.</span></span>  |
|<span data-ttu-id="ded41-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ded41-117">Application</span></span> | <span data-ttu-id="ded41-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="ded41-118">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="ded41-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ded41-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/setUpResourcesFolder

```
## <a name="request-headers"></a><span data-ttu-id="ded41-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ded41-120">Request headers</span></span>
| <span data-ttu-id="ded41-121">标头</span><span class="sxs-lookup"><span data-stu-id="ded41-121">Header</span></span>       | <span data-ttu-id="ded41-122">值</span><span class="sxs-lookup"><span data-stu-id="ded41-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ded41-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ded41-123">Authorization</span></span>  | <span data-ttu-id="ded41-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ded41-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ded41-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ded41-126">Request body</span></span>
<span data-ttu-id="ded41-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ded41-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="ded41-128">响应</span><span class="sxs-lookup"><span data-stu-id="ded41-128">Response</span></span>
<span data-ttu-id="ded41-129">如果成功，此方法返回 `200 Ok` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="ded41-129">If successful, this method returns a `200 Ok` response code.</span></span> <span data-ttu-id="ded41-130">正文将包含提交模型。</span><span class="sxs-lookup"><span data-stu-id="ded41-130">The body will contain the submission model.</span></span>

## <a name="example"></a><span data-ttu-id="ded41-131">示例</span><span class="sxs-lookup"><span data-stu-id="ded41-131">Example</span></span>
<span data-ttu-id="ded41-132">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="ded41-132">The following example shows how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="ded41-133">请求</span><span class="sxs-lookup"><span data-stu-id="ded41-133">Request</span></span>
<span data-ttu-id="ded41-134">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="ded41-134">The following is an example of a request.</span></span>

<!-- {
  "blockType": "request",
  "name": "educationsubmission_setupresourcesfolder"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/beta/education/classes/11012/assignments/19002/submissions/20302/setUpResourcesFolder
```
---


### <a name="response"></a><span data-ttu-id="ded41-135">响应</span><span class="sxs-lookup"><span data-stu-id="ded41-135">Response</span></span>
<span data-ttu-id="ded41-136">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="ded41-136">The following is an example of a response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmission"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 279

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/classes('b07edbef-7420-4b3d-8f7c-d599cf21e069')/assignments('1e5222bd-b7d2-4d64-8a22-74b722ce2fc6')/submissions/$entity",
    "status": "working",
    "submittedDateTime": null,
    "unsubmittedDateTime": null,
    "returnedDateTime": null,
    "resourcesFolderUrl": "https://graph.microsoft.com/v1.0/drives/b!6SQl0y4WHkS2P5MeIsSGpKwfynEIaD1OvPVeH4wbOp_1uyhNwJMSSpseJneB7Z4F/items/01YT2AIJRQLVYT24IWWFAJHMRRNYCB3GE2",
    "id": "803fb5dd-3553-455f-3d94-f79fb54a1003",
    "recipient": {
        "@odata.type": "#microsoft.graph.educationSubmissionIndividualRecipient",
        "userId": "f8bbb2a4-2cdd-4d49-ac81-d4113fc72dc1"
    },
    "submittedBy": {
        "application": null,
        "device": null,
        "user": {
            "id": "f8bbb2a4-2cdd-4d49-ac81-d4113fc72dc1",
            "displayName": null
        }
    },
    "unsubmittedBy": {
        "application": null,
        "device": null,
        "user": {
            "id": null,
            "displayName": null
        }
    },
    "returnedBy": {
        "application": null,
        "device": null,
        "user": {
            "id": null,
            "displayName": null
        }
    },
    "resources@odata.context": "https://graph.microsoft.com/beta/$metadata#education/classes('b07edbef-7420-4b3d-8f7c-d599cf21e069')/assignments('1e5222bd-b7d2-4d64-8a22-74b722ce2fc6')/submissions('803fb5dd-3553-455f-3d94-f79fb54a1003')/resources",
    "resources": [],
    "submittedResources@odata.context": "https://graph.microsoft.com/beta/$metadata#education/classes('b07edbef-7420-4b3d-8f7c-d599cf21e069')/assignments('1e5222bd-b7d2-4d64-8a22-74b722ce2fc6')/submissions('803fb5dd-3553-455f-3d94-f79fb54a1003')/submittedResources",
    "submittedResources": []
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-d4113fc72dc1
2021-05-12 12:00:00 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationSubmission: setUpResourcesFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


