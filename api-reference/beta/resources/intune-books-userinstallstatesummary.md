---
title: userInstallStateSummary 资源类型
description: 包含某个用户的安装状态摘要的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8eb12003c108184739018b62c4ed9d28631103e4
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949393"
---
# <a name="userinstallstatesummary-resource-type"></a><span data-ttu-id="b8725-103">userInstallStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="b8725-103">userInstallStateSummary resource type</span></span>

> <span data-ttu-id="b8725-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b8725-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8725-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b8725-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8725-106">包含某个用户的安装状态摘要的属性。</span><span class="sxs-lookup"><span data-stu-id="b8725-106">Contains properties for the installation state summary for a user.</span></span>

## <a name="methods"></a><span data-ttu-id="b8725-107">方法</span><span class="sxs-lookup"><span data-stu-id="b8725-107">Methods</span></span>
|<span data-ttu-id="b8725-108">方法</span><span class="sxs-lookup"><span data-stu-id="b8725-108">Method</span></span>|<span data-ttu-id="b8725-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="b8725-109">Return Type</span></span>|<span data-ttu-id="b8725-110">说明</span><span class="sxs-lookup"><span data-stu-id="b8725-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b8725-111">列出 userInstallStateSummaries</span><span class="sxs-lookup"><span data-stu-id="b8725-111">List userInstallStateSummaries</span></span>](../api/intune-books-userinstallstatesummary-list.md)|<span data-ttu-id="b8725-112">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b8725-112">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="b8725-113">列出 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b8725-113">List properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) objects.</span></span>|
|[<span data-ttu-id="b8725-114">获取 userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="b8725-114">Get userInstallStateSummary</span></span>](../api/intune-books-userinstallstatesummary-get.md)|[<span data-ttu-id="b8725-115">userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="b8725-115">userInstallStateSummary</span></span>](../resources/intune-books-userinstallstatesummary.md)|<span data-ttu-id="b8725-116">读取 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b8725-116">Read properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>|
|[<span data-ttu-id="b8725-117">创建 userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="b8725-117">Create userInstallStateSummary</span></span>](../api/intune-books-userinstallstatesummary-create.md)|[<span data-ttu-id="b8725-118">userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="b8725-118">userInstallStateSummary</span></span>](../resources/intune-books-userinstallstatesummary.md)|<span data-ttu-id="b8725-119">创建新的 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b8725-119">Create a new [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>|
|[<span data-ttu-id="b8725-120">删除 userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="b8725-120">Delete userInstallStateSummary</span></span>](../api/intune-books-userinstallstatesummary-delete.md)|<span data-ttu-id="b8725-121">无</span><span class="sxs-lookup"><span data-stu-id="b8725-121">None</span></span>|<span data-ttu-id="b8725-122">删除 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)。</span><span class="sxs-lookup"><span data-stu-id="b8725-122">Deletes a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span></span>|
|[<span data-ttu-id="b8725-123">更新 userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="b8725-123">Update userInstallStateSummary</span></span>](../api/intune-books-userinstallstatesummary-update.md)|[<span data-ttu-id="b8725-124">userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="b8725-124">userInstallStateSummary</span></span>](../resources/intune-books-userinstallstatesummary.md)|<span data-ttu-id="b8725-125">更新 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b8725-125">Update the properties of a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b8725-126">属性</span><span class="sxs-lookup"><span data-stu-id="b8725-126">Properties</span></span>
|<span data-ttu-id="b8725-127">属性</span><span class="sxs-lookup"><span data-stu-id="b8725-127">Property</span></span>|<span data-ttu-id="b8725-128">类型</span><span class="sxs-lookup"><span data-stu-id="b8725-128">Type</span></span>|<span data-ttu-id="b8725-129">说明</span><span class="sxs-lookup"><span data-stu-id="b8725-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8725-130">id</span><span class="sxs-lookup"><span data-stu-id="b8725-130">id</span></span>|<span data-ttu-id="b8725-131">String</span><span class="sxs-lookup"><span data-stu-id="b8725-131">String</span></span>|<span data-ttu-id="b8725-132">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b8725-132">Key of the entity.</span></span>|
|<span data-ttu-id="b8725-133">userName</span><span class="sxs-lookup"><span data-stu-id="b8725-133">userName</span></span>|<span data-ttu-id="b8725-134">String</span><span class="sxs-lookup"><span data-stu-id="b8725-134">String</span></span>|<span data-ttu-id="b8725-135">用户名。</span><span class="sxs-lookup"><span data-stu-id="b8725-135">User name.</span></span>|
|<span data-ttu-id="b8725-136">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b8725-136">installedDeviceCount</span></span>|<span data-ttu-id="b8725-137">Int32</span><span class="sxs-lookup"><span data-stu-id="b8725-137">Int32</span></span>|<span data-ttu-id="b8725-138">已安装设备的计数。</span><span class="sxs-lookup"><span data-stu-id="b8725-138">Installed Device Count.</span></span>|
|<span data-ttu-id="b8725-139">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b8725-139">failedDeviceCount</span></span>|<span data-ttu-id="b8725-140">Int32</span><span class="sxs-lookup"><span data-stu-id="b8725-140">Int32</span></span>|<span data-ttu-id="b8725-141">已失败设备的计数。</span><span class="sxs-lookup"><span data-stu-id="b8725-141">Failed Device Count.</span></span>|
|<span data-ttu-id="b8725-142">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b8725-142">notInstalledDeviceCount</span></span>|<span data-ttu-id="b8725-143">Int32</span><span class="sxs-lookup"><span data-stu-id="b8725-143">Int32</span></span>|<span data-ttu-id="b8725-144">Not installed device count。</span><span class="sxs-lookup"><span data-stu-id="b8725-144">Not installed device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8725-145">关系</span><span class="sxs-lookup"><span data-stu-id="b8725-145">Relationships</span></span>
|<span data-ttu-id="b8725-146">关系</span><span class="sxs-lookup"><span data-stu-id="b8725-146">Relationship</span></span>|<span data-ttu-id="b8725-147">类型</span><span class="sxs-lookup"><span data-stu-id="b8725-147">Type</span></span>|<span data-ttu-id="b8725-148">说明</span><span class="sxs-lookup"><span data-stu-id="b8725-148">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8725-149">deviceStates</span><span class="sxs-lookup"><span data-stu-id="b8725-149">deviceStates</span></span>|<span data-ttu-id="b8725-150">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b8725-150">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="b8725-151">电子书的安装状态。</span><span class="sxs-lookup"><span data-stu-id="b8725-151">The install state of the eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b8725-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b8725-152">JSON Representation</span></span>
<span data-ttu-id="b8725-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b8725-153">Here is a JSON representation of the resource.</span></span>
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




