---
title: appLogCollectionRequest 资源类型
description: AppLogCollectionRequest 实体。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 24d6ee782dc50935cffddc9916b04121bf3a1cb1
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943198"
---
# <a name="applogcollectionrequest-resource-type"></a><span data-ttu-id="e3c68-103">appLogCollectionRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="e3c68-103">appLogCollectionRequest resource type</span></span>

> <span data-ttu-id="e3c68-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e3c68-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e3c68-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e3c68-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3c68-106">AppLogCollectionRequest 实体。</span><span class="sxs-lookup"><span data-stu-id="e3c68-106">AppLogCollectionRequest Entity.</span></span>

## <a name="methods"></a><span data-ttu-id="e3c68-107">方法</span><span class="sxs-lookup"><span data-stu-id="e3c68-107">Methods</span></span>
|<span data-ttu-id="e3c68-108">方法</span><span class="sxs-lookup"><span data-stu-id="e3c68-108">Method</span></span>|<span data-ttu-id="e3c68-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="e3c68-109">Return Type</span></span>|<span data-ttu-id="e3c68-110">说明</span><span class="sxs-lookup"><span data-stu-id="e3c68-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e3c68-111">列出 appLogCollectionRequests</span><span class="sxs-lookup"><span data-stu-id="e3c68-111">List appLogCollectionRequests</span></span>](../api/intune-devices-applogcollectionrequest-list.md)|<span data-ttu-id="e3c68-112">[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)集合</span><span class="sxs-lookup"><span data-stu-id="e3c68-112">[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) collection</span></span>|<span data-ttu-id="e3c68-113">列出[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e3c68-113">List properties and relationships of the [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) objects.</span></span>|
|[<span data-ttu-id="e3c68-114">获取 appLogCollectionRequest</span><span class="sxs-lookup"><span data-stu-id="e3c68-114">Get appLogCollectionRequest</span></span>](../api/intune-devices-applogcollectionrequest-get.md)|[<span data-ttu-id="e3c68-115">appLogCollectionRequest</span><span class="sxs-lookup"><span data-stu-id="e3c68-115">appLogCollectionRequest</span></span>](../resources/intune-devices-applogcollectionrequest.md)|<span data-ttu-id="e3c68-116">读取[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e3c68-116">Read properties and relationships of the [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object.</span></span>|
|[<span data-ttu-id="e3c68-117">创建 appLogCollectionRequest</span><span class="sxs-lookup"><span data-stu-id="e3c68-117">Create appLogCollectionRequest</span></span>](../api/intune-devices-applogcollectionrequest-create.md)|[<span data-ttu-id="e3c68-118">appLogCollectionRequest</span><span class="sxs-lookup"><span data-stu-id="e3c68-118">appLogCollectionRequest</span></span>](../resources/intune-devices-applogcollectionrequest.md)|<span data-ttu-id="e3c68-119">创建新的[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e3c68-119">Create a new [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object.</span></span>|
|[<span data-ttu-id="e3c68-120">删除 appLogCollectionRequest</span><span class="sxs-lookup"><span data-stu-id="e3c68-120">Delete appLogCollectionRequest</span></span>](../api/intune-devices-applogcollectionrequest-delete.md)|<span data-ttu-id="e3c68-121">无</span><span class="sxs-lookup"><span data-stu-id="e3c68-121">None</span></span>|<span data-ttu-id="e3c68-122">删除[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)。</span><span class="sxs-lookup"><span data-stu-id="e3c68-122">Deletes a [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md).</span></span>|
|[<span data-ttu-id="e3c68-123">更新 appLogCollectionRequest</span><span class="sxs-lookup"><span data-stu-id="e3c68-123">Update appLogCollectionRequest</span></span>](../api/intune-devices-applogcollectionrequest-update.md)|[<span data-ttu-id="e3c68-124">appLogCollectionRequest</span><span class="sxs-lookup"><span data-stu-id="e3c68-124">appLogCollectionRequest</span></span>](../resources/intune-devices-applogcollectionrequest.md)|<span data-ttu-id="e3c68-125">更新[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e3c68-125">Update the properties of a [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object.</span></span>|
|[<span data-ttu-id="e3c68-126">createDownloadUrl 操作</span><span class="sxs-lookup"><span data-stu-id="e3c68-126">createDownloadUrl action</span></span>](../api/intune-devices-applogcollectionrequest-createdownloadurl.md)|[<span data-ttu-id="e3c68-127">appLogCollectionDownloadDetails</span><span class="sxs-lookup"><span data-stu-id="e3c68-127">appLogCollectionDownloadDetails</span></span>](../resources/intune-devices-applogcollectiondownloaddetails.md)|<span data-ttu-id="e3c68-128">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e3c68-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="e3c68-129">属性</span><span class="sxs-lookup"><span data-stu-id="e3c68-129">Properties</span></span>
|<span data-ttu-id="e3c68-130">属性</span><span class="sxs-lookup"><span data-stu-id="e3c68-130">Property</span></span>|<span data-ttu-id="e3c68-131">类型</span><span class="sxs-lookup"><span data-stu-id="e3c68-131">Type</span></span>|<span data-ttu-id="e3c68-132">说明</span><span class="sxs-lookup"><span data-stu-id="e3c68-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3c68-133">id</span><span class="sxs-lookup"><span data-stu-id="e3c68-133">id</span></span>|<span data-ttu-id="e3c68-134">String</span><span class="sxs-lookup"><span data-stu-id="e3c68-134">String</span></span>|<span data-ttu-id="e3c68-135">唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e3c68-135">The unique Identifier.</span></span> <span data-ttu-id="e3c68-136">这是 userId_DeviceId_AppId id。</span><span class="sxs-lookup"><span data-stu-id="e3c68-136">This is userId_DeviceId_AppId id.</span></span>|
|<span data-ttu-id="e3c68-137">status</span><span class="sxs-lookup"><span data-stu-id="e3c68-137">status</span></span>|[<span data-ttu-id="e3c68-138">appLogUploadState</span><span class="sxs-lookup"><span data-stu-id="e3c68-138">appLogUploadState</span></span>](../resources/intune-devices-apploguploadstate.md)|<span data-ttu-id="e3c68-139">日志上载状态。</span><span class="sxs-lookup"><span data-stu-id="e3c68-139">Log upload status.</span></span> <span data-ttu-id="e3c68-140">可取值为：`pending`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="e3c68-140">Possible values are: `pending`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="e3c68-141">errorMessage</span><span class="sxs-lookup"><span data-stu-id="e3c68-141">errorMessage</span></span>|<span data-ttu-id="e3c68-142">String</span><span class="sxs-lookup"><span data-stu-id="e3c68-142">String</span></span>|<span data-ttu-id="e3c68-143">在上载过程中出现的错误消息</span><span class="sxs-lookup"><span data-stu-id="e3c68-143">Error message if any during the upload process</span></span>|
|<span data-ttu-id="e3c68-144">customLogFolders</span><span class="sxs-lookup"><span data-stu-id="e3c68-144">customLogFolders</span></span>|<span data-ttu-id="e3c68-145">String collection</span><span class="sxs-lookup"><span data-stu-id="e3c68-145">String collection</span></span>|<span data-ttu-id="e3c68-146">日志文件夹的列表。</span><span class="sxs-lookup"><span data-stu-id="e3c68-146">List of log folders.</span></span> |
|<span data-ttu-id="e3c68-147">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="e3c68-147">completedDateTime</span></span>|<span data-ttu-id="e3c68-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3c68-148">DateTimeOffset</span></span>|<span data-ttu-id="e3c68-149">上传日志请求到达终端状态的时间</span><span class="sxs-lookup"><span data-stu-id="e3c68-149">Time at which the upload log request reached a terminal state</span></span>|

## <a name="relationships"></a><span data-ttu-id="e3c68-150">关系</span><span class="sxs-lookup"><span data-stu-id="e3c68-150">Relationships</span></span>
<span data-ttu-id="e3c68-151">无</span><span class="sxs-lookup"><span data-stu-id="e3c68-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e3c68-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e3c68-152">JSON Representation</span></span>
<span data-ttu-id="e3c68-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e3c68-153">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.appLogCollectionRequest"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appLogCollectionRequest",
  "id": "String (identifier)",
  "status": "String",
  "errorMessage": "String",
  "customLogFolders": [
    "String"
  ],
  "completedDateTime": "String (timestamp)"
}
```




