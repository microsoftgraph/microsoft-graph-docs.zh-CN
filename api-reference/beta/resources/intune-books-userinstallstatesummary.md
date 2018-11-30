---
title: userInstallStateSummary 资源类型
description: 包含某个用户的安装状态摘要的属性。
ms.openlocfilehash: 87d3dfbf5132c495c3d2507e94534972b30fd56f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046506"
---
# <a name="userinstallstatesummary-resource-type"></a><span data-ttu-id="fa945-103">userInstallStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="fa945-103">userInstallStateSummary resource type</span></span>

> <span data-ttu-id="fa945-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fa945-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fa945-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fa945-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fa945-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="fa945-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fa945-107">包含某个用户的安装状态摘要的属性。</span><span class="sxs-lookup"><span data-stu-id="fa945-107">Contains properties for the installation state summary for a user.</span></span>
## <a name="methods"></a><span data-ttu-id="fa945-108">方法</span><span class="sxs-lookup"><span data-stu-id="fa945-108">Methods</span></span>
|<span data-ttu-id="fa945-109">方法</span><span class="sxs-lookup"><span data-stu-id="fa945-109">Method</span></span>|<span data-ttu-id="fa945-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="fa945-110">Return Type</span></span>|<span data-ttu-id="fa945-111">说明</span><span class="sxs-lookup"><span data-stu-id="fa945-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="fa945-112">列出 userInstallStateSummaries</span><span class="sxs-lookup"><span data-stu-id="fa945-112">List userInstallStateSummaries</span></span>](../api/intune-books-userinstallstatesummary-list.md)|<span data-ttu-id="fa945-113">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fa945-113">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="fa945-114">列出 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fa945-114">List properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) objects.</span></span>|
|[<span data-ttu-id="fa945-115">获取 userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="fa945-115">Get userInstallStateSummary</span></span>](../api/intune-books-userinstallstatesummary-get.md)|[<span data-ttu-id="fa945-116">userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="fa945-116">userInstallStateSummary</span></span>](../resources/intune-books-userinstallstatesummary.md)|<span data-ttu-id="fa945-117">读取 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fa945-117">Read properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>|
|[<span data-ttu-id="fa945-118">创建 userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="fa945-118">Create userInstallStateSummary</span></span>](../api/intune-books-userinstallstatesummary-create.md)|[<span data-ttu-id="fa945-119">userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="fa945-119">userInstallStateSummary</span></span>](../resources/intune-books-userinstallstatesummary.md)|<span data-ttu-id="fa945-120">创建新的 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fa945-120">Create a new [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>|
|[<span data-ttu-id="fa945-121">删除 userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="fa945-121">Delete userInstallStateSummary</span></span>](../api/intune-books-userinstallstatesummary-delete.md)|<span data-ttu-id="fa945-122">无</span><span class="sxs-lookup"><span data-stu-id="fa945-122">None</span></span>|<span data-ttu-id="fa945-123">删除 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)。</span><span class="sxs-lookup"><span data-stu-id="fa945-123">Deletes a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span></span>|
|[<span data-ttu-id="fa945-124">更新 userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="fa945-124">Update userInstallStateSummary</span></span>](../api/intune-books-userinstallstatesummary-update.md)|[<span data-ttu-id="fa945-125">userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="fa945-125">userInstallStateSummary</span></span>](../resources/intune-books-userinstallstatesummary.md)|<span data-ttu-id="fa945-126">更新 [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="fa945-126">Update the properties of a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="fa945-127">属性</span><span class="sxs-lookup"><span data-stu-id="fa945-127">Properties</span></span>
|<span data-ttu-id="fa945-128">属性</span><span class="sxs-lookup"><span data-stu-id="fa945-128">Property</span></span>|<span data-ttu-id="fa945-129">类型</span><span class="sxs-lookup"><span data-stu-id="fa945-129">Type</span></span>|<span data-ttu-id="fa945-130">说明</span><span class="sxs-lookup"><span data-stu-id="fa945-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa945-131">id</span><span class="sxs-lookup"><span data-stu-id="fa945-131">id</span></span>|<span data-ttu-id="fa945-132">String</span><span class="sxs-lookup"><span data-stu-id="fa945-132">String</span></span>|<span data-ttu-id="fa945-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="fa945-133">Key of the entity.</span></span>|
|<span data-ttu-id="fa945-134">userName</span><span class="sxs-lookup"><span data-stu-id="fa945-134">userName</span></span>|<span data-ttu-id="fa945-135">String</span><span class="sxs-lookup"><span data-stu-id="fa945-135">String</span></span>|<span data-ttu-id="fa945-136">用户名。</span><span class="sxs-lookup"><span data-stu-id="fa945-136">User name.</span></span>|
|<span data-ttu-id="fa945-137">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fa945-137">installedDeviceCount</span></span>|<span data-ttu-id="fa945-138">Int32</span><span class="sxs-lookup"><span data-stu-id="fa945-138">Int32</span></span>|<span data-ttu-id="fa945-139">已安装设备的计数。</span><span class="sxs-lookup"><span data-stu-id="fa945-139">Installed Device Count.</span></span>|
|<span data-ttu-id="fa945-140">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fa945-140">failedDeviceCount</span></span>|<span data-ttu-id="fa945-141">Int32</span><span class="sxs-lookup"><span data-stu-id="fa945-141">Int32</span></span>|<span data-ttu-id="fa945-142">已失败设备的计数。</span><span class="sxs-lookup"><span data-stu-id="fa945-142">Failed Device Count.</span></span>|
|<span data-ttu-id="fa945-143">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fa945-143">notInstalledDeviceCount</span></span>|<span data-ttu-id="fa945-144">Int32</span><span class="sxs-lookup"><span data-stu-id="fa945-144">Int32</span></span>|<span data-ttu-id="fa945-145">Not installed device count。</span><span class="sxs-lookup"><span data-stu-id="fa945-145">Not installed device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fa945-146">关系</span><span class="sxs-lookup"><span data-stu-id="fa945-146">Relationships</span></span>
|<span data-ttu-id="fa945-147">关系</span><span class="sxs-lookup"><span data-stu-id="fa945-147">Relationship</span></span>|<span data-ttu-id="fa945-148">类型</span><span class="sxs-lookup"><span data-stu-id="fa945-148">Type</span></span>|<span data-ttu-id="fa945-149">说明</span><span class="sxs-lookup"><span data-stu-id="fa945-149">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa945-150">deviceStates</span><span class="sxs-lookup"><span data-stu-id="fa945-150">deviceStates</span></span>|<span data-ttu-id="fa945-151">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fa945-151">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="fa945-152">电子书的安装状态。</span><span class="sxs-lookup"><span data-stu-id="fa945-152">The install state of the eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fa945-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fa945-153">JSON Representation</span></span>
<span data-ttu-id="fa945-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fa945-154">Here is a JSON representation of the resource.</span></span>
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





