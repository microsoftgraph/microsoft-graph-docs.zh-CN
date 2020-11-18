---
title: userAppInstallStatus 资源类型
description: 包含用户的安装状态的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6ff97ad83ee8b25194b784d0dcdaafc68bfb7fc0
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49200033"
---
# <a name="userappinstallstatus-resource-type"></a><span data-ttu-id="c69ca-103">userAppInstallStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="c69ca-103">userAppInstallStatus resource type</span></span>

<span data-ttu-id="c69ca-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c69ca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c69ca-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c69ca-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c69ca-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c69ca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c69ca-107">包含用户的安装状态的属性。</span><span class="sxs-lookup"><span data-stu-id="c69ca-107">Contains properties for the installation status for a user.</span></span>

## <a name="methods"></a><span data-ttu-id="c69ca-108">方法</span><span class="sxs-lookup"><span data-stu-id="c69ca-108">Methods</span></span>
|<span data-ttu-id="c69ca-109">方法</span><span class="sxs-lookup"><span data-stu-id="c69ca-109">Method</span></span>|<span data-ttu-id="c69ca-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="c69ca-110">Return Type</span></span>|<span data-ttu-id="c69ca-111">说明</span><span class="sxs-lookup"><span data-stu-id="c69ca-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c69ca-112">列出 userAppInstallStatuses</span><span class="sxs-lookup"><span data-stu-id="c69ca-112">List userAppInstallStatuses</span></span>](../api/intune-apps-userappinstallstatus-list.md)|<span data-ttu-id="c69ca-113">[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c69ca-113">[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) collection</span></span>|<span data-ttu-id="c69ca-114">列出 [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c69ca-114">List properties and relationships of the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) objects.</span></span>|
|[<span data-ttu-id="c69ca-115">获取 userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="c69ca-115">Get userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-get.md)|[<span data-ttu-id="c69ca-116">userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="c69ca-116">userAppInstallStatus</span></span>](../resources/intune-apps-userappinstallstatus.md)|<span data-ttu-id="c69ca-117">读取 [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c69ca-117">Read properties and relationships of the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="c69ca-118">创建 userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="c69ca-118">Create userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-create.md)|[<span data-ttu-id="c69ca-119">userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="c69ca-119">userAppInstallStatus</span></span>](../resources/intune-apps-userappinstallstatus.md)|<span data-ttu-id="c69ca-120">创建新的 [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c69ca-120">Create a new [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="c69ca-121">删除 userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="c69ca-121">Delete userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-delete.md)|<span data-ttu-id="c69ca-122">无</span><span class="sxs-lookup"><span data-stu-id="c69ca-122">None</span></span>|<span data-ttu-id="c69ca-123">删除 [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)。</span><span class="sxs-lookup"><span data-stu-id="c69ca-123">Deletes a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md).</span></span>|
|[<span data-ttu-id="c69ca-124">更新 userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="c69ca-124">Update userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-update.md)|[<span data-ttu-id="c69ca-125">userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="c69ca-125">userAppInstallStatus</span></span>](../resources/intune-apps-userappinstallstatus.md)|<span data-ttu-id="c69ca-126">更新 [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c69ca-126">Update the properties of a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c69ca-127">属性</span><span class="sxs-lookup"><span data-stu-id="c69ca-127">Properties</span></span>
|<span data-ttu-id="c69ca-128">属性</span><span class="sxs-lookup"><span data-stu-id="c69ca-128">Property</span></span>|<span data-ttu-id="c69ca-129">类型</span><span class="sxs-lookup"><span data-stu-id="c69ca-129">Type</span></span>|<span data-ttu-id="c69ca-130">说明</span><span class="sxs-lookup"><span data-stu-id="c69ca-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c69ca-131">id</span><span class="sxs-lookup"><span data-stu-id="c69ca-131">id</span></span>|<span data-ttu-id="c69ca-132">String</span><span class="sxs-lookup"><span data-stu-id="c69ca-132">String</span></span>|<span data-ttu-id="c69ca-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c69ca-133">Key of the entity.</span></span>|
|<span data-ttu-id="c69ca-134">userName</span><span class="sxs-lookup"><span data-stu-id="c69ca-134">userName</span></span>|<span data-ttu-id="c69ca-135">String</span><span class="sxs-lookup"><span data-stu-id="c69ca-135">String</span></span>|<span data-ttu-id="c69ca-136">用户名。</span><span class="sxs-lookup"><span data-stu-id="c69ca-136">User name.</span></span>|
|<span data-ttu-id="c69ca-137">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c69ca-137">userPrincipalName</span></span>|<span data-ttu-id="c69ca-138">String</span><span class="sxs-lookup"><span data-stu-id="c69ca-138">String</span></span>|<span data-ttu-id="c69ca-139">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="c69ca-139">User Principal Name.</span></span>|
|<span data-ttu-id="c69ca-140">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c69ca-140">installedDeviceCount</span></span>|<span data-ttu-id="c69ca-141">Int32</span><span class="sxs-lookup"><span data-stu-id="c69ca-141">Int32</span></span>|<span data-ttu-id="c69ca-142">已安装设备的计数。</span><span class="sxs-lookup"><span data-stu-id="c69ca-142">Installed Device Count.</span></span>|
|<span data-ttu-id="c69ca-143">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c69ca-143">failedDeviceCount</span></span>|<span data-ttu-id="c69ca-144">Int32</span><span class="sxs-lookup"><span data-stu-id="c69ca-144">Int32</span></span>|<span data-ttu-id="c69ca-145">已失败设备的计数。</span><span class="sxs-lookup"><span data-stu-id="c69ca-145">Failed Device Count.</span></span>|
|<span data-ttu-id="c69ca-146">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c69ca-146">notInstalledDeviceCount</span></span>|<span data-ttu-id="c69ca-147">Int32</span><span class="sxs-lookup"><span data-stu-id="c69ca-147">Int32</span></span>|<span data-ttu-id="c69ca-148">Not installed device count。</span><span class="sxs-lookup"><span data-stu-id="c69ca-148">Not installed device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c69ca-149">关系</span><span class="sxs-lookup"><span data-stu-id="c69ca-149">Relationships</span></span>
|<span data-ttu-id="c69ca-150">关系</span><span class="sxs-lookup"><span data-stu-id="c69ca-150">Relationship</span></span>|<span data-ttu-id="c69ca-151">类型</span><span class="sxs-lookup"><span data-stu-id="c69ca-151">Type</span></span>|<span data-ttu-id="c69ca-152">说明</span><span class="sxs-lookup"><span data-stu-id="c69ca-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c69ca-153">应用</span><span class="sxs-lookup"><span data-stu-id="c69ca-153">app</span></span>|[<span data-ttu-id="c69ca-154">mobileApp</span><span class="sxs-lookup"><span data-stu-id="c69ca-154">mobileApp</span></span>](../resources/intune-shared-mobileapp.md)|<span data-ttu-id="c69ca-155">指向移动应用程序的导航链接。</span><span class="sxs-lookup"><span data-stu-id="c69ca-155">The navigation link to the mobile app.</span></span>|
|<span data-ttu-id="c69ca-156">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="c69ca-156">deviceStatuses</span></span>|<span data-ttu-id="c69ca-157">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c69ca-157">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) collection</span></span>|<span data-ttu-id="c69ca-158">设备上的应用程序的安装状态。</span><span class="sxs-lookup"><span data-stu-id="c69ca-158">The install state of the app on devices.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c69ca-159">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c69ca-159">JSON Representation</span></span>
<span data-ttu-id="c69ca-160">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c69ca-160">Here is a JSON representation of the resource.</span></span>
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




