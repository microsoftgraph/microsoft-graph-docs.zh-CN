---
title: userInstallStateSummary 资源类型
description: 包含某个用户的安装状态摘要的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f323aaaa49d9cf19d4322a854986b692d8df543d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49295178"
---
# <a name="userinstallstatesummary-resource-type"></a><span data-ttu-id="94a83-103">userInstallStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="94a83-103">userInstallStateSummary resource type</span></span>

<span data-ttu-id="94a83-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94a83-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="94a83-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="94a83-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="94a83-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="94a83-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94a83-107">包含某个用户的安装状态摘要的属性。</span><span class="sxs-lookup"><span data-stu-id="94a83-107">Contains properties for the installation state summary for a user.</span></span>

## <a name="methods"></a><span data-ttu-id="94a83-108">Methods</span><span class="sxs-lookup"><span data-stu-id="94a83-108">Methods</span></span>
|<span data-ttu-id="94a83-109">方法</span><span class="sxs-lookup"><span data-stu-id="94a83-109">Method</span></span>|<span data-ttu-id="94a83-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="94a83-110">Return Type</span></span>|<span data-ttu-id="94a83-111">Description</span><span class="sxs-lookup"><span data-stu-id="94a83-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="94a83-112">列出 userInstallStateSummaries</span><span class="sxs-lookup"><span data-stu-id="94a83-112">List userInstallStateSummaries</span></span>](../api/intune-books-userinstallstatesummary-list.md)|<span data-ttu-id="94a83-113">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="94a83-113">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="94a83-114">列出 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="94a83-114">List properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) objects.</span></span>|
|[<span data-ttu-id="94a83-115">获取 userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="94a83-115">Get userInstallStateSummary</span></span>](../api/intune-books-userinstallstatesummary-get.md)|[<span data-ttu-id="94a83-116">userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="94a83-116">userInstallStateSummary</span></span>](../resources/intune-books-userinstallstatesummary.md)|<span data-ttu-id="94a83-117">读取 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="94a83-117">Read properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>|
|[<span data-ttu-id="94a83-118">创建 userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="94a83-118">Create userInstallStateSummary</span></span>](../api/intune-books-userinstallstatesummary-create.md)|[<span data-ttu-id="94a83-119">userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="94a83-119">userInstallStateSummary</span></span>](../resources/intune-books-userinstallstatesummary.md)|<span data-ttu-id="94a83-120">创建新的 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="94a83-120">Create a new [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>|
|[<span data-ttu-id="94a83-121">删除 userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="94a83-121">Delete userInstallStateSummary</span></span>](../api/intune-books-userinstallstatesummary-delete.md)|<span data-ttu-id="94a83-122">无</span><span class="sxs-lookup"><span data-stu-id="94a83-122">None</span></span>|<span data-ttu-id="94a83-123">删除 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)。</span><span class="sxs-lookup"><span data-stu-id="94a83-123">Deletes a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span></span>|
|[<span data-ttu-id="94a83-124">更新 userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="94a83-124">Update userInstallStateSummary</span></span>](../api/intune-books-userinstallstatesummary-update.md)|[<span data-ttu-id="94a83-125">userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="94a83-125">userInstallStateSummary</span></span>](../resources/intune-books-userinstallstatesummary.md)|<span data-ttu-id="94a83-126">更新 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="94a83-126">Update the properties of a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="94a83-127">属性</span><span class="sxs-lookup"><span data-stu-id="94a83-127">Properties</span></span>
|<span data-ttu-id="94a83-128">属性</span><span class="sxs-lookup"><span data-stu-id="94a83-128">Property</span></span>|<span data-ttu-id="94a83-129">类型</span><span class="sxs-lookup"><span data-stu-id="94a83-129">Type</span></span>|<span data-ttu-id="94a83-130">说明</span><span class="sxs-lookup"><span data-stu-id="94a83-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94a83-131">id</span><span class="sxs-lookup"><span data-stu-id="94a83-131">id</span></span>|<span data-ttu-id="94a83-132">字符串</span><span class="sxs-lookup"><span data-stu-id="94a83-132">String</span></span>|<span data-ttu-id="94a83-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="94a83-133">Key of the entity.</span></span>|
|<span data-ttu-id="94a83-134">userName</span><span class="sxs-lookup"><span data-stu-id="94a83-134">userName</span></span>|<span data-ttu-id="94a83-135">String</span><span class="sxs-lookup"><span data-stu-id="94a83-135">String</span></span>|<span data-ttu-id="94a83-136">用户名。</span><span class="sxs-lookup"><span data-stu-id="94a83-136">User name.</span></span>|
|<span data-ttu-id="94a83-137">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="94a83-137">installedDeviceCount</span></span>|<span data-ttu-id="94a83-138">Int32</span><span class="sxs-lookup"><span data-stu-id="94a83-138">Int32</span></span>|<span data-ttu-id="94a83-139">已安装设备的计数。</span><span class="sxs-lookup"><span data-stu-id="94a83-139">Installed Device Count.</span></span>|
|<span data-ttu-id="94a83-140">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="94a83-140">failedDeviceCount</span></span>|<span data-ttu-id="94a83-141">Int32</span><span class="sxs-lookup"><span data-stu-id="94a83-141">Int32</span></span>|<span data-ttu-id="94a83-142">已失败设备的计数。</span><span class="sxs-lookup"><span data-stu-id="94a83-142">Failed Device Count.</span></span>|
|<span data-ttu-id="94a83-143">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="94a83-143">notInstalledDeviceCount</span></span>|<span data-ttu-id="94a83-144">Int32</span><span class="sxs-lookup"><span data-stu-id="94a83-144">Int32</span></span>|<span data-ttu-id="94a83-145">Not installed device count。</span><span class="sxs-lookup"><span data-stu-id="94a83-145">Not installed device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="94a83-146">关系</span><span class="sxs-lookup"><span data-stu-id="94a83-146">Relationships</span></span>
|<span data-ttu-id="94a83-147">关系</span><span class="sxs-lookup"><span data-stu-id="94a83-147">Relationship</span></span>|<span data-ttu-id="94a83-148">类型</span><span class="sxs-lookup"><span data-stu-id="94a83-148">Type</span></span>|<span data-ttu-id="94a83-149">Description</span><span class="sxs-lookup"><span data-stu-id="94a83-149">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94a83-150">deviceStates</span><span class="sxs-lookup"><span data-stu-id="94a83-150">deviceStates</span></span>|<span data-ttu-id="94a83-151">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="94a83-151">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="94a83-152">电子书的安装状态。</span><span class="sxs-lookup"><span data-stu-id="94a83-152">The install state of the eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="94a83-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="94a83-153">JSON Representation</span></span>
<span data-ttu-id="94a83-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="94a83-154">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userInstallStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userInstallStateSummary",
  "id": "String (identifier)",
  "userName": "String",
  "installedDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "notInstalledDeviceCount": 1024
}
```




