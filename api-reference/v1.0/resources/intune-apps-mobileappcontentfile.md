---
title: mobileAppContentFile 资源类型
description: 包含与给定 mobileAppContent 版本关联的单个安装程序文件的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4fa2655168ce9d0fdaa1d7842e904716fa6393ae
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37366480"
---
# <a name="mobileappcontentfile-resource-type"></a><span data-ttu-id="51813-103">mobileAppContentFile 资源类型</span><span class="sxs-lookup"><span data-stu-id="51813-103">mobileAppContentFile resource type</span></span>

> <span data-ttu-id="51813-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="51813-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51813-105">包含与给定 mobileAppContent 版本关联的单个安装程序文件的属性。</span><span class="sxs-lookup"><span data-stu-id="51813-105">Contains properties for a single installer file that is associated with a given mobileAppContent version.</span></span>

## <a name="methods"></a><span data-ttu-id="51813-106">方法</span><span class="sxs-lookup"><span data-stu-id="51813-106">Methods</span></span>
|<span data-ttu-id="51813-107">方法</span><span class="sxs-lookup"><span data-stu-id="51813-107">Method</span></span>|<span data-ttu-id="51813-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="51813-108">Return Type</span></span>|<span data-ttu-id="51813-109">说明</span><span class="sxs-lookup"><span data-stu-id="51813-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="51813-110">List mobileAppContentFiles</span><span class="sxs-lookup"><span data-stu-id="51813-110">List mobileAppContentFiles</span></span>](../api/intune-apps-mobileappcontentfile-list.md)|<span data-ttu-id="51813-111">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 集合</span><span class="sxs-lookup"><span data-stu-id="51813-111">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="51813-112">列出 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="51813-112">List properties and relationships of the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) objects.</span></span>|
|[<span data-ttu-id="51813-113">Get mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="51813-113">Get mobileAppContentFile</span></span>](../api/intune-apps-mobileappcontentfile-get.md)|[<span data-ttu-id="51813-114">mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="51813-114">mobileAppContentFile</span></span>](../resources/intune-apps-mobileappcontentfile.md)|<span data-ttu-id="51813-115">读取 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="51813-115">Read properties and relationships of the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>|
|[<span data-ttu-id="51813-116">Create mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="51813-116">Create mobileAppContentFile</span></span>](../api/intune-apps-mobileappcontentfile-create.md)|[<span data-ttu-id="51813-117">mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="51813-117">mobileAppContentFile</span></span>](../resources/intune-apps-mobileappcontentfile.md)|<span data-ttu-id="51813-118">创建新的 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="51813-118">Create a new [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>|
|[<span data-ttu-id="51813-119">Delete mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="51813-119">Delete mobileAppContentFile</span></span>](../api/intune-apps-mobileappcontentfile-delete.md)|<span data-ttu-id="51813-120">无</span><span class="sxs-lookup"><span data-stu-id="51813-120">None</span></span>|<span data-ttu-id="51813-121">删除 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)。</span><span class="sxs-lookup"><span data-stu-id="51813-121">Deletes a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span></span>|
|[<span data-ttu-id="51813-122">Update mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="51813-122">Update mobileAppContentFile</span></span>](../api/intune-apps-mobileappcontentfile-update.md)|[<span data-ttu-id="51813-123">mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="51813-123">mobileAppContentFile</span></span>](../resources/intune-apps-mobileappcontentfile.md)|<span data-ttu-id="51813-124">更新 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="51813-124">Update the properties of a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>|
|[<span data-ttu-id="51813-125">commit 操作</span><span class="sxs-lookup"><span data-stu-id="51813-125">commit action</span></span>](../api/intune-apps-mobileappcontentfile-commit.md)|<span data-ttu-id="51813-126">无</span><span class="sxs-lookup"><span data-stu-id="51813-126">None</span></span>|<span data-ttu-id="51813-127">提交给定应用的文件。</span><span class="sxs-lookup"><span data-stu-id="51813-127">Commits a file of a given app.</span></span>|
|[<span data-ttu-id="51813-128">renewUpload 操作</span><span class="sxs-lookup"><span data-stu-id="51813-128">renewUpload action</span></span>](../api/intune-apps-mobileappcontentfile-renewupload.md)|<span data-ttu-id="51813-129">无</span><span class="sxs-lookup"><span data-stu-id="51813-129">None</span></span>|<span data-ttu-id="51813-130">续订应用程序文件上传的 SAS URI。</span><span class="sxs-lookup"><span data-stu-id="51813-130">Renews the SAS URI for an application file upload.</span></span>|

