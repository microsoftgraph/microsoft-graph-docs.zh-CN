---
title: eBookInstallSummary 资源类型
description: 包含某个设备的书籍安装摘要的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 48c973d32e401dd378ca06db0c11f57e6c07654f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42489165"
---
# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="6fbf1-103">eBookInstallSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="6fbf1-103">eBookInstallSummary resource type</span></span>

<span data-ttu-id="6fbf1-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="6fbf1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6fbf1-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6fbf1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6fbf1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6fbf1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6fbf1-107">包含某个设备的书籍安装摘要的属性。</span><span class="sxs-lookup"><span data-stu-id="6fbf1-107">Contains properties for the installation summary of a book for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="6fbf1-108">方法</span><span class="sxs-lookup"><span data-stu-id="6fbf1-108">Methods</span></span>
|<span data-ttu-id="6fbf1-109">方法</span><span class="sxs-lookup"><span data-stu-id="6fbf1-109">Method</span></span>|<span data-ttu-id="6fbf1-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="6fbf1-110">Return Type</span></span>|<span data-ttu-id="6fbf1-111">说明</span><span class="sxs-lookup"><span data-stu-id="6fbf1-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6fbf1-112">获取 eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="6fbf1-112">Get eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-get.md)|[<span data-ttu-id="6fbf1-113">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="6fbf1-113">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="6fbf1-114">读取 [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6fbf1-114">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="6fbf1-115">更新 eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="6fbf1-115">Update eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-update.md)|[<span data-ttu-id="6fbf1-116">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="6fbf1-116">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="6fbf1-117">更新 [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6fbf1-117">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6fbf1-118">属性</span><span class="sxs-lookup"><span data-stu-id="6fbf1-118">Properties</span></span>
|<span data-ttu-id="6fbf1-119">属性</span><span class="sxs-lookup"><span data-stu-id="6fbf1-119">Property</span></span>|<span data-ttu-id="6fbf1-120">类型</span><span class="sxs-lookup"><span data-stu-id="6fbf1-120">Type</span></span>|<span data-ttu-id="6fbf1-121">说明</span><span class="sxs-lookup"><span data-stu-id="6fbf1-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fbf1-122">id</span><span class="sxs-lookup"><span data-stu-id="6fbf1-122">id</span></span>|<span data-ttu-id="6fbf1-123">String</span><span class="sxs-lookup"><span data-stu-id="6fbf1-123">String</span></span>|<span data-ttu-id="6fbf1-124">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6fbf1-124">Key of the entity.</span></span>|
|<span data-ttu-id="6fbf1-125">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6fbf1-125">installedDeviceCount</span></span>|<span data-ttu-id="6fbf1-126">Int32</span><span class="sxs-lookup"><span data-stu-id="6fbf1-126">Int32</span></span>|<span data-ttu-id="6fbf1-127">已成功安装此书籍的设备数量。</span><span class="sxs-lookup"><span data-stu-id="6fbf1-127">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="6fbf1-128">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6fbf1-128">failedDeviceCount</span></span>|<span data-ttu-id="6fbf1-129">Int32</span><span class="sxs-lookup"><span data-stu-id="6fbf1-129">Int32</span></span>|<span data-ttu-id="6fbf1-130">未能成功安装此书籍的设备数量。</span><span class="sxs-lookup"><span data-stu-id="6fbf1-130">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="6fbf1-131">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6fbf1-131">notInstalledDeviceCount</span></span>|<span data-ttu-id="6fbf1-132">Int32</span><span class="sxs-lookup"><span data-stu-id="6fbf1-132">Int32</span></span>|<span data-ttu-id="6fbf1-133">未安装此书籍的设备数量。</span><span class="sxs-lookup"><span data-stu-id="6fbf1-133">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="6fbf1-134">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="6fbf1-134">installedUserCount</span></span>|<span data-ttu-id="6fbf1-135">Int32</span><span class="sxs-lookup"><span data-stu-id="6fbf1-135">Int32</span></span>|<span data-ttu-id="6fbf1-136">其设备全部成功安装了此书籍的用户数量。</span><span class="sxs-lookup"><span data-stu-id="6fbf1-136">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="6fbf1-137">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="6fbf1-137">failedUserCount</span></span>|<span data-ttu-id="6fbf1-138">Int32</span><span class="sxs-lookup"><span data-stu-id="6fbf1-138">Int32</span></span>|<span data-ttu-id="6fbf1-139">有 1 个或多个设备未能安装此书籍的用户数量。</span><span class="sxs-lookup"><span data-stu-id="6fbf1-139">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="6fbf1-140">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="6fbf1-140">notInstalledUserCount</span></span>|<span data-ttu-id="6fbf1-141">Int32</span><span class="sxs-lookup"><span data-stu-id="6fbf1-141">Int32</span></span>|<span data-ttu-id="6fbf1-142">未安装此书籍的用户数量。</span><span class="sxs-lookup"><span data-stu-id="6fbf1-142">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6fbf1-143">关系</span><span class="sxs-lookup"><span data-stu-id="6fbf1-143">Relationships</span></span>
<span data-ttu-id="6fbf1-144">无</span><span class="sxs-lookup"><span data-stu-id="6fbf1-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6fbf1-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6fbf1-145">JSON Representation</span></span>
<span data-ttu-id="6fbf1-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6fbf1-146">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.eBookInstallSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.eBookInstallSummary",
  "id": "String (identifier)",
  "installedDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "notInstalledDeviceCount": 1024,
  "installedUserCount": 1024,
  "failedUserCount": 1024,
  "notInstalledUserCount": 1024
}
```



