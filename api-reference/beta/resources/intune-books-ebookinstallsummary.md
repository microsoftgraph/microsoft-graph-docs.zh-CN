---
title: eBookInstallSummary 资源类型
description: 包含某个设备的书籍安装摘要的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d4e8952012624a038f497fea3c6b81ad364448a8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415339"
---
# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="a2273-103">eBookInstallSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="a2273-103">eBookInstallSummary resource type</span></span>

> <span data-ttu-id="a2273-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="a2273-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a2273-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a2273-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a2273-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a2273-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2273-107">包含某个设备的书籍安装摘要的属性。</span><span class="sxs-lookup"><span data-stu-id="a2273-107">Contains properties for the installation summary of a book for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="a2273-108">方法</span><span class="sxs-lookup"><span data-stu-id="a2273-108">Methods</span></span>
|<span data-ttu-id="a2273-109">方法</span><span class="sxs-lookup"><span data-stu-id="a2273-109">Method</span></span>|<span data-ttu-id="a2273-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="a2273-110">Return Type</span></span>|<span data-ttu-id="a2273-111">说明</span><span class="sxs-lookup"><span data-stu-id="a2273-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a2273-112">获取 eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="a2273-112">Get eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-get.md)|[<span data-ttu-id="a2273-113">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="a2273-113">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="a2273-114">读取 [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a2273-114">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="a2273-115">更新 eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="a2273-115">Update eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-update.md)|[<span data-ttu-id="a2273-116">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="a2273-116">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="a2273-117">更新 [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a2273-117">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a2273-118">属性</span><span class="sxs-lookup"><span data-stu-id="a2273-118">Properties</span></span>
|<span data-ttu-id="a2273-119">属性</span><span class="sxs-lookup"><span data-stu-id="a2273-119">Property</span></span>|<span data-ttu-id="a2273-120">类型</span><span class="sxs-lookup"><span data-stu-id="a2273-120">Type</span></span>|<span data-ttu-id="a2273-121">说明</span><span class="sxs-lookup"><span data-stu-id="a2273-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2273-122">id</span><span class="sxs-lookup"><span data-stu-id="a2273-122">id</span></span>|<span data-ttu-id="a2273-123">String</span><span class="sxs-lookup"><span data-stu-id="a2273-123">String</span></span>|<span data-ttu-id="a2273-124">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a2273-124">Key of the entity.</span></span>|
|<span data-ttu-id="a2273-125">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a2273-125">installedDeviceCount</span></span>|<span data-ttu-id="a2273-126">Int32</span><span class="sxs-lookup"><span data-stu-id="a2273-126">Int32</span></span>|<span data-ttu-id="a2273-127">已成功安装此书籍的设备数量。</span><span class="sxs-lookup"><span data-stu-id="a2273-127">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="a2273-128">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a2273-128">failedDeviceCount</span></span>|<span data-ttu-id="a2273-129">Int32</span><span class="sxs-lookup"><span data-stu-id="a2273-129">Int32</span></span>|<span data-ttu-id="a2273-130">未能成功安装此书籍的设备数量。</span><span class="sxs-lookup"><span data-stu-id="a2273-130">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="a2273-131">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a2273-131">notInstalledDeviceCount</span></span>|<span data-ttu-id="a2273-132">Int32</span><span class="sxs-lookup"><span data-stu-id="a2273-132">Int32</span></span>|<span data-ttu-id="a2273-133">未安装此书籍的设备数量。</span><span class="sxs-lookup"><span data-stu-id="a2273-133">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="a2273-134">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="a2273-134">installedUserCount</span></span>|<span data-ttu-id="a2273-135">Int32</span><span class="sxs-lookup"><span data-stu-id="a2273-135">Int32</span></span>|<span data-ttu-id="a2273-136">其设备全部成功安装了此书籍的用户数量。</span><span class="sxs-lookup"><span data-stu-id="a2273-136">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="a2273-137">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="a2273-137">failedUserCount</span></span>|<span data-ttu-id="a2273-138">Int32</span><span class="sxs-lookup"><span data-stu-id="a2273-138">Int32</span></span>|<span data-ttu-id="a2273-139">有 1 个或多个设备未能安装此书籍的用户数量。</span><span class="sxs-lookup"><span data-stu-id="a2273-139">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="a2273-140">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="a2273-140">notInstalledUserCount</span></span>|<span data-ttu-id="a2273-141">Int32</span><span class="sxs-lookup"><span data-stu-id="a2273-141">Int32</span></span>|<span data-ttu-id="a2273-142">未安装此书籍的用户数量。</span><span class="sxs-lookup"><span data-stu-id="a2273-142">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a2273-143">关系</span><span class="sxs-lookup"><span data-stu-id="a2273-143">Relationships</span></span>
<span data-ttu-id="a2273-144">无</span><span class="sxs-lookup"><span data-stu-id="a2273-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a2273-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a2273-145">JSON Representation</span></span>
<span data-ttu-id="a2273-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a2273-146">Here is a JSON representation of the resource.</span></span>
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