## <a name="properties"></a><span data-ttu-id="51813-131">属性</span><span class="sxs-lookup"><span data-stu-id="51813-131">Properties</span></span>
|<span data-ttu-id="51813-132">属性</span><span class="sxs-lookup"><span data-stu-id="51813-132">Property</span></span>|<span data-ttu-id="51813-133">类型</span><span class="sxs-lookup"><span data-stu-id="51813-133">Type</span></span>|<span data-ttu-id="51813-134">说明</span><span class="sxs-lookup"><span data-stu-id="51813-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51813-135">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="51813-135">azureStorageUri</span></span>|<span data-ttu-id="51813-136">String</span><span class="sxs-lookup"><span data-stu-id="51813-136">String</span></span>|<span data-ttu-id="51813-137">Azure 存储 URI。</span><span class="sxs-lookup"><span data-stu-id="51813-137">The Azure Storage URI.</span></span>|
|<span data-ttu-id="51813-138">isCommitted</span><span class="sxs-lookup"><span data-stu-id="51813-138">isCommitted</span></span>|<span data-ttu-id="51813-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="51813-139">Boolean</span></span>|<span data-ttu-id="51813-140">指示文件是否已提交的值。</span><span class="sxs-lookup"><span data-stu-id="51813-140">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="51813-141">id</span><span class="sxs-lookup"><span data-stu-id="51813-141">id</span></span>|<span data-ttu-id="51813-142">String</span><span class="sxs-lookup"><span data-stu-id="51813-142">String</span></span>|<span data-ttu-id="51813-143">文件 ID。</span><span class="sxs-lookup"><span data-stu-id="51813-143">The File Id.</span></span>|
|<span data-ttu-id="51813-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="51813-144">createdDateTime</span></span>|<span data-ttu-id="51813-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51813-145">DateTimeOffset</span></span>|<span data-ttu-id="51813-146">创建文件的时间。</span><span class="sxs-lookup"><span data-stu-id="51813-146">The time the file was created.</span></span>|
|<span data-ttu-id="51813-147">name</span><span class="sxs-lookup"><span data-stu-id="51813-147">name</span></span>|<span data-ttu-id="51813-148">String</span><span class="sxs-lookup"><span data-stu-id="51813-148">String</span></span>|<span data-ttu-id="51813-149">文件名称。</span><span class="sxs-lookup"><span data-stu-id="51813-149">the file name.</span></span>|
|<span data-ttu-id="51813-150">size</span><span class="sxs-lookup"><span data-stu-id="51813-150">size</span></span>|<span data-ttu-id="51813-151">Int64</span><span class="sxs-lookup"><span data-stu-id="51813-151">Int64</span></span>|<span data-ttu-id="51813-152">加密前的文件大小。</span><span class="sxs-lookup"><span data-stu-id="51813-152">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="51813-153">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="51813-153">sizeEncrypted</span></span>|<span data-ttu-id="51813-154">Int64</span><span class="sxs-lookup"><span data-stu-id="51813-154">Int64</span></span>|<span data-ttu-id="51813-155">加密后的文件大小。</span><span class="sxs-lookup"><span data-stu-id="51813-155">The size of the file after encryption.</span></span>|
|<span data-ttu-id="51813-156">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="51813-156">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="51813-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51813-157">DateTimeOffset</span></span>|<span data-ttu-id="51813-158">Azure 存储 URI 的到期时间。</span><span class="sxs-lookup"><span data-stu-id="51813-158">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="51813-159">manifest</span><span class="sxs-lookup"><span data-stu-id="51813-159">manifest</span></span>|<span data-ttu-id="51813-160">Binary</span><span class="sxs-lookup"><span data-stu-id="51813-160">Binary</span></span>|<span data-ttu-id="51813-161">清单信息。</span><span class="sxs-lookup"><span data-stu-id="51813-161">The manifest information.</span></span>|
|<span data-ttu-id="51813-162">uploadState</span><span class="sxs-lookup"><span data-stu-id="51813-162">uploadState</span></span>|[<span data-ttu-id="51813-163">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="51813-163">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="51813-164">当前上传请求的状态。</span><span class="sxs-lookup"><span data-stu-id="51813-164">The state of the current upload request.</span></span> <span data-ttu-id="51813-165">可取值为：`success`、`transientError`、`error`、`unknown`、`azureStorageUriRequestSuccess`、`azureStorageUriRequestPending`、`azureStorageUriRequestFailed`、`azureStorageUriRequestTimedOut`、`azureStorageUriRenewalSuccess`、`azureStorageUriRenewalPending`、`azureStorageUriRenewalFailed`、`azureStorageUriRenewalTimedOut`、`commitFileSuccess`、`commitFilePending`、`commitFileFailed`、`commitFileTimedOut`。</span><span class="sxs-lookup"><span data-stu-id="51813-165">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="51813-166">关系</span><span class="sxs-lookup"><span data-stu-id="51813-166">Relationships</span></span>
<span data-ttu-id="51813-167">无</span><span class="sxs-lookup"><span data-stu-id="51813-167">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="51813-168">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="51813-168">JSON Representation</span></span>
<span data-ttu-id="51813-169">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="51813-169">Here is a JSON representation of the resource.</span></span>
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




