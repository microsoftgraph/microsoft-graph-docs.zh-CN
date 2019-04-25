---
title: 创建 outlookTaskFolder
description: 在用户邮箱的默认任务组 (`My Tasks`) 中创建一个任务文件夹。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 16f54dffc1ff2fff71a22658a2418be99fde7353
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32539630"
---
# <a name="create-outlooktaskfolder"></a><span data-ttu-id="a53ef-103">创建 outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="a53ef-103">Create outlookTaskFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a53ef-104">在用户邮箱的默认任务组 (`My Tasks`) 中创建一个任务文件夹。</span><span class="sxs-lookup"><span data-stu-id="a53ef-104">Create a task folder in the default task group (`My Tasks`) of the user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="a53ef-105">权限</span><span class="sxs-lookup"><span data-stu-id="a53ef-105">Permissions</span></span>
<span data-ttu-id="a53ef-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a53ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a53ef-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="a53ef-108">Permission type</span></span>      | <span data-ttu-id="a53ef-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a53ef-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a53ef-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a53ef-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a53ef-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a53ef-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="a53ef-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a53ef-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a53ef-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a53ef-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="a53ef-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="a53ef-114">Application</span></span> | <span data-ttu-id="a53ef-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a53ef-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a53ef-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a53ef-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/taskFolders
POST /users/{id|userPrincipalName}/outlook/taskFolders
```
## <a name="request-headers"></a><span data-ttu-id="a53ef-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="a53ef-117">Request headers</span></span>
| <span data-ttu-id="a53ef-118">名称</span><span class="sxs-lookup"><span data-stu-id="a53ef-118">Name</span></span>       | <span data-ttu-id="a53ef-119">说明</span><span class="sxs-lookup"><span data-stu-id="a53ef-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a53ef-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="a53ef-120">Authorization</span></span>  | <span data-ttu-id="a53ef-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a53ef-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a53ef-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="a53ef-123">Request body</span></span>
<span data-ttu-id="a53ef-124">在请求正文中, 提供[outlookTaskFolder](../resources/outlooktaskfolder.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a53ef-124">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a53ef-125">响应</span><span class="sxs-lookup"><span data-stu-id="a53ef-125">Response</span></span>

<span data-ttu-id="a53ef-126">如果成功, 此方法在`201 Created`响应正文中返回响应代码和[outlookTaskFolder](../resources/outlooktaskfolder.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a53ef-126">If successful, this method returns `201 Created` response code and [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a53ef-127">示例</span><span class="sxs-lookup"><span data-stu-id="a53ef-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a53ef-128">请求</span><span class="sxs-lookup"><span data-stu-id="a53ef-128">Request</span></span>
<span data-ttu-id="a53ef-129">下面的示例在用户邮箱的默认任务组 (`My Tasks`) 中创建名为 "志愿者" 的任务文件夹。</span><span class="sxs-lookup"><span data-stu-id="a53ef-129">The following example creates a task folder called Volunteer in the default task group (`My Tasks`) of the user's mailbox.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_outlooktaskfolder_from_outlookuser"
}-->
```http
POST https://graph.microsoft.com/beta/me/outlook/taskfolders 
Content-type: application/json
Content-length: 60

{
  "name": "Volunteer"
}
```
<span data-ttu-id="a53ef-130">在请求正文中, 提供[outlookTaskFolder](../resources/outlooktaskfolder.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a53ef-130">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="a53ef-131">响应</span><span class="sxs-lookup"><span data-stu-id="a53ef-131">Response</span></span>
<span data-ttu-id="a53ef-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a53ef-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskFolder"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 151

{
  "id": "AAMkADIyAAAhrbPWAAA=",
  "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAIbAGig==",
  "isDefaultFolder": false,
  "name": "Volunteer",
  "parentGroupKey": "0006f0b7-0000-0000-c000-000000000046"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create outlookTaskFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlookuser-post-taskfolders.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
