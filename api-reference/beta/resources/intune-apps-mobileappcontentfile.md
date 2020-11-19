---
title: mobileAppContentFile 资源类型
description: 包含与给定 mobileAppContent 版本关联的单个安装程序文件的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a5004a7b5d7ee1c38e559c41a86155cd89506af3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49281010"
---
# <a name="mobileappcontentfile-resource-type"></a><span data-ttu-id="d5df3-103">mobileAppContentFile 资源类型</span><span class="sxs-lookup"><span data-stu-id="d5df3-103">mobileAppContentFile resource type</span></span>

<span data-ttu-id="d5df3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5df3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d5df3-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d5df3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d5df3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d5df3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5df3-107">包含与给定 mobileAppContent 版本关联的单个安装程序文件的属性。</span><span class="sxs-lookup"><span data-stu-id="d5df3-107">Contains properties for a single installer file that is associated with a given mobileAppContent version.</span></span>

## <a name="methods"></a><span data-ttu-id="d5df3-108">Methods</span><span class="sxs-lookup"><span data-stu-id="d5df3-108">Methods</span></span>
|<span data-ttu-id="d5df3-109">方法</span><span class="sxs-lookup"><span data-stu-id="d5df3-109">Method</span></span>|<span data-ttu-id="d5df3-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="d5df3-110">Return Type</span></span>|<span data-ttu-id="d5df3-111">Description</span><span class="sxs-lookup"><span data-stu-id="d5df3-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d5df3-112">List mobileAppContentFiles</span><span class="sxs-lookup"><span data-stu-id="d5df3-112">List mobileAppContentFiles</span></span>](../api/intune-apps-mobileappcontentfile-list.md)|<span data-ttu-id="d5df3-113">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d5df3-113">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="d5df3-114">列出 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d5df3-114">List properties and relationships of the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) objects.</span></span>|
|[<span data-ttu-id="d5df3-115">Get mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="d5df3-115">Get mobileAppContentFile</span></span>](../api/intune-apps-mobileappcontentfile-get.md)|[<span data-ttu-id="d5df3-116">mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="d5df3-116">mobileAppContentFile</span></span>](../resources/intune-apps-mobileappcontentfile.md)|<span data-ttu-id="d5df3-117">读取 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d5df3-117">Read properties and relationships of the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>|
|[<span data-ttu-id="d5df3-118">Create mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="d5df3-118">Create mobileAppContentFile</span></span>](../api/intune-apps-mobileappcontentfile-create.md)|[<span data-ttu-id="d5df3-119">mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="d5df3-119">mobileAppContentFile</span></span>](../resources/intune-apps-mobileappcontentfile.md)|<span data-ttu-id="d5df3-120">创建新的 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d5df3-120">Create a new [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>|
|[<span data-ttu-id="d5df3-121">Delete mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="d5df3-121">Delete mobileAppContentFile</span></span>](../api/intune-apps-mobileappcontentfile-delete.md)|<span data-ttu-id="d5df3-122">无</span><span class="sxs-lookup"><span data-stu-id="d5df3-122">None</span></span>|<span data-ttu-id="d5df3-123">删除 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)。</span><span class="sxs-lookup"><span data-stu-id="d5df3-123">Deletes a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span></span>|
|[<span data-ttu-id="d5df3-124">Update mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="d5df3-124">Update mobileAppContentFile</span></span>](../api/intune-apps-mobileappcontentfile-update.md)|[<span data-ttu-id="d5df3-125">mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="d5df3-125">mobileAppContentFile</span></span>](../resources/intune-apps-mobileappcontentfile.md)|<span data-ttu-id="d5df3-126">更新 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d5df3-126">Update the properties of a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>|
|[<span data-ttu-id="d5df3-127">commit 操作</span><span class="sxs-lookup"><span data-stu-id="d5df3-127">commit action</span></span>](../api/intune-apps-mobileappcontentfile-commit.md)|<span data-ttu-id="d5df3-128">无</span><span class="sxs-lookup"><span data-stu-id="d5df3-128">None</span></span>|<span data-ttu-id="d5df3-129">提交给定应用的文件。</span><span class="sxs-lookup"><span data-stu-id="d5df3-129">Commits a file of a given app.</span></span>|
|[<span data-ttu-id="d5df3-130">renewUpload 操作</span><span class="sxs-lookup"><span data-stu-id="d5df3-130">renewUpload action</span></span>](../api/intune-apps-mobileappcontentfile-renewupload.md)|<span data-ttu-id="d5df3-131">无</span><span class="sxs-lookup"><span data-stu-id="d5df3-131">None</span></span>|<span data-ttu-id="d5df3-132">续订应用程序文件上传的 SAS URI。</span><span class="sxs-lookup"><span data-stu-id="d5df3-132">Renews the SAS URI for an application file upload.</span></span>|

