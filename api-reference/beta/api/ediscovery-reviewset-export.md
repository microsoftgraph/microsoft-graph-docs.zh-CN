---
title: reviewSet： export
description: 从 reviewSet 启动导出。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 2620f72eced3bc9f5c6fb02e5e034a6116af5f2c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772855"
---
# <a name="reviewset-export"></a><span data-ttu-id="4f616-103">reviewSet： export</span><span class="sxs-lookup"><span data-stu-id="4f616-103">reviewSet: export</span></span>

<span data-ttu-id="4f616-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="4f616-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f616-105">从 **reviewSet 中启动导出**。</span><span class="sxs-lookup"><span data-stu-id="4f616-105">Initiate an export from a **reviewSet**.</span></span>  <span data-ttu-id="4f616-106">有关详细信息，请参阅在高级电子数据展示 [中从审阅集导出文档](/microsoft-365/compliance/export-documents-from-review-set)。</span><span class="sxs-lookup"><span data-stu-id="4f616-106">For details, see [Export documents from a review set in Advanced eDiscovery](/microsoft-365/compliance/export-documents-from-review-set).</span></span>

## <a name="permissions"></a><span data-ttu-id="4f616-107">权限</span><span class="sxs-lookup"><span data-stu-id="4f616-107">Permissions</span></span>

