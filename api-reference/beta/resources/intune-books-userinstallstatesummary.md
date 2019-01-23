---
title: userInstallStateSummary 资源类型
description: 包含某个用户的安装状态摘要的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cecb608467efa312ea218197707cc14d55f3da04
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399330"
---
# <a name="userinstallstatesummary-resource-type"></a><span data-ttu-id="54924-103">userInstallStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="54924-103">userInstallStateSummary resource type</span></span>

> <span data-ttu-id="54924-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="54924-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="54924-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="54924-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="54924-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="54924-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54924-107">包含某个用户的安装状态摘要的属性。</span><span class="sxs-lookup"><span data-stu-id="54924-107">Contains properties for the installation state summary for a user.</span></span>

## <a name="methods"></a><span data-ttu-id="54924-108">方法</span><span class="sxs-lookup"><span data-stu-id="54924-108">Methods</span></span>
|<span data-ttu-id="54924-109">方法</span><span class="sxs-lookup"><span data-stu-id="54924-109">Method</span></span>|<span data-ttu-id="54924-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="54924-110">Return Type</span></span>|<span data-ttu-id="54924-111">说明</span><span class="sxs-lookup"><span data-stu-id="54924-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="54924-112">列出 userInstallStateSummaries</span><span class="sxs-lookup"><span data-stu-id="54924-112">List userInstallStateSummaries</span></span>](../api/intune-books-userinstallstatesummary-list.md)|<span data-ttu-id="54924-113">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="54924-113">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="54924-114">列出 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="54924-114">List properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) objects.</span></span>|
|[<span data-ttu-id="54924-115">获取 userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="54924-115">Get userInstallStateSummary</span></span>](../api/intune-books-userinstallstatesummary-get.md)|[<span data-ttu-id="54924-116">userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="54924-116">userInstallStateSummary</span></span>](../resources/intune-books-userinstallstatesummary.md)|<span data-ttu-id="54924-117">读取 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="54924-117">Read properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>|
|[<span data-ttu-id="54924-118">创建 userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="54924-118">Create userInstallStateSummary</span></span>](../api/intune-books-userinstallstatesummary-create.md)|[<span data-ttu-id="54924-119">userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="54924-119">userInstallStateSummary</span></span>](../resources/intune-books-userinstallstatesummary.md)|<span data-ttu-id="54924-120">创建新的 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="54924-120">Create a new [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>|
|[<span data-ttu-id="54924-121">删除 userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="54924-121">Delete userInstallStateSummary</span></span>](../api/intune-books-userinstallstatesummary-delete.md)|<span data-ttu-id="54924-122">无</span><span class="sxs-lookup"><span data-stu-id="54924-122">None</span></span>|<span data-ttu-id="54924-123">删除 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)。</span><span class="sxs-lookup"><span data-stu-id="54924-123">Deletes a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span></span>|
|[<span data-ttu-id="54924-124">更新 userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="54924-124">Update userInstallStateSummary</span></span>](../api/intune-books-userinstallstatesummary-update.md)|[<span data-ttu-id="54924-125">userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="54924-125">userInstallStateSummary</span></span>](../resources/intune-books-userinstallstatesummary.md)|<span data-ttu-id="54924-126">更新 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="54924-126">Update the properties of a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="54924-127">属性</span><span class="sxs-lookup"><span data-stu-id="54924-127">Properties</span></span>
|<span data-ttu-id="54924-128">属性</span><span class="sxs-lookup"><span data-stu-id="54924-128">Property</span></span>|<span data-ttu-id="54924-129">类型</span><span class="sxs-lookup"><span data-stu-id="54924-129">Type</span></span>|<span data-ttu-id="54924-130">说明</span><span class="sxs-lookup"><span data-stu-id="54924-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54924-131">id</span><span class="sxs-lookup"><span data-stu-id="54924-131">id</span></span>|<span data-ttu-id="54924-132">String</span><span class="sxs-lookup"><span data-stu-id="54924-132">String</span></span>|<span data-ttu-id="54924-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="54924-133">Key of the entity.</span></span>|
|<span data-ttu-id="54924-134">userName</span><span class="sxs-lookup"><span data-stu-id="54924-134">userName</span></span>|<span data-ttu-id="54924-135">String</span><span class="sxs-lookup"><span data-stu-id="54924-135">String</span></span>|<span data-ttu-id="54924-136">用户名。</span><span class="sxs-lookup"><span data-stu-id="54924-136">User name.</span></span>|
|<span data-ttu-id="54924-137">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="54924-137">installedDeviceCount</span></span>|<span data-ttu-id="54924-138">Int32</span><span class="sxs-lookup"><span data-stu-id="54924-138">Int32</span></span>|<span data-ttu-id="54924-139">已安装设备的计数。</span><span class="sxs-lookup"><span data-stu-id="54924-139">Installed Device Count.</span></span>|
|<span data-ttu-id="54924-140">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="54924-140">failedDeviceCount</span></span>|<span data-ttu-id="54924-141">Int32</span><span class="sxs-lookup"><span data-stu-id="54924-141">Int32</span></span>|<span data-ttu-id="54924-142">已失败设备的计数。</span><span class="sxs-lookup"><span data-stu-id="54924-142">Failed Device Count.</span></span>|
|<span data-ttu-id="54924-143">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="54924-143">notInstalledDeviceCount</span></span>|<span data-ttu-id="54924-144">Int32</span><span class="sxs-lookup"><span data-stu-id="54924-144">Int32</span></span>|<span data-ttu-id="54924-145">Not installed device count。</span><span class="sxs-lookup"><span data-stu-id="54924-145">Not installed device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="54924-146">关系</span><span class="sxs-lookup"><span data-stu-id="54924-146">Relationships</span></span>
|<span data-ttu-id="54924-147">关系</span><span class="sxs-lookup"><span data-stu-id="54924-147">Relationship</span></span>|<span data-ttu-id="54924-148">类型</span><span class="sxs-lookup"><span data-stu-id="54924-148">Type</span></span>|<span data-ttu-id="54924-149">说明</span><span class="sxs-lookup"><span data-stu-id="54924-149">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54924-150">deviceStates</span><span class="sxs-lookup"><span data-stu-id="54924-150">deviceStates</span></span>|<span data-ttu-id="54924-151">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="54924-151">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="54924-152">电子书的安装状态。</span><span class="sxs-lookup"><span data-stu-id="54924-152">The install state of the eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="54924-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="54924-153">JSON Representation</span></span>
<span data-ttu-id="54924-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="54924-154">Here is a JSON representation of the resource.</span></span>
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




