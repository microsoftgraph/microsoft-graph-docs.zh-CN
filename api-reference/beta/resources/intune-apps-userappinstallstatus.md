---
title: userAppInstallStatus 资源类型
description: 包含用户的安装状态属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f17a504537b1230de175e033779441627f5f98be
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938011"
---
# <a name="userappinstallstatus-resource-type"></a><span data-ttu-id="51ef4-103">userAppInstallStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="51ef4-103">userAppInstallStatus resource type</span></span>

> <span data-ttu-id="51ef4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="51ef4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="51ef4-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="51ef4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="51ef4-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="51ef4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="51ef4-107">包含用户的安装状态属性。</span><span class="sxs-lookup"><span data-stu-id="51ef4-107">Contains properties for the installation status for a user.</span></span>
## <a name="methods"></a><span data-ttu-id="51ef4-108">方法</span><span class="sxs-lookup"><span data-stu-id="51ef4-108">Methods</span></span>
|<span data-ttu-id="51ef4-109">方法</span><span class="sxs-lookup"><span data-stu-id="51ef4-109">Method</span></span>|<span data-ttu-id="51ef4-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="51ef4-110">Return Type</span></span>|<span data-ttu-id="51ef4-111">说明</span><span class="sxs-lookup"><span data-stu-id="51ef4-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="51ef4-112">列表 userAppInstallStatuses</span><span class="sxs-lookup"><span data-stu-id="51ef4-112">List userAppInstallStatuses</span></span>](../api/intune-apps-userappinstallstatus-list.md)|<span data-ttu-id="51ef4-113">[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)集合</span><span class="sxs-lookup"><span data-stu-id="51ef4-113">[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) collection</span></span>|<span data-ttu-id="51ef4-114">列出属性和[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="51ef4-114">List properties and relationships of the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) objects.</span></span>|
|[<span data-ttu-id="51ef4-115">获取 userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="51ef4-115">Get userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-get.md)|[<span data-ttu-id="51ef4-116">userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="51ef4-116">userAppInstallStatus</span></span>](../resources/intune-apps-userappinstallstatus.md)|<span data-ttu-id="51ef4-117">读取属性和[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="51ef4-117">Read properties and relationships of the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="51ef4-118">创建 userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="51ef4-118">Create userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-create.md)|[<span data-ttu-id="51ef4-119">userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="51ef4-119">userAppInstallStatus</span></span>](../resources/intune-apps-userappinstallstatus.md)|<span data-ttu-id="51ef4-120">创建新的[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)对象。</span><span class="sxs-lookup"><span data-stu-id="51ef4-120">Create a new [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="51ef4-121">删除 userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="51ef4-121">Delete userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-delete.md)|<span data-ttu-id="51ef4-122">无</span><span class="sxs-lookup"><span data-stu-id="51ef4-122">None</span></span>|<span data-ttu-id="51ef4-123">删除[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)。</span><span class="sxs-lookup"><span data-stu-id="51ef4-123">Deletes a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md).</span></span>|
|[<span data-ttu-id="51ef4-124">更新 userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="51ef4-124">Update userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-update.md)|[<span data-ttu-id="51ef4-125">userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="51ef4-125">userAppInstallStatus</span></span>](../resources/intune-apps-userappinstallstatus.md)|<span data-ttu-id="51ef4-126">更新[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="51ef4-126">Update the properties of a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="51ef4-127">属性</span><span class="sxs-lookup"><span data-stu-id="51ef4-127">Properties</span></span>
|<span data-ttu-id="51ef4-128">属性</span><span class="sxs-lookup"><span data-stu-id="51ef4-128">Property</span></span>|<span data-ttu-id="51ef4-129">类型</span><span class="sxs-lookup"><span data-stu-id="51ef4-129">Type</span></span>|<span data-ttu-id="51ef4-130">说明</span><span class="sxs-lookup"><span data-stu-id="51ef4-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51ef4-131">id</span><span class="sxs-lookup"><span data-stu-id="51ef4-131">id</span></span>|<span data-ttu-id="51ef4-132">String</span><span class="sxs-lookup"><span data-stu-id="51ef4-132">String</span></span>|<span data-ttu-id="51ef4-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="51ef4-133">Key of the entity.</span></span>|
|<span data-ttu-id="51ef4-134">userName</span><span class="sxs-lookup"><span data-stu-id="51ef4-134">userName</span></span>|<span data-ttu-id="51ef4-135">String</span><span class="sxs-lookup"><span data-stu-id="51ef4-135">String</span></span>|<span data-ttu-id="51ef4-136">用户名。</span><span class="sxs-lookup"><span data-stu-id="51ef4-136">User name.</span></span>|
|<span data-ttu-id="51ef4-137">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="51ef4-137">userPrincipalName</span></span>|<span data-ttu-id="51ef4-138">字符串</span><span class="sxs-lookup"><span data-stu-id="51ef4-138">String</span></span>|<span data-ttu-id="51ef4-139">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="51ef4-139">User Principal Name.</span></span>|
|<span data-ttu-id="51ef4-140">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="51ef4-140">installedDeviceCount</span></span>|<span data-ttu-id="51ef4-141">Int32</span><span class="sxs-lookup"><span data-stu-id="51ef4-141">Int32</span></span>|<span data-ttu-id="51ef4-142">已安装设备的计数。</span><span class="sxs-lookup"><span data-stu-id="51ef4-142">Installed Device Count.</span></span>|
|<span data-ttu-id="51ef4-143">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="51ef4-143">failedDeviceCount</span></span>|<span data-ttu-id="51ef4-144">Int32</span><span class="sxs-lookup"><span data-stu-id="51ef4-144">Int32</span></span>|<span data-ttu-id="51ef4-145">已失败设备的计数。</span><span class="sxs-lookup"><span data-stu-id="51ef4-145">Failed Device Count.</span></span>|
|<span data-ttu-id="51ef4-146">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="51ef4-146">notInstalledDeviceCount</span></span>|<span data-ttu-id="51ef4-147">Int32</span><span class="sxs-lookup"><span data-stu-id="51ef4-147">Int32</span></span>|<span data-ttu-id="51ef4-148">Not installed device count。</span><span class="sxs-lookup"><span data-stu-id="51ef4-148">Not installed device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="51ef4-149">关系</span><span class="sxs-lookup"><span data-stu-id="51ef4-149">Relationships</span></span>
|<span data-ttu-id="51ef4-150">关系</span><span class="sxs-lookup"><span data-stu-id="51ef4-150">Relationship</span></span>|<span data-ttu-id="51ef4-151">类型</span><span class="sxs-lookup"><span data-stu-id="51ef4-151">Type</span></span>|<span data-ttu-id="51ef4-152">说明</span><span class="sxs-lookup"><span data-stu-id="51ef4-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51ef4-153">应用程序</span><span class="sxs-lookup"><span data-stu-id="51ef4-153">app</span></span>|[<span data-ttu-id="51ef4-154">mobileApp</span><span class="sxs-lookup"><span data-stu-id="51ef4-154">mobileApp</span></span>](../resources/intune-apps-mobileapp.md)|<span data-ttu-id="51ef4-155">导航到移动应用程序链接。</span><span class="sxs-lookup"><span data-stu-id="51ef4-155">The navigation link to the mobile app.</span></span>|
|<span data-ttu-id="51ef4-156">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="51ef4-156">deviceStatuses</span></span>|<span data-ttu-id="51ef4-157">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)集合</span><span class="sxs-lookup"><span data-stu-id="51ef4-157">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) collection</span></span>|<span data-ttu-id="51ef4-158">在设备上应用程序的安装状态。</span><span class="sxs-lookup"><span data-stu-id="51ef4-158">The install state of the app on devices.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="51ef4-159">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="51ef4-159">JSON Representation</span></span>
<span data-ttu-id="51ef4-160">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="51ef4-160">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userAppInstallStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userAppInstallStatus",
  "id": "String (identifier)",
  "userName": "String",
  "userPrincipalName": "String",
  "installedDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "notInstalledDeviceCount": 1024
}
```





