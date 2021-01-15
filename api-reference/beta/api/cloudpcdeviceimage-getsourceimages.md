---
title: cloudPcDeviceImage：getSourceImages
description: 查看 Azure 订阅中所有托管映像资源的列表。 这些源图像可以上载并用于云电脑。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 1ddd7fdef827328f6f72b52af5a992e9f0d69653
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872777"
---
# <a name="cloudpcdeviceimage-getsourceimages"></a><span data-ttu-id="cd44d-104">cloudPcDeviceImage：getSourceImages</span><span class="sxs-lookup"><span data-stu-id="cd44d-104">cloudPcDeviceImage: getSourceImages</span></span>

<span data-ttu-id="cd44d-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd44d-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cd44d-106">获取 [cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cd44d-106">Get [cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) objects.</span></span> <span data-ttu-id="cd44d-107">查看 Azure Active Directory 订阅中所有托管映像资源的列表。</span><span class="sxs-lookup"><span data-stu-id="cd44d-107">View a list of all the managed image resources from your Azure Active Directory subscriptions.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="permissions"></a><span data-ttu-id="cd44d-108">权限</span><span class="sxs-lookup"><span data-stu-id="cd44d-108">Permissions</span></span>

<span data-ttu-id="cd44d-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cd44d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd44d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="cd44d-111">Permission type</span></span>|<span data-ttu-id="cd44d-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cd44d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cd44d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cd44d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cd44d-114">CloudPC.Read.All、CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd44d-114">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="cd44d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cd44d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd44d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cd44d-116">Not supported.</span></span>|
|<span data-ttu-id="cd44d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="cd44d-117">Application</span></span>|<span data-ttu-id="cd44d-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="cd44d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd44d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cd44d-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/deviceImages/getSourceImages
```

## <a name="request-headers"></a><span data-ttu-id="cd44d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="cd44d-120">Request headers</span></span>

|<span data-ttu-id="cd44d-121">名称</span><span class="sxs-lookup"><span data-stu-id="cd44d-121">Name</span></span>|<span data-ttu-id="cd44d-122">说明</span><span class="sxs-lookup"><span data-stu-id="cd44d-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="cd44d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd44d-123">Authorization</span></span>|<span data-ttu-id="cd44d-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cd44d-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd44d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="cd44d-126">Request body</span></span>

<span data-ttu-id="cd44d-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cd44d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cd44d-128">响应</span><span class="sxs-lookup"><span data-stu-id="cd44d-128">Response</span></span>

<span data-ttu-id="cd44d-129">如果成功，此函数在响应正文中返回响应代码和 `200 OK` [cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="cd44d-129">If successful, this function returns a `200 OK` response code and a [cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cd44d-130">示例</span><span class="sxs-lookup"><span data-stu-id="cd44d-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cd44d-131">请求</span><span class="sxs-lookup"><span data-stu-id="cd44d-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="cd44d-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="cd44d-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "cloudpcdeviceimage_getsourceimages"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/deviceImages/getSourceImages
```
# <a name="c"></a>[<span data-ttu-id="cd44d-133">C#</span><span class="sxs-lookup"><span data-stu-id="cd44d-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/cloudpcdeviceimage-getsourceimages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cd44d-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cd44d-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/cloudpcdeviceimage-getsourceimages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cd44d-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cd44d-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/cloudpcdeviceimage-getsourceimages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cd44d-136">Java</span><span class="sxs-lookup"><span data-stu-id="cd44d-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/cloudpcdeviceimage-getsourceimages-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cd44d-137">响应</span><span class="sxs-lookup"><span data-stu-id="cd44d-137">Response</span></span>

<span data-ttu-id="cd44d-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="cd44d-138">**Note:** The response object shown here might be shortened for readability.</span></span>
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
