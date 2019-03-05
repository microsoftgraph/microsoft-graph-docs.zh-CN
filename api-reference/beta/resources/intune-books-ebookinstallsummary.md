---
title: eBookInstallSummary 资源类型
description: 包含某个设备的书籍安装摘要的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 52d08d00bfbc26e0b72ddf53404eff8d55bb72b9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151238"
---
# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="b0fba-103">eBookInstallSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="b0fba-103">eBookInstallSummary resource type</span></span>

> <span data-ttu-id="b0fba-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b0fba-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0fba-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b0fba-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0fba-106">包含某个设备的书籍安装摘要的属性。</span><span class="sxs-lookup"><span data-stu-id="b0fba-106">Contains properties for the installation summary of a book for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="b0fba-107">方法</span><span class="sxs-lookup"><span data-stu-id="b0fba-107">Methods</span></span>
|<span data-ttu-id="b0fba-108">方法</span><span class="sxs-lookup"><span data-stu-id="b0fba-108">Method</span></span>|<span data-ttu-id="b0fba-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="b0fba-109">Return Type</span></span>|<span data-ttu-id="b0fba-110">说明</span><span class="sxs-lookup"><span data-stu-id="b0fba-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b0fba-111">获取 eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="b0fba-111">Get eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-get.md)|[<span data-ttu-id="b0fba-112">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="b0fba-112">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="b0fba-113">读取 [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b0fba-113">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="b0fba-114">更新 eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="b0fba-114">Update eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-update.md)|[<span data-ttu-id="b0fba-115">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="b0fba-115">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="b0fba-116">更新 [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b0fba-116">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b0fba-117">属性</span><span class="sxs-lookup"><span data-stu-id="b0fba-117">Properties</span></span>
|<span data-ttu-id="b0fba-118">属性</span><span class="sxs-lookup"><span data-stu-id="b0fba-118">Property</span></span>|<span data-ttu-id="b0fba-119">类型</span><span class="sxs-lookup"><span data-stu-id="b0fba-119">Type</span></span>|<span data-ttu-id="b0fba-120">说明</span><span class="sxs-lookup"><span data-stu-id="b0fba-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0fba-121">id</span><span class="sxs-lookup"><span data-stu-id="b0fba-121">id</span></span>|<span data-ttu-id="b0fba-122">String</span><span class="sxs-lookup"><span data-stu-id="b0fba-122">String</span></span>|<span data-ttu-id="b0fba-123">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b0fba-123">Key of the entity.</span></span>|
|<span data-ttu-id="b0fba-124">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b0fba-124">installedDeviceCount</span></span>|<span data-ttu-id="b0fba-125">Int32</span><span class="sxs-lookup"><span data-stu-id="b0fba-125">Int32</span></span>|<span data-ttu-id="b0fba-126">已成功安装此书籍的设备数量。</span><span class="sxs-lookup"><span data-stu-id="b0fba-126">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="b0fba-127">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b0fba-127">failedDeviceCount</span></span>|<span data-ttu-id="b0fba-128">Int32</span><span class="sxs-lookup"><span data-stu-id="b0fba-128">Int32</span></span>|<span data-ttu-id="b0fba-129">未能成功安装此书籍的设备数量。</span><span class="sxs-lookup"><span data-stu-id="b0fba-129">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="b0fba-130">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b0fba-130">notInstalledDeviceCount</span></span>|<span data-ttu-id="b0fba-131">Int32</span><span class="sxs-lookup"><span data-stu-id="b0fba-131">Int32</span></span>|<span data-ttu-id="b0fba-132">未安装此书籍的设备数量。</span><span class="sxs-lookup"><span data-stu-id="b0fba-132">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="b0fba-133">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="b0fba-133">installedUserCount</span></span>|<span data-ttu-id="b0fba-134">Int32</span><span class="sxs-lookup"><span data-stu-id="b0fba-134">Int32</span></span>|<span data-ttu-id="b0fba-135">其设备全部成功安装了此书籍的用户数量。</span><span class="sxs-lookup"><span data-stu-id="b0fba-135">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="b0fba-136">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="b0fba-136">failedUserCount</span></span>|<span data-ttu-id="b0fba-137">Int32</span><span class="sxs-lookup"><span data-stu-id="b0fba-137">Int32</span></span>|<span data-ttu-id="b0fba-138">有 1 个或多个设备未能安装此书籍的用户数量。</span><span class="sxs-lookup"><span data-stu-id="b0fba-138">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="b0fba-139">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="b0fba-139">notInstalledUserCount</span></span>|<span data-ttu-id="b0fba-140">Int32</span><span class="sxs-lookup"><span data-stu-id="b0fba-140">Int32</span></span>|<span data-ttu-id="b0fba-141">未安装此书籍的用户数量。</span><span class="sxs-lookup"><span data-stu-id="b0fba-141">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0fba-142">关系</span><span class="sxs-lookup"><span data-stu-id="b0fba-142">Relationships</span></span>
<span data-ttu-id="b0fba-143">无</span><span class="sxs-lookup"><span data-stu-id="b0fba-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b0fba-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b0fba-144">JSON Representation</span></span>
<span data-ttu-id="b0fba-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b0fba-145">Here is a JSON representation of the resource.</span></span>
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




