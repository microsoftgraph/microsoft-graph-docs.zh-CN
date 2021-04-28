---
title: 共享的列表
description: 计算得出的见解，可返回与用户共享的文件列表。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 0b799be314ce9f2519d7174c84f9349b09bbd5c3
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050421"
---
# <a name="list-shared"></a><span data-ttu-id="2ab92-103">共享的列表</span><span class="sxs-lookup"><span data-stu-id="2ab92-103">List shared</span></span>

<span data-ttu-id="2ab92-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ab92-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2ab92-105">包含与用户共享的文档列表的计算见解。</span><span class="sxs-lookup"><span data-stu-id="2ab92-105">Calculated insight that includes the list of documents shared with a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="2ab92-106">权限</span><span class="sxs-lookup"><span data-stu-id="2ab92-106">Permissions</span></span>
<span data-ttu-id="2ab92-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2ab92-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ab92-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2ab92-109">Permission type</span></span>      | <span data-ttu-id="2ab92-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2ab92-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2ab92-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2ab92-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2ab92-112">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ab92-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="2ab92-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2ab92-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ab92-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2ab92-114">Not supported.</span></span>    |
|<span data-ttu-id="2ab92-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2ab92-115">Application</span></span> | <span data-ttu-id="2ab92-116">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ab92-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2ab92-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2ab92-117">HTTP request</span></span>
<span data-ttu-id="2ab92-118">获取与登录用户共享的文档列表。</span><span class="sxs-lookup"><span data-stu-id="2ab92-118">Get a list of documents shared with the signed-in user.</span></span>

><span data-ttu-id="2ab92-119">**注意**：只有用户才能使用用户的 ID 或主体名称提出请求。</span><span class="sxs-lookup"><span data-stu-id="2ab92-119">**Note**: Only the user can make requests using the user's id or principal name.</span></span>

```http
GET /me/insights/shared
GET /users/{id | userPrincipalName}/insights/shared
```

<span data-ttu-id="2ab92-120">展开共享 **见解所引用** 的资源：</span><span class="sxs-lookup"><span data-stu-id="2ab92-120">Expand the resource referenced by a **shared** insight:</span></span>
```http
GET https://graph.microsoft.com/v1.0/me/insights/shared/{id}/resource
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2ab92-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2ab92-121">Optional query parameters</span></span>
<span data-ttu-id="2ab92-122">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="2ab92-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="2ab92-123">可以使用查询 `$filter` 参数筛选共享项目。</span><span class="sxs-lookup"><span data-stu-id="2ab92-123">You can use the `$filter` query parameter to filter shared items.</span></span> <span data-ttu-id="2ab92-124">例如，根据 **类型**：</span><span class="sxs-lookup"><span data-stu-id="2ab92-124">For example, based on **type**:</span></span>

`https://graph.microsoft.com/v1.0/me/insights/shared?$filter=ResourceVisualization/Type eq 'PowerPoint'`

<span data-ttu-id="2ab92-125">请参阅 [resourceVisualization](../resources/insights-resourcevisualization.md)中可以按筛选的可用容器类型和类型。</span><span class="sxs-lookup"><span data-stu-id="2ab92-125">See the available container types and types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>

<span data-ttu-id="2ab92-126">还可以检索特定用户共享的文件。</span><span class="sxs-lookup"><span data-stu-id="2ab92-126">You can also retrieve files shared by a specific user.</span></span> <span data-ttu-id="2ab92-127">例如，通过指定 `lastshared/sharedby/address` 属性：</span><span class="sxs-lookup"><span data-stu-id="2ab92-127">For example, by specifying the `lastshared/sharedby/address` property:</span></span>

`https://graph.microsoft.com/v1.0/me/insights/shared?$filter=lastshared/sharedby/address eq 'kellygraham@contoso.com'`

<span data-ttu-id="2ab92-128">请参阅 [sharingDetail](../resources/insights-sharingdetail.md) 复杂类型。</span><span class="sxs-lookup"><span data-stu-id="2ab92-128">See the [sharingDetail](../resources/insights-sharingdetail.md) complex type.</span></span>