<span data-ttu-id="4f616-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4f616-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f616-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4f616-110">Permission type</span></span>|<span data-ttu-id="4f616-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4f616-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f616-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4f616-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4f616-113">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f616-113">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="4f616-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4f616-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f616-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4f616-115">Not supported.</span></span>|
|<span data-ttu-id="4f616-116">Application</span><span class="sxs-lookup"><span data-stu-id="4f616-116">Application</span></span>|<span data-ttu-id="4f616-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="4f616-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f616-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4f616-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/reviewsets/{reviewsetId}/export
```

## <a name="request-headers"></a><span data-ttu-id="4f616-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4f616-119">Request headers</span></span>

|<span data-ttu-id="4f616-120">名称</span><span class="sxs-lookup"><span data-stu-id="4f616-120">Name</span></span>|<span data-ttu-id="4f616-121">说明</span><span class="sxs-lookup"><span data-stu-id="4f616-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4f616-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f616-122">Authorization</span></span>|<span data-ttu-id="4f616-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4f616-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4f616-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4f616-125">Content-Type</span></span>|<span data-ttu-id="4f616-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="4f616-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f616-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="4f616-128">Request body</span></span>

<span data-ttu-id="4f616-129">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4f616-129">In the request body, supply a JSON representation of the parameters.</span></span>

<span data-ttu-id="4f616-130">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="4f616-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="4f616-131">参数</span><span class="sxs-lookup"><span data-stu-id="4f616-131">Parameter</span></span>|<span data-ttu-id="4f616-132">类型</span><span class="sxs-lookup"><span data-stu-id="4f616-132">Type</span></span>|<span data-ttu-id="4f616-133">说明</span><span class="sxs-lookup"><span data-stu-id="4f616-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f616-134">outputName</span><span class="sxs-lookup"><span data-stu-id="4f616-134">outputName</span></span>|<span data-ttu-id="4f616-135">字符串</span><span class="sxs-lookup"><span data-stu-id="4f616-135">String</span></span>| <span data-ttu-id="4f616-136">导出的名称。</span><span class="sxs-lookup"><span data-stu-id="4f616-136">Name of the export.</span></span> <span data-ttu-id="4f616-137">必需。</span><span class="sxs-lookup"><span data-stu-id="4f616-137">Required.</span></span> |
|<span data-ttu-id="4f616-138">description</span><span class="sxs-lookup"><span data-stu-id="4f616-138">description</span></span>|<span data-ttu-id="4f616-139">字符串</span><span class="sxs-lookup"><span data-stu-id="4f616-139">String</span></span>| <span data-ttu-id="4f616-140">导出说明</span><span class="sxs-lookup"><span data-stu-id="4f616-140">Description of the export</span></span> |
|<span data-ttu-id="4f616-141">azureBlobContainer</span><span class="sxs-lookup"><span data-stu-id="4f616-141">azureBlobContainer</span></span>|<span data-ttu-id="4f616-142">字符串</span><span class="sxs-lookup"><span data-stu-id="4f616-142">String</span></span>| <span data-ttu-id="4f616-143">导出到你自己的 Azure 存储帐户时，这是容器 URL。</span><span class="sxs-lookup"><span data-stu-id="4f616-143">When exporting to your own Azure storage account, this is the container URL.</span></span> |
|<span data-ttu-id="4f616-144">azureBlobToken</span><span class="sxs-lookup"><span data-stu-id="4f616-144">azureBlobToken</span></span>|<span data-ttu-id="4f616-145">字符串</span><span class="sxs-lookup"><span data-stu-id="4f616-145">String</span></span>| <span data-ttu-id="4f616-146">导出到你自己的 Azure 存储帐户时，容器 URL 的 SAS 令牌。</span><span class="sxs-lookup"><span data-stu-id="4f616-146">When exporting to your own Azure storage account, SAS token for the container URL.</span></span> |
|<span data-ttu-id="4f616-147">exportOptions</span><span class="sxs-lookup"><span data-stu-id="4f616-147">exportOptions</span></span>| [<span data-ttu-id="4f616-148">microsoft.graph.ediscovery.exportOptions</span><span class="sxs-lookup"><span data-stu-id="4f616-148">microsoft.graph.ediscovery.exportOptions</span></span>](../resources/ediscovery-caseexportoperation.md#exportoptions-values) |<span data-ttu-id="4f616-149">指定控制导出格式的选项。</span><span class="sxs-lookup"><span data-stu-id="4f616-149">Specifies options that control the format of the export.</span></span> <span data-ttu-id="4f616-150">可取值为：`originalFiles`、`text`、`pdfReplacement`、`fileInfo`、`tags`。</span><span class="sxs-lookup"><span data-stu-id="4f616-150">Possible values are: `originalFiles`, `text`, `pdfReplacement`, `fileInfo`, `tags`.</span></span>|
|<span data-ttu-id="4f616-151">exportStructure</span><span class="sxs-lookup"><span data-stu-id="4f616-151">exportStructure</span></span>|[<span data-ttu-id="4f616-152">microsoft.graph.ediscovery.exportFileStructure</span><span class="sxs-lookup"><span data-stu-id="4f616-152">microsoft.graph.ediscovery.exportFileStructure</span></span>](../resources/ediscovery-caseexportoperation.md#exportfilestructure-values)| <span data-ttu-id="4f616-153">控制导出的文件结构和打包的选项。</span><span class="sxs-lookup"><span data-stu-id="4f616-153">Options that control file structure and packaging of the export.</span></span> <span data-ttu-id="4f616-154">可取值为：`none`、`directory`、`pst`。</span><span class="sxs-lookup"><span data-stu-id="4f616-154">Possible values are: `none`, `directory`, `pst`.</span></span>|

## <a name="response"></a><span data-ttu-id="4f616-155">响应</span><span class="sxs-lookup"><span data-stu-id="4f616-155">Response</span></span>

<span data-ttu-id="4f616-156">如果导出成功启动，此操作将返回 `202 Accepted` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="4f616-156">If the export is started successfully, this action returns a `202 Accepted` response code.</span></span> <span data-ttu-id="4f616-157">响应还将包含标头，其中包含为处理导出而创建的 `Location` [caseExportOperation](../resources/ediscovery-caseexportoperation.md) 的位置。</span><span class="sxs-lookup"><span data-stu-id="4f616-157">The response will also contain a `Location` header, which contains the location of the [caseExportOperation](../resources/ediscovery-caseexportoperation.md) that was created to handle the export.</span></span> <span data-ttu-id="4f616-158">通过向位置发送 GET 请求来检查导出操作的状态，成功完成后， [状态](../resources/ediscovery-caseoperation.md#caseoperationstatus-values) 将更改为 `succeeded` 。</span><span class="sxs-lookup"><span data-stu-id="4f616-158">Check the status of the export operation by making a GET request to the location, when successfully completed, the [status](../resources/ediscovery-caseoperation.md#caseoperationstatus-values) will change to `succeeded`.</span></span>

## <a name="examples"></a><span data-ttu-id="4f616-159">示例</span><span class="sxs-lookup"><span data-stu-id="4f616-159">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4f616-160">请求</span><span class="sxs-lookup"><span data-stu-id="4f616-160">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="4f616-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="4f616-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reviewset_export"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/99e865fc-e29f-479a-ba83-9e58eb017103/reviewsets/e44ac2cb-f8b4-4fd8-aa1c-1391b46ba9cc/export
Content-Type: application/json
Content-length: 186

{
  "outputName": "2020-12-06 Contoso investigation export",
  "description": "Export for the Contoso investigation",
  "exportOptions": "originalFiles,fileInfo,tags",
  "exportStructure": "directory"
}
```
# <a name="c"></a>[<span data-ttu-id="4f616-162">C#</span><span class="sxs-lookup"><span data-stu-id="4f616-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reviewset-export-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4f616-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4f616-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reviewset-export-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4f616-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4f616-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reviewset-export-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4f616-165">Java</span><span class="sxs-lookup"><span data-stu-id="4f616-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reviewset-export-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4f616-166">响应</span><span class="sxs-lookup"><span data-stu-id="4f616-166">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 202 Accepted
cache-control: no-cache,
client-request-id: 3ec98906-7187-927e-5203-2ed4533175c6,
location: https://graph.microsoft.com/beta/compliance/ediscovery/cases('5b840b94-f821-4c4a-8cad-3a90062bf51a')/operations('2ad2da7c7dbb404abfbbb28b7b6babd6'),
request-id: 9e6b9230-113c-49de-8f7d-ecb90d35b0de
```
