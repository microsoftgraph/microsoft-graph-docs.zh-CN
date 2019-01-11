---
title: mobileAppContentFile 资源类型
description: 包含与给定 mobileAppContent 版本关联的单个安装程序文件的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b27f34830c4266b35deafbc67b5c5536f10aec1c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891474"
---
# <a name="mobileappcontentfile-resource-type"></a><span data-ttu-id="cb42a-103">mobileAppContentFile 资源类型</span><span class="sxs-lookup"><span data-stu-id="cb42a-103">mobileAppContentFile resource type</span></span>

> <span data-ttu-id="cb42a-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="cb42a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cb42a-105">包含与给定 mobileAppContent 版本关联的单个安装程序文件的属性。</span><span class="sxs-lookup"><span data-stu-id="cb42a-105">Contains properties for a single installer file that is associated with a given mobileAppContent version.</span></span>
## <a name="methods"></a><span data-ttu-id="cb42a-106">方法</span><span class="sxs-lookup"><span data-stu-id="cb42a-106">Methods</span></span>
|<span data-ttu-id="cb42a-107">方法</span><span class="sxs-lookup"><span data-stu-id="cb42a-107">Method</span></span>|<span data-ttu-id="cb42a-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="cb42a-108">Return Type</span></span>|<span data-ttu-id="cb42a-109">说明</span><span class="sxs-lookup"><span data-stu-id="cb42a-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cb42a-110">List mobileAppContentFiles</span><span class="sxs-lookup"><span data-stu-id="cb42a-110">List mobileAppContentFiles</span></span>](../api/intune-apps-mobileappcontentfile-list.md)|<span data-ttu-id="cb42a-111">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cb42a-111">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="cb42a-112">列出 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cb42a-112">List properties and relationships of the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) objects.</span></span>|
|[<span data-ttu-id="cb42a-113">Get mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="cb42a-113">Get mobileAppContentFile</span></span>](../api/intune-apps-mobileappcontentfile-get.md)|[<span data-ttu-id="cb42a-114">mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="cb42a-114">mobileAppContentFile</span></span>](../resources/intune-apps-mobileappcontentfile.md)|<span data-ttu-id="cb42a-115">读取 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cb42a-115">Read properties and relationships of the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>|
|[<span data-ttu-id="cb42a-116">Create mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="cb42a-116">Create mobileAppContentFile</span></span>](../api/intune-apps-mobileappcontentfile-create.md)|[<span data-ttu-id="cb42a-117">mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="cb42a-117">mobileAppContentFile</span></span>](../resources/intune-apps-mobileappcontentfile.md)|<span data-ttu-id="cb42a-118">创建新的 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cb42a-118">Create a new [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>|
|[<span data-ttu-id="cb42a-119">Delete mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="cb42a-119">Delete mobileAppContentFile</span></span>](../api/intune-apps-mobileappcontentfile-delete.md)|<span data-ttu-id="cb42a-120">无</span><span class="sxs-lookup"><span data-stu-id="cb42a-120">None</span></span>|<span data-ttu-id="cb42a-121">删除 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)。</span><span class="sxs-lookup"><span data-stu-id="cb42a-121">Deletes a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span></span>|
|[<span data-ttu-id="cb42a-122">Update mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="cb42a-122">Update mobileAppContentFile</span></span>](../api/intune-apps-mobileappcontentfile-update.md)|[<span data-ttu-id="cb42a-123">mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="cb42a-123">mobileAppContentFile</span></span>](../resources/intune-apps-mobileappcontentfile.md)|<span data-ttu-id="cb42a-124">更新 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="cb42a-124">Update the properties of a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>|
|[<span data-ttu-id="cb42a-125">commit 操作</span><span class="sxs-lookup"><span data-stu-id="cb42a-125">commit action</span></span>](../api/intune-apps-mobileappcontentfile-commit.md)|<span data-ttu-id="cb42a-126">无</span><span class="sxs-lookup"><span data-stu-id="cb42a-126">None</span></span>|<span data-ttu-id="cb42a-127">提交给定应用的文件。</span><span class="sxs-lookup"><span data-stu-id="cb42a-127">Commits a file of a given app.</span></span>|
|[<span data-ttu-id="cb42a-128">renewUpload 操作</span><span class="sxs-lookup"><span data-stu-id="cb42a-128">renewUpload action</span></span>](../api/intune-apps-mobileappcontentfile-renewupload.md)|<span data-ttu-id="cb42a-129">无</span><span class="sxs-lookup"><span data-stu-id="cb42a-129">None</span></span>|<span data-ttu-id="cb42a-130">续订应用程序文件上传的 SAS URI。</span><span class="sxs-lookup"><span data-stu-id="cb42a-130">Renews the SAS URI for an application file upload.</span></span>|

