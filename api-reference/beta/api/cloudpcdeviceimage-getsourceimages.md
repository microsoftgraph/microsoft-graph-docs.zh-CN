---
title: cloudPcDeviceImage：getSourceImages
description: 查看 Azure 订阅中所有托管图像资源的列表。 这些源图像可以上载并用于云电脑。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 338f05f7ae2645c76b9ddb34a0d1af6f29beb35f
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52546845"
---
# <a name="cloudpcdeviceimage-getsourceimages"></a><span data-ttu-id="d73f3-104">cloudPcDeviceImage：getSourceImages</span><span class="sxs-lookup"><span data-stu-id="d73f3-104">cloudPcDeviceImage: getSourceImages</span></span>

<span data-ttu-id="d73f3-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d73f3-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d73f3-106">获取 [cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d73f3-106">Get [cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) objects.</span></span> <span data-ttu-id="d73f3-107">查看你的订阅的所有托管映像资源Azure Active Directory列表。</span><span class="sxs-lookup"><span data-stu-id="d73f3-107">View a list of all the managed image resources from your Azure Active Directory subscriptions.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="permissions"></a><span data-ttu-id="d73f3-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="d73f3-108">Permissions</span></span>

<span data-ttu-id="d73f3-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d73f3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d73f3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d73f3-111">Permission type</span></span>|<span data-ttu-id="d73f3-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d73f3-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d73f3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d73f3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d73f3-114">CloudPC.Read.All、CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d73f3-114">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="d73f3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d73f3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d73f3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d73f3-116">Not supported.</span></span>|
|<span data-ttu-id="d73f3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d73f3-117">Application</span></span>|<span data-ttu-id="d73f3-118">CloudPC.Read.All、CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d73f3-118">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d73f3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d73f3-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/deviceImages/getSourceImages
```

## <a name="request-headers"></a><span data-ttu-id="d73f3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d73f3-120">Request headers</span></span>

|<span data-ttu-id="d73f3-121">名称</span><span class="sxs-lookup"><span data-stu-id="d73f3-121">Name</span></span>|<span data-ttu-id="d73f3-122">说明</span><span class="sxs-lookup"><span data-stu-id="d73f3-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d73f3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d73f3-123">Authorization</span></span>|<span data-ttu-id="d73f3-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d73f3-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d73f3-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d73f3-126">Request body</span></span>

<span data-ttu-id="d73f3-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d73f3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d73f3-128">响应</span><span class="sxs-lookup"><span data-stu-id="d73f3-128">Response</span></span>

<span data-ttu-id="d73f3-129">如果成功，此函数在响应正文中返回 响应代码和 `200 OK` [cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="d73f3-129">If successful, this function returns a `200 OK` response code and a [cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d73f3-130">示例</span><span class="sxs-lookup"><span data-stu-id="d73f3-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d73f3-131">请求</span><span class="sxs-lookup"><span data-stu-id="d73f3-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d73f3-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="d73f3-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "cloudpcdeviceimage_getsourceimages"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/deviceImages/getSourceImages
```
# <a name="c"></a>[<span data-ttu-id="d73f3-133">C#</span><span class="sxs-lookup"><span data-stu-id="d73f3-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/cloudpcdeviceimage-getsourceimages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d73f3-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d73f3-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/cloudpcdeviceimage-getsourceimages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d73f3-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d73f3-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/cloudpcdeviceimage-getsourceimages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d73f3-136">Java</span><span class="sxs-lookup"><span data-stu-id="d73f3-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/cloudpcdeviceimage-getsourceimages-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d73f3-137">响应</span><span class="sxs-lookup"><span data-stu-id="d73f3-137">Response</span></span>

<span data-ttu-id="d73f3-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d73f3-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.cloudPcSourceDeviceImage)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.cloudPcSourceDeviceImage",
      "id": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG/providers/Microsoft.Compute/images/ExampleImage",
      "displayName": "Display Name value"
    }
  ]
}
```
