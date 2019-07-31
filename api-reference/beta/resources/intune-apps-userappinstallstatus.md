---
title: userAppInstallStatus 资源类型
description: 包含用户的安装状态的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b3d25b512a088900971c6471e1f66296858a5081
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005056"
---
# <a name="userappinstallstatus-resource-type"></a><span data-ttu-id="116b8-103">userAppInstallStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="116b8-103">userAppInstallStatus resource type</span></span>

> <span data-ttu-id="116b8-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="116b8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="116b8-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="116b8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="116b8-106">包含用户的安装状态的属性。</span><span class="sxs-lookup"><span data-stu-id="116b8-106">Contains properties for the installation status for a user.</span></span>

## <a name="methods"></a><span data-ttu-id="116b8-107">方法</span><span class="sxs-lookup"><span data-stu-id="116b8-107">Methods</span></span>
|<span data-ttu-id="116b8-108">方法</span><span class="sxs-lookup"><span data-stu-id="116b8-108">Method</span></span>|<span data-ttu-id="116b8-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="116b8-109">Return Type</span></span>|<span data-ttu-id="116b8-110">说明</span><span class="sxs-lookup"><span data-stu-id="116b8-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="116b8-111">列出 userAppInstallStatuses</span><span class="sxs-lookup"><span data-stu-id="116b8-111">List userAppInstallStatuses</span></span>](../api/intune-apps-userappinstallstatus-list.md)|<span data-ttu-id="116b8-112">[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)集合</span><span class="sxs-lookup"><span data-stu-id="116b8-112">[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) collection</span></span>|<span data-ttu-id="116b8-113">列出[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="116b8-113">List properties and relationships of the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) objects.</span></span>|
|[<span data-ttu-id="116b8-114">获取 userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="116b8-114">Get userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-get.md)|[<span data-ttu-id="116b8-115">userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="116b8-115">userAppInstallStatus</span></span>](../resources/intune-apps-userappinstallstatus.md)|<span data-ttu-id="116b8-116">读取[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="116b8-116">Read properties and relationships of the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="116b8-117">创建 userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="116b8-117">Create userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-create.md)|[<span data-ttu-id="116b8-118">userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="116b8-118">userAppInstallStatus</span></span>](../resources/intune-apps-userappinstallstatus.md)|<span data-ttu-id="116b8-119">创建新的[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)对象。</span><span class="sxs-lookup"><span data-stu-id="116b8-119">Create a new [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="116b8-120">删除 userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="116b8-120">Delete userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-delete.md)|<span data-ttu-id="116b8-121">无</span><span class="sxs-lookup"><span data-stu-id="116b8-121">None</span></span>|<span data-ttu-id="116b8-122">删除[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)。</span><span class="sxs-lookup"><span data-stu-id="116b8-122">Deletes a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md).</span></span>|
|[<span data-ttu-id="116b8-123">更新 userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="116b8-123">Update userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-update.md)|[<span data-ttu-id="116b8-124">userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="116b8-124">userAppInstallStatus</span></span>](../resources/intune-apps-userappinstallstatus.md)|<span data-ttu-id="116b8-125">更新[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="116b8-125">Update the properties of a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="116b8-126">属性</span><span class="sxs-lookup"><span data-stu-id="116b8-126">Properties</span></span>
|<span data-ttu-id="116b8-127">属性</span><span class="sxs-lookup"><span data-stu-id="116b8-127">Property</span></span>|<span data-ttu-id="116b8-128">类型</span><span class="sxs-lookup"><span data-stu-id="116b8-128">Type</span></span>|<span data-ttu-id="116b8-129">说明</span><span class="sxs-lookup"><span data-stu-id="116b8-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="116b8-130">id</span><span class="sxs-lookup"><span data-stu-id="116b8-130">id</span></span>|<span data-ttu-id="116b8-131">String</span><span class="sxs-lookup"><span data-stu-id="116b8-131">String</span></span>|<span data-ttu-id="116b8-132">实体的键。</span><span class="sxs-lookup"><span data-stu-id="116b8-132">Key of the entity.</span></span>|
|<span data-ttu-id="116b8-133">userName</span><span class="sxs-lookup"><span data-stu-id="116b8-133">userName</span></span>|<span data-ttu-id="116b8-134">String</span><span class="sxs-lookup"><span data-stu-id="116b8-134">String</span></span>|<span data-ttu-id="116b8-135">用户名。</span><span class="sxs-lookup"><span data-stu-id="116b8-135">User name.</span></span>|
|<span data-ttu-id="116b8-136">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="116b8-136">userPrincipalName</span></span>|<span data-ttu-id="116b8-137">String</span><span class="sxs-lookup"><span data-stu-id="116b8-137">String</span></span>|<span data-ttu-id="116b8-138">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="116b8-138">User Principal Name.</span></span>|
|<span data-ttu-id="116b8-139">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="116b8-139">installedDeviceCount</span></span>|<span data-ttu-id="116b8-140">Int32</span><span class="sxs-lookup"><span data-stu-id="116b8-140">Int32</span></span>|<span data-ttu-id="116b8-141">已安装设备的计数。</span><span class="sxs-lookup"><span data-stu-id="116b8-141">Installed Device Count.</span></span>|
|<span data-ttu-id="116b8-142">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="116b8-142">failedDeviceCount</span></span>|<span data-ttu-id="116b8-143">Int32</span><span class="sxs-lookup"><span data-stu-id="116b8-143">Int32</span></span>|<span data-ttu-id="116b8-144">已失败设备的计数。</span><span class="sxs-lookup"><span data-stu-id="116b8-144">Failed Device Count.</span></span>|
|<span data-ttu-id="116b8-145">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="116b8-145">notInstalledDeviceCount</span></span>|<span data-ttu-id="116b8-146">Int32</span><span class="sxs-lookup"><span data-stu-id="116b8-146">Int32</span></span>|<span data-ttu-id="116b8-147">Not installed device count。</span><span class="sxs-lookup"><span data-stu-id="116b8-147">Not installed device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="116b8-148">关系</span><span class="sxs-lookup"><span data-stu-id="116b8-148">Relationships</span></span>
|<span data-ttu-id="116b8-149">关系</span><span class="sxs-lookup"><span data-stu-id="116b8-149">Relationship</span></span>|<span data-ttu-id="116b8-150">类型</span><span class="sxs-lookup"><span data-stu-id="116b8-150">Type</span></span>|<span data-ttu-id="116b8-151">说明</span><span class="sxs-lookup"><span data-stu-id="116b8-151">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="116b8-152">应用程序</span><span class="sxs-lookup"><span data-stu-id="116b8-152">app</span></span>|[<span data-ttu-id="116b8-153">mobileApp</span><span class="sxs-lookup"><span data-stu-id="116b8-153">mobileApp</span></span>](../resources/intune-apps-mobileapp.md)|<span data-ttu-id="116b8-154">指向移动应用程序的导航链接。</span><span class="sxs-lookup"><span data-stu-id="116b8-154">The navigation link to the mobile app.</span></span>|
|<span data-ttu-id="116b8-155">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="116b8-155">deviceStatuses</span></span>|<span data-ttu-id="116b8-156">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)集合</span><span class="sxs-lookup"><span data-stu-id="116b8-156">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) collection</span></span>|<span data-ttu-id="116b8-157">设备上的应用程序的安装状态。</span><span class="sxs-lookup"><span data-stu-id="116b8-157">The install state of the app on devices.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="116b8-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="116b8-158">JSON Representation</span></span>
<span data-ttu-id="116b8-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="116b8-159">Here is a JSON representation of the resource.</span></span>
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





