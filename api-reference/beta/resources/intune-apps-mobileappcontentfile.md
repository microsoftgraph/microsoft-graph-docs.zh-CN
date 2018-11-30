---
title: mobileAppContentFile 资源类型
description: 包含与给定 mobileAppContent 版本关联的单个安装程序文件的属性。
ms.openlocfilehash: 72467995e4d586df54a6c3cb2295e37cd9b9c6ce
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046455"
---
# <a name="mobileappcontentfile-resource-type"></a><span data-ttu-id="e5620-103">mobileAppContentFile 资源类型</span><span class="sxs-lookup"><span data-stu-id="e5620-103">mobileAppContentFile resource type</span></span>

> <span data-ttu-id="e5620-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e5620-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e5620-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e5620-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e5620-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e5620-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e5620-107">包含与给定 mobileAppContent 版本关联的单个安装程序文件的属性。</span><span class="sxs-lookup"><span data-stu-id="e5620-107">Contains properties for a single installer file that is associated with a given mobileAppContent version.</span></span>
## <a name="methods"></a><span data-ttu-id="e5620-108">方法</span><span class="sxs-lookup"><span data-stu-id="e5620-108">Methods</span></span>
|<span data-ttu-id="e5620-109">方法</span><span class="sxs-lookup"><span data-stu-id="e5620-109">Method</span></span>|<span data-ttu-id="e5620-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="e5620-110">Return Type</span></span>|<span data-ttu-id="e5620-111">说明</span><span class="sxs-lookup"><span data-stu-id="e5620-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e5620-112">List mobileAppContentFiles</span><span class="sxs-lookup"><span data-stu-id="e5620-112">List mobileAppContentFiles</span></span>](../api/intune-apps-mobileappcontentfile-list.md)|<span data-ttu-id="e5620-113">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e5620-113">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="e5620-114">列出 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e5620-114">List properties and relationships of the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) objects.</span></span>|
|[<span data-ttu-id="e5620-115">Get mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="e5620-115">Get mobileAppContentFile</span></span>](../api/intune-apps-mobileappcontentfile-get.md)|[<span data-ttu-id="e5620-116">mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="e5620-116">mobileAppContentFile</span></span>](../resources/intune-apps-mobileappcontentfile.md)|<span data-ttu-id="e5620-117">读取 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e5620-117">Read properties and relationships of the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>|
|[<span data-ttu-id="e5620-118">Create mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="e5620-118">Create mobileAppContentFile</span></span>](../api/intune-apps-mobileappcontentfile-create.md)|[<span data-ttu-id="e5620-119">mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="e5620-119">mobileAppContentFile</span></span>](../resources/intune-apps-mobileappcontentfile.md)|<span data-ttu-id="e5620-120">创建新的 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e5620-120">Create a new [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>|
|[<span data-ttu-id="e5620-121">Delete mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="e5620-121">Delete mobileAppContentFile</span></span>](../api/intune-apps-mobileappcontentfile-delete.md)|<span data-ttu-id="e5620-122">无</span><span class="sxs-lookup"><span data-stu-id="e5620-122">None</span></span>|<span data-ttu-id="e5620-123">删除 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)。</span><span class="sxs-lookup"><span data-stu-id="e5620-123">Deletes a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span></span>|
|[<span data-ttu-id="e5620-124">Update mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="e5620-124">Update mobileAppContentFile</span></span>](../api/intune-apps-mobileappcontentfile-update.md)|[<span data-ttu-id="e5620-125">mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="e5620-125">mobileAppContentFile</span></span>](../resources/intune-apps-mobileappcontentfile.md)|<span data-ttu-id="e5620-126">更新 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e5620-126">Update the properties of a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>|
|[<span data-ttu-id="e5620-127">commit 操作</span><span class="sxs-lookup"><span data-stu-id="e5620-127">commit action</span></span>](../api/intune-apps-mobileappcontentfile-commit.md)|<span data-ttu-id="e5620-128">无</span><span class="sxs-lookup"><span data-stu-id="e5620-128">None</span></span>|<span data-ttu-id="e5620-129">提交给定应用的文件。</span><span class="sxs-lookup"><span data-stu-id="e5620-129">Commits a file of a given app.</span></span>|
|[<span data-ttu-id="e5620-130">renewUpload 操作</span><span class="sxs-lookup"><span data-stu-id="e5620-130">renewUpload action</span></span>](../api/intune-apps-mobileappcontentfile-renewupload.md)|<span data-ttu-id="e5620-131">无</span><span class="sxs-lookup"><span data-stu-id="e5620-131">None</span></span>|<span data-ttu-id="e5620-132">续订应用程序文件上传的 SAS URI。</span><span class="sxs-lookup"><span data-stu-id="e5620-132">Renews the SAS URI for an application file upload.</span></span>|

