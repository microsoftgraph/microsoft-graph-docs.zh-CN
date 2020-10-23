---
title: userInstallStateSummary 资源类型
description: 包含某个用户的安装状态摘要的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8372687b174c5c7e1997227df48bac82afecffa4
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48694016"
---
# <a name="userinstallstatesummary-resource-type"></a><span data-ttu-id="a61e7-103">userInstallStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="a61e7-103">userInstallStateSummary resource type</span></span>

<span data-ttu-id="a61e7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a61e7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a61e7-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a61e7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a61e7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a61e7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a61e7-107">包含某个用户的安装状态摘要的属性。</span><span class="sxs-lookup"><span data-stu-id="a61e7-107">Contains properties for the installation state summary for a user.</span></span>

## <a name="methods"></a><span data-ttu-id="a61e7-108">Methods</span><span class="sxs-lookup"><span data-stu-id="a61e7-108">Methods</span></span>
|<span data-ttu-id="a61e7-109">方法</span><span class="sxs-lookup"><span data-stu-id="a61e7-109">Method</span></span>|<span data-ttu-id="a61e7-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="a61e7-110">Return Type</span></span>|<span data-ttu-id="a61e7-111">说明</span><span class="sxs-lookup"><span data-stu-id="a61e7-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a61e7-112">列出 userInstallStateSummaries</span><span class="sxs-lookup"><span data-stu-id="a61e7-112">List userInstallStateSummaries</span></span>](../api/intune-books-userinstallstatesummary-list.md)|<span data-ttu-id="a61e7-113">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a61e7-113">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="a61e7-114">列出 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a61e7-114">List properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) objects.</span></span>|
|[<span data-ttu-id="a61e7-115">获取 userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="a61e7-115">Get userInstallStateSummary</span></span>](../api/intune-books-userinstallstatesummary-get.md)|[<span data-ttu-id="a61e7-116">userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="a61e7-116">userInstallStateSummary</span></span>](../resources/intune-books-userinstallstatesummary.md)|<span data-ttu-id="a61e7-117">读取 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a61e7-117">Read properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>|
|[<span data-ttu-id="a61e7-118">创建 userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="a61e7-118">Create userInstallStateSummary</span></span>](../api/intune-books-userinstallstatesummary-create.md)|[<span data-ttu-id="a61e7-119">userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="a61e7-119">userInstallStateSummary</span></span>](../resources/intune-books-userinstallstatesummary.md)|<span data-ttu-id="a61e7-120">创建新的 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a61e7-120">Create a new [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>|
|[<span data-ttu-id="a61e7-121">删除 userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="a61e7-121">Delete userInstallStateSummary</span></span>](../api/intune-books-userinstallstatesummary-delete.md)|<span data-ttu-id="a61e7-122">无</span><span class="sxs-lookup"><span data-stu-id="a61e7-122">None</span></span>|<span data-ttu-id="a61e7-123">删除 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)。</span><span class="sxs-lookup"><span data-stu-id="a61e7-123">Deletes a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span></span>|
|[<span data-ttu-id="a61e7-124">更新 userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="a61e7-124">Update userInstallStateSummary</span></span>](../api/intune-books-userinstallstatesummary-update.md)|[<span data-ttu-id="a61e7-125">userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="a61e7-125">userInstallStateSummary</span></span>](../resources/intune-books-userinstallstatesummary.md)|<span data-ttu-id="a61e7-126">更新 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a61e7-126">Update the properties of a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a61e7-127">属性</span><span class="sxs-lookup"><span data-stu-id="a61e7-127">Properties</span></span>
|<span data-ttu-id="a61e7-128">属性</span><span class="sxs-lookup"><span data-stu-id="a61e7-128">Property</span></span>|<span data-ttu-id="a61e7-129">类型</span><span class="sxs-lookup"><span data-stu-id="a61e7-129">Type</span></span>|<span data-ttu-id="a61e7-130">说明</span><span class="sxs-lookup"><span data-stu-id="a61e7-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a61e7-131">id</span><span class="sxs-lookup"><span data-stu-id="a61e7-131">id</span></span>|<span data-ttu-id="a61e7-132">String</span><span class="sxs-lookup"><span data-stu-id="a61e7-132">String</span></span>|<span data-ttu-id="a61e7-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a61e7-133">Key of the entity.</span></span>|
|<span data-ttu-id="a61e7-134">userName</span><span class="sxs-lookup"><span data-stu-id="a61e7-134">userName</span></span>|<span data-ttu-id="a61e7-135">String</span><span class="sxs-lookup"><span data-stu-id="a61e7-135">String</span></span>|<span data-ttu-id="a61e7-136">用户名。</span><span class="sxs-lookup"><span data-stu-id="a61e7-136">User name.</span></span>|
|<span data-ttu-id="a61e7-137">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a61e7-137">installedDeviceCount</span></span>|<span data-ttu-id="a61e7-138">Int32</span><span class="sxs-lookup"><span data-stu-id="a61e7-138">Int32</span></span>|<span data-ttu-id="a61e7-139">已安装设备的计数。</span><span class="sxs-lookup"><span data-stu-id="a61e7-139">Installed Device Count.</span></span>|
|<span data-ttu-id="a61e7-140">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a61e7-140">failedDeviceCount</span></span>|<span data-ttu-id="a61e7-141">Int32</span><span class="sxs-lookup"><span data-stu-id="a61e7-141">Int32</span></span>|<span data-ttu-id="a61e7-142">已失败设备的计数。</span><span class="sxs-lookup"><span data-stu-id="a61e7-142">Failed Device Count.</span></span>|
|<span data-ttu-id="a61e7-143">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a61e7-143">notInstalledDeviceCount</span></span>|<span data-ttu-id="a61e7-144">Int32</span><span class="sxs-lookup"><span data-stu-id="a61e7-144">Int32</span></span>|<span data-ttu-id="a61e7-145">Not installed device count。</span><span class="sxs-lookup"><span data-stu-id="a61e7-145">Not installed device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a61e7-146">关系</span><span class="sxs-lookup"><span data-stu-id="a61e7-146">Relationships</span></span>
|<span data-ttu-id="a61e7-147">关系</span><span class="sxs-lookup"><span data-stu-id="a61e7-147">Relationship</span></span>|<span data-ttu-id="a61e7-148">类型</span><span class="sxs-lookup"><span data-stu-id="a61e7-148">Type</span></span>|<span data-ttu-id="a61e7-149">说明</span><span class="sxs-lookup"><span data-stu-id="a61e7-149">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a61e7-150">deviceStates</span><span class="sxs-lookup"><span data-stu-id="a61e7-150">deviceStates</span></span>|<span data-ttu-id="a61e7-151">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a61e7-151">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="a61e7-152">电子书的安装状态。</span><span class="sxs-lookup"><span data-stu-id="a61e7-152">The install state of the eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a61e7-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a61e7-153">JSON Representation</span></span>
<span data-ttu-id="a61e7-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a61e7-154">Here is a JSON representation of the resource.</span></span>
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





