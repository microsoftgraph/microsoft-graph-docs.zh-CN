---
title: userAppInstallStatus 资源类型
description: 包含用户的安装状态的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ccae01f74466c839e602d5f7b5c62536fc409a15
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026843"
---
# <a name="userappinstallstatus-resource-type"></a><span data-ttu-id="321dc-103">userAppInstallStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="321dc-103">userAppInstallStatus resource type</span></span>

<span data-ttu-id="321dc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="321dc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="321dc-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="321dc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="321dc-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="321dc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="321dc-107">包含用户的安装状态的属性。</span><span class="sxs-lookup"><span data-stu-id="321dc-107">Contains properties for the installation status for a user.</span></span>

## <a name="methods"></a><span data-ttu-id="321dc-108">方法</span><span class="sxs-lookup"><span data-stu-id="321dc-108">Methods</span></span>
|<span data-ttu-id="321dc-109">方法</span><span class="sxs-lookup"><span data-stu-id="321dc-109">Method</span></span>|<span data-ttu-id="321dc-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="321dc-110">Return Type</span></span>|<span data-ttu-id="321dc-111">说明</span><span class="sxs-lookup"><span data-stu-id="321dc-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="321dc-112">列出 userAppInstallStatuses</span><span class="sxs-lookup"><span data-stu-id="321dc-112">List userAppInstallStatuses</span></span>](../api/intune-apps-userappinstallstatus-list.md)|<span data-ttu-id="321dc-113">[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="321dc-113">[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) collection</span></span>|<span data-ttu-id="321dc-114">列出 [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="321dc-114">List properties and relationships of the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) objects.</span></span>|
|[<span data-ttu-id="321dc-115">获取 userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="321dc-115">Get userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-get.md)|[<span data-ttu-id="321dc-116">userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="321dc-116">userAppInstallStatus</span></span>](../resources/intune-apps-userappinstallstatus.md)|<span data-ttu-id="321dc-117">读取 [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="321dc-117">Read properties and relationships of the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="321dc-118">创建 userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="321dc-118">Create userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-create.md)|[<span data-ttu-id="321dc-119">userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="321dc-119">userAppInstallStatus</span></span>](../resources/intune-apps-userappinstallstatus.md)|<span data-ttu-id="321dc-120">创建新的 [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="321dc-120">Create a new [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="321dc-121">删除 userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="321dc-121">Delete userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-delete.md)|<span data-ttu-id="321dc-122">无</span><span class="sxs-lookup"><span data-stu-id="321dc-122">None</span></span>|<span data-ttu-id="321dc-123">删除 [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)。</span><span class="sxs-lookup"><span data-stu-id="321dc-123">Deletes a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md).</span></span>|
|[<span data-ttu-id="321dc-124">更新 userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="321dc-124">Update userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-update.md)|[<span data-ttu-id="321dc-125">userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="321dc-125">userAppInstallStatus</span></span>](../resources/intune-apps-userappinstallstatus.md)|<span data-ttu-id="321dc-126">更新 [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="321dc-126">Update the properties of a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="321dc-127">属性</span><span class="sxs-lookup"><span data-stu-id="321dc-127">Properties</span></span>
|<span data-ttu-id="321dc-128">属性</span><span class="sxs-lookup"><span data-stu-id="321dc-128">Property</span></span>|<span data-ttu-id="321dc-129">类型</span><span class="sxs-lookup"><span data-stu-id="321dc-129">Type</span></span>|<span data-ttu-id="321dc-130">说明</span><span class="sxs-lookup"><span data-stu-id="321dc-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="321dc-131">id</span><span class="sxs-lookup"><span data-stu-id="321dc-131">id</span></span>|<span data-ttu-id="321dc-132">String</span><span class="sxs-lookup"><span data-stu-id="321dc-132">String</span></span>|<span data-ttu-id="321dc-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="321dc-133">Key of the entity.</span></span>|
|<span data-ttu-id="321dc-134">userName</span><span class="sxs-lookup"><span data-stu-id="321dc-134">userName</span></span>|<span data-ttu-id="321dc-135">String</span><span class="sxs-lookup"><span data-stu-id="321dc-135">String</span></span>|<span data-ttu-id="321dc-136">用户名。</span><span class="sxs-lookup"><span data-stu-id="321dc-136">User name.</span></span>|
|<span data-ttu-id="321dc-137">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="321dc-137">userPrincipalName</span></span>|<span data-ttu-id="321dc-138">String</span><span class="sxs-lookup"><span data-stu-id="321dc-138">String</span></span>|<span data-ttu-id="321dc-139">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="321dc-139">User Principal Name.</span></span>|
|<span data-ttu-id="321dc-140">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="321dc-140">installedDeviceCount</span></span>|<span data-ttu-id="321dc-141">Int32</span><span class="sxs-lookup"><span data-stu-id="321dc-141">Int32</span></span>|<span data-ttu-id="321dc-142">已安装设备的计数。</span><span class="sxs-lookup"><span data-stu-id="321dc-142">Installed Device Count.</span></span>|
|<span data-ttu-id="321dc-143">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="321dc-143">failedDeviceCount</span></span>|<span data-ttu-id="321dc-144">Int32</span><span class="sxs-lookup"><span data-stu-id="321dc-144">Int32</span></span>|<span data-ttu-id="321dc-145">已失败设备的计数。</span><span class="sxs-lookup"><span data-stu-id="321dc-145">Failed Device Count.</span></span>|
|<span data-ttu-id="321dc-146">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="321dc-146">notInstalledDeviceCount</span></span>|<span data-ttu-id="321dc-147">Int32</span><span class="sxs-lookup"><span data-stu-id="321dc-147">Int32</span></span>|<span data-ttu-id="321dc-148">Not installed device count。</span><span class="sxs-lookup"><span data-stu-id="321dc-148">Not installed device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="321dc-149">关系</span><span class="sxs-lookup"><span data-stu-id="321dc-149">Relationships</span></span>
|<span data-ttu-id="321dc-150">关系</span><span class="sxs-lookup"><span data-stu-id="321dc-150">Relationship</span></span>|<span data-ttu-id="321dc-151">类型</span><span class="sxs-lookup"><span data-stu-id="321dc-151">Type</span></span>|<span data-ttu-id="321dc-152">说明</span><span class="sxs-lookup"><span data-stu-id="321dc-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="321dc-153">应用程序</span><span class="sxs-lookup"><span data-stu-id="321dc-153">app</span></span>|[<span data-ttu-id="321dc-154">mobileApp</span><span class="sxs-lookup"><span data-stu-id="321dc-154">mobileApp</span></span>](../resources/intune-shared-mobileapp.md)|<span data-ttu-id="321dc-155">指向移动应用程序的导航链接。</span><span class="sxs-lookup"><span data-stu-id="321dc-155">The navigation link to the mobile app.</span></span>|
|<span data-ttu-id="321dc-156">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="321dc-156">deviceStatuses</span></span>|<span data-ttu-id="321dc-157">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="321dc-157">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) collection</span></span>|<span data-ttu-id="321dc-158">设备上的应用程序的安装状态。</span><span class="sxs-lookup"><span data-stu-id="321dc-158">The install state of the app on devices.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="321dc-159">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="321dc-159">JSON Representation</span></span>
<span data-ttu-id="321dc-160">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="321dc-160">Here is a JSON representation of the resource.</span></span>
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