## <a name="properties"></a><span data-ttu-id="d5df3-133">属性</span><span class="sxs-lookup"><span data-stu-id="d5df3-133">Properties</span></span>
|<span data-ttu-id="d5df3-134">属性</span><span class="sxs-lookup"><span data-stu-id="d5df3-134">Property</span></span>|<span data-ttu-id="d5df3-135">类型</span><span class="sxs-lookup"><span data-stu-id="d5df3-135">Type</span></span>|<span data-ttu-id="d5df3-136">Description</span><span class="sxs-lookup"><span data-stu-id="d5df3-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5df3-137">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="d5df3-137">azureStorageUri</span></span>|<span data-ttu-id="d5df3-138">String</span><span class="sxs-lookup"><span data-stu-id="d5df3-138">String</span></span>|<span data-ttu-id="d5df3-139">Azure 存储 URI。</span><span class="sxs-lookup"><span data-stu-id="d5df3-139">The Azure Storage URI.</span></span>|
|<span data-ttu-id="d5df3-140">isCommitted</span><span class="sxs-lookup"><span data-stu-id="d5df3-140">isCommitted</span></span>|<span data-ttu-id="d5df3-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="d5df3-141">Boolean</span></span>|<span data-ttu-id="d5df3-142">指示文件是否已提交的值。</span><span class="sxs-lookup"><span data-stu-id="d5df3-142">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="d5df3-143">id</span><span class="sxs-lookup"><span data-stu-id="d5df3-143">id</span></span>|<span data-ttu-id="d5df3-144">字符串</span><span class="sxs-lookup"><span data-stu-id="d5df3-144">String</span></span>|<span data-ttu-id="d5df3-145">文件 ID。</span><span class="sxs-lookup"><span data-stu-id="d5df3-145">The File Id.</span></span>|
|<span data-ttu-id="d5df3-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d5df3-146">createdDateTime</span></span>|<span data-ttu-id="d5df3-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5df3-147">DateTimeOffset</span></span>|<span data-ttu-id="d5df3-148">创建文件的时间。</span><span class="sxs-lookup"><span data-stu-id="d5df3-148">The time the file was created.</span></span>|
|<span data-ttu-id="d5df3-149">name</span><span class="sxs-lookup"><span data-stu-id="d5df3-149">name</span></span>|<span data-ttu-id="d5df3-150">字符串</span><span class="sxs-lookup"><span data-stu-id="d5df3-150">String</span></span>|<span data-ttu-id="d5df3-151">文件名称。</span><span class="sxs-lookup"><span data-stu-id="d5df3-151">the file name.</span></span>|
|<span data-ttu-id="d5df3-152">size</span><span class="sxs-lookup"><span data-stu-id="d5df3-152">size</span></span>|<span data-ttu-id="d5df3-153">Int64</span><span class="sxs-lookup"><span data-stu-id="d5df3-153">Int64</span></span>|<span data-ttu-id="d5df3-154">加密前的文件大小。</span><span class="sxs-lookup"><span data-stu-id="d5df3-154">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="d5df3-155">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="d5df3-155">sizeEncrypted</span></span>|<span data-ttu-id="d5df3-156">Int64</span><span class="sxs-lookup"><span data-stu-id="d5df3-156">Int64</span></span>|<span data-ttu-id="d5df3-157">加密后的文件大小。</span><span class="sxs-lookup"><span data-stu-id="d5df3-157">The size of the file after encryption.</span></span>|
|<span data-ttu-id="d5df3-158">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d5df3-158">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="d5df3-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5df3-159">DateTimeOffset</span></span>|<span data-ttu-id="d5df3-160">Azure 存储 URI 的到期时间。</span><span class="sxs-lookup"><span data-stu-id="d5df3-160">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="d5df3-161">manifest</span><span class="sxs-lookup"><span data-stu-id="d5df3-161">manifest</span></span>|<span data-ttu-id="d5df3-162">Binary</span><span class="sxs-lookup"><span data-stu-id="d5df3-162">Binary</span></span>|<span data-ttu-id="d5df3-163">清单信息。</span><span class="sxs-lookup"><span data-stu-id="d5df3-163">The manifest information.</span></span>|
|<span data-ttu-id="d5df3-164">uploadState</span><span class="sxs-lookup"><span data-stu-id="d5df3-164">uploadState</span></span>|[<span data-ttu-id="d5df3-165">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="d5df3-165">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="d5df3-166">当前上传请求的状态。</span><span class="sxs-lookup"><span data-stu-id="d5df3-166">The state of the current upload request.</span></span> <span data-ttu-id="d5df3-167">可取值为：`success`、`transientError`、`error`、`unknown`、`azureStorageUriRequestSuccess`、`azureStorageUriRequestPending`、`azureStorageUriRequestFailed`、`azureStorageUriRequestTimedOut`、`azureStorageUriRenewalSuccess`、`azureStorageUriRenewalPending`、`azureStorageUriRenewalFailed`、`azureStorageUriRenewalTimedOut`、`commitFileSuccess`、`commitFilePending`、`commitFileFailed`、`commitFileTimedOut`。</span><span class="sxs-lookup"><span data-stu-id="d5df3-167">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|
|<span data-ttu-id="d5df3-168">isFrameworkFile</span><span class="sxs-lookup"><span data-stu-id="d5df3-168">isFrameworkFile</span></span>|<span data-ttu-id="d5df3-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="d5df3-169">Boolean</span></span>|<span data-ttu-id="d5df3-170">一个指示文件是否为框架文件的值。</span><span class="sxs-lookup"><span data-stu-id="d5df3-170">A value indicating whether the file is a framework file.</span></span>|
|<span data-ttu-id="d5df3-171">isDependency</span><span class="sxs-lookup"><span data-stu-id="d5df3-171">isDependency</span></span>|<span data-ttu-id="d5df3-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="d5df3-172">Boolean</span></span>|<span data-ttu-id="d5df3-173">内容文件是否依赖于主要内容文件。</span><span class="sxs-lookup"><span data-stu-id="d5df3-173">Whether the content file is a dependency for the main content file.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d5df3-174">关系</span><span class="sxs-lookup"><span data-stu-id="d5df3-174">Relationships</span></span>
<span data-ttu-id="d5df3-175">无</span><span class="sxs-lookup"><span data-stu-id="d5df3-175">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d5df3-176">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d5df3-176">JSON Representation</span></span>
<span data-ttu-id="d5df3-177">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d5df3-177">Here is a JSON representation of the resource.</span></span>
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




