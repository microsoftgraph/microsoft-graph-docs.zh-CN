---
title: eBookInstallSummary 资源类型
description: 包含某个设备的书籍安装摘要的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3d3a5d1ce5c05d0a8c20a79aea2fd3562ab2170c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915940"
---
# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="37cf5-103">eBookInstallSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="37cf5-103">eBookInstallSummary resource type</span></span>

> <span data-ttu-id="37cf5-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="37cf5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="37cf5-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="37cf5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="37cf5-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="37cf5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="37cf5-107">包含某个设备的书籍安装摘要的属性。</span><span class="sxs-lookup"><span data-stu-id="37cf5-107">Contains properties for the installation summary of a book for a device.</span></span>
## <a name="methods"></a><span data-ttu-id="37cf5-108">方法</span><span class="sxs-lookup"><span data-stu-id="37cf5-108">Methods</span></span>
|<span data-ttu-id="37cf5-109">方法</span><span class="sxs-lookup"><span data-stu-id="37cf5-109">Method</span></span>|<span data-ttu-id="37cf5-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="37cf5-110">Return Type</span></span>|<span data-ttu-id="37cf5-111">说明</span><span class="sxs-lookup"><span data-stu-id="37cf5-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="37cf5-112">获取 eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="37cf5-112">Get eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-get.md)|[<span data-ttu-id="37cf5-113">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="37cf5-113">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="37cf5-114">读取 [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="37cf5-114">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="37cf5-115">更新 eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="37cf5-115">Update eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-update.md)|[<span data-ttu-id="37cf5-116">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="37cf5-116">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="37cf5-117">更新 [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="37cf5-117">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="37cf5-118">属性</span><span class="sxs-lookup"><span data-stu-id="37cf5-118">Properties</span></span>
|<span data-ttu-id="37cf5-119">属性</span><span class="sxs-lookup"><span data-stu-id="37cf5-119">Property</span></span>|<span data-ttu-id="37cf5-120">类型</span><span class="sxs-lookup"><span data-stu-id="37cf5-120">Type</span></span>|<span data-ttu-id="37cf5-121">说明</span><span class="sxs-lookup"><span data-stu-id="37cf5-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37cf5-122">id</span><span class="sxs-lookup"><span data-stu-id="37cf5-122">id</span></span>|<span data-ttu-id="37cf5-123">String</span><span class="sxs-lookup"><span data-stu-id="37cf5-123">String</span></span>|<span data-ttu-id="37cf5-124">实体的键。</span><span class="sxs-lookup"><span data-stu-id="37cf5-124">Key of the entity.</span></span>|
|<span data-ttu-id="37cf5-125">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="37cf5-125">installedDeviceCount</span></span>|<span data-ttu-id="37cf5-126">Int32</span><span class="sxs-lookup"><span data-stu-id="37cf5-126">Int32</span></span>|<span data-ttu-id="37cf5-127">已成功安装此书籍的设备数量。</span><span class="sxs-lookup"><span data-stu-id="37cf5-127">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="37cf5-128">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="37cf5-128">failedDeviceCount</span></span>|<span data-ttu-id="37cf5-129">Int32</span><span class="sxs-lookup"><span data-stu-id="37cf5-129">Int32</span></span>|<span data-ttu-id="37cf5-130">未能成功安装此书籍的设备数量。</span><span class="sxs-lookup"><span data-stu-id="37cf5-130">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="37cf5-131">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="37cf5-131">notInstalledDeviceCount</span></span>|<span data-ttu-id="37cf5-132">Int32</span><span class="sxs-lookup"><span data-stu-id="37cf5-132">Int32</span></span>|<span data-ttu-id="37cf5-133">未安装此书籍的设备数量。</span><span class="sxs-lookup"><span data-stu-id="37cf5-133">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="37cf5-134">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="37cf5-134">installedUserCount</span></span>|<span data-ttu-id="37cf5-135">Int32</span><span class="sxs-lookup"><span data-stu-id="37cf5-135">Int32</span></span>|<span data-ttu-id="37cf5-136">其设备全部成功安装了此书籍的用户数量。</span><span class="sxs-lookup"><span data-stu-id="37cf5-136">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="37cf5-137">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="37cf5-137">failedUserCount</span></span>|<span data-ttu-id="37cf5-138">Int32</span><span class="sxs-lookup"><span data-stu-id="37cf5-138">Int32</span></span>|<span data-ttu-id="37cf5-139">有 1 个或多个设备未能安装此书籍的用户数量。</span><span class="sxs-lookup"><span data-stu-id="37cf5-139">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="37cf5-140">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="37cf5-140">notInstalledUserCount</span></span>|<span data-ttu-id="37cf5-141">Int32</span><span class="sxs-lookup"><span data-stu-id="37cf5-141">Int32</span></span>|<span data-ttu-id="37cf5-142">未安装此书籍的用户数量。</span><span class="sxs-lookup"><span data-stu-id="37cf5-142">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="37cf5-143">关系</span><span class="sxs-lookup"><span data-stu-id="37cf5-143">Relationships</span></span>
<span data-ttu-id="37cf5-144">无</span><span class="sxs-lookup"><span data-stu-id="37cf5-144">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="37cf5-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="37cf5-145">JSON Representation</span></span>
<span data-ttu-id="37cf5-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="37cf5-146">Here is a JSON representation of the resource.</span></span>
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





