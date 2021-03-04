---
title: reviewSet：export
description: 从 reviewSet 启动导出。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 7ee3744470cf5fac31abad2d4cc53ba47a0feca5
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446031"
---
# <a name="reviewset-export"></a><span data-ttu-id="f926b-103">reviewSet：export</span><span class="sxs-lookup"><span data-stu-id="f926b-103">reviewSet: export</span></span>

<span data-ttu-id="f926b-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="f926b-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f926b-105">从 **reviewSet** 启动导出。</span><span class="sxs-lookup"><span data-stu-id="f926b-105">Initiate an export from a **reviewSet**.</span></span>  <span data-ttu-id="f926b-106">有关详细信息，请参阅 ["从高级电子数据展示"中的审阅](/microsoft-365/compliance/export-documents-from-review-set)集导出文档。</span><span class="sxs-lookup"><span data-stu-id="f926b-106">For details, see [Export documents from a review set in Advanced eDiscovery](/microsoft-365/compliance/export-documents-from-review-set).</span></span>

## <a name="permissions"></a><span data-ttu-id="f926b-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="f926b-107">Permissions</span></span>

<span data-ttu-id="f926b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f926b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f926b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f926b-110">Permission type</span></span>|<span data-ttu-id="f926b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f926b-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f926b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f926b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f926b-113">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f926b-113">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="f926b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f926b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f926b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f926b-115">Not supported.</span></span>|
|<span data-ttu-id="f926b-116">Application</span><span class="sxs-lookup"><span data-stu-id="f926b-116">Application</span></span>|<span data-ttu-id="f926b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f926b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f926b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f926b-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/reviewsets/{reviewsetId}/export
```

## <a name="request-headers"></a><span data-ttu-id="f926b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f926b-119">Request headers</span></span>

|<span data-ttu-id="f926b-120">名称</span><span class="sxs-lookup"><span data-stu-id="f926b-120">Name</span></span>|<span data-ttu-id="f926b-121">说明</span><span class="sxs-lookup"><span data-stu-id="f926b-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f926b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f926b-122">Authorization</span></span>|<span data-ttu-id="f926b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f926b-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f926b-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f926b-125">Content-Type</span></span>|<span data-ttu-id="f926b-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="f926b-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f926b-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="f926b-128">Request body</span></span>

<span data-ttu-id="f926b-129">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f926b-129">In the request body, supply a JSON representation of the parameters.</span></span>

<span data-ttu-id="f926b-130">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="f926b-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f926b-131">参数</span><span class="sxs-lookup"><span data-stu-id="f926b-131">Parameter</span></span>|<span data-ttu-id="f926b-132">类型</span><span class="sxs-lookup"><span data-stu-id="f926b-132">Type</span></span>|<span data-ttu-id="f926b-133">说明</span><span class="sxs-lookup"><span data-stu-id="f926b-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f926b-134">outputName</span><span class="sxs-lookup"><span data-stu-id="f926b-134">outputName</span></span>|<span data-ttu-id="f926b-135">String</span><span class="sxs-lookup"><span data-stu-id="f926b-135">String</span></span>| <span data-ttu-id="f926b-136">导出的名称。</span><span class="sxs-lookup"><span data-stu-id="f926b-136">Name of the export.</span></span> <span data-ttu-id="f926b-137">必需。</span><span class="sxs-lookup"><span data-stu-id="f926b-137">Required.</span></span> |
|<span data-ttu-id="f926b-138">description</span><span class="sxs-lookup"><span data-stu-id="f926b-138">description</span></span>|<span data-ttu-id="f926b-139">String</span><span class="sxs-lookup"><span data-stu-id="f926b-139">String</span></span>| <span data-ttu-id="f926b-140">导出说明</span><span class="sxs-lookup"><span data-stu-id="f926b-140">Description of the export</span></span> |
|<span data-ttu-id="f926b-141">azureBlobContainer</span><span class="sxs-lookup"><span data-stu-id="f926b-141">azureBlobContainer</span></span>|<span data-ttu-id="f926b-142">String</span><span class="sxs-lookup"><span data-stu-id="f926b-142">String</span></span>| <span data-ttu-id="f926b-143">导出到你自己的 Azure 存储帐户时，这是容器 URL。</span><span class="sxs-lookup"><span data-stu-id="f926b-143">When exporting to your own Azure storage account, this is the container URL.</span></span> |
|<span data-ttu-id="f926b-144">azureBlobToken</span><span class="sxs-lookup"><span data-stu-id="f926b-144">azureBlobToken</span></span>|<span data-ttu-id="f926b-145">String</span><span class="sxs-lookup"><span data-stu-id="f926b-145">String</span></span>| <span data-ttu-id="f926b-146">导出到你自己的 Azure 存储帐户时，容器 URL 的 SAS 令牌。</span><span class="sxs-lookup"><span data-stu-id="f926b-146">When exporting to your own Azure storage account, SAS token for the container URL.</span></span> |
|<span data-ttu-id="f926b-147">exportOptions</span><span class="sxs-lookup"><span data-stu-id="f926b-147">exportOptions</span></span>| [<span data-ttu-id="f926b-148">microsoft.graph.ediscovery.exportOptions</span><span class="sxs-lookup"><span data-stu-id="f926b-148">microsoft.graph.ediscovery.exportOptions</span></span>](../resources/ediscovery-caseexportoperation.md#exportoptions-values) |<span data-ttu-id="f926b-149">指定控制导出格式的选项。</span><span class="sxs-lookup"><span data-stu-id="f926b-149">Specifies options that control the format of the export.</span></span> <span data-ttu-id="f926b-150">可取值为：`originalFiles`、`text`、`pdfReplacement`、`fileInfo`、`tags`。</span><span class="sxs-lookup"><span data-stu-id="f926b-150">Possible values are: `originalFiles`, `text`, `pdfReplacement`, `fileInfo`, `tags`.</span></span>|
|<span data-ttu-id="f926b-151">exportStructure</span><span class="sxs-lookup"><span data-stu-id="f926b-151">exportStructure</span></span>|[<span data-ttu-id="f926b-152">microsoft.graph.ediscovery.exportFileStructure</span><span class="sxs-lookup"><span data-stu-id="f926b-152">microsoft.graph.ediscovery.exportFileStructure</span></span>](../resources/ediscovery-caseexportoperation.md#exportfilestructure-values)| <span data-ttu-id="f926b-153">控制导出的文件结构和打包的选项。</span><span class="sxs-lookup"><span data-stu-id="f926b-153">Options that control file structure and packaging of the export.</span></span> <span data-ttu-id="f926b-154">可取值为：`none`、`directory`、`pst`。</span><span class="sxs-lookup"><span data-stu-id="f926b-154">Possible values are: `none`, `directory`, `pst`.</span></span>|

## <a name="response"></a><span data-ttu-id="f926b-155">响应</span><span class="sxs-lookup"><span data-stu-id="f926b-155">Response</span></span>

<span data-ttu-id="f926b-156">如果导出成功启动，此操作将返回 `202 Accepted` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="f926b-156">If the export is started successfully, this action returns a `202 Accepted` response code.</span></span> <span data-ttu-id="f926b-157">响应还将包含一个标头，其中包含为处理导出而创建的 `Location` [caseExportOperation](../resources/ediscovery-caseexportoperation.md) 的位置。</span><span class="sxs-lookup"><span data-stu-id="f926b-157">The response will also contain a `Location` header, which contains the location of the [caseExportOperation](../resources/ediscovery-caseexportoperation.md) that was created to handle the export.</span></span> <span data-ttu-id="f926b-158">通过向位置提出 GET 请求来检查导出操作的状态，成功完成后， [状态将更改为](../resources/ediscovery-caseoperation.md#caseoperationstatus-values) `succeeded` 。</span><span class="sxs-lookup"><span data-stu-id="f926b-158">Check the status of the export operation by making a GET request to the location, when successfully completed, the [status](../resources/ediscovery-caseoperation.md#caseoperationstatus-values) will change to `succeeded`.</span></span>

## <a name="examples"></a><span data-ttu-id="f926b-159">示例</span><span class="sxs-lookup"><span data-stu-id="f926b-159">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f926b-160">请求</span><span class="sxs-lookup"><span data-stu-id="f926b-160">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="f926b-161">响应</span><span class="sxs-lookup"><span data-stu-id="f926b-161">Response</span></span>

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
