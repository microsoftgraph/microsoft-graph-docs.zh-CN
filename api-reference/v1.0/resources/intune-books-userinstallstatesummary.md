---
title: userInstallStateSummary 资源类型
description: 包含某个用户的安装状态摘要的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5e7c219ef2128f6d15a0efc6e98ec781e2c47ffe
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262571"
---
# <a name="userinstallstatesummary-resource-type"></a><span data-ttu-id="94244-103">userInstallStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="94244-103">userInstallStateSummary resource type</span></span>

> <span data-ttu-id="94244-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="94244-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94244-105">包含某个用户的安装状态摘要的属性。</span><span class="sxs-lookup"><span data-stu-id="94244-105">Contains properties for the installation state summary for a user.</span></span>

## <a name="methods"></a><span data-ttu-id="94244-106">方法</span><span class="sxs-lookup"><span data-stu-id="94244-106">Methods</span></span>
|<span data-ttu-id="94244-107">方法</span><span class="sxs-lookup"><span data-stu-id="94244-107">Method</span></span>|<span data-ttu-id="94244-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="94244-108">Return Type</span></span>|<span data-ttu-id="94244-109">说明</span><span class="sxs-lookup"><span data-stu-id="94244-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="94244-110">列出 userInstallStateSummaries</span><span class="sxs-lookup"><span data-stu-id="94244-110">List userInstallStateSummaries</span></span>](../api/intune-books-userinstallstatesummary-list.md)|<span data-ttu-id="94244-111">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="94244-111">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="94244-112">列出 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="94244-112">List properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) objects.</span></span>|
|[<span data-ttu-id="94244-113">获取 userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="94244-113">Get userInstallStateSummary</span></span>](../api/intune-books-userinstallstatesummary-get.md)|[<span data-ttu-id="94244-114">userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="94244-114">userInstallStateSummary</span></span>](../resources/intune-books-userinstallstatesummary.md)|<span data-ttu-id="94244-115">读取 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="94244-115">Read properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>|
|[<span data-ttu-id="94244-116">创建 userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="94244-116">Create userInstallStateSummary</span></span>](../api/intune-books-userinstallstatesummary-create.md)|[<span data-ttu-id="94244-117">userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="94244-117">userInstallStateSummary</span></span>](../resources/intune-books-userinstallstatesummary.md)|<span data-ttu-id="94244-118">创建新的 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="94244-118">Create a new [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>|
|[<span data-ttu-id="94244-119">删除 userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="94244-119">Delete userInstallStateSummary</span></span>](../api/intune-books-userinstallstatesummary-delete.md)|<span data-ttu-id="94244-120">无</span><span class="sxs-lookup"><span data-stu-id="94244-120">None</span></span>|<span data-ttu-id="94244-121">删除 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)。</span><span class="sxs-lookup"><span data-stu-id="94244-121">Deletes a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span></span>|
|[<span data-ttu-id="94244-122">更新 userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="94244-122">Update userInstallStateSummary</span></span>](../api/intune-books-userinstallstatesummary-update.md)|[<span data-ttu-id="94244-123">userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="94244-123">userInstallStateSummary</span></span>](../resources/intune-books-userinstallstatesummary.md)|<span data-ttu-id="94244-124">更新 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="94244-124">Update the properties of a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="94244-125">属性</span><span class="sxs-lookup"><span data-stu-id="94244-125">Properties</span></span>
|<span data-ttu-id="94244-126">属性</span><span class="sxs-lookup"><span data-stu-id="94244-126">Property</span></span>|<span data-ttu-id="94244-127">类型</span><span class="sxs-lookup"><span data-stu-id="94244-127">Type</span></span>|<span data-ttu-id="94244-128">说明</span><span class="sxs-lookup"><span data-stu-id="94244-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94244-129">id</span><span class="sxs-lookup"><span data-stu-id="94244-129">id</span></span>|<span data-ttu-id="94244-130">字符串</span><span class="sxs-lookup"><span data-stu-id="94244-130">String</span></span>|<span data-ttu-id="94244-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="94244-131">Key of the entity.</span></span>|
|<span data-ttu-id="94244-132">userName</span><span class="sxs-lookup"><span data-stu-id="94244-132">userName</span></span>|<span data-ttu-id="94244-133">String</span><span class="sxs-lookup"><span data-stu-id="94244-133">String</span></span>|<span data-ttu-id="94244-134">用户名。</span><span class="sxs-lookup"><span data-stu-id="94244-134">User name.</span></span>|
|<span data-ttu-id="94244-135">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="94244-135">installedDeviceCount</span></span>|<span data-ttu-id="94244-136">Int32</span><span class="sxs-lookup"><span data-stu-id="94244-136">Int32</span></span>|<span data-ttu-id="94244-137">已安装设备的计数。</span><span class="sxs-lookup"><span data-stu-id="94244-137">Installed Device Count.</span></span>|
|<span data-ttu-id="94244-138">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="94244-138">failedDeviceCount</span></span>|<span data-ttu-id="94244-139">Int32</span><span class="sxs-lookup"><span data-stu-id="94244-139">Int32</span></span>|<span data-ttu-id="94244-140">已失败设备的计数。</span><span class="sxs-lookup"><span data-stu-id="94244-140">Failed Device Count.</span></span>|
|<span data-ttu-id="94244-141">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="94244-141">notInstalledDeviceCount</span></span>|<span data-ttu-id="94244-142">Int32</span><span class="sxs-lookup"><span data-stu-id="94244-142">Int32</span></span>|<span data-ttu-id="94244-143">Not installed device count。</span><span class="sxs-lookup"><span data-stu-id="94244-143">Not installed device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="94244-144">关系</span><span class="sxs-lookup"><span data-stu-id="94244-144">Relationships</span></span>
|<span data-ttu-id="94244-145">关系</span><span class="sxs-lookup"><span data-stu-id="94244-145">Relationship</span></span>|<span data-ttu-id="94244-146">类型</span><span class="sxs-lookup"><span data-stu-id="94244-146">Type</span></span>|<span data-ttu-id="94244-147">说明</span><span class="sxs-lookup"><span data-stu-id="94244-147">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94244-148">deviceStates</span><span class="sxs-lookup"><span data-stu-id="94244-148">deviceStates</span></span>|<span data-ttu-id="94244-149">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="94244-149">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="94244-150">电子书的安装状态。</span><span class="sxs-lookup"><span data-stu-id="94244-150">The install state of the eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="94244-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="94244-151">JSON Representation</span></span>
<span data-ttu-id="94244-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="94244-152">Here is a JSON representation of the resource.</span></span>
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



