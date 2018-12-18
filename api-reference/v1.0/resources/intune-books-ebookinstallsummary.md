---
title: eBookInstallSummary 资源类型
description: 包含某个设备的书籍安装摘要的属性。
author: tfitzmac
ms.openlocfilehash: 4f94c82a0d7cd234206586829981c62ba7d0a959
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344273"
---
# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="9a740-103">eBookInstallSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="9a740-103">eBookInstallSummary resource type</span></span>

> <span data-ttu-id="9a740-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9a740-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9a740-105">包含某个设备的书籍安装摘要的属性。</span><span class="sxs-lookup"><span data-stu-id="9a740-105">Contains properties for the installation summary of a book for a device.</span></span>
## <a name="methods"></a><span data-ttu-id="9a740-106">方法</span><span class="sxs-lookup"><span data-stu-id="9a740-106">Methods</span></span>
|<span data-ttu-id="9a740-107">方法</span><span class="sxs-lookup"><span data-stu-id="9a740-107">Method</span></span>|<span data-ttu-id="9a740-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="9a740-108">Return Type</span></span>|<span data-ttu-id="9a740-109">说明</span><span class="sxs-lookup"><span data-stu-id="9a740-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9a740-110">获取 eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="9a740-110">Get eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-get.md)|[<span data-ttu-id="9a740-111">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="9a740-111">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="9a740-112">读取 [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9a740-112">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="9a740-113">更新 eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="9a740-113">Update eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-update.md)|[<span data-ttu-id="9a740-114">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="9a740-114">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="9a740-115">更新 [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9a740-115">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9a740-116">属性</span><span class="sxs-lookup"><span data-stu-id="9a740-116">Properties</span></span>
|<span data-ttu-id="9a740-117">属性</span><span class="sxs-lookup"><span data-stu-id="9a740-117">Property</span></span>|<span data-ttu-id="9a740-118">类型</span><span class="sxs-lookup"><span data-stu-id="9a740-118">Type</span></span>|<span data-ttu-id="9a740-119">说明</span><span class="sxs-lookup"><span data-stu-id="9a740-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a740-120">id</span><span class="sxs-lookup"><span data-stu-id="9a740-120">id</span></span>|<span data-ttu-id="9a740-121">String</span><span class="sxs-lookup"><span data-stu-id="9a740-121">String</span></span>|<span data-ttu-id="9a740-122">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9a740-122">Key of the entity.</span></span>|
|<span data-ttu-id="9a740-123">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9a740-123">installedDeviceCount</span></span>|<span data-ttu-id="9a740-124">Int32</span><span class="sxs-lookup"><span data-stu-id="9a740-124">Int32</span></span>|<span data-ttu-id="9a740-125">已成功安装此书籍的设备数量。</span><span class="sxs-lookup"><span data-stu-id="9a740-125">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="9a740-126">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9a740-126">failedDeviceCount</span></span>|<span data-ttu-id="9a740-127">Int32</span><span class="sxs-lookup"><span data-stu-id="9a740-127">Int32</span></span>|<span data-ttu-id="9a740-128">未能成功安装此书籍的设备数量。</span><span class="sxs-lookup"><span data-stu-id="9a740-128">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="9a740-129">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9a740-129">notInstalledDeviceCount</span></span>|<span data-ttu-id="9a740-130">Int32</span><span class="sxs-lookup"><span data-stu-id="9a740-130">Int32</span></span>|<span data-ttu-id="9a740-131">未安装此书籍的设备数量。</span><span class="sxs-lookup"><span data-stu-id="9a740-131">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="9a740-132">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="9a740-132">installedUserCount</span></span>|<span data-ttu-id="9a740-133">Int32</span><span class="sxs-lookup"><span data-stu-id="9a740-133">Int32</span></span>|<span data-ttu-id="9a740-134">其设备全部成功安装了此书籍的用户数量。</span><span class="sxs-lookup"><span data-stu-id="9a740-134">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="9a740-135">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="9a740-135">failedUserCount</span></span>|<span data-ttu-id="9a740-136">Int32</span><span class="sxs-lookup"><span data-stu-id="9a740-136">Int32</span></span>|<span data-ttu-id="9a740-137">有 1 个或多个设备未能安装此书籍的用户数量。</span><span class="sxs-lookup"><span data-stu-id="9a740-137">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="9a740-138">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="9a740-138">notInstalledUserCount</span></span>|<span data-ttu-id="9a740-139">Int32</span><span class="sxs-lookup"><span data-stu-id="9a740-139">Int32</span></span>|<span data-ttu-id="9a740-140">未安装此书籍的用户数量。</span><span class="sxs-lookup"><span data-stu-id="9a740-140">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9a740-141">关系</span><span class="sxs-lookup"><span data-stu-id="9a740-141">Relationships</span></span>
<span data-ttu-id="9a740-142">无</span><span class="sxs-lookup"><span data-stu-id="9a740-142">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9a740-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9a740-143">JSON Representation</span></span>
<span data-ttu-id="9a740-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9a740-144">Here is a JSON representation of the resource.</span></span>
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



