---
title: eBookInstallSummary 资源类型
description: 包含某个设备的书籍安装摘要的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a68033930abb413ab7c2640381120b86c9873359
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37355958"
---
# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="3f792-103">eBookInstallSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="3f792-103">eBookInstallSummary resource type</span></span>

> <span data-ttu-id="3f792-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3f792-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f792-105">包含某个设备的书籍安装摘要的属性。</span><span class="sxs-lookup"><span data-stu-id="3f792-105">Contains properties for the installation summary of a book for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="3f792-106">方法</span><span class="sxs-lookup"><span data-stu-id="3f792-106">Methods</span></span>
|<span data-ttu-id="3f792-107">方法</span><span class="sxs-lookup"><span data-stu-id="3f792-107">Method</span></span>|<span data-ttu-id="3f792-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="3f792-108">Return Type</span></span>|<span data-ttu-id="3f792-109">说明</span><span class="sxs-lookup"><span data-stu-id="3f792-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3f792-110">获取 eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="3f792-110">Get eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-get.md)|[<span data-ttu-id="3f792-111">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="3f792-111">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="3f792-112">读取 [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3f792-112">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="3f792-113">更新 eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="3f792-113">Update eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-update.md)|[<span data-ttu-id="3f792-114">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="3f792-114">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="3f792-115">更新 [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3f792-115">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3f792-116">属性</span><span class="sxs-lookup"><span data-stu-id="3f792-116">Properties</span></span>
|<span data-ttu-id="3f792-117">属性</span><span class="sxs-lookup"><span data-stu-id="3f792-117">Property</span></span>|<span data-ttu-id="3f792-118">类型</span><span class="sxs-lookup"><span data-stu-id="3f792-118">Type</span></span>|<span data-ttu-id="3f792-119">说明</span><span class="sxs-lookup"><span data-stu-id="3f792-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f792-120">id</span><span class="sxs-lookup"><span data-stu-id="3f792-120">id</span></span>|<span data-ttu-id="3f792-121">String</span><span class="sxs-lookup"><span data-stu-id="3f792-121">String</span></span>|<span data-ttu-id="3f792-122">实体的键。</span><span class="sxs-lookup"><span data-stu-id="3f792-122">Key of the entity.</span></span>|
|<span data-ttu-id="3f792-123">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3f792-123">installedDeviceCount</span></span>|<span data-ttu-id="3f792-124">Int32</span><span class="sxs-lookup"><span data-stu-id="3f792-124">Int32</span></span>|<span data-ttu-id="3f792-125">已成功安装此书籍的设备数量。</span><span class="sxs-lookup"><span data-stu-id="3f792-125">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="3f792-126">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3f792-126">failedDeviceCount</span></span>|<span data-ttu-id="3f792-127">Int32</span><span class="sxs-lookup"><span data-stu-id="3f792-127">Int32</span></span>|<span data-ttu-id="3f792-128">未能成功安装此书籍的设备数量。</span><span class="sxs-lookup"><span data-stu-id="3f792-128">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="3f792-129">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3f792-129">notInstalledDeviceCount</span></span>|<span data-ttu-id="3f792-130">Int32</span><span class="sxs-lookup"><span data-stu-id="3f792-130">Int32</span></span>|<span data-ttu-id="3f792-131">未安装此书籍的设备数量。</span><span class="sxs-lookup"><span data-stu-id="3f792-131">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="3f792-132">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="3f792-132">installedUserCount</span></span>|<span data-ttu-id="3f792-133">Int32</span><span class="sxs-lookup"><span data-stu-id="3f792-133">Int32</span></span>|<span data-ttu-id="3f792-134">其设备全部成功安装了此书籍的用户数量。</span><span class="sxs-lookup"><span data-stu-id="3f792-134">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="3f792-135">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="3f792-135">failedUserCount</span></span>|<span data-ttu-id="3f792-136">Int32</span><span class="sxs-lookup"><span data-stu-id="3f792-136">Int32</span></span>|<span data-ttu-id="3f792-137">有 1 个或多个设备未能安装此书籍的用户数量。</span><span class="sxs-lookup"><span data-stu-id="3f792-137">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="3f792-138">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="3f792-138">notInstalledUserCount</span></span>|<span data-ttu-id="3f792-139">Int32</span><span class="sxs-lookup"><span data-stu-id="3f792-139">Int32</span></span>|<span data-ttu-id="3f792-140">未安装此书籍的用户数量。</span><span class="sxs-lookup"><span data-stu-id="3f792-140">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3f792-141">关系</span><span class="sxs-lookup"><span data-stu-id="3f792-141">Relationships</span></span>
<span data-ttu-id="3f792-142">无</span><span class="sxs-lookup"><span data-stu-id="3f792-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3f792-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3f792-143">JSON Representation</span></span>
<span data-ttu-id="3f792-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3f792-144">Here is a JSON representation of the resource.</span></span>
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




