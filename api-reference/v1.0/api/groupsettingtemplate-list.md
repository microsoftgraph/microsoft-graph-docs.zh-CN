---
title: List groupSettingTemplates
description: 组设置模板表示一组模板，用于创建组设置并在租户内使用。此操作将检索可用 groupSettingTemplates 对象的列表。
ms.openlocfilehash: e3a92b174b4d1d95cbbf22385b56484441a6e3eb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011170"
---
# <a name="list-groupsettingtemplates"></a><span data-ttu-id="03393-104">List groupSettingTemplates</span><span class="sxs-lookup"><span data-stu-id="03393-104">List groupSettingTemplates</span></span>

<span data-ttu-id="03393-p102">组设置模板表示一组模板，用于创建组设置并在租户内使用。此操作将检索可用 groupSettingTemplates 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="03393-p102">Group setting templates represents a set of templates  from which group settings may be created and used within a tenant.  This operation retrieves the list of available groupSettingTemplates objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="03393-107">权限</span><span class="sxs-lookup"><span data-stu-id="03393-107">Permissions</span></span>

<span data-ttu-id="03393-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="03393-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="03393-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="03393-110">Permission type</span></span>      | <span data-ttu-id="03393-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="03393-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="03393-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="03393-112">Delegated (work or school account)</span></span> | <span data-ttu-id="03393-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="03393-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="03393-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="03393-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03393-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="03393-115">Not supported.</span></span>    |
|<span data-ttu-id="03393-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="03393-116">Application</span></span> | <span data-ttu-id="03393-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03393-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="03393-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="03393-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupSettingTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="03393-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="03393-119">Optional query parameters</span></span>
<span data-ttu-id="03393-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="03393-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

> <span data-ttu-id="03393-121">**注意：** 不支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="03393-121">**Note:** $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="03393-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="03393-122">Request headers</span></span>
| <span data-ttu-id="03393-123">名称</span><span class="sxs-lookup"><span data-stu-id="03393-123">Name</span></span> | <span data-ttu-id="03393-124">说明</span><span class="sxs-lookup"><span data-stu-id="03393-124">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="03393-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="03393-125">Authorization</span></span>  | <span data-ttu-id="03393-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="03393-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="03393-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="03393-128">Request body</span></span>
<span data-ttu-id="03393-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="03393-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="03393-130">响应</span><span class="sxs-lookup"><span data-stu-id="03393-130">Response</span></span>

<span data-ttu-id="03393-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [groupSettingTemplate](../resources/groupsettingtemplate.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="03393-131">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/groupsettingtemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03393-132">示例</span><span class="sxs-lookup"><span data-stu-id="03393-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="03393-133">请求</span><span class="sxs-lookup"><span data-stu-id="03393-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groupsettingtemplates"
}-->
```http
GET https://graph.microsoft.com/v1.0/groupSettingTemplates
```
##### <a name="response"></a><span data-ttu-id="03393-134">响应</span><span class="sxs-lookup"><span data-stu-id="03393-134">Response</span></span>

<span data-ttu-id="03393-p105">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="03393-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSettingTemplate",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1770

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groupSettingTemplates",
    "value": [
                {
                    "id": "62375ab9-6b52-47ed-826b-58e47e0e304b",
                    "deletedDateTime": null,
                    "displayName": "Group.Unified",
                    "description": "Setting templates define the different settings that can be used for the associated ObjectSettings. This template defines settings that can be used for Unified Groups.",
                    "values": [
                        {
                            "name": "CustomBlockedWordsList",
                            "type": "System.String",
                            "defaultValue": "",
                            "description": "A comma-delimited list of blocked words for Unified Group displayName and mailNickName."
                        },
                        {
                            "name": "EnableMSStandardBlockedWords",
                            "type": "System.Boolean",
                            "defaultValue": "false",
                            "description": "A flag indicating whether or not to enable the Microsoft Standard list of blocked words for Unified Group displayName and mailNickName."
                        },
                        {
                            "name": "ClassificationDescriptions",
                            "type": "System.String",
                            "defaultValue": "",
                            "description": "A comma-delimited list of structured strings describing the classification values in the ClassificationList. The structure of the string is: Value: Description"
                        }
                    ]
                }
            ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groupSettingTemplates",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->