## <a name="properties"></a><span data-ttu-id="cb42a-131">属性</span><span class="sxs-lookup"><span data-stu-id="cb42a-131">Properties</span></span>
|<span data-ttu-id="cb42a-132">属性</span><span class="sxs-lookup"><span data-stu-id="cb42a-132">Property</span></span>|<span data-ttu-id="cb42a-133">类型</span><span class="sxs-lookup"><span data-stu-id="cb42a-133">Type</span></span>|<span data-ttu-id="cb42a-134">说明</span><span class="sxs-lookup"><span data-stu-id="cb42a-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb42a-135">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="cb42a-135">azureStorageUri</span></span>|<span data-ttu-id="cb42a-136">String</span><span class="sxs-lookup"><span data-stu-id="cb42a-136">String</span></span>|<span data-ttu-id="cb42a-137">Azure 存储 URI。</span><span class="sxs-lookup"><span data-stu-id="cb42a-137">The Azure Storage URI.</span></span>|
|<span data-ttu-id="cb42a-138">isCommitted</span><span class="sxs-lookup"><span data-stu-id="cb42a-138">isCommitted</span></span>|<span data-ttu-id="cb42a-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb42a-139">Boolean</span></span>|<span data-ttu-id="cb42a-140">指示文件是否已提交的值。</span><span class="sxs-lookup"><span data-stu-id="cb42a-140">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="cb42a-141">id</span><span class="sxs-lookup"><span data-stu-id="cb42a-141">id</span></span>|<span data-ttu-id="cb42a-142">String</span><span class="sxs-lookup"><span data-stu-id="cb42a-142">String</span></span>|<span data-ttu-id="cb42a-143">文件 ID。</span><span class="sxs-lookup"><span data-stu-id="cb42a-143">The File Id.</span></span>|
|<span data-ttu-id="cb42a-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cb42a-144">createdDateTime</span></span>|<span data-ttu-id="cb42a-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb42a-145">DateTimeOffset</span></span>|<span data-ttu-id="cb42a-146">创建文件的时间。</span><span class="sxs-lookup"><span data-stu-id="cb42a-146">The time the file was created.</span></span>|
|<span data-ttu-id="cb42a-147">name</span><span class="sxs-lookup"><span data-stu-id="cb42a-147">name</span></span>|<span data-ttu-id="cb42a-148">String</span><span class="sxs-lookup"><span data-stu-id="cb42a-148">String</span></span>|<span data-ttu-id="cb42a-149">文件名称。</span><span class="sxs-lookup"><span data-stu-id="cb42a-149">the file name.</span></span>|
|<span data-ttu-id="cb42a-150">size</span><span class="sxs-lookup"><span data-stu-id="cb42a-150">size</span></span>|<span data-ttu-id="cb42a-151">Int64</span><span class="sxs-lookup"><span data-stu-id="cb42a-151">Int64</span></span>|<span data-ttu-id="cb42a-152">加密前的文件大小。</span><span class="sxs-lookup"><span data-stu-id="cb42a-152">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="cb42a-153">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="cb42a-153">sizeEncrypted</span></span>|<span data-ttu-id="cb42a-154">Int64</span><span class="sxs-lookup"><span data-stu-id="cb42a-154">Int64</span></span>|<span data-ttu-id="cb42a-155">加密后的文件大小。</span><span class="sxs-lookup"><span data-stu-id="cb42a-155">The size of the file after encryption.</span></span>|
|<span data-ttu-id="cb42a-156">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="cb42a-156">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="cb42a-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb42a-157">DateTimeOffset</span></span>|<span data-ttu-id="cb42a-158">Azure 存储 URI 的到期时间。</span><span class="sxs-lookup"><span data-stu-id="cb42a-158">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="cb42a-159">manifest</span><span class="sxs-lookup"><span data-stu-id="cb42a-159">manifest</span></span>|<span data-ttu-id="cb42a-160">Binary</span><span class="sxs-lookup"><span data-stu-id="cb42a-160">Binary</span></span>|<span data-ttu-id="cb42a-161">清单信息。</span><span class="sxs-lookup"><span data-stu-id="cb42a-161">The manifest information.</span></span>|
|<span data-ttu-id="cb42a-162">uploadState</span><span class="sxs-lookup"><span data-stu-id="cb42a-162">uploadState</span></span>|[<span data-ttu-id="cb42a-163">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="cb42a-163">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="cb42a-164">当前上传请求的状态。</span><span class="sxs-lookup"><span data-stu-id="cb42a-164">The state of the current upload request.</span></span> <span data-ttu-id="cb42a-165">可取值为：`success`、`transientError`、`error`、`unknown`、`azureStorageUriRequestSuccess`、`azureStorageUriRequestPending`、`azureStorageUriRequestFailed`、`azureStorageUriRequestTimedOut`、`azureStorageUriRenewalSuccess`、`azureStorageUriRenewalPending`、`azureStorageUriRenewalFailed`、`azureStorageUriRenewalTimedOut`、`commitFileSuccess`、`commitFilePending`、`commitFileFailed`、`commitFileTimedOut`。</span><span class="sxs-lookup"><span data-stu-id="cb42a-165">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cb42a-166">关系</span><span class="sxs-lookup"><span data-stu-id="cb42a-166">Relationships</span></span>
<span data-ttu-id="cb42a-167">无</span><span class="sxs-lookup"><span data-stu-id="cb42a-167">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="cb42a-168">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cb42a-168">JSON Representation</span></span>
<span data-ttu-id="cb42a-169">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cb42a-169">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppContentFile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppContentFile",
  "azureStorageUri": "String",
  "isCommitted": true,
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "name": "String",
  "size": 1024,
  "sizeEncrypted": 1024,
  "azureStorageUriExpirationDateTime": "String (timestamp)",
  "manifest": "binary",
  "uploadState": "String"
}
```



