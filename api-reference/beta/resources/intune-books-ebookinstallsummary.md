---
title: eBookInstallSummary 资源类型
description: 包含某个设备的书籍安装摘要的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f4132bf41a3081bc9b5234cfcd0066508baf1dee
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49295409"
---
# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="6c752-103">eBookInstallSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="6c752-103">eBookInstallSummary resource type</span></span>

<span data-ttu-id="6c752-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c752-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6c752-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6c752-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c752-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6c752-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c752-107">包含某个设备的书籍安装摘要的属性。</span><span class="sxs-lookup"><span data-stu-id="6c752-107">Contains properties for the installation summary of a book for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="6c752-108">Methods</span><span class="sxs-lookup"><span data-stu-id="6c752-108">Methods</span></span>
|<span data-ttu-id="6c752-109">方法</span><span class="sxs-lookup"><span data-stu-id="6c752-109">Method</span></span>|<span data-ttu-id="6c752-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="6c752-110">Return Type</span></span>|<span data-ttu-id="6c752-111">Description</span><span class="sxs-lookup"><span data-stu-id="6c752-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6c752-112">获取 eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="6c752-112">Get eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-get.md)|[<span data-ttu-id="6c752-113">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="6c752-113">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="6c752-114">读取 [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6c752-114">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="6c752-115">更新 eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="6c752-115">Update eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-update.md)|[<span data-ttu-id="6c752-116">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="6c752-116">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="6c752-117">更新 [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6c752-117">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6c752-118">属性</span><span class="sxs-lookup"><span data-stu-id="6c752-118">Properties</span></span>
|<span data-ttu-id="6c752-119">属性</span><span class="sxs-lookup"><span data-stu-id="6c752-119">Property</span></span>|<span data-ttu-id="6c752-120">类型</span><span class="sxs-lookup"><span data-stu-id="6c752-120">Type</span></span>|<span data-ttu-id="6c752-121">说明</span><span class="sxs-lookup"><span data-stu-id="6c752-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c752-122">id</span><span class="sxs-lookup"><span data-stu-id="6c752-122">id</span></span>|<span data-ttu-id="6c752-123">字符串</span><span class="sxs-lookup"><span data-stu-id="6c752-123">String</span></span>|<span data-ttu-id="6c752-124">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6c752-124">Key of the entity.</span></span>|
|<span data-ttu-id="6c752-125">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6c752-125">installedDeviceCount</span></span>|<span data-ttu-id="6c752-126">Int32</span><span class="sxs-lookup"><span data-stu-id="6c752-126">Int32</span></span>|<span data-ttu-id="6c752-127">已成功安装此书籍的设备数量。</span><span class="sxs-lookup"><span data-stu-id="6c752-127">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="6c752-128">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6c752-128">failedDeviceCount</span></span>|<span data-ttu-id="6c752-129">Int32</span><span class="sxs-lookup"><span data-stu-id="6c752-129">Int32</span></span>|<span data-ttu-id="6c752-130">未能成功安装此书籍的设备数量。</span><span class="sxs-lookup"><span data-stu-id="6c752-130">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="6c752-131">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6c752-131">notInstalledDeviceCount</span></span>|<span data-ttu-id="6c752-132">Int32</span><span class="sxs-lookup"><span data-stu-id="6c752-132">Int32</span></span>|<span data-ttu-id="6c752-133">未安装此书籍的设备数量。</span><span class="sxs-lookup"><span data-stu-id="6c752-133">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="6c752-134">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="6c752-134">installedUserCount</span></span>|<span data-ttu-id="6c752-135">Int32</span><span class="sxs-lookup"><span data-stu-id="6c752-135">Int32</span></span>|<span data-ttu-id="6c752-136">其设备全部成功安装了此书籍的用户数量。</span><span class="sxs-lookup"><span data-stu-id="6c752-136">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="6c752-137">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="6c752-137">failedUserCount</span></span>|<span data-ttu-id="6c752-138">Int32</span><span class="sxs-lookup"><span data-stu-id="6c752-138">Int32</span></span>|<span data-ttu-id="6c752-139">有 1 个或多个设备未能安装此书籍的用户数量。</span><span class="sxs-lookup"><span data-stu-id="6c752-139">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="6c752-140">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="6c752-140">notInstalledUserCount</span></span>|<span data-ttu-id="6c752-141">Int32</span><span class="sxs-lookup"><span data-stu-id="6c752-141">Int32</span></span>|<span data-ttu-id="6c752-142">未安装此书籍的用户数量。</span><span class="sxs-lookup"><span data-stu-id="6c752-142">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6c752-143">关系</span><span class="sxs-lookup"><span data-stu-id="6c752-143">Relationships</span></span>
<span data-ttu-id="6c752-144">无</span><span class="sxs-lookup"><span data-stu-id="6c752-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6c752-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6c752-145">JSON Representation</span></span>
<span data-ttu-id="6c752-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6c752-146">Here is a JSON representation of the resource.</span></span>
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




