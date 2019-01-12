---
title: userInstallStateSummary 资源类型
description: 包含某个用户的安装状态摘要的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6835dcad87fbf16a8dc81b6c9f9ab124a9834a3c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931851"
---
# <a name="userinstallstatesummary-resource-type"></a><span data-ttu-id="a86b9-103">userInstallStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="a86b9-103">userInstallStateSummary resource type</span></span>

> <span data-ttu-id="a86b9-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a86b9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a86b9-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a86b9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a86b9-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a86b9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a86b9-107">包含某个用户的安装状态摘要的属性。</span><span class="sxs-lookup"><span data-stu-id="a86b9-107">Contains properties for the installation state summary for a user.</span></span>
## <a name="methods"></a><span data-ttu-id="a86b9-108">方法</span><span class="sxs-lookup"><span data-stu-id="a86b9-108">Methods</span></span>
|<span data-ttu-id="a86b9-109">方法</span><span class="sxs-lookup"><span data-stu-id="a86b9-109">Method</span></span>|<span data-ttu-id="a86b9-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="a86b9-110">Return Type</span></span>|<span data-ttu-id="a86b9-111">说明</span><span class="sxs-lookup"><span data-stu-id="a86b9-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a86b9-112">列出 userInstallStateSummaries</span><span class="sxs-lookup"><span data-stu-id="a86b9-112">List userInstallStateSummaries</span></span>](../api/intune-books-userinstallstatesummary-list.md)|<span data-ttu-id="a86b9-113">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a86b9-113">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="a86b9-114">列出 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a86b9-114">List properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) objects.</span></span>|
|[<span data-ttu-id="a86b9-115">获取 userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="a86b9-115">Get userInstallStateSummary</span></span>](../api/intune-books-userinstallstatesummary-get.md)|[<span data-ttu-id="a86b9-116">userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="a86b9-116">userInstallStateSummary</span></span>](../resources/intune-books-userinstallstatesummary.md)|<span data-ttu-id="a86b9-117">读取 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a86b9-117">Read properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>|
|[<span data-ttu-id="a86b9-118">创建 userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="a86b9-118">Create userInstallStateSummary</span></span>](../api/intune-books-userinstallstatesummary-create.md)|[<span data-ttu-id="a86b9-119">userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="a86b9-119">userInstallStateSummary</span></span>](../resources/intune-books-userinstallstatesummary.md)|<span data-ttu-id="a86b9-120">创建新的 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a86b9-120">Create a new [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>|
|[<span data-ttu-id="a86b9-121">删除 userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="a86b9-121">Delete userInstallStateSummary</span></span>](../api/intune-books-userinstallstatesummary-delete.md)|<span data-ttu-id="a86b9-122">无</span><span class="sxs-lookup"><span data-stu-id="a86b9-122">None</span></span>|<span data-ttu-id="a86b9-123">删除 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)。</span><span class="sxs-lookup"><span data-stu-id="a86b9-123">Deletes a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span></span>|
|[<span data-ttu-id="a86b9-124">更新 userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="a86b9-124">Update userInstallStateSummary</span></span>](../api/intune-books-userinstallstatesummary-update.md)|[<span data-ttu-id="a86b9-125">userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="a86b9-125">userInstallStateSummary</span></span>](../resources/intune-books-userinstallstatesummary.md)|<span data-ttu-id="a86b9-126">更新 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a86b9-126">Update the properties of a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a86b9-127">属性</span><span class="sxs-lookup"><span data-stu-id="a86b9-127">Properties</span></span>
|<span data-ttu-id="a86b9-128">属性</span><span class="sxs-lookup"><span data-stu-id="a86b9-128">Property</span></span>|<span data-ttu-id="a86b9-129">类型</span><span class="sxs-lookup"><span data-stu-id="a86b9-129">Type</span></span>|<span data-ttu-id="a86b9-130">说明</span><span class="sxs-lookup"><span data-stu-id="a86b9-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a86b9-131">id</span><span class="sxs-lookup"><span data-stu-id="a86b9-131">id</span></span>|<span data-ttu-id="a86b9-132">String</span><span class="sxs-lookup"><span data-stu-id="a86b9-132">String</span></span>|<span data-ttu-id="a86b9-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a86b9-133">Key of the entity.</span></span>|
|<span data-ttu-id="a86b9-134">userName</span><span class="sxs-lookup"><span data-stu-id="a86b9-134">userName</span></span>|<span data-ttu-id="a86b9-135">String</span><span class="sxs-lookup"><span data-stu-id="a86b9-135">String</span></span>|<span data-ttu-id="a86b9-136">用户名。</span><span class="sxs-lookup"><span data-stu-id="a86b9-136">User name.</span></span>|
|<span data-ttu-id="a86b9-137">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a86b9-137">installedDeviceCount</span></span>|<span data-ttu-id="a86b9-138">Int32</span><span class="sxs-lookup"><span data-stu-id="a86b9-138">Int32</span></span>|<span data-ttu-id="a86b9-139">已安装设备的计数。</span><span class="sxs-lookup"><span data-stu-id="a86b9-139">Installed Device Count.</span></span>|
|<span data-ttu-id="a86b9-140">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a86b9-140">failedDeviceCount</span></span>|<span data-ttu-id="a86b9-141">Int32</span><span class="sxs-lookup"><span data-stu-id="a86b9-141">Int32</span></span>|<span data-ttu-id="a86b9-142">已失败设备的计数。</span><span class="sxs-lookup"><span data-stu-id="a86b9-142">Failed Device Count.</span></span>|
|<span data-ttu-id="a86b9-143">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a86b9-143">notInstalledDeviceCount</span></span>|<span data-ttu-id="a86b9-144">Int32</span><span class="sxs-lookup"><span data-stu-id="a86b9-144">Int32</span></span>|<span data-ttu-id="a86b9-145">Not installed device count。</span><span class="sxs-lookup"><span data-stu-id="a86b9-145">Not installed device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a86b9-146">关系</span><span class="sxs-lookup"><span data-stu-id="a86b9-146">Relationships</span></span>
|<span data-ttu-id="a86b9-147">关系</span><span class="sxs-lookup"><span data-stu-id="a86b9-147">Relationship</span></span>|<span data-ttu-id="a86b9-148">类型</span><span class="sxs-lookup"><span data-stu-id="a86b9-148">Type</span></span>|<span data-ttu-id="a86b9-149">说明</span><span class="sxs-lookup"><span data-stu-id="a86b9-149">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a86b9-150">deviceStates</span><span class="sxs-lookup"><span data-stu-id="a86b9-150">deviceStates</span></span>|<span data-ttu-id="a86b9-151">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a86b9-151">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="a86b9-152">电子书的安装状态。</span><span class="sxs-lookup"><span data-stu-id="a86b9-152">The install state of the eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a86b9-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a86b9-153">JSON Representation</span></span>
<span data-ttu-id="a86b9-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a86b9-154">Here is a JSON representation of the resource.</span></span>
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





