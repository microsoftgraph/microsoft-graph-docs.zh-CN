---
title: eBookInstallSummary 资源类型
description: 包含某个设备的书籍安装摘要的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8ef27a3da7f79bb42955c594e58be6732b029c06
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36335177"
---
# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="7e84a-103">eBookInstallSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="7e84a-103">eBookInstallSummary resource type</span></span>

> <span data-ttu-id="7e84a-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7e84a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7e84a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7e84a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e84a-106">包含某个设备的书籍安装摘要的属性。</span><span class="sxs-lookup"><span data-stu-id="7e84a-106">Contains properties for the installation summary of a book for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="7e84a-107">方法</span><span class="sxs-lookup"><span data-stu-id="7e84a-107">Methods</span></span>
|<span data-ttu-id="7e84a-108">方法</span><span class="sxs-lookup"><span data-stu-id="7e84a-108">Method</span></span>|<span data-ttu-id="7e84a-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="7e84a-109">Return Type</span></span>|<span data-ttu-id="7e84a-110">说明</span><span class="sxs-lookup"><span data-stu-id="7e84a-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7e84a-111">获取 eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="7e84a-111">Get eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-get.md)|[<span data-ttu-id="7e84a-112">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="7e84a-112">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="7e84a-113">读取 [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7e84a-113">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="7e84a-114">更新 eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="7e84a-114">Update eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-update.md)|[<span data-ttu-id="7e84a-115">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="7e84a-115">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="7e84a-116">更新 [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7e84a-116">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7e84a-117">属性</span><span class="sxs-lookup"><span data-stu-id="7e84a-117">Properties</span></span>
|<span data-ttu-id="7e84a-118">属性</span><span class="sxs-lookup"><span data-stu-id="7e84a-118">Property</span></span>|<span data-ttu-id="7e84a-119">类型</span><span class="sxs-lookup"><span data-stu-id="7e84a-119">Type</span></span>|<span data-ttu-id="7e84a-120">说明</span><span class="sxs-lookup"><span data-stu-id="7e84a-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e84a-121">id</span><span class="sxs-lookup"><span data-stu-id="7e84a-121">id</span></span>|<span data-ttu-id="7e84a-122">String</span><span class="sxs-lookup"><span data-stu-id="7e84a-122">String</span></span>|<span data-ttu-id="7e84a-123">实体的键。</span><span class="sxs-lookup"><span data-stu-id="7e84a-123">Key of the entity.</span></span>|
|<span data-ttu-id="7e84a-124">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7e84a-124">installedDeviceCount</span></span>|<span data-ttu-id="7e84a-125">Int32</span><span class="sxs-lookup"><span data-stu-id="7e84a-125">Int32</span></span>|<span data-ttu-id="7e84a-126">已成功安装此书籍的设备数量。</span><span class="sxs-lookup"><span data-stu-id="7e84a-126">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="7e84a-127">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7e84a-127">failedDeviceCount</span></span>|<span data-ttu-id="7e84a-128">Int32</span><span class="sxs-lookup"><span data-stu-id="7e84a-128">Int32</span></span>|<span data-ttu-id="7e84a-129">未能成功安装此书籍的设备数量。</span><span class="sxs-lookup"><span data-stu-id="7e84a-129">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="7e84a-130">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7e84a-130">notInstalledDeviceCount</span></span>|<span data-ttu-id="7e84a-131">Int32</span><span class="sxs-lookup"><span data-stu-id="7e84a-131">Int32</span></span>|<span data-ttu-id="7e84a-132">未安装此书籍的设备数量。</span><span class="sxs-lookup"><span data-stu-id="7e84a-132">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="7e84a-133">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="7e84a-133">installedUserCount</span></span>|<span data-ttu-id="7e84a-134">Int32</span><span class="sxs-lookup"><span data-stu-id="7e84a-134">Int32</span></span>|<span data-ttu-id="7e84a-135">其设备全部成功安装了此书籍的用户数量。</span><span class="sxs-lookup"><span data-stu-id="7e84a-135">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="7e84a-136">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="7e84a-136">failedUserCount</span></span>|<span data-ttu-id="7e84a-137">Int32</span><span class="sxs-lookup"><span data-stu-id="7e84a-137">Int32</span></span>|<span data-ttu-id="7e84a-138">有 1 个或多个设备未能安装此书籍的用户数量。</span><span class="sxs-lookup"><span data-stu-id="7e84a-138">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="7e84a-139">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="7e84a-139">notInstalledUserCount</span></span>|<span data-ttu-id="7e84a-140">Int32</span><span class="sxs-lookup"><span data-stu-id="7e84a-140">Int32</span></span>|<span data-ttu-id="7e84a-141">未安装此书籍的用户数量。</span><span class="sxs-lookup"><span data-stu-id="7e84a-141">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7e84a-142">关系</span><span class="sxs-lookup"><span data-stu-id="7e84a-142">Relationships</span></span>
<span data-ttu-id="7e84a-143">无</span><span class="sxs-lookup"><span data-stu-id="7e84a-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7e84a-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7e84a-144">JSON Representation</span></span>
<span data-ttu-id="7e84a-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7e84a-145">Here is a JSON representation of the resource.</span></span>
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