## <a name="request-headers"></a><span data-ttu-id="2ab92-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="2ab92-129">Request headers</span></span>
| <span data-ttu-id="2ab92-130">标头</span><span class="sxs-lookup"><span data-stu-id="2ab92-130">Header</span></span>       |  <span data-ttu-id="2ab92-131">值</span><span class="sxs-lookup"><span data-stu-id="2ab92-131">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="2ab92-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ab92-132">Authorization</span></span>  | <span data-ttu-id="2ab92-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2ab92-p104">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="2ab92-135">接受</span><span class="sxs-lookup"><span data-stu-id="2ab92-135">Accept</span></span>  | <span data-ttu-id="2ab92-136">application/json</span><span class="sxs-lookup"><span data-stu-id="2ab92-136">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ab92-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="2ab92-137">Request body</span></span>
<span data-ttu-id="2ab92-138">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2ab92-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ab92-139">响应</span><span class="sxs-lookup"><span data-stu-id="2ab92-139">Response</span></span>

<span data-ttu-id="2ab92-140">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和[](../resources/insights-shared.md)共享项列表。</span><span class="sxs-lookup"><span data-stu-id="2ab92-140">If successful, this method returns a `200 OK` response code and a list of [shared](../resources/insights-shared.md) items in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2ab92-141">示例</span><span class="sxs-lookup"><span data-stu-id="2ab92-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2ab92-142">请求</span><span class="sxs-lookup"><span data-stu-id="2ab92-142">Request</span></span>

<span data-ttu-id="2ab92-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2ab92-143">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/v1.0/me/insights/shared
```

##### <a name="response"></a><span data-ttu-id="2ab92-144">响应</span><span class="sxs-lookup"><span data-stu-id="2ab92-144">Response</span></span>

<span data-ttu-id="2ab92-145">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="2ab92-145">Here is an example of the response.</span></span> <span data-ttu-id="2ab92-146">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2ab92-146">Note: The response object shown here might be shortened for readability.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "AWb0Qy4TEA1KhLW-k1L5mSjtxZAcxDFkTKiTNA-2kZDTXzrMX_4FhECOU0bKZVj1uReivYoYYoJNqTeuC-x1Agtm9EMuExANSoS1vpNS-ZkoBA",
            "lastShared": {
                "sharedDateTime": "2021-03-23T08:41:05Z",
                "sharingType": "Direct",
                "sharedBy": {
                    "displayName": "Megan Bowen",
                    "address": "MeganB@contoso.com",
                    "id": "3e0c9f05-b9b8-4cf5-9b35-a4e11b24b5b7"
                },
                "sharingReference": {}
            },
            "resourceVisualization": {
                "title": "CE Annual Report",
                "type": "Word",
                "mediaType": "application/vnd.openxmlformats-officedocument.wordprocessingml.document",
                "previewImageUrl": "https://contoso-my.sharepoint.com/_api/v2.0/drives/b!ZvRDLhMQDUqEtb6TUvmZKO3FkBzEMWRMqJM0D7aRkNNfOsxf_gWEQI5TRsplWPW5/items/01K6ZMU4QXUK6YUGDCQJG2SN5OBPWHKAQL/thumbnails/0/small/thumbnailContent",
                "previewText": "Contoso Annual Report Anne Wallace Sales Contoso today announced financial results for its most recent fi",
                "containerWebUrl": "https://contoso-my.sharepoint.com/personal/meganb_m365x841051_onmicrosoft_com/Documents/Forms/All.aspx",
                "containerDisplayName": "Megan Bowen",
                "containerType": "OneDriveBusiness"
            },
            "resourceReference": {
                "webUrl": "https://contoso-my.sharepoint.com/personal/meganb_m365x841051_onmicrosoft_com/_layouts/15/Doc.aspx?sourcedoc=%7B8ABDA217-6218-4D82-A937-AE0BEC75020B%7D&file=CE%20Annual%20Report.docx&action=default&mobileredirect=true&DefaultItemOpen=1",
                "id": "drives/b!ZvRDLhMQDUqEtb6TUvmZKO3FkBzEMWRMqJM0D7aRkNNfOsxf_gWEQI5TRsplWPW5/items/01K6ZMU4QXUK6YUGDCQJG2SN5OBPWHKAQL",
                "type": "microsoft.graph.driveItem"
            }
        }
    ]
}
```
