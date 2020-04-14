---
title: userInstallStateSummary 资源类型
description: 包含某个用户的安装状态摘要的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5da69650bd7cbf835a893f699fa6baf5b6df10dd
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43437404"
---
# <a name="userinstallstatesummary-resource-type"></a><span data-ttu-id="1656c-103">userInstallStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="1656c-103">userInstallStateSummary resource type</span></span>

<span data-ttu-id="1656c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1656c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1656c-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1656c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1656c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1656c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1656c-107">包含某个用户的安装状态摘要的属性。</span><span class="sxs-lookup"><span data-stu-id="1656c-107">Contains properties for the installation state summary for a user.</span></span>

## <a name="methods"></a><span data-ttu-id="1656c-108">方法</span><span class="sxs-lookup"><span data-stu-id="1656c-108">Methods</span></span>
|<span data-ttu-id="1656c-109">方法</span><span class="sxs-lookup"><span data-stu-id="1656c-109">Method</span></span>|<span data-ttu-id="1656c-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="1656c-110">Return Type</span></span>|<span data-ttu-id="1656c-111">说明</span><span class="sxs-lookup"><span data-stu-id="1656c-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1656c-112">列出 userInstallStateSummaries</span><span class="sxs-lookup"><span data-stu-id="1656c-112">List userInstallStateSummaries</span></span>](../api/intune-books-userinstallstatesummary-list.md)|<span data-ttu-id="1656c-113">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1656c-113">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="1656c-114">列出 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1656c-114">List properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) objects.</span></span>|
|[<span data-ttu-id="1656c-115">获取 userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="1656c-115">Get userInstallStateSummary</span></span>](../api/intune-books-userinstallstatesummary-get.md)|[<span data-ttu-id="1656c-116">userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="1656c-116">userInstallStateSummary</span></span>](../resources/intune-books-userinstallstatesummary.md)|<span data-ttu-id="1656c-117">读取 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1656c-117">Read properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>|
|[<span data-ttu-id="1656c-118">创建 userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="1656c-118">Create userInstallStateSummary</span></span>](../api/intune-books-userinstallstatesummary-create.md)|[<span data-ttu-id="1656c-119">userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="1656c-119">userInstallStateSummary</span></span>](../resources/intune-books-userinstallstatesummary.md)|<span data-ttu-id="1656c-120">创建新的 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1656c-120">Create a new [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>|
|[<span data-ttu-id="1656c-121">删除 userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="1656c-121">Delete userInstallStateSummary</span></span>](../api/intune-books-userinstallstatesummary-delete.md)|<span data-ttu-id="1656c-122">无</span><span class="sxs-lookup"><span data-stu-id="1656c-122">None</span></span>|<span data-ttu-id="1656c-123">删除 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)。</span><span class="sxs-lookup"><span data-stu-id="1656c-123">Deletes a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span></span>|
|[<span data-ttu-id="1656c-124">更新 userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="1656c-124">Update userInstallStateSummary</span></span>](../api/intune-books-userinstallstatesummary-update.md)|[<span data-ttu-id="1656c-125">userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="1656c-125">userInstallStateSummary</span></span>](../resources/intune-books-userinstallstatesummary.md)|<span data-ttu-id="1656c-126">更新 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1656c-126">Update the properties of a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1656c-127">属性</span><span class="sxs-lookup"><span data-stu-id="1656c-127">Properties</span></span>
|<span data-ttu-id="1656c-128">属性</span><span class="sxs-lookup"><span data-stu-id="1656c-128">Property</span></span>|<span data-ttu-id="1656c-129">类型</span><span class="sxs-lookup"><span data-stu-id="1656c-129">Type</span></span>|<span data-ttu-id="1656c-130">说明</span><span class="sxs-lookup"><span data-stu-id="1656c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1656c-131">id</span><span class="sxs-lookup"><span data-stu-id="1656c-131">id</span></span>|<span data-ttu-id="1656c-132">String</span><span class="sxs-lookup"><span data-stu-id="1656c-132">String</span></span>|<span data-ttu-id="1656c-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1656c-133">Key of the entity.</span></span>|
|<span data-ttu-id="1656c-134">userName</span><span class="sxs-lookup"><span data-stu-id="1656c-134">userName</span></span>|<span data-ttu-id="1656c-135">String</span><span class="sxs-lookup"><span data-stu-id="1656c-135">String</span></span>|<span data-ttu-id="1656c-136">用户名。</span><span class="sxs-lookup"><span data-stu-id="1656c-136">User name.</span></span>|
|<span data-ttu-id="1656c-137">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1656c-137">installedDeviceCount</span></span>|<span data-ttu-id="1656c-138">Int32</span><span class="sxs-lookup"><span data-stu-id="1656c-138">Int32</span></span>|<span data-ttu-id="1656c-139">已安装设备的计数。</span><span class="sxs-lookup"><span data-stu-id="1656c-139">Installed Device Count.</span></span>|
|<span data-ttu-id="1656c-140">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1656c-140">failedDeviceCount</span></span>|<span data-ttu-id="1656c-141">Int32</span><span class="sxs-lookup"><span data-stu-id="1656c-141">Int32</span></span>|<span data-ttu-id="1656c-142">已失败设备的计数。</span><span class="sxs-lookup"><span data-stu-id="1656c-142">Failed Device Count.</span></span>|
|<span data-ttu-id="1656c-143">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1656c-143">notInstalledDeviceCount</span></span>|<span data-ttu-id="1656c-144">Int32</span><span class="sxs-lookup"><span data-stu-id="1656c-144">Int32</span></span>|<span data-ttu-id="1656c-145">Not installed device count。</span><span class="sxs-lookup"><span data-stu-id="1656c-145">Not installed device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1656c-146">关系</span><span class="sxs-lookup"><span data-stu-id="1656c-146">Relationships</span></span>
|<span data-ttu-id="1656c-147">关系</span><span class="sxs-lookup"><span data-stu-id="1656c-147">Relationship</span></span>|<span data-ttu-id="1656c-148">类型</span><span class="sxs-lookup"><span data-stu-id="1656c-148">Type</span></span>|<span data-ttu-id="1656c-149">说明</span><span class="sxs-lookup"><span data-stu-id="1656c-149">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1656c-150">deviceStates</span><span class="sxs-lookup"><span data-stu-id="1656c-150">deviceStates</span></span>|<span data-ttu-id="1656c-151">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1656c-151">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="1656c-152">电子书的安装状态。</span><span class="sxs-lookup"><span data-stu-id="1656c-152">The install state of the eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1656c-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1656c-153">JSON Representation</span></span>
<span data-ttu-id="1656c-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1656c-154">Here is a JSON representation of the resource.</span></span>
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



