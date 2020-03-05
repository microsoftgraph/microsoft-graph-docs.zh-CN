---
title: userInstallStateSummary 资源类型
description: 包含某个用户的安装状态摘要的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4a9b615868d97f9df7c708ee5264240dd32f1284
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42488549"
---
# <a name="userinstallstatesummary-resource-type"></a><span data-ttu-id="e963c-103">userInstallStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="e963c-103">userInstallStateSummary resource type</span></span>

<span data-ttu-id="e963c-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="e963c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e963c-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e963c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e963c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e963c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e963c-107">包含某个用户的安装状态摘要的属性。</span><span class="sxs-lookup"><span data-stu-id="e963c-107">Contains properties for the installation state summary for a user.</span></span>

## <a name="methods"></a><span data-ttu-id="e963c-108">方法</span><span class="sxs-lookup"><span data-stu-id="e963c-108">Methods</span></span>
|<span data-ttu-id="e963c-109">方法</span><span class="sxs-lookup"><span data-stu-id="e963c-109">Method</span></span>|<span data-ttu-id="e963c-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="e963c-110">Return Type</span></span>|<span data-ttu-id="e963c-111">说明</span><span class="sxs-lookup"><span data-stu-id="e963c-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e963c-112">列出 userInstallStateSummaries</span><span class="sxs-lookup"><span data-stu-id="e963c-112">List userInstallStateSummaries</span></span>](../api/intune-books-userinstallstatesummary-list.md)|<span data-ttu-id="e963c-113">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e963c-113">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="e963c-114">列出 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e963c-114">List properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) objects.</span></span>|
|[<span data-ttu-id="e963c-115">获取 userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="e963c-115">Get userInstallStateSummary</span></span>](../api/intune-books-userinstallstatesummary-get.md)|[<span data-ttu-id="e963c-116">userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="e963c-116">userInstallStateSummary</span></span>](../resources/intune-books-userinstallstatesummary.md)|<span data-ttu-id="e963c-117">读取 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e963c-117">Read properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>|
|[<span data-ttu-id="e963c-118">创建 userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="e963c-118">Create userInstallStateSummary</span></span>](../api/intune-books-userinstallstatesummary-create.md)|[<span data-ttu-id="e963c-119">userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="e963c-119">userInstallStateSummary</span></span>](../resources/intune-books-userinstallstatesummary.md)|<span data-ttu-id="e963c-120">创建新的 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e963c-120">Create a new [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>|
|[<span data-ttu-id="e963c-121">删除 userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="e963c-121">Delete userInstallStateSummary</span></span>](../api/intune-books-userinstallstatesummary-delete.md)|<span data-ttu-id="e963c-122">无</span><span class="sxs-lookup"><span data-stu-id="e963c-122">None</span></span>|<span data-ttu-id="e963c-123">删除 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)。</span><span class="sxs-lookup"><span data-stu-id="e963c-123">Deletes a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span></span>|
|[<span data-ttu-id="e963c-124">更新 userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="e963c-124">Update userInstallStateSummary</span></span>](../api/intune-books-userinstallstatesummary-update.md)|[<span data-ttu-id="e963c-125">userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="e963c-125">userInstallStateSummary</span></span>](../resources/intune-books-userinstallstatesummary.md)|<span data-ttu-id="e963c-126">更新 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e963c-126">Update the properties of a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e963c-127">属性</span><span class="sxs-lookup"><span data-stu-id="e963c-127">Properties</span></span>
|<span data-ttu-id="e963c-128">属性</span><span class="sxs-lookup"><span data-stu-id="e963c-128">Property</span></span>|<span data-ttu-id="e963c-129">类型</span><span class="sxs-lookup"><span data-stu-id="e963c-129">Type</span></span>|<span data-ttu-id="e963c-130">说明</span><span class="sxs-lookup"><span data-stu-id="e963c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e963c-131">id</span><span class="sxs-lookup"><span data-stu-id="e963c-131">id</span></span>|<span data-ttu-id="e963c-132">String</span><span class="sxs-lookup"><span data-stu-id="e963c-132">String</span></span>|<span data-ttu-id="e963c-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e963c-133">Key of the entity.</span></span>|
|<span data-ttu-id="e963c-134">userName</span><span class="sxs-lookup"><span data-stu-id="e963c-134">userName</span></span>|<span data-ttu-id="e963c-135">String</span><span class="sxs-lookup"><span data-stu-id="e963c-135">String</span></span>|<span data-ttu-id="e963c-136">用户名。</span><span class="sxs-lookup"><span data-stu-id="e963c-136">User name.</span></span>|
|<span data-ttu-id="e963c-137">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e963c-137">installedDeviceCount</span></span>|<span data-ttu-id="e963c-138">Int32</span><span class="sxs-lookup"><span data-stu-id="e963c-138">Int32</span></span>|<span data-ttu-id="e963c-139">已安装设备的计数。</span><span class="sxs-lookup"><span data-stu-id="e963c-139">Installed Device Count.</span></span>|
|<span data-ttu-id="e963c-140">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e963c-140">failedDeviceCount</span></span>|<span data-ttu-id="e963c-141">Int32</span><span class="sxs-lookup"><span data-stu-id="e963c-141">Int32</span></span>|<span data-ttu-id="e963c-142">已失败设备的计数。</span><span class="sxs-lookup"><span data-stu-id="e963c-142">Failed Device Count.</span></span>|
|<span data-ttu-id="e963c-143">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e963c-143">notInstalledDeviceCount</span></span>|<span data-ttu-id="e963c-144">Int32</span><span class="sxs-lookup"><span data-stu-id="e963c-144">Int32</span></span>|<span data-ttu-id="e963c-145">Not installed device count。</span><span class="sxs-lookup"><span data-stu-id="e963c-145">Not installed device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e963c-146">关系</span><span class="sxs-lookup"><span data-stu-id="e963c-146">Relationships</span></span>
|<span data-ttu-id="e963c-147">关系</span><span class="sxs-lookup"><span data-stu-id="e963c-147">Relationship</span></span>|<span data-ttu-id="e963c-148">类型</span><span class="sxs-lookup"><span data-stu-id="e963c-148">Type</span></span>|<span data-ttu-id="e963c-149">说明</span><span class="sxs-lookup"><span data-stu-id="e963c-149">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e963c-150">deviceStates</span><span class="sxs-lookup"><span data-stu-id="e963c-150">deviceStates</span></span>|<span data-ttu-id="e963c-151">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e963c-151">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="e963c-152">电子书的安装状态。</span><span class="sxs-lookup"><span data-stu-id="e963c-152">The install state of the eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e963c-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e963c-153">JSON Representation</span></span>
<span data-ttu-id="e963c-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e963c-154">Here is a JSON representation of the resource.</span></span>
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



