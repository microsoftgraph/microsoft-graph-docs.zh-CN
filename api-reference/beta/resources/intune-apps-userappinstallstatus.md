---
title: userAppInstallStatus 资源类型
description: 包含用户的安装状态的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 951685d7acef566ab4761bc97906d5dc4b50ea6f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42491020"
---
# <a name="userappinstallstatus-resource-type"></a><span data-ttu-id="cb300-103">userAppInstallStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="cb300-103">userAppInstallStatus resource type</span></span>

<span data-ttu-id="cb300-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="cb300-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cb300-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cb300-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cb300-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cb300-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb300-107">包含用户的安装状态的属性。</span><span class="sxs-lookup"><span data-stu-id="cb300-107">Contains properties for the installation status for a user.</span></span>

## <a name="methods"></a><span data-ttu-id="cb300-108">方法</span><span class="sxs-lookup"><span data-stu-id="cb300-108">Methods</span></span>
|<span data-ttu-id="cb300-109">方法</span><span class="sxs-lookup"><span data-stu-id="cb300-109">Method</span></span>|<span data-ttu-id="cb300-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="cb300-110">Return Type</span></span>|<span data-ttu-id="cb300-111">说明</span><span class="sxs-lookup"><span data-stu-id="cb300-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cb300-112">列出 userAppInstallStatuses</span><span class="sxs-lookup"><span data-stu-id="cb300-112">List userAppInstallStatuses</span></span>](../api/intune-apps-userappinstallstatus-list.md)|<span data-ttu-id="cb300-113">[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)集合</span><span class="sxs-lookup"><span data-stu-id="cb300-113">[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) collection</span></span>|<span data-ttu-id="cb300-114">列出[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cb300-114">List properties and relationships of the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) objects.</span></span>|
|[<span data-ttu-id="cb300-115">获取 userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="cb300-115">Get userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-get.md)|[<span data-ttu-id="cb300-116">userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="cb300-116">userAppInstallStatus</span></span>](../resources/intune-apps-userappinstallstatus.md)|<span data-ttu-id="cb300-117">读取[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cb300-117">Read properties and relationships of the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="cb300-118">创建 userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="cb300-118">Create userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-create.md)|[<span data-ttu-id="cb300-119">userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="cb300-119">userAppInstallStatus</span></span>](../resources/intune-apps-userappinstallstatus.md)|<span data-ttu-id="cb300-120">创建新的[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)对象。</span><span class="sxs-lookup"><span data-stu-id="cb300-120">Create a new [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="cb300-121">删除 userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="cb300-121">Delete userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-delete.md)|<span data-ttu-id="cb300-122">无</span><span class="sxs-lookup"><span data-stu-id="cb300-122">None</span></span>|<span data-ttu-id="cb300-123">删除[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)。</span><span class="sxs-lookup"><span data-stu-id="cb300-123">Deletes a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md).</span></span>|
|[<span data-ttu-id="cb300-124">更新 userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="cb300-124">Update userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-update.md)|[<span data-ttu-id="cb300-125">userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="cb300-125">userAppInstallStatus</span></span>](../resources/intune-apps-userappinstallstatus.md)|<span data-ttu-id="cb300-126">更新[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="cb300-126">Update the properties of a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="cb300-127">属性</span><span class="sxs-lookup"><span data-stu-id="cb300-127">Properties</span></span>
|<span data-ttu-id="cb300-128">属性</span><span class="sxs-lookup"><span data-stu-id="cb300-128">Property</span></span>|<span data-ttu-id="cb300-129">类型</span><span class="sxs-lookup"><span data-stu-id="cb300-129">Type</span></span>|<span data-ttu-id="cb300-130">说明</span><span class="sxs-lookup"><span data-stu-id="cb300-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb300-131">id</span><span class="sxs-lookup"><span data-stu-id="cb300-131">id</span></span>|<span data-ttu-id="cb300-132">String</span><span class="sxs-lookup"><span data-stu-id="cb300-132">String</span></span>|<span data-ttu-id="cb300-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="cb300-133">Key of the entity.</span></span>|
|<span data-ttu-id="cb300-134">userName</span><span class="sxs-lookup"><span data-stu-id="cb300-134">userName</span></span>|<span data-ttu-id="cb300-135">String</span><span class="sxs-lookup"><span data-stu-id="cb300-135">String</span></span>|<span data-ttu-id="cb300-136">用户名。</span><span class="sxs-lookup"><span data-stu-id="cb300-136">User name.</span></span>|
|<span data-ttu-id="cb300-137">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="cb300-137">userPrincipalName</span></span>|<span data-ttu-id="cb300-138">String</span><span class="sxs-lookup"><span data-stu-id="cb300-138">String</span></span>|<span data-ttu-id="cb300-139">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="cb300-139">User Principal Name.</span></span>|
|<span data-ttu-id="cb300-140">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cb300-140">installedDeviceCount</span></span>|<span data-ttu-id="cb300-141">Int32</span><span class="sxs-lookup"><span data-stu-id="cb300-141">Int32</span></span>|<span data-ttu-id="cb300-142">已安装设备的计数。</span><span class="sxs-lookup"><span data-stu-id="cb300-142">Installed Device Count.</span></span>|
|<span data-ttu-id="cb300-143">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cb300-143">failedDeviceCount</span></span>|<span data-ttu-id="cb300-144">Int32</span><span class="sxs-lookup"><span data-stu-id="cb300-144">Int32</span></span>|<span data-ttu-id="cb300-145">已失败设备的计数。</span><span class="sxs-lookup"><span data-stu-id="cb300-145">Failed Device Count.</span></span>|
|<span data-ttu-id="cb300-146">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cb300-146">notInstalledDeviceCount</span></span>|<span data-ttu-id="cb300-147">Int32</span><span class="sxs-lookup"><span data-stu-id="cb300-147">Int32</span></span>|<span data-ttu-id="cb300-148">Not installed device count。</span><span class="sxs-lookup"><span data-stu-id="cb300-148">Not installed device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cb300-149">关系</span><span class="sxs-lookup"><span data-stu-id="cb300-149">Relationships</span></span>
|<span data-ttu-id="cb300-150">关系</span><span class="sxs-lookup"><span data-stu-id="cb300-150">Relationship</span></span>|<span data-ttu-id="cb300-151">类型</span><span class="sxs-lookup"><span data-stu-id="cb300-151">Type</span></span>|<span data-ttu-id="cb300-152">说明</span><span class="sxs-lookup"><span data-stu-id="cb300-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb300-153">应用程序</span><span class="sxs-lookup"><span data-stu-id="cb300-153">app</span></span>|[<span data-ttu-id="cb300-154">mobileApp</span><span class="sxs-lookup"><span data-stu-id="cb300-154">mobileApp</span></span>](../resources/intune-shared-mobileapp.md)|<span data-ttu-id="cb300-155">指向移动应用程序的导航链接。</span><span class="sxs-lookup"><span data-stu-id="cb300-155">The navigation link to the mobile app.</span></span>|
|<span data-ttu-id="cb300-156">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="cb300-156">deviceStatuses</span></span>|<span data-ttu-id="cb300-157">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)集合</span><span class="sxs-lookup"><span data-stu-id="cb300-157">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) collection</span></span>|<span data-ttu-id="cb300-158">设备上的应用程序的安装状态。</span><span class="sxs-lookup"><span data-stu-id="cb300-158">The install state of the app on devices.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cb300-159">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cb300-159">JSON Representation</span></span>
<span data-ttu-id="cb300-160">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cb300-160">Here is a JSON representation of the resource.</span></span>
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



