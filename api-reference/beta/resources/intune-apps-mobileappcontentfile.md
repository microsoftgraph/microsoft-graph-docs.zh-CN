---
title: mobileAppContentFile 资源类型
description: 包含与给定 mobileAppContent 版本关联的单个安装程序文件的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ebb51c5c5c19cfeefd849861f800c817d481d0c8
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797837"
---
# <a name="mobileappcontentfile-resource-type"></a><span data-ttu-id="d491e-103">mobileAppContentFile 资源类型</span><span class="sxs-lookup"><span data-stu-id="d491e-103">mobileAppContentFile resource type</span></span>

> <span data-ttu-id="d491e-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d491e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d491e-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d491e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d491e-106">包含与给定 mobileAppContent 版本关联的单个安装程序文件的属性。</span><span class="sxs-lookup"><span data-stu-id="d491e-106">Contains properties for a single installer file that is associated with a given mobileAppContent version.</span></span>

## <a name="methods"></a><span data-ttu-id="d491e-107">方法</span><span class="sxs-lookup"><span data-stu-id="d491e-107">Methods</span></span>
|<span data-ttu-id="d491e-108">方法</span><span class="sxs-lookup"><span data-stu-id="d491e-108">Method</span></span>|<span data-ttu-id="d491e-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="d491e-109">Return Type</span></span>|<span data-ttu-id="d491e-110">说明</span><span class="sxs-lookup"><span data-stu-id="d491e-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d491e-111">List mobileAppContentFiles</span><span class="sxs-lookup"><span data-stu-id="d491e-111">List mobileAppContentFiles</span></span>](../api/intune-apps-mobileappcontentfile-list.md)|<span data-ttu-id="d491e-112">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d491e-112">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="d491e-113">列出 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d491e-113">List properties and relationships of the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) objects.</span></span>|
|[<span data-ttu-id="d491e-114">Get mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="d491e-114">Get mobileAppContentFile</span></span>](../api/intune-apps-mobileappcontentfile-get.md)|[<span data-ttu-id="d491e-115">mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="d491e-115">mobileAppContentFile</span></span>](../resources/intune-apps-mobileappcontentfile.md)|<span data-ttu-id="d491e-116">读取 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d491e-116">Read properties and relationships of the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>|
|[<span data-ttu-id="d491e-117">Create mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="d491e-117">Create mobileAppContentFile</span></span>](../api/intune-apps-mobileappcontentfile-create.md)|[<span data-ttu-id="d491e-118">mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="d491e-118">mobileAppContentFile</span></span>](../resources/intune-apps-mobileappcontentfile.md)|<span data-ttu-id="d491e-119">创建新的 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d491e-119">Create a new [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>|
|[<span data-ttu-id="d491e-120">Delete mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="d491e-120">Delete mobileAppContentFile</span></span>](../api/intune-apps-mobileappcontentfile-delete.md)|<span data-ttu-id="d491e-121">None</span><span class="sxs-lookup"><span data-stu-id="d491e-121">None</span></span>|<span data-ttu-id="d491e-122">删除 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)。</span><span class="sxs-lookup"><span data-stu-id="d491e-122">Deletes a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span></span>|
|[<span data-ttu-id="d491e-123">Update mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="d491e-123">Update mobileAppContentFile</span></span>](../api/intune-apps-mobileappcontentfile-update.md)|[<span data-ttu-id="d491e-124">mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="d491e-124">mobileAppContentFile</span></span>](../resources/intune-apps-mobileappcontentfile.md)|<span data-ttu-id="d491e-125">更新 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d491e-125">Update the properties of a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>|
|[<span data-ttu-id="d491e-126">commit 操作</span><span class="sxs-lookup"><span data-stu-id="d491e-126">commit action</span></span>](../api/intune-apps-mobileappcontentfile-commit.md)|<span data-ttu-id="d491e-127">None</span><span class="sxs-lookup"><span data-stu-id="d491e-127">None</span></span>|<span data-ttu-id="d491e-128">提交给定应用的文件。</span><span class="sxs-lookup"><span data-stu-id="d491e-128">Commits a file of a given app.</span></span>|
|[<span data-ttu-id="d491e-129">renewUpload 操作</span><span class="sxs-lookup"><span data-stu-id="d491e-129">renewUpload action</span></span>](../api/intune-apps-mobileappcontentfile-renewupload.md)|<span data-ttu-id="d491e-130">无</span><span class="sxs-lookup"><span data-stu-id="d491e-130">None</span></span>|<span data-ttu-id="d491e-131">续订应用程序文件上传的 SAS URI。</span><span class="sxs-lookup"><span data-stu-id="d491e-131">Renews the SAS URI for an application file upload.</span></span>|