## <a name="properties"></a><span data-ttu-id="e5620-133">属性</span><span class="sxs-lookup"><span data-stu-id="e5620-133">Properties</span></span>
|<span data-ttu-id="e5620-134">属性</span><span class="sxs-lookup"><span data-stu-id="e5620-134">Property</span></span>|<span data-ttu-id="e5620-135">类型</span><span class="sxs-lookup"><span data-stu-id="e5620-135">Type</span></span>|<span data-ttu-id="e5620-136">说明</span><span class="sxs-lookup"><span data-stu-id="e5620-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5620-137">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="e5620-137">azureStorageUri</span></span>|<span data-ttu-id="e5620-138">String</span><span class="sxs-lookup"><span data-stu-id="e5620-138">String</span></span>|<span data-ttu-id="e5620-139">Azure 存储 URI。</span><span class="sxs-lookup"><span data-stu-id="e5620-139">The Azure Storage URI.</span></span>|
|<span data-ttu-id="e5620-140">isCommitted</span><span class="sxs-lookup"><span data-stu-id="e5620-140">isCommitted</span></span>|<span data-ttu-id="e5620-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5620-141">Boolean</span></span>|<span data-ttu-id="e5620-142">指示文件是否已提交的值。</span><span class="sxs-lookup"><span data-stu-id="e5620-142">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="e5620-143">id</span><span class="sxs-lookup"><span data-stu-id="e5620-143">id</span></span>|<span data-ttu-id="e5620-144">String</span><span class="sxs-lookup"><span data-stu-id="e5620-144">String</span></span>|<span data-ttu-id="e5620-145">文件 ID。</span><span class="sxs-lookup"><span data-stu-id="e5620-145">The File Id.</span></span>|
|<span data-ttu-id="e5620-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e5620-146">createdDateTime</span></span>|<span data-ttu-id="e5620-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5620-147">DateTimeOffset</span></span>|<span data-ttu-id="e5620-148">创建文件的时间。</span><span class="sxs-lookup"><span data-stu-id="e5620-148">The time the file was created.</span></span>|
|<span data-ttu-id="e5620-149">name</span><span class="sxs-lookup"><span data-stu-id="e5620-149">name</span></span>|<span data-ttu-id="e5620-150">String</span><span class="sxs-lookup"><span data-stu-id="e5620-150">String</span></span>|<span data-ttu-id="e5620-151">文件名称。</span><span class="sxs-lookup"><span data-stu-id="e5620-151">the file name.</span></span>|
|<span data-ttu-id="e5620-152">size</span><span class="sxs-lookup"><span data-stu-id="e5620-152">size</span></span>|<span data-ttu-id="e5620-153">Int64</span><span class="sxs-lookup"><span data-stu-id="e5620-153">Int64</span></span>|<span data-ttu-id="e5620-154">加密前的文件大小。</span><span class="sxs-lookup"><span data-stu-id="e5620-154">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="e5620-155">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="e5620-155">sizeEncrypted</span></span>|<span data-ttu-id="e5620-156">Int64</span><span class="sxs-lookup"><span data-stu-id="e5620-156">Int64</span></span>|<span data-ttu-id="e5620-157">加密后的文件大小。</span><span class="sxs-lookup"><span data-stu-id="e5620-157">The size of the file after encryption.</span></span>|
|<span data-ttu-id="e5620-158">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="e5620-158">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="e5620-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5620-159">DateTimeOffset</span></span>|<span data-ttu-id="e5620-160">Azure 存储 URI 的到期时间。</span><span class="sxs-lookup"><span data-stu-id="e5620-160">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="e5620-161">manifest</span><span class="sxs-lookup"><span data-stu-id="e5620-161">manifest</span></span>|<span data-ttu-id="e5620-162">Binary</span><span class="sxs-lookup"><span data-stu-id="e5620-162">Binary</span></span>|<span data-ttu-id="e5620-163">清单信息。</span><span class="sxs-lookup"><span data-stu-id="e5620-163">The manifest information.</span></span>|
|<span data-ttu-id="e5620-164">uploadState</span><span class="sxs-lookup"><span data-stu-id="e5620-164">uploadState</span></span>|[<span data-ttu-id="e5620-165">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="e5620-165">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="e5620-166">当前上传请求的状态。</span><span class="sxs-lookup"><span data-stu-id="e5620-166">The state of the current upload request.</span></span> <span data-ttu-id="e5620-167">可取值为：`success`、`transientError`、`error`、`unknown`、`azureStorageUriRequestSuccess`、`azureStorageUriRequestPending`、`azureStorageUriRequestFailed`、`azureStorageUriRequestTimedOut`、`azureStorageUriRenewalSuccess`、`azureStorageUriRenewalPending`、`azureStorageUriRenewalFailed`、`azureStorageUriRenewalTimedOut`、`commitFileSuccess`、`commitFilePending`、`commitFileFailed`、`commitFileTimedOut`。</span><span class="sxs-lookup"><span data-stu-id="e5620-167">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|
|<span data-ttu-id="e5620-168">isFrameworkFile</span><span class="sxs-lookup"><span data-stu-id="e5620-168">isFrameworkFile</span></span>|<span data-ttu-id="e5620-169">布尔</span><span class="sxs-lookup"><span data-stu-id="e5620-169">Boolean</span></span>|<span data-ttu-id="e5620-170">指示文件是否框架文件的值。</span><span class="sxs-lookup"><span data-stu-id="e5620-170">A value indicating whether the file is a framework file.</span></span>|
|<span data-ttu-id="e5620-171">isDependency</span><span class="sxs-lookup"><span data-stu-id="e5620-171">isDependency</span></span>|<span data-ttu-id="e5620-172">布尔</span><span class="sxs-lookup"><span data-stu-id="e5620-172">Boolean</span></span>|<span data-ttu-id="e5620-173">内容的文件是否依赖关系的主要内容文件。</span><span class="sxs-lookup"><span data-stu-id="e5620-173">Whether the content file is a dependency for the main content file.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e5620-174">Relationships</span><span class="sxs-lookup"><span data-stu-id="e5620-174">Relationships</span></span>
<span data-ttu-id="e5620-175">无</span><span class="sxs-lookup"><span data-stu-id="e5620-175">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e5620-176">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e5620-176">JSON Representation</span></span>
<span data-ttu-id="e5620-177">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e5620-177">Here is a JSON representation of the resource.</span></span>
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