## <a name="properties"></a><span data-ttu-id="d491e-132">属性</span><span class="sxs-lookup"><span data-stu-id="d491e-132">Properties</span></span>
|<span data-ttu-id="d491e-133">属性</span><span class="sxs-lookup"><span data-stu-id="d491e-133">Property</span></span>|<span data-ttu-id="d491e-134">类型</span><span class="sxs-lookup"><span data-stu-id="d491e-134">Type</span></span>|<span data-ttu-id="d491e-135">说明</span><span class="sxs-lookup"><span data-stu-id="d491e-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d491e-136">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="d491e-136">azureStorageUri</span></span>|<span data-ttu-id="d491e-137">String</span><span class="sxs-lookup"><span data-stu-id="d491e-137">String</span></span>|<span data-ttu-id="d491e-138">Azure 存储 URI。</span><span class="sxs-lookup"><span data-stu-id="d491e-138">The Azure Storage URI.</span></span>|
|<span data-ttu-id="d491e-139">isCommitted</span><span class="sxs-lookup"><span data-stu-id="d491e-139">isCommitted</span></span>|<span data-ttu-id="d491e-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="d491e-140">Boolean</span></span>|<span data-ttu-id="d491e-141">指示文件是否已提交的值。</span><span class="sxs-lookup"><span data-stu-id="d491e-141">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="d491e-142">id</span><span class="sxs-lookup"><span data-stu-id="d491e-142">id</span></span>|<span data-ttu-id="d491e-143">String</span><span class="sxs-lookup"><span data-stu-id="d491e-143">String</span></span>|<span data-ttu-id="d491e-144">文件 ID。</span><span class="sxs-lookup"><span data-stu-id="d491e-144">The File Id.</span></span>|
|<span data-ttu-id="d491e-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d491e-145">createdDateTime</span></span>|<span data-ttu-id="d491e-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d491e-146">DateTimeOffset</span></span>|<span data-ttu-id="d491e-147">创建文件的时间。</span><span class="sxs-lookup"><span data-stu-id="d491e-147">The time the file was created.</span></span>|
|<span data-ttu-id="d491e-148">name</span><span class="sxs-lookup"><span data-stu-id="d491e-148">name</span></span>|<span data-ttu-id="d491e-149">String</span><span class="sxs-lookup"><span data-stu-id="d491e-149">String</span></span>|<span data-ttu-id="d491e-150">文件名称。</span><span class="sxs-lookup"><span data-stu-id="d491e-150">the file name.</span></span>|
|<span data-ttu-id="d491e-151">size</span><span class="sxs-lookup"><span data-stu-id="d491e-151">size</span></span>|<span data-ttu-id="d491e-152">Int64</span><span class="sxs-lookup"><span data-stu-id="d491e-152">Int64</span></span>|<span data-ttu-id="d491e-153">加密前的文件大小。</span><span class="sxs-lookup"><span data-stu-id="d491e-153">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="d491e-154">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="d491e-154">sizeEncrypted</span></span>|<span data-ttu-id="d491e-155">Int64</span><span class="sxs-lookup"><span data-stu-id="d491e-155">Int64</span></span>|<span data-ttu-id="d491e-156">加密后的文件大小。</span><span class="sxs-lookup"><span data-stu-id="d491e-156">The size of the file after encryption.</span></span>|
|<span data-ttu-id="d491e-157">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d491e-157">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="d491e-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d491e-158">DateTimeOffset</span></span>|<span data-ttu-id="d491e-159">Azure 存储 URI 的到期时间。</span><span class="sxs-lookup"><span data-stu-id="d491e-159">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="d491e-160">manifest</span><span class="sxs-lookup"><span data-stu-id="d491e-160">manifest</span></span>|<span data-ttu-id="d491e-161">Binary</span><span class="sxs-lookup"><span data-stu-id="d491e-161">Binary</span></span>|<span data-ttu-id="d491e-162">清单信息。</span><span class="sxs-lookup"><span data-stu-id="d491e-162">The manifest information.</span></span>|
|<span data-ttu-id="d491e-163">uploadState</span><span class="sxs-lookup"><span data-stu-id="d491e-163">uploadState</span></span>|[<span data-ttu-id="d491e-164">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="d491e-164">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="d491e-165">当前上传请求的状态。</span><span class="sxs-lookup"><span data-stu-id="d491e-165">The state of the current upload request.</span></span> <span data-ttu-id="d491e-166">可取值为：`success`、`transientError`、`error`、`unknown`、`azureStorageUriRequestSuccess`、`azureStorageUriRequestPending`、`azureStorageUriRequestFailed`、`azureStorageUriRequestTimedOut`、`azureStorageUriRenewalSuccess`、`azureStorageUriRenewalPending`、`azureStorageUriRenewalFailed`、`azureStorageUriRenewalTimedOut`、`commitFileSuccess`、`commitFilePending`、`commitFileFailed`、`commitFileTimedOut`。</span><span class="sxs-lookup"><span data-stu-id="d491e-166">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|
|<span data-ttu-id="d491e-167">isFrameworkFile</span><span class="sxs-lookup"><span data-stu-id="d491e-167">isFrameworkFile</span></span>|<span data-ttu-id="d491e-168">布尔值</span><span class="sxs-lookup"><span data-stu-id="d491e-168">Boolean</span></span>|<span data-ttu-id="d491e-169">一个指示文件是否为框架文件的值。</span><span class="sxs-lookup"><span data-stu-id="d491e-169">A value indicating whether the file is a framework file.</span></span>|
|<span data-ttu-id="d491e-170">isDependency</span><span class="sxs-lookup"><span data-stu-id="d491e-170">isDependency</span></span>|<span data-ttu-id="d491e-171">布尔值</span><span class="sxs-lookup"><span data-stu-id="d491e-171">Boolean</span></span>|<span data-ttu-id="d491e-172">内容文件是否依赖于主要内容文件。</span><span class="sxs-lookup"><span data-stu-id="d491e-172">Whether the content file is a dependency for the main content file.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d491e-173">关系</span><span class="sxs-lookup"><span data-stu-id="d491e-173">Relationships</span></span>
<span data-ttu-id="d491e-174">无</span><span class="sxs-lookup"><span data-stu-id="d491e-174">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d491e-175">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d491e-175">JSON Representation</span></span>
<span data-ttu-id="d491e-176">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d491e-176">Here is a JSON representation of the resource.</span></span>
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
  "uploadState": "String",
  "isFrameworkFile": true,
  "isDependency": true
}
```



